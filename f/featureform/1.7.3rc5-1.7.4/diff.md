# Comparing `tmp/featureform-1.7.3rc5.tar.gz` & `tmp/featureform-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featureform-1.7.3rc5.tar", last modified: Thu Apr 13 02:00:56 2023, max compression
+gzip compressed data, was "featureform-1.7.4.tar", last modified: Wed Apr 26 21:20:25 2023, max compression
```

## Comparing `featureform-1.7.3rc5.tar` & `featureform-1.7.4.tar`

### file list

```diff
@@ -1,358 +1,367 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.818579 featureform-1.7.3rc5/
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-13 02:00:56.818579 featureform-1.7.3rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-13 02:00:56.818579 featureform-1.7.3rc5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.778579 featureform-1.7.3rc5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.782579 featureform-1.7.3rc5/src/featureform/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.778579 featureform-1.7.3rc5/src/featureform/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.786579 featureform-1.7.3rc5/src/featureform/dashboard/out/
--rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.786579 featureform-1.7.3rc5/src/featureform/dashboard/out/[type]/
--rw-r--r--   0 runner    (1001) docker     (123)    19241 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/[type]/[entity].html
--rw-r--r--   0 runner    (1001) docker     (123)    17140 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/[type].html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.778579 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.778579 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.786579 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.810579 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)    83561 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js
--rw-r--r--   0 runner    (1001) docker     (123)    74481 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js
--rw-r--r--   0 runner    (1001) docker     (123)    21739 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js
--rw-r--r--   0 runner    (1001) docker     (123)   201393 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js
--rw-r--r--   0 runner    (1001) docker     (123)   130270 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js
--rw-r--r--   0 runner    (1001) docker     (123)   104027 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.814579 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/pages/404-baaca4b2f4acc755.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.814579 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-b07f3c4463890639.js
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-751a928da9d524e9.js
--rw-r--r--   0 runner    (1001) docker     (123)  3582042 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/pages/_app-01b1894ee40506d5.js
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/pages/_error-3f70f2d61eb8c6dd.js
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/pages/connections-1d67ba61869dece6.js
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/pages/search-175858e61ba25631.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.814579 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
--rw-r--r--   0 runner    (1001) docker     (123)    35679 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.ab502da8667e6dc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.d1d39a9bd6ac45b9.js
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.42d8625dbbdd27ed.js
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.17a13e6bcda1e1f3.js
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.ac01f4f7ac16a003.js
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.0e0594706d30fbd8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.2b3348708365f9ef.js
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.5e3fe34e0eab5fdb.js
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.5d313969242bf8d5.js
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js
--rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.bd5b619f107eee8f.js
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js
--rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.22a1c7ff76f01643.js
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.c3ce1ad33d9983e2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js
--rw-r--r--   0 runner    (1001) docker     (123)    33525 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js
--rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.3eb6beae8084d868.js
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.28bbfbd268843c68.js
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js
--rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.814579 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.814579 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)    81048 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.814579 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.814579 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.814579 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)    27023 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/connections.html
--rw-r--r--   0 runner    (1001) docker     (123)    35774 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17121 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.818579 featureform-1.7.3rc5/src/featureform/dashboard/out/static/
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/Capital_One_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/Kubernetes_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/Postgresql_elephant.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/Redis_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    61862 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/Snowflake_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/amazon-dynamoDB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/amazon_redshift.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/amazon_s3.svg
--rw-r--r--   0 runner    (1001) docker     (123)    26573 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/apache_cassandra.svg
--rw-r--r--   0 runner    (1001) docker     (123)    60161 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/apache_hadoop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/azure_storage_accounts.svg
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/google_bigquery.svg
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/google_cloud_storage.svg
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/google_firestore.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/logo192.png
--rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/logo512.png
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/mongoDB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-13 02:00:50.000000 featureform-1.7.3rc5/src/featureform/dashboard/out/static/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/dashboard_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    16410 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/get_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    19935 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/get_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/list_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    89078 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/local_dash_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.818579 featureform-1.7.3rc5/src/featureform/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-04-13 02:00:15.000000 featureform-1.7.3rc5/src/featureform/proto/metadata.proto
--rw-r--r--   0 runner    (1001) docker     (123)    23240 2023-04-13 02:00:17.000000 featureform-1.7.3rc5/src/featureform/proto/metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   102266 2023-04-13 02:00:17.000000 featureform-1.7.3rc5/src/featureform/proto/metadata_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-13 02:00:15.000000 featureform-1.7.3rc5/src/featureform/proto/serving.proto
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-13 02:00:16.000000 featureform-1.7.3rc5/src/featureform/proto/serving_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-13 02:00:16.000000 featureform-1.7.3rc5/src/featureform/proto/serving_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   154066 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/register_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    48878 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/search_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    32534 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/serving.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/serving_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    24494 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/sqlite_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/tls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/type_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/src/featureform/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.782579 featureform-1.7.3rc5/src/featureform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-13 02:00:56.000000 featureform-1.7.3rc5/src/featureform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32703 2023-04-13 02:00:56.000000 featureform-1.7.3rc5/src/featureform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 02:00:56.000000 featureform-1.7.3rc5/src/featureform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 02:00:56.000000 featureform-1.7.3rc5/src/featureform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-13 02:00:56.000000 featureform-1.7.3rc5/src/featureform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 02:00:56.000000 featureform-1.7.3rc5/src/featureform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:00:56.818579 featureform-1.7.3rc5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/tests/test_class_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/tests/test_executor_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/tests/test_getting_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/tests/test_localmode_include_label_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/tests/test_localmode_lag_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/tests/test_serving_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/tests/test_spark_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/tests/test_tags_and_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-13 01:59:42.000000 featureform-1.7.3rc5/tests/test_updating_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.870674 featureform-1.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-04-26 21:19:01.000000 featureform-1.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 21:19:01.000000 featureform-1.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-26 21:20:25.870674 featureform-1.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-26 21:19:01.000000 featureform-1.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-26 21:19:01.000000 featureform-1.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-26 21:20:25.870674 featureform-1.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.818674 featureform-1.7.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.822674 featureform-1.7.4/src/featureform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.818674 featureform-1.7.4/src/featureform/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.822674 featureform-1.7.4/src/featureform/dashboard/out/
+-rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.822674 featureform-1.7.4/src/featureform/dashboard/out/[type]/
+-rw-r--r--   0 runner    (1001) docker     (123)    17956 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/[type]/[entity].html
+-rw-r--r--   0 runner    (1001) docker     (123)    17188 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/[type].html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.818674 featureform-1.7.4/src/featureform/dashboard/out/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.818674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.822674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/8yA-hIcHsUSF2wPeJxwZa/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.822674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.850674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)    83561 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    74481 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21739 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   201393 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js
+-rw-r--r--   0 runner    (1001) docker     (123)   130270 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)   104027 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.854674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/404-baaca4b2f4acc755.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.854674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-b07f3c4463890639.js
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-751a928da9d524e9.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3583019 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/_app-a764893ff9420ec0.js
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/_error-3f70f2d61eb8c6dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/connections-1d67ba61869dece6.js
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/search-175858e61ba25631.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.854674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
+-rw-r--r--   0 runner    (1001) docker     (123)    35679 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.ab502da8667e6dc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.d1d39a9bd6ac45b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.42d8625dbbdd27ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.17a13e6bcda1e1f3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.ac01f4f7ac16a003.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.0e0594706d30fbd8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.2b3348708365f9ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.5e3fe34e0eab5fdb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.5d313969242bf8d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.bd5b619f107eee8f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.22a1c7ff76f01643.js
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.c3ce1ad33d9983e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33525 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.3eb6beae8084d868.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.28bbfbd268843c68.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.854674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.854674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    81048 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.854674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.854674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27046 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/connections.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35824 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.866675 featureform-1.7.4/src/featureform/dashboard/out/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/Capital_One_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/Kubernetes_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/Postgresql_elephant.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/Redis_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    61862 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/Snowflake_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/amazon-dynamoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/amazon_redshift.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/amazon_s3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26573 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/apache_cassandra.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    60161 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/apache_hadoop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/azure_storage_accounts.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/google_bigquery.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/google_cloud_storage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/google_firestore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/mongoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/dashboard_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16410 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/get_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19935 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/get_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/list_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89285 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/local_dash_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/local_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.866675 featureform-1.7.4/src/featureform/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-04-26 21:19:43.000000 featureform-1.7.4/src/featureform/proto/metadata.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    23763 2023-04-26 21:19:45.000000 featureform-1.7.4/src/featureform/proto/metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102266 2023-04-26 21:19:45.000000 featureform-1.7.4/src/featureform/proto/metadata_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-26 21:19:43.000000 featureform-1.7.4/src/featureform/proto/serving.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-26 21:19:44.000000 featureform-1.7.4/src/featureform/proto/serving_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-26 21:19:44.000000 featureform-1.7.4/src/featureform/proto/serving_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166823 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/register_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56884 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/search_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33912 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/serving.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/serving_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/sqlite_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/type_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.822674 featureform-1.7.4/src/featureform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-26 21:20:25.000000 featureform-1.7.4/src/featureform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32977 2023-04-26 21:20:25.000000 featureform-1.7.4/src/featureform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:20:25.000000 featureform-1.7.4/src/featureform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 21:20:25.000000 featureform-1.7.4/src/featureform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-26 21:20:25.000000 featureform-1.7.4/src/featureform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 21:20:25.000000 featureform-1.7.4/src/featureform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.870674 featureform-1.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_class_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_executor_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_getting_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_localmode_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_localmode_include_label_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_localmode_lag_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_ondemand_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_resource_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_serving_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_source_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_spark_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_tags_and_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_updating_provider.py
```

### Comparing `featureform-1.7.3rc5/LICENSE` & `featureform-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/PKG-INFO` & `featureform-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform
-Version: 1.7.3rc5
+Version: 1.7.4
 Summary: Package for the Featureform Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/embeddinghub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `featureform-1.7.3rc5/README.md` & `featureform-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/setup.cfg` & `featureform-1.7.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = featureform
-version = 1.7.3rc5
+version = 1.7.4
 author = FeatureForm, Inc.
 author_email = hello@featureform.com
 description = Package for the Featureform Feature Store
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://featureform.com
 project_urls = 
@@ -21,26 +21,29 @@
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	click>=7.1.2
 	protobuf>=3.20.0
 	typeguard<3.0.0
 	grpcio>=1.47.0
-	numpy==1.21.6
+	numpy>=1.21.6
 	pandas==1.3.5
 	pandasql>=0.7.3
 	typing_extensions>=4.1.1
 	dataclasses==0.6
 	flask==2.2.1
 	Flask-Cors==3.0.10
 	validators>=0.20.0
-	dill==0.3.5.1
+	dill>=0.3.6
 	pandasql==0.7.3
 	sqlalchemy<2.0.0
 	requests
+	rich
+	pyarrow
+	fastparquet
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	featureform = featureform.cli:cli
```

### Comparing `featureform-1.7.3rc5/src/featureform/cli.py` & `featureform-1.7.4/src/featureform/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import click
-from featureform import ResourceClient
+from .client import Client
 from .list import *
 from .get import *
 import os
 from flask import Flask
 from .dashboard_metadata import dashboard_app
 import validators
 import urllib.request
@@ -69,35 +69,37 @@
 
     elif host == None:
         host = os.getenv('FEATUREFORM_HOST')
         if host == None:
             raise ValueError(
                 "Host value must be set with --host flag or in env as FEATUREFORM_HOST")
 
-    rc = ResourceClient(host=host, local=local, insecure=insecure, cert_path=cert)
+    client = Client(host=host, local=local, insecure=insecure, cert_path=cert)
 
-    rc_get_functions_variant = {
-        "feature": rc.print_feature,
-        "label": rc.print_label,
-        "source": rc.print_source,
-        "trainingset": rc.print_training_set,
-        "training-set": rc.print_training_set
+    resource_get_functions_variant = {
+        "feature": client.print_feature,
+        "label": client.print_label,
+        "source": client.print_source,
+        "trainingset": client.print_training_set,
+        "training-set": client.print_training_set,
     }
 
-    rc_get_functions = {
-        "user": rc.get_user,
-        "model": rc.get_model,
-        "entity": rc.get_entity,
-        "provider": rc.get_provider
+    resource_get_functions = {
+        "user": client.get_user,
+        "model": client.get_model,
+        "entity": client.get_entity,
+        "provider": client.get_provider,
     }
 
-    if resource_type in rc_get_functions_variant:
-        rc_get_functions_variant[resource_type](name=name, variant=variant, local=local)
-    elif resource_type in rc_get_functions:
-        rc_get_functions[resource_type](name=name, local=local)
+    if resource_type in resource_get_functions_variant:
+        resource_get_functions_variant[resource_type](
+            name=name, variant=variant, local=local
+        )
+    elif resource_type in resource_get_functions:
+        resource_get_functions[resource_type](name=name, local=local)
     else:
         raise ValueError("Resource type not found")
 
 
 @cli.command()
 @click.option("--host",
               "host",
@@ -121,30 +123,30 @@
 
     elif host == None:
         host = os.getenv('FEATUREFORM_HOST')
         if host == None:
             raise ValueError(
                 "Host value must be set with --host flag or in env as FEATUREFORM_HOST")
 
-    rc = ResourceClient(host=host, local=local, insecure=insecure, cert_path=cert)
+    client = Client(host=host, local=local, insecure=insecure, cert_path=cert)
 
-    rc_list_functions = {
-        "features": rc.list_features,
-        "labels": rc.list_labels,
-        "sources": rc.list_sources,
-        "trainingsets": rc.list_training_sets,
-        "training-sets": rc.list_training_sets,
-        "users": rc.list_users,
-        "models": rc.list_models,
-        "entities": rc.list_entities,
-        "providers": rc.list_providers
+    resource_list_functions = {
+        "features": client.list_features,
+        "labels": client.list_labels,
+        "sources": client.list_sources,
+        "trainingsets": client.list_training_sets,
+        "training-sets": client.list_training_sets,
+        "users": client.list_users,
+        "models": client.list_models,
+        "entities": client.list_entities,
+        "providers": client.list_providers,
     }
 
-    if resource_type in rc_list_functions:
-        rc_list_functions[resource_type](local=local)
+    if resource_type in resource_list_functions:
+        resource_list_functions[resource_type](local=local)
     else:
         raise ValueError("Resource type not found")
 
 
 app = Flask(__name__)
 app.register_blueprint(dashboard_app)
 
@@ -169,26 +171,33 @@
               help="Disables TLS verification")
 @click.option("--local",
               is_flag=True,
               help="Enable local mode")
 @click.option("--dry-run",
               is_flag=True,
               help="Checks the definitions without applying them")
-def apply(host, cert, insecure, local, files, dry_run):
+@click.option("--no-wait",
+              is_flag=True,
+              help="Applies the resources asynchronously")
+def apply(host, cert, insecure, local, files, dry_run, no_wait):
     for file in files:
         if os.path.isfile(file):
             read_file(file)
         elif validators.url(file):
             read_url(file)
         else:
             raise ValueError(
                 f"Argument must be a path to a file or URL with a valid schema (http:// or https://): {file}")
 
-    rc = ResourceClient(host=host, local=local, insecure=insecure, cert_path=cert, dry_run=dry_run)
-    rc.apply()
+    client = Client(
+        host=host, local=local, insecure=insecure, cert_path=cert, dry_run=dry_run
+    )
+    asynchronous = no_wait
+    client.apply(asynchronous=asynchronous)
+
 
 @cli.command()
 @click.option("--query",
               "-q",
               "query",
               required=True,
               help="The phrase to search resources (e.g. 'quick').")
@@ -203,16 +212,16 @@
 @click.option("--insecure",
               is_flag=True,
               help="Disables TLS verification")
 @click.option("--local",
               is_flag=True,
               help="Enable local mode")
 def search(query, host, cert, insecure, local):
-    rc = ResourceClient(host=host, local=local, insecure=insecure, cert_path=cert)
-    results = rc.search(query, local)
+    client = Client(host=host, local=local, insecure=insecure, cert_path=cert)
+    results = client.search(query, local)
     if local:
         format_rows("NAME", "VARIANT", "TYPE")
         for r in results:
             desc = r["description"][:cutoff_length] + "..." if len(r["description"]) > 0 else ""
             format_rows(r["name"], r["variant"], r["resource_type"])
```

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/404.html` & `featureform-1.7.4/src/featureform/dashboard/out/404.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-01b1894ee40506d5.js" defer=""></script><script src="/_next/static/chunks/pages/404-baaca4b2f4acc755.js" defer=""></script><script src="/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_buildManifest.js" defer=""></script><script src="/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/404-baaca4b2f4acc755.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -560,8 +560,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>404</b></li></ol></nav></div><div><h1>404 Not Found :(</h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"tM9MEYWwbsEHYQ8l3Xl7G","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>404</b></li></ol></nav></div><div data-testid="notFoundId"><h1>404 Not Found :(</h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"8yA-hIcHsUSF2wPeJxwZa","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/[type]/[entity].html` & `featureform-1.7.4/src/featureform/dashboard/out/[type]/[entity].html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-01b1894ee40506d5.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-b07f3c4463890639.js" defer=""></script><script src="/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_buildManifest.js" defer=""></script><script src="/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-b07f3c4463890639.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -560,8 +560,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><a href="/[type]">[type]</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[entity]</b></li></ol></nav></div><div><div class="MuiContainer-root MuiContainer-maxWidthXl"><div class="MuiPaper-root MuiPaper-elevation3 MuiPaper-rounded"><div class="MuiContainer-root MuiContainer-maxWidthSm"><div aria-busy="true" class=""><svg width="40" height="40" viewBox="0 0 120 30" xmlns="http://www.w3.org/2000/svg" fill="grey" aria-label="audio-loading"><circle cx="15" cy="15" r="15"><animate attributeName="r" from="15" to="15" begin="0s" dur="0.8s" values="15;9;15" calcMode="linear" repeatCount="indefinite"></animate><animate attributeName="fillOpacity" from="1" to="1" begin="0s" dur="0.8s" values="1;.5;1" calcMode="linear" repeatCount="indefinite"></animate></circle><circle cx="60" cy="15" r="9" attributeName="fillOpacity" from="1" to="0.3"><animate attributeName="r" from="9" to="9" begin="0s" dur="0.8s" values="9;15;9" calcMode="linear" repeatCount="indefinite"></animate><animate attributeName="fillOpacity" from="0.5" to="0.5" begin="0s" dur="0.8s" values=".5;1;.5" calcMode="linear" repeatCount="indefinite"></animate></circle><circle cx="105" cy="15" r="15"><animate attributeName="r" from="15" to="15" begin="0s" dur="0.8s" values="15;9;15" calcMode="linear" repeatCount="indefinite"></animate><animate attributeName="fillOpacity" from="1" to="1" begin="0s" dur="0.8s" values="1;.5;1" calcMode="linear" repeatCount="indefinite"></animate></circle></svg></div></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"tM9MEYWwbsEHYQ8l3Xl7G","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><a href="/[type]">[type]</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[entity]</b></li></ol></nav></div><div><div data-testid="notFoundId"><h1>404 Not Found :(</h1></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"8yA-hIcHsUSF2wPeJxwZa","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

#### html2text {}

```diff
@@ -10,7 +10,8 @@
    4. .css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-
       select:none;user-select:none;width:1em;height:1em;display:inline-
       block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-
       shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1)
       0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:
       1.5rem;}
    5. [entity]
+****** 404 Not Found :( ******
```

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/[type].html` & `featureform-1.7.4/src/featureform/dashboard/out/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-01b1894ee40506d5.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-751a928da9d524e9.js" defer=""></script><script src="/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_buildManifest.js" defer=""></script><script src="/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/search-175858e61ba25631.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -306,14 +306,27 @@
   }
   .MuiPaper-elevation23 {
     box-shadow: 0px 11px 14px -7px rgba(0,0,0,0.2),0px 23px 36px 3px rgba(0,0,0,0.14),0px 9px 44px 8px rgba(0,0,0,0.12);
   }
   .MuiPaper-elevation24 {
     box-shadow: 0px 11px 15px -7px rgba(0,0,0,0.2),0px 24px 38px 3px rgba(0,0,0,0.14),0px 9px 46px 8px rgba(0,0,0,0.12);
   }
+  .MuiList-root {
+    margin: 0;
+    padding: 0;
+    position: relative;
+    list-style: none;
+  }
+  .MuiList-padding {
+    padding-top: 8px;
+    padding-bottom: 8px;
+  }
+  .MuiList-subheader {
+    padding-top: 0;
+  }
   .MuiToolbar-root {
     display: flex;
     position: relative;
     align-items: center;
   }
   .MuiToolbar-gutters {
     padding-left: 16px;
@@ -516,14 +529,35 @@
     font-size: 18px;
   }
   .jss14 {
     align-items: auto;
     margin-left: 0.2em;
     margin-right: 0.2em;
   }
+  .jss15 {
+    border: 2px solid #F5F6F7;
+    background: rgba(255, 255, 255, 1);
+    border-radius: 16px;
+  }
+  .jss16 {
+    color: black;
+    padding: 0;
+    background: transparent;
+    box-shadow: none;
+    padding-left: 32px;
+    padding-right: 32px;
+  }
+  .jss17 {
+    padding: 8px;
+    padding-top: 32px;
+  }
+  .jss18 {
+    display: inline;
+    line-height: 1.2;
+  }
   .jss2 {
     width: 100%;
     diplay: flex;
   }
   .jss3 {
     color: black;
     width: 100%;
@@ -560,8 +594,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[type]</b></li></ol></nav></div><div><div><h1>404 Not Found :(</h1></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"tM9MEYWwbsEHYQ8l3Xl7G","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Search</b></li></ol></nav></div><div><div><div class="MuiContainer-root jss15 MuiContainer-maxWidthXl"><h4 class="MuiTypography-root jss17 MuiTypography-h4" style="display:flex"><div style="color:gray">No results for: </div><b></b></h4><div><nav class="MuiList-root jss15 MuiList-padding"></nav></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"8yA-hIcHsUSF2wPeJxwZa","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -2,9 +2,9 @@
    1. Home
    2. .css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-
       select:none;user-select:none;width:1em;height:1em;display:inline-
       block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-
       shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1)
       0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:
       1.5rem;}
-   3. [type]
-****** 404 Not Found :( ******
+   3. Search
+No results for:Â
```

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/pages/_app-01b1894ee40506d5.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/_app-a764893ff9420ec0.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -87239,17 +87239,17 @@
                             marginLeft: "0.2em",
                             marginRight: "0.2em",
                             alignItems: "auto"
                         }
                     }
                 }),
                 y = function() {
-                    for (var a = x(), b = (0, r.useRouter)().asPath.split("/"); b.length > 0 && 0 === b[0].length;) b.shift();
+                    for (var a = x(), b = (0, r.useRouter)().asPath.split("?").shift().split("/"); b.length > 0 && 0 === b[0].length;) b.shift();
                     var c = function(a) {
-                            return a[0].toUpperCase() + a.slice(1).toLowerCase()
+                            return a ? a[0].toUpperCase() + a.slice(1).toLowerCase() : ""
                         },
                         d = function(a, b) {
                             return a + "/" + b
                         };
                     return (0, g.jsx)("div", {
                         className: a.root,
                         children: b.length > 0 ? (0, g.jsxs)(v.Z, {
@@ -87617,31 +87617,39 @@
                     b = ao(),
                     c = (0, E.Z)(h.useState(!1), 2),
                     d = c[0],
                     e = c[1],
                     f = (0, E.Z)(h.useState(null), 2),
                     i = f[0],
                     j = f[1];
-                return (0, h.useEffect)(function() {
+                (0, h.useEffect)(function() {
                     "/" !== a.pathname ? e(!0) : e(!1)
-                }, [a]), (0, g.jsx)("div", {
+                }, [a]);
+                var k = function(b) {
+                    null == b || b.preventDefault(), a.push("/")
+                };
+                return (0, g.jsx)("div", {
                     className: b.root,
                     children: (0, g.jsx)(al.Z, {
                         position: "static",
                         className: b.appbar,
                         children: (0, g.jsxs)(am.Z, {
                             className: b.toolbar,
                             children: [(0, g.jsx)("div", {
                                 className: b.title,
                                 children: (0, g.jsx)("img", {
                                     src: "/static/FeatureForm_Logo_Full_Black.svg",
                                     height: 30,
                                     alt: "Featureform",
+                                    onClick: k,
                                     component: "div",
                                     nowrap: "true",
+                                    style: {
+                                        cursor: "pointer"
+                                    },
                                     sx: {
                                         flexGrow: 1,
                                         display: {
                                             xs: "none",
                                             sm: "block"
                                         }
                                     }
@@ -87884,15 +87892,15 @@
             k = window.location.hostname, l = window.location.port;
             var m = "//" + k + ":" + l,
                 n = {
                     port: "7700",
                     host: k,
                     apiKey: ""
                 };
-            void 0 !== h.env.REACT_APP_API_URL && (m = h.env.REACT_APP_API_URL.trim());
+            h.env.REACT_APP_API_URL && (m = h.env.REACT_APP_API_URL.trim()), h.env.NEXT_PUBLIC_REACT_APP_API_URL && (m = h.env.NEXT_PUBLIC_REACT_APP_API_URL.trim());
             var o = m + "/prometheus";
             void 0 !== h.env.REACT_APP_PROMETHEUS_URL && (o = h.env.REACT_APP_PROMETHEUS_URL.trim());
             var p = function() {
                 function a() {
                     (0, d.Z)(this, a)
                 }
                 return (0, e.Z)(a, [{
@@ -88291,15 +88299,15 @@
                 };
             b.Z = k
         },
         75457: function(a, b, c) {
             "use strict";
             c.d(b, {
                 Z: function() {
-                    return aF
+                    return aG
                 }
             });
             var d = c(99534),
                 e = c(85893),
                 f = c(67294),
                 g = c(14416),
                 h = c(50462),
@@ -89421,15 +89429,15 @@
                                                 }), (0, e.jsx)(y.Z, {
                                                     variant: "outlined",
                                                     className: Q.linkChip,
                                                     size: "small",
                                                     onClick: X,
                                                     label: I.entity
                                                 })]
-                                            }), I.location && (0, e.jsxs)("div", {
+                                            }), I.location && !I["is-on-demand"] && (0, e.jsxs)("div", {
                                                 className: Q.linkBox,
                                                 children: [(0, e.jsxs)(r.Z, {
                                                     variant: "body1",
                                                     className: Q.typeTitle,
                                                     children: [(0, e.jsx)("b", {
                                                         children: "Columns:"
                                                     }), " "]
@@ -89439,14 +89447,29 @@
                                                         children: "Entity:"
                                                     }), " ", I.location.Entity, "\xa0", (0, e.jsx)("b", {
                                                         children: "Value:"
                                                     }), " ", I.location.Value, "\xa0", (0, e.jsx)("b", {
                                                         children: "Timestamp:"
                                                     }), " ", I.location.TS]
                                                 })]
+                                            }), I.location && I["is-on-demand"] && (0, e.jsxs)("div", {
+                                                className: Q.linkBox,
+                                                children: [(0, e.jsxs)(r.Z, {
+                                                    variant: "body1",
+                                                    className: Q.typeTitle,
+                                                    children: [(0, e.jsx)("b", {
+                                                        children: "Feature Variant Type:"
+                                                    }), " "]
+                                                }), (0, e.jsx)(y.Z, {
+                                                    variant: "outlined",
+                                                    className: Q.linkChip,
+                                                    size: "small",
+                                                    onClick: function() {},
+                                                    label: "On-Demand"
+                                                })]
                                             })]
                                         }), (null === (b = I.tags) || void 0 === b ? void 0 : b.length) > 0 && (0, e.jsx)(v.Z, {
                                             item: !0,
                                             xs: !0,
                                             children: (0, e.jsx)(O, {
                                                 attributes: I.tags,
                                                 title: "Tags"
@@ -89597,57 +89620,64 @@
                                 name: c,
                                 variant: d
                             }))
                         }
                     }
                 },
                 aD = function() {
-                    return (0, e.jsx)(w.Z, {
-                        maxWidth: "xl",
-                        children: (0, e.jsx)(az.Z, {
-                            elevation: 3,
-                            children: (0, e.jsx)(w.Z, {
-                                maxWidth: "sm",
-                                children: (0, e.jsx)(ay.Z, {
-                                    type: "ThreeDots",
-                                    color: "grey",
-                                    height: 40,
-                                    width: 40
+                    return (0, e.jsx)("div", {
+                        "data-testid": "loadingDotsId",
+                        children: (0, e.jsx)(w.Z, {
+                            maxWidth: "xl",
+                            children: (0, e.jsx)(az.Z, {
+                                elevation: 3,
+                                children: (0, e.jsx)(w.Z, {
+                                    maxWidth: "sm",
+                                    children: (0, e.jsx)(ay.Z, {
+                                        type: "ThreeDots",
+                                        color: "grey",
+                                        height: 40,
+                                        width: 40
+                                    })
                                 })
                             })
                         })
                     })
                 },
                 aE = function(a) {
+                    var b, c;
+                    return !(null == a ? void 0 : null === (b = a.resources) || void 0 === b ? void 0 : b.name) && !(null == a ? void 0 : null === (c = a.resources) || void 0 === c ? void 0 : c.type)
+                },
+                aF = function(a) {
                     var b, c = a.api,
                         g = a.entityPage,
                         h = a.activeVariants,
                         i = a.type,
                         j = a.entity,
                         k = (0, d.Z)(a, ["api", "entityPage", "activeVariants", "type", "entity"]),
                         l = ar.Z[ar.Z.pathToType[i]],
                         m = k.fetch;
                     return (0, f.useEffect)(function() {
-                        m(c, i, j)
+                        c && i && j && m(c, i, j)
                     }, [i, j]), (0, e.jsx)("div", {
-                        children: g.failed ? (0, e.jsx)(aB.Z, {}) : 0 === Object.keys(b = g).length && b.constructor === Object || g.loading ? (0, e.jsx)(aD, {}) : (0, e.jsx)(ax, {
+                        children: g.failed || !g.loading && aE(g) ? (0, e.jsx)(aB.Z, {}) : g.loading || 0 === Object.keys(b = g).length && b.constructor === Object ? (0, e.jsx)(aD, {}) : (0, e.jsx)(ax, {
                             entity: g,
                             setVariant: k.setVariant,
                             activeVariants: h,
                             typePath: i,
                             resourceType: l
                         })
                     })
                 },
-                aF = (0, g.$j)(function(a) {
+                aG = (0, g.$j)(function(a) {
                     return {
                         entityPage: a.entityPage,
                         activeVariants: a.selectedVariant
                     }
-                }, aC)(aE)
+                }, aC)(aF)
         },
         50462: function(a, b, c) {
             "use strict";
             c.d(b, {
                 H: function() {
                     return k
                 }
@@ -89956,14 +89986,15 @@
         },
         99520: function(a, b, c) {
             "use strict";
             var d = c(85893);
             c(67294);
             var e = function() {
                 return (0, d.jsx)("div", {
+                    "data-testid": "notFoundId",
                     children: (0, d.jsx)("h1", {
                         children: "404 Not Found :("
                     })
                 })
             };
             b.Z = e
         },
@@ -90908,15 +90939,15 @@
                     reducers: {
                         set: function(a, b) {
                             var c = b.payload,
                                 d = c.type,
                                 f = c.name,
                                 g = c.variant,
                                 h = d;
-                            void 0 !== e.Z.typeToName[d] && (h = e.Z.typeToName[d]), a[h][f] = g
+                            e.Z.typeToName[d] && (h = e.Z.typeToName[d]), a[h] && (a[h][f] = g)
                         }
                     }
                 }),
                 i = h.actions.set;
             b.ZP = h.reducer
         },
         7169: function(a, b, c) {
@@ -90927,18 +90958,17 @@
                 g = c(67294),
                 h = c(41120),
                 i = c(35117),
                 j = c(59693),
                 k = c(88995),
                 l = c(41749),
                 m = c(11163),
-                n = c.n(m),
-                o = c(43832),
-                p = c(41598),
-                q = (0, h.Z)(function(a) {
+                n = c(43832),
+                o = c(41598),
+                p = (0, h.Z)(function(a) {
                     return (0, i.Z)({
                         search: (0, d.Z)({
                             position: "relative",
                             borderRadius: a.shape.borderRadius,
                             backgroundColor: (0, j.Fq)(a.palette.common.white, .15),
                             "&:hover": {
                                 backgroundColor: (0, j.Fq)(a.palette.common.white, .25)
@@ -90992,64 +91022,73 @@
                             background: "transparent",
                             boxShadow: "none",
                             color: "black",
                             alignSelf: "center"
                         }
                     })
                 }),
-                r = function(a) {
-                    a.input, a.setQuery;
+                q = function(a) {
                     var b = a.homePage,
                         c = function(a) {
-                            n().push("/search?q=" + i)
-                        },
-                        d = q(),
-                        h = (0, e.Z)(g.useState(""), 2),
-                        i = h[0],
-                        j = h[1];
+                            a.preventDefault();
+                            var b = "/search?q=" + (null == j ? void 0 : j.trim());
+                            h.push(b)
+                        },
+                        d = p(),
+                        h = (0, m.useRouter)(),
+                        i = (0, e.Z)(g.useState(""), 2),
+                        j = i[0],
+                        q = i[1];
                     return (0, f.jsx)("div", {
                         className: d.search,
                         children: (0, f.jsx)(l.Z, {
                             container: !0,
                             item: !0,
                             justifyContent: "center",
                             direction: "row",
-                            children: (0, f.jsxs)(o.Z, {
+                            children: (0, f.jsxs)(n.Z, {
                                 className: d.border,
                                 children: [(0, f.jsx)("div", {
                                     className: d.searchIcon,
                                     children: (0, f.jsx)(k.Z, {})
-                                }), (0, f.jsx)(p.Z, {
+                                }), (0, f.jsx)(o.Z, {
                                     placeholder: "Search...",
                                     onChange: function(a) {
-                                        j(a.target.value)
+                                        var b, c = a.target.value;
+                                        if ("" === c) {
+                                            q(c);
+                                            return
+                                        }
+                                        var d = null !== (b = a.target.value) && void 0 !== b ? b : "";
+                                        d.trim() && q(d)
                                     },
-                                    defaultValue: "",
+                                    value: j,
                                     onKeyDown: function(a) {
-                                        return 13 === a.keyCode && i.length > 0 ? c(a) : ""
+                                        "Enter" === a.key && j && c(a)
                                     },
                                     classes: {
                                         root: d.inputRoot,
                                         input: b ? d.inputInputHome : d.inputTopBar
                                     },
                                     inputProps: {
-                                        "aria-label": "search "
+                                        "aria-label": "search",
+                                        "data-testid": "searchInputId"
                                     }
                                 })]
                             })
                         })
                     })
                 };
-            b.Z = r
+            b.Z = q
         },
         88277: function(a, b, c) {
             "use strict";
             c.d(b, {
                 Z: function() {
-                    return D
+                    return E
                 }
             });
             var d = c(99534),
                 e = c(85893),
                 f = c(67294),
                 g = c(14416),
                 h = c(26042),
@@ -91058,17 +91097,17 @@
                 k = c.n(j),
                 l = c(41120),
                 m = c(22318),
                 n = c(28889),
                 o = c(62822),
                 p = c(50998),
                 q = c(95757),
-                r = c(43832);
-            c(21286);
-            var s = c(11163);
+                r = c(43832),
+                s = c(21286),
+                t = c(11163);
             (function(a) {
                 var b = a.children,
                     c = a.value,
                     f = a.index,
                     g = (0, d.Z)(a, ["children", "value", "index"]);
                 return (0, e.jsx)("div", (0, i.Z)((0, h.Z)({
                     role: "tabpanel",
@@ -91082,15 +91121,15 @@
                     })
                 }))
             }).propTypes = {
                 children: k().node,
                 index: k().any.isRequired,
                 value: k().any.isRequired
             };
-            var t = (0, l.Z)(function(a) {
+            var u = (0, l.Z)(function(a) {
                     return {
                         root: {
                             borderRadius: 16,
                             background: "rgba(255, 255, 255, 1)",
                             border: "2px solid ".concat(a.palette.border.main)
                         },
                         appbar: {
@@ -91107,165 +91146,173 @@
                         },
                         resultTitle: {
                             display: "inline",
                             lineHeight: 1.2
                         }
                     }
                 }),
-                u = function(a) {
-                    var b = a.results,
-                        c = a.search_query,
-                        d = a.setVariant,
-                        f = t();
-                    return (0, e.jsx)("div", {
-                        children: (0, e.jsxs)(r.Z, {
-                            maxWidth: "xl",
-                            className: f.root,
-                            children: [(0, e.jsxs)(m.Z, {
-                                className: f.searchTitle,
-                                variant: "h4",
-                                style: {
-                                    display: "flex"
-                                },
-                                children: [b.length > 0 ? (0, e.jsx)("div", {
-                                    style: {
-                                        color: "gray"
-                                    },
-                                    children: "Results for:\xa0"
-                                }) : (0, e.jsx)("div", {
-                                    style: {
-                                        color: "gray"
-                                    },
-                                    children: "No results for:\xa0"
-                                }), (0, e.jsx)("b", {
-                                    children: c
-                                })]
-                            }), (0, e.jsx)(v, {
-                                contents: b,
-                                setVariant: d
-                            })]
-                        })
-                    })
-                },
                 v = function(a) {
                     var b = a.type,
                         c = a.contents,
                         d = a.setVariant,
-                        f = t(),
-                        g = {};
-                    console.log(c);
-                    var h = c.filter(function(a) {
+                        f = u(),
+                        g = {},
+                        h = [];
+                    return (null == c ? void 0 : c.length) && (h = c.filter(function(a) {
                         return !(a.Name + "." + a.Variant + "." + a.Type in g) && (g[a.Name + "." + a.Variant + "." + a.Type] = a.Variant, !0)
-                    });
-                    return (0, e.jsx)("div", {
+                    })), (0, e.jsx)("div", {
                         children: (0, e.jsx)(o.Z, {
                             className: f.root,
                             component: "nav",
                             children: h.map(function(a, c) {
-                                return (0, e.jsx)(w, {
+                                return (0, e.jsx)(x, {
                                     type: b,
                                     content: a,
                                     setVariant: d
                                 }, c)
                             })
                         })
                     })
                 },
-                w = function(a) {
-                    var b = a.type,
-                        c = a.content,
-                        d = a.setVariant,
-                        f = function(a) {
-                            resourceType.hasVariants && d(a.Type, a.Name, a.Variant), h.push(resourceType.urlPathResource(a.Name))
+                w = {
+                    FEATURE: "Feature",
+                    FEATURE_VARIANT: "Feature",
+                    LABEL: "Label",
+                    LABEL_VARIANT: "Label",
+                    TRAINING_SET: "TrainingSet",
+                    TRAINING_SET_VARIANT: "TrainingSet",
+                    SOURCE: "Source",
+                    SOURCE_VARIANT: "Source",
+                    PROVIDER: "Provider",
+                    ENTITY: "Entity",
+                    MODEL: "Model",
+                    USER: "User"
+                },
+                x = function(a) {
+                    a.type;
+                    var b = a.content,
+                        c = a.setVariant,
+                        d = function(a) {
+                            (null == h ? void 0 : h.hasVariants) && c(a.Type, a.Name, a.Variant), g.push(h.urlPathResource(a.Name))
                         },
-                        g = t(),
-                        h = (0, s.useRouter)();
-                    return console.log("content", c), console.log("type", b), console.log("found resource type"), (0, e.jsx)("div", {
+                        f = u(),
+                        g = (0, t.useRouter)(),
+                        h = s.Z[w[b.Type]];
+                    return (0, e.jsx)(e.Fragment, {
                         children: (0, e.jsx)(p.Z, {
                             button: !0,
                             alignItems: "flex-start",
+                            onClick: function() {
+                                return d(b)
+                            },
                             children: (0, e.jsx)(q.Z, {
                                 primary: (0, e.jsxs)("div", {
                                     children: [(0, e.jsxs)("div", {
                                         children: [(0, e.jsx)("div", {
-                                            className: g.resultTitle,
-                                            children: console.log("CLASS")
+                                            className: f.resultTitle
                                         }), (0, e.jsx)(m.Z, {
-                                            className: g.resultTitle,
+                                            className: f.resultTitle,
                                             variant: "h6",
-                                            children: c.Name
+                                            children: b.Name
                                         }), " "]
                                     }), (0, e.jsx)("div", {
                                         style: {
                                             width: "0.5em"
                                         },
                                         children: "   "
                                     }), (0, e.jsx)(m.Z, {
                                         style: {
                                             opacity: .5
                                         },
-                                        className: g.resultTitle,
+                                        className: f.resultTitle,
                                         variant: "body1",
-                                        children: c.Variant
+                                        children: b.Variant
                                     })]
-                                }),
-                                onClick: function() {
-                                    return f(c)
-                                }
+                                })
                             })
                         })
                     })
                 },
-                x = u,
-                y = c(75820),
-                z = c(93432),
-                A = function(a) {
+                y = function(a) {
+                    var b = a.results,
+                        c = a.search_query,
+                        d = a.setVariant,
+                        f = u();
+                    return (0, e.jsx)("div", {
+                        children: (0, e.jsxs)(r.Z, {
+                            maxWidth: "xl",
+                            className: f.root,
+                            children: [(0, e.jsxs)(m.Z, {
+                                className: f.searchTitle,
+                                variant: "h4",
+                                style: {
+                                    display: "flex"
+                                },
+                                children: [(null == b ? void 0 : b.length) > 0 ? (0, e.jsx)("div", {
+                                    style: {
+                                        color: "gray"
+                                    },
+                                    children: "Results for:\xa0"
+                                }) : (0, e.jsx)("div", {
+                                    style: {
+                                        color: "gray"
+                                    },
+                                    children: "No results for:\xa0"
+                                }), (0, e.jsx)("b", {
+                                    children: c
+                                })]
+                            }), (0, e.jsx)(v, {
+                                contents: b,
+                                setVariant: d
+                            })]
+                        })
+                    })
+                },
+                z = c(75820),
+                A = c(93432),
+                B = function(a) {
                     return {
                         fetch: function(b, c) {
-                            return a((0, y.on)({
+                            return a((0, z.on)({
                                 api: b,
                                 query: c
                             }))
                         },
                         setVariant: function(b, c, d) {
-                            a((0, z.jO)({
+                            a((0, A.jO)({
                                 type: b,
                                 name: c,
                                 variant: d
                             }))
                         }
                     }
                 },
-                B = function(a) {
+                C = function(a) {
                     var b, c = a.searchResults,
                         g = a.api,
                         h = a.setVariant,
                         i = (0, d.Z)(a, ["searchResults", "api", "setVariant"]),
-                        j = (b = (0, s.useRouter)(), new URLSearchParams(b.query)).get("q"),
+                        j = (b = (0, t.useRouter)(), new URLSearchParams(b.query)).get("q"),
                         k = i.fetch;
                     return (0, f.useEffect)(function() {
                         k(g, j)
                     }, [j, g, k]), (0, e.jsx)("div", {
-                        children: c.resources ? (0, e.jsxs)("div", {
-                            children: [console.log("blah", c.resources), (0, e.jsx)(x, {
-                                results: c.resources,
-                                search_query: j,
-                                setVariant: h
-                            })]
-                        }) : (0, e.jsx)("div", {
-                            children: "No Results"
+                        children: (0, e.jsx)(y, {
+                            results: null == c ? void 0 : c.resources,
+                            search_query: j,
+                            setVariant: h
                         })
                     })
                 },
-                C = function(a) {
+                D = function(a) {
                     return {
                         searchResults: a.searchResults
                     }
                 },
-                D = (0, g.$j)(C, A)(B)
+                E = (0, g.$j)(D, B)(C)
         },
         75820: function(a, b, c) {
             "use strict";
             c.d(b, {
                 on: function() {
                     return k
                 }
@@ -91278,16 +91325,16 @@
                 k = (0, j.hg)("searchResults/fetchSearch", (e = (0, f.Z)(i().mark(function a(b, c) {
                     var d, e, f, g;
                     return i().wrap(function(a) {
                         for (;;) switch (a.prev = a.next) {
                             case 0:
                                 return d = b.api, e = b.query, f = c.signal, a.next = 3, d.fetchSearch(e, f);
                             case 3:
-                                return g = a.sent, console.log("got search"), console.log(g), a.abrupt("return", g);
-                            case 7:
+                                return g = a.sent, a.abrupt("return", g);
+                            case 5:
                             case "end":
                                 return a.stop()
                         }
                     }, a)
                 })), function(a, b) {
                     return e.apply(this, arguments)
                 })),
```

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_buildManifest.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js` & `featureform-1.7.4/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/connections.html` & `featureform-1.7.4/src/featureform/dashboard/out/connections.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-01b1894ee40506d5.js" defer=""></script><script src="/_next/static/chunks/pages/connections-1d67ba61869dece6.js" defer=""></script><script src="/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_buildManifest.js" defer=""></script><script src="/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/connections-1d67ba61869dece6.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -1058,8 +1058,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Connections</b></li></ol></nav></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center MuiGrid-grid-lg-12"></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"tM9MEYWwbsEHYQ8l3Xl7G","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Connections</b></li></ol></nav></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center MuiGrid-grid-lg-12"></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"8yA-hIcHsUSF2wPeJxwZa","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/index.html` & `featureform-1.7.4/src/featureform/dashboard/out/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>Featureform Dashboard</title><meta name="next-head-count" content="3"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-01b1894ee40506d5.js" defer=""></script><script src="/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js" defer=""></script><script src="/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_buildManifest.js" defer=""></script><script src="/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>Featureform Dashboard</title><meta name="next-head-count" content="3"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -1456,8 +1456,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><div></div></div><div><div class="jss15"><div class="jss16"><div class="jss17"></div><div class="jss23"><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-justify-content-xs-center"><div class="MuiContainer-root jss25 MuiContainer-maxWidthLg"><div class="jss24"><svg class="MuiSvgIcon-root" focusable="false" viewBox="0 0 24 24" aria-hidden="true"><path d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"></path></svg></div><div class="MuiInputBase-root jss26"><input type="text" placeholder="Search..." value="" aria-label="search " class="MuiInputBase-input jss27"/></div></div></div></div></div><div class="jss20"><div class="jss21"><div class="jss19"><h5 class="MuiTypography-root MuiTypography-h5"></h5></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center"><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div></div></div></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"tM9MEYWwbsEHYQ8l3Xl7G","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><div></div></div><div><div class="jss15"><div class="jss16"><div class="jss17"></div><div class="jss23"><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-justify-content-xs-center"><div class="MuiContainer-root jss25 MuiContainer-maxWidthLg"><div class="jss24"><svg class="MuiSvgIcon-root" focusable="false" viewBox="0 0 24 24" aria-hidden="true"><path d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"></path></svg></div><div class="MuiInputBase-root jss26"><input type="text" placeholder="Search..." value="" aria-label="search" data-testid="searchInputId" class="MuiInputBase-input jss27"/></div></div></div></div></div><div class="jss20"><div class="jss21"><div class="jss19"><h5 class="MuiTypography-root MuiTypography-h5"></h5></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center"><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div></div></div></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"8yA-hIcHsUSF2wPeJxwZa","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/search.html` & `featureform-1.7.4/src/featureform/dashboard/out/[type].html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-01b1894ee40506d5.js" defer=""></script><script src="/_next/static/chunks/pages/search-175858e61ba25631.js" defer=""></script><script src="/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_buildManifest.js" defer=""></script><script src="/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-751a928da9d524e9.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -560,8 +560,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Search</b></li></ol></nav></div><div><div>No Results</div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"tM9MEYWwbsEHYQ8l3Xl7G","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[type]</b></li></ol></nav></div><div><div data-testid="notFoundId"><h1>404 Not Found :(</h1></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"8yA-hIcHsUSF2wPeJxwZa","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

#### html2text {}

```diff
@@ -2,9 +2,9 @@
    1. Home
    2. .css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-
       select:none;user-select:none;width:1em;height:1em;display:inline-
       block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-
       shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1)
       0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:
       1.5rem;}
-   3. Search
-No Results
+   3. [type]
+****** 404 Not Found :( ******
```

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/Apache_Spark_logo.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/Apache_Spark_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/Capital_One_logo.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/Capital_One_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/Featureform_logo_pink.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/Featureform_logo_pink.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/Kubernetes_logo.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/Kubernetes_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/Postgresql_elephant.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/Postgresql_elephant.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/Redis_Logo.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/Redis_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/Snowflake_Logo.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/Snowflake_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/amazon-dynamoDB.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/amazon-dynamoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/amazon_redshift.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/amazon_redshift.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/amazon_s3.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/amazon_s3.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/apache_cassandra.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/apache_cassandra.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/apache_hadoop.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/apache_hadoop.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/apple-touch-icon.png` & `featureform-1.7.4/src/featureform/dashboard/out/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/azure_storage_accounts.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/azure_storage_accounts.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/favicon.ico` & `featureform-1.7.4/src/featureform/dashboard/out/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/google_bigquery.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/google_bigquery.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/google_cloud_storage.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/google_cloud_storage.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/google_firestore.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/google_firestore.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/logo192.png` & `featureform-1.7.4/src/featureform/dashboard/out/static/logo192.png`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/logo512.png` & `featureform-1.7.4/src/featureform/dashboard/out/static/logo512.png`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/mongoDB.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/mongoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard/out/static/safari-pinned-tab.svg` & `featureform-1.7.4/src/featureform/dashboard/out/static/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/dashboard_metadata.py` & `featureform-1.7.4/src/featureform/dashboard_metadata.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/get.py` & `featureform-1.7.4/src/featureform/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,23 +79,27 @@
     except grpc._channel._MultiThreadedRendezvous:
         print(f"{resource_type} not found.")
 
 def get_feature_variant_info(stub, name, variant):
     searchNameVariant = metadata_pb2.NameVariant(name=name, variant=variant)
     try:
         for x in stub.GetFeatureVariants(iter([searchNameVariant])):
-            format_rows([("NAME: ", x.name), 
+            status = x.status.Status._enum_type.values[x.status.status].name
+            rows = [("NAME: ", x.name),
             ("VARIANT: ", x.variant), 
             ("TYPE:", x.type), 
             ("ENTITY:", x.entity),
             ("OWNER:", x.owner),
             ("DESCRIPTION:", x.description),
             ("PROVIDER:", x.provider),
             ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name)
-            ])
+            ]
+            if status == "FAILED":
+                rows.append(("ERROR: ", x.status.error_message))
+            format_rows(rows)
             format_tags_and_properties(x.tags, x.properties)
             format_pg("SOURCE: ")
             format_rows([("NAME", "VARIANT"), (x.source.name, x.source.variant)])
             format_pg("TRAINING SETS:")
             format_rows("NAME", "VARIANT")
             for t in x.trainingsets:
                 format_rows(t.name, t.variant)
@@ -104,22 +108,26 @@
     except grpc._channel._MultiThreadedRendezvous:
         print("Feature variant not found.")
 
 def get_label_variant_info(stub, name, variant):
     searchNameVariant = metadata_pb2.NameVariant(name=name, variant=variant)
     try:
         for x in stub.GetLabelVariants(iter([searchNameVariant])):
-            format_rows([("NAME: ", x.name),
+            status = x.status.Status._enum_type.values[x.status.status].name
+            rows = [("NAME: ", x.name),
             ("VARIANT: ", x.variant), 
             ("TYPE:", x.type), 
             ("ENTITY:", x.entity), 
             ("OWNER:", x.owner), 
             ("DESCRIPTION:", x.description),
             ("PROVIDER:", x.provider),
-            ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name)])
+            ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name)]
+            if status == "FAILED":
+                rows.append(("ERROR: ", x.status.error_message))
+            format_rows(rows)
             format_tags_and_properties(x.tags, x.properties)
             format_pg("SOURCE: ")
             format_rows([("NAME", "VARIANT"), (x.source.name, x.source.variant)])
             format_pg("TRAINING SETS:")
             format_rows("NAME", "VARIANT")
             for t in x.trainingsets:
                 format_rows(t.name, t.variant)
@@ -128,21 +136,25 @@
     except grpc._channel._MultiThreadedRendezvous:
         print("Label variant not found.")
 
 def get_source_variant_info(stub, name, variant):
     searchNameVariant = metadata_pb2.NameVariant(name=name, variant=variant)
     try:
         for x in stub.GetSourceVariants(iter([searchNameVariant])):
-            format_rows([("NAME: ", x.name),
+            status = x.status.Status._enum_type.values[x.status.status].name
+            rows = [("NAME: ", x.name),
             ("VARIANT: ", x.variant), 
             ("OWNER:", x.owner),
             ("DESCRIPTION:", x.description),
             ("PROVIDER:", x.provider),
             ("TABLE:", x.table),
-            ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name)])
+            ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name)]
+            if status == "FAILED":
+                rows.append(("ERROR: ", x.status.error_message))
+            format_rows(rows)
             format_tags_and_properties(x.tags, x.properties)
             format_pg("DEFINITION:")
             print("TRANSFORMATION")
             print(x.transformation.SQLTransformation.query)
             format_pg("SOURCES")
             format_rows("NAME", "VARIANT")
             for s in x.transformation.SQLTransformation.source:
@@ -166,20 +178,24 @@
     except grpc._channel._MultiThreadedRendezvous:
         print("Source variant not found.")
 
 def get_training_set_variant_info(stub, name, variant):
     searchNameVariant = metadata_pb2.NameVariant(name=name, variant=variant)
     try:
         for x in stub.GetTrainingSetVariants(iter([searchNameVariant])):
-            format_rows([("NAME: ", x.name),
+            status = x.status.Status._enum_type.values[x.status.status].name
+            rows = [("NAME: ", x.name),
             ("VARIANT: ", x.variant),
             ("OWNER:", x.owner),
             ("DESCRIPTION:", x.description),
             ("PROVIDER:", x.provider),
-            ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name)])
+            ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name)]
+            if status == "FAILED":
+                rows.append(("ERROR: ", x.status.error_message))
+            format_rows(rows)
             format_tags_and_properties(x.tags, x.properties)
             format_pg("LABEL: ")
             format_rows([("NAME", "VARIANT"), (x.label.name, x.label.variant)])
             format_pg("FEATURES:")
             format_rows("NAME", "VARIANT")
             for f in x.features:
                 format_rows(f.name, f.variant)
@@ -188,20 +204,24 @@
     except grpc._channel._MultiThreadedRendezvous:
         print("Training set variant not found.")
 
 def get_provider_info(stub, name):
     searchName = metadata_pb2.Name(name=name)
     try:
         for x in stub.GetProviders(iter([searchName])):
-            format_rows([("NAME: ", x.name),
+            status = x.status.Status._enum_type.values[x.status.status].name
+            rows = [("NAME: ", x.name),
             ("DESCRIPTION: ", x.description),
             ("TYPE: ", x.type),
             ("SOFTWARE: ", x.software),
             ("TEAM: ", x.team),
-            ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name)])
+            ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name)]
+            if status == "FAILED":
+                rows.append(("ERROR: ", x.status.error_message))
+            format_rows(rows)
             format_tags_and_properties(x.tags, x.properties)
             format_pg("SOURCES:")
             format_rows("NAME", "VARIANT")
             for s in x.sources:
                 format_rows(s.name, s.variant)
             format_pg("FEATURES:")
             format_rows("NAME", "VARIANT")
```

### Comparing `featureform-1.7.3rc5/src/featureform/get_local.py` & `featureform-1.7.4/src/featureform/get_local.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/get_test.py` & `featureform-1.7.4/src/featureform/get_test.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/list.py` & `featureform-1.7.4/src/featureform/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     format_rows("NAME", "VARIANT", "STATUS")
     res = sorted([received for received in stub_list_functions[resource_type][0](metadata_pb2.Empty())], key=lambda x:x.name)
     for f in res:
         for v in f.variants:
             searchNameVariant = metadata_pb2.NameVariant(name=f.name, variant=v)
             for x in stub_list_functions[resource_type][1](iter([searchNameVariant])):
                 if x.variant == f.default_variant:
-                    format_rows(f.name, f"{f.default_variant} (default)", f.status.Status._enum_type.values[f.status.status].name)
+                    format_rows(f.name, f"{f.default_variant} (default)", x.status.Status._enum_type.values[x.status.status].name)
                 else:
                     format_rows(x.name, x.variant, x.status.Status._enum_type.values[x.status.status].name)
     return res
 
 def list_name_variant_status_desc(stub, resource_type):
     stub_list_functions = {
         "source": [stub.ListSources, stub.GetSourceVariants],
@@ -63,11 +63,11 @@
     format_rows("NAME", "VARIANT", "STATUS", "DESCRIPTION")
     res = sorted([received for received in stub_list_functions[resource_type][0](metadata_pb2.Empty())], key=lambda x:x.name)
     for f in res:
         for v in f.variants:
             searchNameVariant = metadata_pb2.NameVariant(name=f.name, variant=v)
             for x in stub_list_functions[resource_type][1](iter([searchNameVariant])):
                 if x.variant == f.default_variant:
-                    format_rows(f.name, f"{f.default_variant} (default)", f.status.Status._enum_type.values[f.status.status].name, x.description)
+                    format_rows(f.name, f"{f.default_variant} (default)", x.status.Status._enum_type.values[x.status.status].name, x.description)
                 else:
                     format_rows(x.name, x.variant, x.status.Status._enum_type.values[x.status.status].name, x.description)
     return res
```

### Comparing `featureform-1.7.3rc5/src/featureform/list_local.py` & `featureform-1.7.4/src/featureform/list_local.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/list_test.py` & `featureform-1.7.4/src/featureform/list_test.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/local_dash_test.py` & `featureform-1.7.4/src/featureform/local_dash_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1972,16 +1972,20 @@
 
 
 def check_objs(path, test_obj, client):
     response = client.get(path)
     assert response.status == "200 OK"
     json_resource = json.loads(response.data.decode())
     removed_created_json = remove_keys(json_resource, ["created", "definition"])
-    print("++++++++++ ACTUAL", removed_created_json)
-    assert removed_created_json == test_obj
+    if isinstance(removed_created_json, dict):
+        assert test_obj == removed_created_json
+    elif isinstance(removed_created_json, list):
+        actual = {obj["name"]: obj for obj in removed_created_json}
+        expected = {obj["name"]: obj for obj in test_obj}
+        assert actual == expected
 
 
 def test_features(client):
     check_objs("/data/features", features, client)
 
 
 def test_labels(client):
```

### Comparing `featureform-1.7.3rc5/src/featureform/proto/metadata.proto` & `featureform-1.7.4/src/featureform/proto/metadata.proto`

 * *Files 4% similar despite different names*

```diff
@@ -139,33 +139,44 @@
 
 message Columns {
     string entity = 1;
     string value = 2;
     string ts = 3;
 }
 
+message PythonFunction {
+    bytes query = 1;
+}
+
+enum ComputationMode {
+    PRECOMPUTED = 0;
+    CLIENT_COMPUTED = 1;
+}
+
 message FeatureVariant {
     string name = 1;
     string variant = 2;
     NameVariant source = 3;
     string type = 4;
     string entity = 5;
     google.protobuf.Timestamp created = 6;
     string owner = 7;
     string description = 8;
     string provider = 9;
     ResourceStatus status = 10;
     repeated NameVariant trainingsets = 11;
     oneof location {
         Columns columns = 12;
+        PythonFunction function = 17;
     }
     google.protobuf.Timestamp last_updated = 13;
     string schedule = 14;
     Tags tags = 15;
     Properties properties = 16;
+    ComputationMode mode = 18;
 }
 
 message FeatureLag {
     string feature = 1;
     string variant = 2;
     string name = 3;
     google.protobuf.Duration lag = 4;
```

### Comparing `featureform-1.7.3rc5/src/featureform/proto/metadata_pb2.py` & `featureform-1.7.4/src/featureform/proto/metadata_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,28 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n featureform/proto/metadata.proto\x12\"featureform.serving.metadata.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\"\x14\n\x04Name\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xbc\x01\n\x0eResourceStatus\x12I\n\x06status\x18\x01 \x01(\x0e\x32\x39.featureform.serving.metadata.proto.ResourceStatus.Status\x12\x15\n\rerror_message\x18\x02 \x01(\t\"H\n\x06Status\x12\r\n\tNO_STATUS\x10\x00\x12\x0b\n\x07\x43REATED\x10\x01\x12\x0b\n\x07PENDING\x10\x02\x12\t\n\x05READY\x10\x03\x12\n\n\x06\x46\x41ILED\x10\x04\"\x98\x01\n\nResourceID\x12\x41\n\x08resource\x18\x01 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12G\n\rresource_type\x18\x02 \x01(\x0e\x32\x30.featureform.serving.metadata.proto.ResourceType\"\x9b\x01\n\x10SetStatusRequest\x12\x43\n\x0bresource_id\x18\x01 \x01(\x0b\x32..featureform.serving.metadata.proto.ResourceID\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\"n\n\x15ScheduleChangeRequest\x12\x43\n\x0bresource_id\x18\x01 \x01(\x0b\x32..featureform.serving.metadata.proto.ResourceID\x12\x10\n\x08schedule\x18\x02 \x01(\t\",\n\x0bNameVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\"\x07\n\x05\x45mpty\"\x86\x01\n\x07\x46\x65\x61ture\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"4\n\x07\x43olumns\x12\x0e\n\x06\x65ntity\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\n\n\x02ts\x18\x03 \x01(\t\"\x88\x05\n\x0e\x46\x65\x61tureVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12?\n\x06source\x18\x03 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x0e\n\x06\x65ntity\x18\x05 \x01(\t\x12+\n\x07\x63reated\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05owner\x18\x07 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12\x10\n\x08provider\x18\t \x01(\t\x12\x42\n\x06status\x18\n \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x45\n\x0ctrainingsets\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x07\x63olumns\x18\x0c \x01(\x0b\x32+.featureform.serving.metadata.proto.ColumnsH\x00\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x0e \x01(\t\x12\x36\n\x04tags\x18\x0f \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x10 \x01(\x0b\x32..featureform.serving.metadata.proto.PropertiesB\n\n\x08location\"d\n\nFeatureLag\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12&\n\x03lag\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\"\x84\x01\n\x05Label\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\xc2\x04\n\x0cLabelVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12?\n\x06source\x18\x05 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x0e\n\x06\x65ntity\x18\x06 \x01(\t\x12+\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05owner\x18\x08 \x01(\t\x12\x10\n\x08provider\x18\t \x01(\t\x12\x42\n\x06status\x18\n \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x45\n\x0ctrainingsets\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x07\x63olumns\x18\x0c \x01(\x0b\x32+.featureform.serving.metadata.proto.ColumnsH\x00\x12\x36\n\x04tags\x18\r \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x0e \x01(\x0b\x32..featureform.serving.metadata.proto.PropertiesB\n\n\x08location\"\xc3\x04\n\x08Provider\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08software\x18\x04 \x01(\t\x12\x0c\n\x04team\x18\x05 \x01(\t\x12\x19\n\x11serialized_config\x18\x06 \x01(\x0c\x12\x42\n\x06status\x18\x07 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12@\n\x07sources\x18\x08 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x41\n\x08\x66\x65\x61tures\x18\t \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\n \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x0c \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\r \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\x8a\x01\n\x0bTrainingSet\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\xe3\x04\n\x12TrainingSetVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12+\n\x07\x63reated\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08provider\x18\x06 \x01(\t\x12\x42\n\x06status\x18\x07 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x08 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x05label\x18\t \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x0e \x01(\t\x12\x44\n\x0c\x66\x65\x61ture_lags\x18\x0f \x03(\x0b\x32..featureform.serving.metadata.proto.FeatureLag\x12\x36\n\x04tags\x18\x10 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x11 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xb6\x03\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x42\n\x06status\x18\x03 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x06 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x07 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x08 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xf1\x02\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x41\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x06 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x07 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xe1\x03\n\x04User\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12@\n\x07sources\x18\x06 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x08 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\t \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\x85\x01\n\x06Source\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\x93\x06\n\rSourceVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12L\n\x0etransformation\x18\x0e \x01(\x0b\x32\x32.featureform.serving.metadata.proto.TransformationH\x00\x12\x46\n\x0bprimaryData\x18\x0f \x01(\x0b\x32/.featureform.serving.metadata.proto.PrimaryDataH\x00\x12\r\n\x05owner\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x10\n\x08provider\x18\x06 \x01(\t\x12+\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x06status\x18\x08 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\r\n\x05table\x18\t \x01(\t\x12\x45\n\x0ctrainingsets\x18\n \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x41\n\x08\x66\x65\x61tures\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x0c \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x10 \x01(\t\x12\x36\n\x04tags\x18\x11 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x12 \x01(\x0b\x32..featureform.serving.metadata.proto.PropertiesB\x0c\n\ndefinition\"\x95\x02\n\x0eTransformation\x12R\n\x11SQLTransformation\x18\x01 \x01(\x0b\x32\x35.featureform.serving.metadata.proto.SQLTransformationH\x00\x12P\n\x10\x44\x46Transformation\x18\x02 \x01(\x0b\x32\x34.featureform.serving.metadata.proto.DFTransformationH\x00\x12M\n\x0fkubernetes_args\x18\x03 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.KubernetesArgsH\x01\x42\x06\n\x04typeB\x06\n\x04\x61rgs\"o\n\x17KubernetesResourceSpecs\x12\x13\n\x0b\x63pu_request\x18\x01 \x01(\t\x12\x11\n\tcpu_limit\x18\x02 \x01(\t\x12\x16\n\x0ememory_request\x18\x03 \x01(\t\x12\x14\n\x0cmemory_limit\x18\x04 \x01(\t\"r\n\x0eKubernetesArgs\x12\x14\n\x0c\x64ocker_image\x18\x01 \x01(\t\x12J\n\x05specs\x18\x02 \x01(\x0b\x32;.featureform.serving.metadata.proto.KubernetesResourceSpecs\"c\n\x11SQLTransformation\x12\r\n\x05query\x18\x01 \x01(\t\x12?\n\x06source\x18\x02 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\"b\n\x10\x44\x46Transformation\x12\r\n\x05query\x18\x01 \x01(\x0c\x12?\n\x06inputs\x18\x02 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\"_\n\x0bPrimaryData\x12\x44\n\x05table\x18\x01 \x01(\x0b\x32\x33.featureform.serving.metadata.proto.PrimarySQLTableH\x00\x42\n\n\x08location\"\x1f\n\x0fPrimarySQLTable\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x13\n\x04Tags\x12\x0b\n\x03tag\x18\x01 \x03(\t\"+\n\x08Property\x12\x16\n\x0cstring_value\x18\x01 \x01(\tH\x00\x42\x07\n\x05value\"\xbb\x01\n\nProperties\x12N\n\x08property\x18\x01 \x03(\x0b\x32<.featureform.serving.metadata.proto.Properties.PropertyEntry\x1a]\n\rPropertyEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12;\n\x05value\x18\x02 \x01(\x0b\x32,.featureform.serving.metadata.proto.Property:\x02\x38\x01*\xc9\x01\n\x0cResourceType\x12\x0b\n\x07\x46\x45\x41TURE\x10\x00\x12\t\n\x05LABEL\x10\x01\x12\x10\n\x0cTRAINING_SET\x10\x02\x12\n\n\x06SOURCE\x10\x03\x12\x13\n\x0f\x46\x45\x41TURE_VARIANT\x10\x04\x12\x11\n\rLABEL_VARIANT\x10\x05\x12\x18\n\x14TRAINING_SET_VARIANT\x10\x06\x12\x12\n\x0eSOURCE_VARIANT\x10\x07\x12\x0c\n\x08PROVIDER\x10\x08\x12\n\n\x06\x45NTITY\x10\t\x12\t\n\x05MODEL\x10\n\x12\x08\n\x04USER\x10\x0b\x32\x88\x1a\n\x08Metadata\x12h\n\x0cListFeatures\x12).featureform.serving.metadata.proto.Empty\x1a+.featureform.serving.metadata.proto.Feature0\x01\x12u\n\x14\x43reateFeatureVariant\x12\x32.featureform.serving.metadata.proto.FeatureVariant\x1a).featureform.serving.metadata.proto.Empty\x12h\n\x0bGetFeatures\x12(.featureform.serving.metadata.proto.Name\x1a+.featureform.serving.metadata.proto.Feature(\x01\x30\x01\x12}\n\x12GetFeatureVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x32.featureform.serving.metadata.proto.FeatureVariant(\x01\x30\x01\x12\x64\n\nListLabels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Label0\x01\x12q\n\x12\x43reateLabelVariant\x12\x30.featureform.serving.metadata.proto.LabelVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x64\n\tGetLabels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Label(\x01\x30\x01\x12y\n\x10GetLabelVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x30.featureform.serving.metadata.proto.LabelVariant(\x01\x30\x01\x12p\n\x10ListTrainingSets\x12).featureform.serving.metadata.proto.Empty\x1a/.featureform.serving.metadata.proto.TrainingSet0\x01\x12}\n\x18\x43reateTrainingSetVariant\x12\x36.featureform.serving.metadata.proto.TrainingSetVariant\x1a).featureform.serving.metadata.proto.Empty\x12p\n\x0fGetTrainingSets\x12(.featureform.serving.metadata.proto.Name\x1a/.featureform.serving.metadata.proto.TrainingSet(\x01\x30\x01\x12\x85\x01\n\x16GetTrainingSetVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x36.featureform.serving.metadata.proto.TrainingSetVariant(\x01\x30\x01\x12\x66\n\x0bListSources\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Source0\x01\x12s\n\x13\x43reateSourceVariant\x12\x31.featureform.serving.metadata.proto.SourceVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x66\n\nGetSources\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Source(\x01\x30\x01\x12{\n\x11GetSourceVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x31.featureform.serving.metadata.proto.SourceVariant(\x01\x30\x01\x12\x62\n\tListUsers\x12).featureform.serving.metadata.proto.Empty\x1a(.featureform.serving.metadata.proto.User0\x01\x12\x61\n\nCreateUser\x12(.featureform.serving.metadata.proto.User\x1a).featureform.serving.metadata.proto.Empty\x12\x62\n\x08GetUsers\x12(.featureform.serving.metadata.proto.Name\x1a(.featureform.serving.metadata.proto.User(\x01\x30\x01\x12j\n\rListProviders\x12).featureform.serving.metadata.proto.Empty\x1a,.featureform.serving.metadata.proto.Provider0\x01\x12i\n\x0e\x43reateProvider\x12,.featureform.serving.metadata.proto.Provider\x1a).featureform.serving.metadata.proto.Empty\x12j\n\x0cGetProviders\x12(.featureform.serving.metadata.proto.Name\x1a,.featureform.serving.metadata.proto.Provider(\x01\x30\x01\x12g\n\x0cListEntities\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Entity0\x01\x12\x65\n\x0c\x43reateEntity\x12*.featureform.serving.metadata.proto.Entity\x1a).featureform.serving.metadata.proto.Empty\x12g\n\x0bGetEntities\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Entity(\x01\x30\x01\x12\x64\n\nListModels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Model0\x01\x12\x63\n\x0b\x43reateModel\x12).featureform.serving.metadata.proto.Model\x1a).featureform.serving.metadata.proto.Empty\x12\x64\n\tGetModels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Model(\x01\x30\x01\x12t\n\x11SetResourceStatus\x12\x34.featureform.serving.metadata.proto.SetStatusRequest\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x15RequestScheduleChange\x12\x39.featureform.serving.metadata.proto.ScheduleChangeRequest\x1a).featureform.serving.metadata.proto.Empty2\x8d\x19\n\x03\x41pi\x12\x61\n\nCreateUser\x12(.featureform.serving.metadata.proto.User\x1a).featureform.serving.metadata.proto.Empty\x12i\n\x0e\x43reateProvider\x12,.featureform.serving.metadata.proto.Provider\x1a).featureform.serving.metadata.proto.Empty\x12s\n\x13\x43reateSourceVariant\x12\x31.featureform.serving.metadata.proto.SourceVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x65\n\x0c\x43reateEntity\x12*.featureform.serving.metadata.proto.Entity\x1a).featureform.serving.metadata.proto.Empty\x12u\n\x14\x43reateFeatureVariant\x12\x32.featureform.serving.metadata.proto.FeatureVariant\x1a).featureform.serving.metadata.proto.Empty\x12q\n\x12\x43reateLabelVariant\x12\x30.featureform.serving.metadata.proto.LabelVariant\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x18\x43reateTrainingSetVariant\x12\x36.featureform.serving.metadata.proto.TrainingSetVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x63\n\x0b\x43reateModel\x12).featureform.serving.metadata.proto.Model\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x15RequestScheduleChange\x12\x39.featureform.serving.metadata.proto.ScheduleChangeRequest\x1a).featureform.serving.metadata.proto.Empty\x12\x62\n\x08GetUsers\x12(.featureform.serving.metadata.proto.Name\x1a(.featureform.serving.metadata.proto.User(\x01\x30\x01\x12h\n\x0bGetFeatures\x12(.featureform.serving.metadata.proto.Name\x1a+.featureform.serving.metadata.proto.Feature(\x01\x30\x01\x12}\n\x12GetFeatureVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x32.featureform.serving.metadata.proto.FeatureVariant(\x01\x30\x01\x12\x64\n\tGetLabels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Label(\x01\x30\x01\x12y\n\x10GetLabelVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x30.featureform.serving.metadata.proto.LabelVariant(\x01\x30\x01\x12p\n\x0fGetTrainingSets\x12(.featureform.serving.metadata.proto.Name\x1a/.featureform.serving.metadata.proto.TrainingSet(\x01\x30\x01\x12\x85\x01\n\x16GetTrainingSetVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x36.featureform.serving.metadata.proto.TrainingSetVariant(\x01\x30\x01\x12\x66\n\nGetSources\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Source(\x01\x30\x01\x12{\n\x11GetSourceVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x31.featureform.serving.metadata.proto.SourceVariant(\x01\x30\x01\x12j\n\x0cGetProviders\x12(.featureform.serving.metadata.proto.Name\x1a,.featureform.serving.metadata.proto.Provider(\x01\x30\x01\x12g\n\x0bGetEntities\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Entity(\x01\x30\x01\x12\x64\n\tGetModels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Model(\x01\x30\x01\x12h\n\x0cListFeatures\x12).featureform.serving.metadata.proto.Empty\x1a+.featureform.serving.metadata.proto.Feature0\x01\x12\x64\n\nListLabels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Label0\x01\x12p\n\x10ListTrainingSets\x12).featureform.serving.metadata.proto.Empty\x1a/.featureform.serving.metadata.proto.TrainingSet0\x01\x12\x66\n\x0bListSources\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Source0\x01\x12\x62\n\tListUsers\x12).featureform.serving.metadata.proto.Empty\x1a(.featureform.serving.metadata.proto.User0\x01\x12j\n\rListProviders\x12).featureform.serving.metadata.proto.Empty\x1a,.featureform.serving.metadata.proto.Provider0\x01\x12g\n\x0cListEntities\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Entity0\x01\x12\x64\n\nListModels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Model0\x01\x42\'Z%github.com/featureform/metadata/protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n featureform/proto/metadata.proto\x12\"featureform.serving.metadata.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\"\x14\n\x04Name\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xbc\x01\n\x0eResourceStatus\x12I\n\x06status\x18\x01 \x01(\x0e\x32\x39.featureform.serving.metadata.proto.ResourceStatus.Status\x12\x15\n\rerror_message\x18\x02 \x01(\t\"H\n\x06Status\x12\r\n\tNO_STATUS\x10\x00\x12\x0b\n\x07\x43REATED\x10\x01\x12\x0b\n\x07PENDING\x10\x02\x12\t\n\x05READY\x10\x03\x12\n\n\x06\x46\x41ILED\x10\x04\"\x98\x01\n\nResourceID\x12\x41\n\x08resource\x18\x01 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12G\n\rresource_type\x18\x02 \x01(\x0e\x32\x30.featureform.serving.metadata.proto.ResourceType\"\x9b\x01\n\x10SetStatusRequest\x12\x43\n\x0bresource_id\x18\x01 \x01(\x0b\x32..featureform.serving.metadata.proto.ResourceID\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\"n\n\x15ScheduleChangeRequest\x12\x43\n\x0bresource_id\x18\x01 \x01(\x0b\x32..featureform.serving.metadata.proto.ResourceID\x12\x10\n\x08schedule\x18\x02 \x01(\t\",\n\x0bNameVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\"\x07\n\x05\x45mpty\"\x86\x01\n\x07\x46\x65\x61ture\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"4\n\x07\x43olumns\x12\x0e\n\x06\x65ntity\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\n\n\x02ts\x18\x03 \x01(\t\"\x1f\n\x0ePythonFunction\x12\r\n\x05query\x18\x01 \x01(\x0c\"\x93\x06\n\x0e\x46\x65\x61tureVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12?\n\x06source\x18\x03 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x0e\n\x06\x65ntity\x18\x05 \x01(\t\x12+\n\x07\x63reated\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05owner\x18\x07 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12\x10\n\x08provider\x18\t \x01(\t\x12\x42\n\x06status\x18\n \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x45\n\x0ctrainingsets\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x07\x63olumns\x18\x0c \x01(\x0b\x32+.featureform.serving.metadata.proto.ColumnsH\x00\x12\x46\n\x08\x66unction\x18\x11 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.PythonFunctionH\x00\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x0e \x01(\t\x12\x36\n\x04tags\x18\x0f \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x10 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\x12\x41\n\x04mode\x18\x12 \x01(\x0e\x32\x33.featureform.serving.metadata.proto.ComputationModeB\n\n\x08location\"d\n\nFeatureLag\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12&\n\x03lag\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\"\x84\x01\n\x05Label\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\xc2\x04\n\x0cLabelVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12?\n\x06source\x18\x05 \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x0e\n\x06\x65ntity\x18\x06 \x01(\t\x12+\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05owner\x18\x08 \x01(\t\x12\x10\n\x08provider\x18\t \x01(\t\x12\x42\n\x06status\x18\n \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x45\n\x0ctrainingsets\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x07\x63olumns\x18\x0c \x01(\x0b\x32+.featureform.serving.metadata.proto.ColumnsH\x00\x12\x36\n\x04tags\x18\r \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x0e \x01(\x0b\x32..featureform.serving.metadata.proto.PropertiesB\n\n\x08location\"\xc3\x04\n\x08Provider\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08software\x18\x04 \x01(\t\x12\x0c\n\x04team\x18\x05 \x01(\t\x12\x19\n\x11serialized_config\x18\x06 \x01(\x0c\x12\x42\n\x06status\x18\x07 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12@\n\x07sources\x18\x08 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x41\n\x08\x66\x65\x61tures\x18\t \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\n \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x0c \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\r \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\x8a\x01\n\x0bTrainingSet\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\xe3\x04\n\x12TrainingSetVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12+\n\x07\x63reated\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08provider\x18\x06 \x01(\t\x12\x42\n\x06status\x18\x07 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x08 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12>\n\x05label\x18\t \x01(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x0e \x01(\t\x12\x44\n\x0c\x66\x65\x61ture_lags\x18\x0f \x03(\x0b\x32..featureform.serving.metadata.proto.FeatureLag\x12\x36\n\x04tags\x18\x10 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x11 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xb6\x03\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x42\n\x06status\x18\x03 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x06 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x07 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x08 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xf1\x02\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x41\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x06 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x07 \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\xe1\x03\n\x04User\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x41\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x04 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x45\n\x0ctrainingsets\x18\x05 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12@\n\x07sources\x18\x06 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x36\n\x04tags\x18\x08 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\t \x01(\x0b\x32..featureform.serving.metadata.proto.Properties\"\x85\x01\n\x06Source\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x42\n\x06status\x18\x02 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\x17\n\x0f\x64\x65\x66\x61ult_variant\x18\x03 \x01(\t\x12\x10\n\x08variants\x18\x04 \x03(\t\"\x93\x06\n\rSourceVariant\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07variant\x18\x02 \x01(\t\x12L\n\x0etransformation\x18\x0e \x01(\x0b\x32\x32.featureform.serving.metadata.proto.TransformationH\x00\x12\x46\n\x0bprimaryData\x18\x0f \x01(\x0b\x32/.featureform.serving.metadata.proto.PrimaryDataH\x00\x12\r\n\x05owner\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x10\n\x08provider\x18\x06 \x01(\t\x12+\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x06status\x18\x08 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.ResourceStatus\x12\r\n\x05table\x18\t \x01(\t\x12\x45\n\x0ctrainingsets\x18\n \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x41\n\x08\x66\x65\x61tures\x18\x0b \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12?\n\x06labels\x18\x0c \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\x12\x30\n\x0clast_updated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08schedule\x18\x10 \x01(\t\x12\x36\n\x04tags\x18\x11 \x01(\x0b\x32(.featureform.serving.metadata.proto.Tags\x12\x42\n\nproperties\x18\x12 \x01(\x0b\x32..featureform.serving.metadata.proto.PropertiesB\x0c\n\ndefinition\"\x95\x02\n\x0eTransformation\x12R\n\x11SQLTransformation\x18\x01 \x01(\x0b\x32\x35.featureform.serving.metadata.proto.SQLTransformationH\x00\x12P\n\x10\x44\x46Transformation\x18\x02 \x01(\x0b\x32\x34.featureform.serving.metadata.proto.DFTransformationH\x00\x12M\n\x0fkubernetes_args\x18\x03 \x01(\x0b\x32\x32.featureform.serving.metadata.proto.KubernetesArgsH\x01\x42\x06\n\x04typeB\x06\n\x04\x61rgs\"o\n\x17KubernetesResourceSpecs\x12\x13\n\x0b\x63pu_request\x18\x01 \x01(\t\x12\x11\n\tcpu_limit\x18\x02 \x01(\t\x12\x16\n\x0ememory_request\x18\x03 \x01(\t\x12\x14\n\x0cmemory_limit\x18\x04 \x01(\t\"r\n\x0eKubernetesArgs\x12\x14\n\x0c\x64ocker_image\x18\x01 \x01(\t\x12J\n\x05specs\x18\x02 \x01(\x0b\x32;.featureform.serving.metadata.proto.KubernetesResourceSpecs\"c\n\x11SQLTransformation\x12\r\n\x05query\x18\x01 \x01(\t\x12?\n\x06source\x18\x02 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\"b\n\x10\x44\x46Transformation\x12\r\n\x05query\x18\x01 \x01(\x0c\x12?\n\x06inputs\x18\x02 \x03(\x0b\x32/.featureform.serving.metadata.proto.NameVariant\"_\n\x0bPrimaryData\x12\x44\n\x05table\x18\x01 \x01(\x0b\x32\x33.featureform.serving.metadata.proto.PrimarySQLTableH\x00\x42\n\n\x08location\"\x1f\n\x0fPrimarySQLTable\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x13\n\x04Tags\x12\x0b\n\x03tag\x18\x01 \x03(\t\"+\n\x08Property\x12\x16\n\x0cstring_value\x18\x01 \x01(\tH\x00\x42\x07\n\x05value\"\xbb\x01\n\nProperties\x12N\n\x08property\x18\x01 \x03(\x0b\x32<.featureform.serving.metadata.proto.Properties.PropertyEntry\x1a]\n\rPropertyEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12;\n\x05value\x18\x02 \x01(\x0b\x32,.featureform.serving.metadata.proto.Property:\x02\x38\x01*\xc9\x01\n\x0cResourceType\x12\x0b\n\x07\x46\x45\x41TURE\x10\x00\x12\t\n\x05LABEL\x10\x01\x12\x10\n\x0cTRAINING_SET\x10\x02\x12\n\n\x06SOURCE\x10\x03\x12\x13\n\x0f\x46\x45\x41TURE_VARIANT\x10\x04\x12\x11\n\rLABEL_VARIANT\x10\x05\x12\x18\n\x14TRAINING_SET_VARIANT\x10\x06\x12\x12\n\x0eSOURCE_VARIANT\x10\x07\x12\x0c\n\x08PROVIDER\x10\x08\x12\n\n\x06\x45NTITY\x10\t\x12\t\n\x05MODEL\x10\n\x12\x08\n\x04USER\x10\x0b*7\n\x0f\x43omputationMode\x12\x0f\n\x0bPRECOMPUTED\x10\x00\x12\x13\n\x0f\x43LIENT_COMPUTED\x10\x01\x32\x88\x1a\n\x08Metadata\x12h\n\x0cListFeatures\x12).featureform.serving.metadata.proto.Empty\x1a+.featureform.serving.metadata.proto.Feature0\x01\x12u\n\x14\x43reateFeatureVariant\x12\x32.featureform.serving.metadata.proto.FeatureVariant\x1a).featureform.serving.metadata.proto.Empty\x12h\n\x0bGetFeatures\x12(.featureform.serving.metadata.proto.Name\x1a+.featureform.serving.metadata.proto.Feature(\x01\x30\x01\x12}\n\x12GetFeatureVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x32.featureform.serving.metadata.proto.FeatureVariant(\x01\x30\x01\x12\x64\n\nListLabels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Label0\x01\x12q\n\x12\x43reateLabelVariant\x12\x30.featureform.serving.metadata.proto.LabelVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x64\n\tGetLabels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Label(\x01\x30\x01\x12y\n\x10GetLabelVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x30.featureform.serving.metadata.proto.LabelVariant(\x01\x30\x01\x12p\n\x10ListTrainingSets\x12).featureform.serving.metadata.proto.Empty\x1a/.featureform.serving.metadata.proto.TrainingSet0\x01\x12}\n\x18\x43reateTrainingSetVariant\x12\x36.featureform.serving.metadata.proto.TrainingSetVariant\x1a).featureform.serving.metadata.proto.Empty\x12p\n\x0fGetTrainingSets\x12(.featureform.serving.metadata.proto.Name\x1a/.featureform.serving.metadata.proto.TrainingSet(\x01\x30\x01\x12\x85\x01\n\x16GetTrainingSetVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x36.featureform.serving.metadata.proto.TrainingSetVariant(\x01\x30\x01\x12\x66\n\x0bListSources\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Source0\x01\x12s\n\x13\x43reateSourceVariant\x12\x31.featureform.serving.metadata.proto.SourceVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x66\n\nGetSources\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Source(\x01\x30\x01\x12{\n\x11GetSourceVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x31.featureform.serving.metadata.proto.SourceVariant(\x01\x30\x01\x12\x62\n\tListUsers\x12).featureform.serving.metadata.proto.Empty\x1a(.featureform.serving.metadata.proto.User0\x01\x12\x61\n\nCreateUser\x12(.featureform.serving.metadata.proto.User\x1a).featureform.serving.metadata.proto.Empty\x12\x62\n\x08GetUsers\x12(.featureform.serving.metadata.proto.Name\x1a(.featureform.serving.metadata.proto.User(\x01\x30\x01\x12j\n\rListProviders\x12).featureform.serving.metadata.proto.Empty\x1a,.featureform.serving.metadata.proto.Provider0\x01\x12i\n\x0e\x43reateProvider\x12,.featureform.serving.metadata.proto.Provider\x1a).featureform.serving.metadata.proto.Empty\x12j\n\x0cGetProviders\x12(.featureform.serving.metadata.proto.Name\x1a,.featureform.serving.metadata.proto.Provider(\x01\x30\x01\x12g\n\x0cListEntities\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Entity0\x01\x12\x65\n\x0c\x43reateEntity\x12*.featureform.serving.metadata.proto.Entity\x1a).featureform.serving.metadata.proto.Empty\x12g\n\x0bGetEntities\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Entity(\x01\x30\x01\x12\x64\n\nListModels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Model0\x01\x12\x63\n\x0b\x43reateModel\x12).featureform.serving.metadata.proto.Model\x1a).featureform.serving.metadata.proto.Empty\x12\x64\n\tGetModels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Model(\x01\x30\x01\x12t\n\x11SetResourceStatus\x12\x34.featureform.serving.metadata.proto.SetStatusRequest\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x15RequestScheduleChange\x12\x39.featureform.serving.metadata.proto.ScheduleChangeRequest\x1a).featureform.serving.metadata.proto.Empty2\x8d\x19\n\x03\x41pi\x12\x61\n\nCreateUser\x12(.featureform.serving.metadata.proto.User\x1a).featureform.serving.metadata.proto.Empty\x12i\n\x0e\x43reateProvider\x12,.featureform.serving.metadata.proto.Provider\x1a).featureform.serving.metadata.proto.Empty\x12s\n\x13\x43reateSourceVariant\x12\x31.featureform.serving.metadata.proto.SourceVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x65\n\x0c\x43reateEntity\x12*.featureform.serving.metadata.proto.Entity\x1a).featureform.serving.metadata.proto.Empty\x12u\n\x14\x43reateFeatureVariant\x12\x32.featureform.serving.metadata.proto.FeatureVariant\x1a).featureform.serving.metadata.proto.Empty\x12q\n\x12\x43reateLabelVariant\x12\x30.featureform.serving.metadata.proto.LabelVariant\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x18\x43reateTrainingSetVariant\x12\x36.featureform.serving.metadata.proto.TrainingSetVariant\x1a).featureform.serving.metadata.proto.Empty\x12\x63\n\x0b\x43reateModel\x12).featureform.serving.metadata.proto.Model\x1a).featureform.serving.metadata.proto.Empty\x12}\n\x15RequestScheduleChange\x12\x39.featureform.serving.metadata.proto.ScheduleChangeRequest\x1a).featureform.serving.metadata.proto.Empty\x12\x62\n\x08GetUsers\x12(.featureform.serving.metadata.proto.Name\x1a(.featureform.serving.metadata.proto.User(\x01\x30\x01\x12h\n\x0bGetFeatures\x12(.featureform.serving.metadata.proto.Name\x1a+.featureform.serving.metadata.proto.Feature(\x01\x30\x01\x12}\n\x12GetFeatureVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x32.featureform.serving.metadata.proto.FeatureVariant(\x01\x30\x01\x12\x64\n\tGetLabels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Label(\x01\x30\x01\x12y\n\x10GetLabelVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x30.featureform.serving.metadata.proto.LabelVariant(\x01\x30\x01\x12p\n\x0fGetTrainingSets\x12(.featureform.serving.metadata.proto.Name\x1a/.featureform.serving.metadata.proto.TrainingSet(\x01\x30\x01\x12\x85\x01\n\x16GetTrainingSetVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x36.featureform.serving.metadata.proto.TrainingSetVariant(\x01\x30\x01\x12\x66\n\nGetSources\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Source(\x01\x30\x01\x12{\n\x11GetSourceVariants\x12/.featureform.serving.metadata.proto.NameVariant\x1a\x31.featureform.serving.metadata.proto.SourceVariant(\x01\x30\x01\x12j\n\x0cGetProviders\x12(.featureform.serving.metadata.proto.Name\x1a,.featureform.serving.metadata.proto.Provider(\x01\x30\x01\x12g\n\x0bGetEntities\x12(.featureform.serving.metadata.proto.Name\x1a*.featureform.serving.metadata.proto.Entity(\x01\x30\x01\x12\x64\n\tGetModels\x12(.featureform.serving.metadata.proto.Name\x1a).featureform.serving.metadata.proto.Model(\x01\x30\x01\x12h\n\x0cListFeatures\x12).featureform.serving.metadata.proto.Empty\x1a+.featureform.serving.metadata.proto.Feature0\x01\x12\x64\n\nListLabels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Label0\x01\x12p\n\x10ListTrainingSets\x12).featureform.serving.metadata.proto.Empty\x1a/.featureform.serving.metadata.proto.TrainingSet0\x01\x12\x66\n\x0bListSources\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Source0\x01\x12\x62\n\tListUsers\x12).featureform.serving.metadata.proto.Empty\x1a(.featureform.serving.metadata.proto.User0\x01\x12j\n\rListProviders\x12).featureform.serving.metadata.proto.Empty\x1a,.featureform.serving.metadata.proto.Provider0\x01\x12g\n\x0cListEntities\x12).featureform.serving.metadata.proto.Empty\x1a*.featureform.serving.metadata.proto.Entity0\x01\x12\x64\n\nListModels\x12).featureform.serving.metadata.proto.Empty\x1a).featureform.serving.metadata.proto.Model0\x01\x42\'Z%github.com/featureform/metadata/protob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'featureform.proto.metadata_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z%github.com/featureform/metadata/proto'
   _PROPERTIES_PROPERTYENTRY._options = None
   _PROPERTIES_PROPERTYENTRY._serialized_options = b'8\001'
-  _RESOURCETYPE._serialized_start=7147
-  _RESOURCETYPE._serialized_end=7348
+  _RESOURCETYPE._serialized_start=7319
+  _RESOURCETYPE._serialized_end=7520
+  _COMPUTATIONMODE._serialized_start=7522
+  _COMPUTATIONMODE._serialized_end=7577
   _NAME._serialized_start=137
   _NAME._serialized_end=157
   _RESOURCESTATUS._serialized_start=160
   _RESOURCESTATUS._serialized_end=348
   _RESOURCESTATUS_STATUS._serialized_start=276
   _RESOURCESTATUS_STATUS._serialized_end=348
   _RESOURCEID._serialized_start=351
@@ -43,58 +45,60 @@
   _NAMEVARIANT._serialized_end=819
   _EMPTY._serialized_start=821
   _EMPTY._serialized_end=828
   _FEATURE._serialized_start=831
   _FEATURE._serialized_end=965
   _COLUMNS._serialized_start=967
   _COLUMNS._serialized_end=1019
-  _FEATUREVARIANT._serialized_start=1022
-  _FEATUREVARIANT._serialized_end=1670
-  _FEATURELAG._serialized_start=1672
-  _FEATURELAG._serialized_end=1772
-  _LABEL._serialized_start=1775
-  _LABEL._serialized_end=1907
-  _LABELVARIANT._serialized_start=1910
-  _LABELVARIANT._serialized_end=2488
-  _PROVIDER._serialized_start=2491
-  _PROVIDER._serialized_end=3070
-  _TRAININGSET._serialized_start=3073
-  _TRAININGSET._serialized_end=3211
-  _TRAININGSETVARIANT._serialized_start=3214
-  _TRAININGSETVARIANT._serialized_end=3825
-  _ENTITY._serialized_start=3828
-  _ENTITY._serialized_end=4266
-  _MODEL._serialized_start=4269
-  _MODEL._serialized_end=4638
-  _USER._serialized_start=4641
-  _USER._serialized_end=5122
-  _SOURCE._serialized_start=5125
-  _SOURCE._serialized_end=5258
-  _SOURCEVARIANT._serialized_start=5261
-  _SOURCEVARIANT._serialized_end=6048
-  _TRANSFORMATION._serialized_start=6051
-  _TRANSFORMATION._serialized_end=6328
-  _KUBERNETESRESOURCESPECS._serialized_start=6330
-  _KUBERNETESRESOURCESPECS._serialized_end=6441
-  _KUBERNETESARGS._serialized_start=6443
-  _KUBERNETESARGS._serialized_end=6557
-  _SQLTRANSFORMATION._serialized_start=6559
-  _SQLTRANSFORMATION._serialized_end=6658
-  _DFTRANSFORMATION._serialized_start=6660
-  _DFTRANSFORMATION._serialized_end=6758
-  _PRIMARYDATA._serialized_start=6760
-  _PRIMARYDATA._serialized_end=6855
-  _PRIMARYSQLTABLE._serialized_start=6857
-  _PRIMARYSQLTABLE._serialized_end=6888
-  _TAGS._serialized_start=6890
-  _TAGS._serialized_end=6909
-  _PROPERTY._serialized_start=6911
-  _PROPERTY._serialized_end=6954
-  _PROPERTIES._serialized_start=6957
-  _PROPERTIES._serialized_end=7144
-  _PROPERTIES_PROPERTYENTRY._serialized_start=7051
-  _PROPERTIES_PROPERTYENTRY._serialized_end=7144
-  _METADATA._serialized_start=7351
-  _METADATA._serialized_end=10687
-  _API._serialized_start=10690
-  _API._serialized_end=13903
+  _PYTHONFUNCTION._serialized_start=1021
+  _PYTHONFUNCTION._serialized_end=1052
+  _FEATUREVARIANT._serialized_start=1055
+  _FEATUREVARIANT._serialized_end=1842
+  _FEATURELAG._serialized_start=1844
+  _FEATURELAG._serialized_end=1944
+  _LABEL._serialized_start=1947
+  _LABEL._serialized_end=2079
+  _LABELVARIANT._serialized_start=2082
+  _LABELVARIANT._serialized_end=2660
+  _PROVIDER._serialized_start=2663
+  _PROVIDER._serialized_end=3242
+  _TRAININGSET._serialized_start=3245
+  _TRAININGSET._serialized_end=3383
+  _TRAININGSETVARIANT._serialized_start=3386
+  _TRAININGSETVARIANT._serialized_end=3997
+  _ENTITY._serialized_start=4000
+  _ENTITY._serialized_end=4438
+  _MODEL._serialized_start=4441
+  _MODEL._serialized_end=4810
+  _USER._serialized_start=4813
+  _USER._serialized_end=5294
+  _SOURCE._serialized_start=5297
+  _SOURCE._serialized_end=5430
+  _SOURCEVARIANT._serialized_start=5433
+  _SOURCEVARIANT._serialized_end=6220
+  _TRANSFORMATION._serialized_start=6223
+  _TRANSFORMATION._serialized_end=6500
+  _KUBERNETESRESOURCESPECS._serialized_start=6502
+  _KUBERNETESRESOURCESPECS._serialized_end=6613
+  _KUBERNETESARGS._serialized_start=6615
+  _KUBERNETESARGS._serialized_end=6729
+  _SQLTRANSFORMATION._serialized_start=6731
+  _SQLTRANSFORMATION._serialized_end=6830
+  _DFTRANSFORMATION._serialized_start=6832
+  _DFTRANSFORMATION._serialized_end=6930
+  _PRIMARYDATA._serialized_start=6932
+  _PRIMARYDATA._serialized_end=7027
+  _PRIMARYSQLTABLE._serialized_start=7029
+  _PRIMARYSQLTABLE._serialized_end=7060
+  _TAGS._serialized_start=7062
+  _TAGS._serialized_end=7081
+  _PROPERTY._serialized_start=7083
+  _PROPERTY._serialized_end=7126
+  _PROPERTIES._serialized_start=7129
+  _PROPERTIES._serialized_end=7316
+  _PROPERTIES_PROPERTYENTRY._serialized_start=7223
+  _PROPERTIES_PROPERTYENTRY._serialized_end=7316
+  _METADATA._serialized_start=7580
+  _METADATA._serialized_end=10916
+  _API._serialized_start=10919
+  _API._serialized_end=14132
 # @@protoc_insertion_point(module_scope)
```

### Comparing `featureform-1.7.3rc5/src/featureform/proto/metadata_pb2_grpc.py` & `featureform-1.7.4/src/featureform/proto/metadata_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/proto/serving.proto` & `featureform-1.7.4/src/featureform/proto/serving.proto`

 * *Files 6% similar despite different names*

```diff
@@ -57,9 +57,10 @@
         string str_value = 1;
         int32 int_value = 2;
         float float_value = 3;
         double double_value = 4;
         int64  int64_value = 5;
         int32  int32_value = 6;
         bool   bool_value = 7;
+        bytes on_demand_function = 8;
     }
 }
```

### Comparing `featureform-1.7.3rc5/src/featureform/proto/serving_pb2.py` & `featureform-1.7.4/src/featureform/proto/serving_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66\x65\x61tureform/proto/serving.proto\x12\x19\x66\x65\x61tureform.serving.proto\"\x15\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\"}\n\x13TrainingDataRequest\x12\x35\n\x02id\x18\x01 \x01(\x0b\x32).featureform.serving.proto.TrainingDataID\x12/\n\x05model\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Model\"/\n\x0eTrainingDataID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"v\n\x0fTrainingDataRow\x12\x32\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\x12/\n\x05label\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Value\"\xb3\x01\n\x13\x46\x65\x61tureServeRequest\x12\x36\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32$.featureform.serving.proto.FeatureID\x12\x33\n\x08\x65ntities\x18\x02 \x03(\x0b\x32!.featureform.serving.proto.Entity\x12/\n\x05model\x18\x03 \x01(\x0b\x32 .featureform.serving.proto.Model\">\n\nFeatureRow\x12\x30\n\x06values\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\"*\n\tFeatureID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"%\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xad\x01\n\x05Value\x12\x13\n\tstr_value\x18\x01 \x01(\tH\x00\x12\x13\n\tint_value\x18\x02 \x01(\x05H\x00\x12\x15\n\x0b\x66loat_value\x18\x03 \x01(\x02H\x00\x12\x16\n\x0c\x64ouble_value\x18\x04 \x01(\x01H\x00\x12\x15\n\x0bint64_value\x18\x05 \x01(\x03H\x00\x12\x15\n\x0bint32_value\x18\x06 \x01(\x05H\x00\x12\x14\n\nbool_value\x18\x07 \x01(\x08H\x00\x42\x07\n\x05value2\xe2\x01\n\x07\x46\x65\x61ture\x12n\n\x0cTrainingData\x12..featureform.serving.proto.TrainingDataRequest\x1a*.featureform.serving.proto.TrainingDataRow\"\x00\x30\x01\x12g\n\x0c\x46\x65\x61tureServe\x12..featureform.serving.proto.FeatureServeRequest\x1a%.featureform.serving.proto.FeatureRow\"\x00\x42\x1eZ\x1cgithub.com/featureform/protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66\x65\x61tureform/proto/serving.proto\x12\x19\x66\x65\x61tureform.serving.proto\"\x15\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\"}\n\x13TrainingDataRequest\x12\x35\n\x02id\x18\x01 \x01(\x0b\x32).featureform.serving.proto.TrainingDataID\x12/\n\x05model\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Model\"/\n\x0eTrainingDataID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"v\n\x0fTrainingDataRow\x12\x32\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\x12/\n\x05label\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Value\"\xb3\x01\n\x13\x46\x65\x61tureServeRequest\x12\x36\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32$.featureform.serving.proto.FeatureID\x12\x33\n\x08\x65ntities\x18\x02 \x03(\x0b\x32!.featureform.serving.proto.Entity\x12/\n\x05model\x18\x03 \x01(\x0b\x32 .featureform.serving.proto.Model\">\n\nFeatureRow\x12\x30\n\x06values\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\"*\n\tFeatureID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"%\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xcb\x01\n\x05Value\x12\x13\n\tstr_value\x18\x01 \x01(\tH\x00\x12\x13\n\tint_value\x18\x02 \x01(\x05H\x00\x12\x15\n\x0b\x66loat_value\x18\x03 \x01(\x02H\x00\x12\x16\n\x0c\x64ouble_value\x18\x04 \x01(\x01H\x00\x12\x15\n\x0bint64_value\x18\x05 \x01(\x03H\x00\x12\x15\n\x0bint32_value\x18\x06 \x01(\x05H\x00\x12\x14\n\nbool_value\x18\x07 \x01(\x08H\x00\x12\x1c\n\x12on_demand_function\x18\x08 \x01(\x0cH\x00\x42\x07\n\x05value2\xe2\x01\n\x07\x46\x65\x61ture\x12n\n\x0cTrainingData\x12..featureform.serving.proto.TrainingDataRequest\x1a*.featureform.serving.proto.TrainingDataRow\"\x00\x30\x01\x12g\n\x0c\x46\x65\x61tureServe\x12..featureform.serving.proto.FeatureServeRequest\x1a%.featureform.serving.proto.FeatureRow\"\x00\x42\x1eZ\x1cgithub.com/featureform/protob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'featureform.proto.serving_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\034github.com/featureform/proto'
@@ -34,11 +34,11 @@
   _FEATUREROW._serialized_start=563
   _FEATUREROW._serialized_end=625
   _FEATUREID._serialized_start=627
   _FEATUREID._serialized_end=669
   _ENTITY._serialized_start=671
   _ENTITY._serialized_end=708
   _VALUE._serialized_start=711
-  _VALUE._serialized_end=884
-  _FEATURE._serialized_start=887
-  _FEATURE._serialized_end=1113
+  _VALUE._serialized_end=914
+  _FEATURE._serialized_start=917
+  _FEATURE._serialized_end=1143
 # @@protoc_insertion_point(module_scope)
```

### Comparing `featureform-1.7.3rc5/src/featureform/proto/serving_pb2_grpc.py` & `featureform-1.7.4/src/featureform/proto/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/register.py` & `featureform-1.7.4/src/featureform/register.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,238 +1,185 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
-
 from os.path import exists
 from datetime import timedelta
 from typeguard import typechecked
 from typing import Dict, Tuple, Callable, List, Union
+import warnings
+import inspect
 
 import dill
 import pandas as pd
 
 from .get import *
 from .list import *
 from .get_local import *
 from .list_local import *
 from .sqlite_metadata import SQLiteMetadata
 from .tls import insecure_channel, secure_channel
-from .resources import (
-    ColumnTypes,
-    Model,
-    ResourceState,
-    Provider,
-    RedisConfig,
-    FirestoreConfig,
-    CassandraConfig,
-    DynamodbConfig,
-    MongoDBConfig,
-    PostgresConfig,
-    SnowflakeConfig,
-    LocalConfig,
-    RedshiftConfig,
-    BigQueryConfig,
-    SparkConfig,
-    AzureFileStoreConfig,
-    OnlineBlobConfig,
-    K8sConfig,
-    S3StoreConfig,
-    GCSFileStoreConfig,
-    User,
-    Location,
-    Source,
-    PrimaryData,
-    SQLTable,
-    SQLTransformation,
-    DFTransformation,
-    Entity,
-    Feature,
-    Label,
-    ResourceColumnMapping,
-    TrainingSet,
-    ProviderReference,
-    EntityReference,
-    SourceReference,
-    ExecutorCredentials,
-    ResourceRedefinedError,
-    ResourceStatus,
-    Transformation,
-    K8sArgs,
-    AWSCredentials,
-    GCPCredentials,
-    HDFSConfig,
-    K8sResourceSpecs,
-    FilePrefix,
-)
+from .resources import ColumnTypes, Model, ResourceState, Provider, RedisConfig, FirestoreConfig, CassandraConfig, DynamodbConfig, \
+    MongoDBConfig, PostgresConfig, SnowflakeConfig, LocalConfig, RedshiftConfig, BigQueryConfig, SparkConfig, \
+    AzureFileStoreConfig, OnlineBlobConfig, K8sConfig, S3StoreConfig, GCSFileStoreConfig, User, Location, Source, PrimaryData, SQLTable, \
+    SQLTransformation, DFTransformation, Entity, Feature, Label, ResourceColumnMapping, TrainingSet, ProviderReference, \
+    EntityReference, SourceReference, ExecutorCredentials, ResourceRedefinedError, ResourceStatus, Transformation, \
+    K8sArgs, AWSCredentials, GCPCredentials, HDFSConfig, K8sResourceSpecs, FilePrefix, OnDemandFeature
 
 from .proto import metadata_pb2_grpc as ff_grpc
 from .search_local import search_local
 from .search import search
+from .enums import FileFormat
 
 NameVariant = Tuple[str, str]
 
 s3_config = S3StoreConfig("", "", AWSCredentials("id", "secret"))
 NON_INFERENCE_STORES = [s3_config.type()]
 
 
 class EntityRegistrar:
+
     def __init__(self, registrar, entity):
         self.__registrar = registrar
         self.__entity = entity
 
     def name(self) -> str:
         return self.__entity.name
 
 
 class UserRegistrar:
+
     def __init__(self, registrar, user):
         self.__registrar = registrar
         self.__user = user
 
     def name(self) -> str:
         return self.__user.name
 
     def make_default_owner(self):
         self.__registrar.set_default_owner(self.name())
 
 
 class OfflineProvider:
+
     def __init__(self, registrar, provider):
         self.__registrar = registrar
         self.__provider = provider
 
     def name(self) -> str:
         return self.__provider.name
 
 
 class OfflineSQLProvider(OfflineProvider):
+
     def __init__(self, registrar, provider):
         super().__init__(registrar, provider)
         self.__registrar = registrar
         self.__provider = provider
 
-    def register_table(
-        self,
-        name: str,
-        table: str,
-        variant: str = "default",
-        owner: Union[str, UserRegistrar] = "",
-        description: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_table(self,
+                       name: str,
+                       table: str,
+                       variant: str = "default",
+                       owner: Union[str, UserRegistrar] = "",
+                       description: str = "",
+                       tags: List[str] = [],
+                       properties: dict = {}):
         """Register a SQL table as a primary data source.
 
         Args:
             name (str): Name of table to be registered
             variant (str): Name of variant to be registered
             table (str): Name of SQL table
             owner (Union[str, UserRegistrar]): Owner
             description (str): Description of table to be registered
 
         Returns:
             source (ColumnSourceRegistrar): source
         """
-        return self.__registrar.register_primary_data(
-            name=name,
-            variant=variant,
-            location=SQLTable(table),
-            owner=owner,
-            provider=self.name(),
-            description=description,
-            tags=tags,
-            properties=properties,
-        )
-
-    def sql_transformation(
-        self,
-        owner: Union[str, UserRegistrar] = "",
-        variant: str = "default",
-        name: str = "",
-        schedule: str = "",
-        description: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
-        return self.__registrar.sql_transformation(
-            name=name,
-            variant=variant,
-            owner=owner,
-            schedule=schedule,
-            provider=self.name(),
-            description=description,
-            tags=tags,
-            properties=properties,
-        )
+        return self.__registrar.register_primary_data(name=name,
+                                                      variant=variant,
+                                                      location=SQLTable(table),
+                                                      owner=owner,
+                                                      provider=self.name(),
+                                                      description=description,
+                                                      tags=tags,
+                                                      properties=properties)
+
+    def sql_transformation(self,
+                           owner: Union[str, UserRegistrar] = "",
+                           variant: str = "default",
+                           name: str = "",
+                           schedule: str = "",
+                           description: str = "",
+                           tags: List[str] = [],
+                           properties: dict = {}):
+        return self.__registrar.sql_transformation(name=name,
+                                                   variant=variant,
+                                                   owner=owner,
+                                                   schedule=schedule,
+                                                   provider=self.name(),
+                                                   description=description,
+                                                   tags=tags,
+                                                   properties=properties)
 
 
 class OfflineSparkProvider(OfflineProvider):
     def __init__(self, registrar, provider):
         super().__init__(registrar, provider)
         self.__registrar = registrar
         self.__provider = provider
 
-    def register_file(
-        self,
-        name: str,
-        file_path: str,
-        variant: str = "default",
-        owner: Union[str, UserRegistrar] = "",
-        description: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_file(self,
+                        name: str,
+                        file_path: str,
+                        variant: str = "default",
+                        owner: Union[str, UserRegistrar] = "",
+                        description: str = "",
+                        tags: List[str] = [],
+                        properties: dict = {}):
         """Register a Spark data source as a primary data source.
 
         Args:
             name (str): Name of table to be registered
             variant (str): Name of variant to be registered
             file_path (str): The path to file
             owner (Union[str, UserRegistrar]): Owner
             description (str): Description of table to be registered
 
         Returns:
             source (ColumnSourceRegistrar): source
         """
-        return self.__registrar.register_primary_data(
-            name=name,
-            variant=variant,
-            location=SQLTable(file_path),
-            owner=owner,
-            provider=self.name(),
-            description=description,
-            tags=tags,
-            properties=properties,
-        )
-
-    def register_parquet_file(
-        self,
-        name: str,
-        file_path: str,
-        variant: str = "default",
-        owner: Union[str, UserRegistrar] = "",
-        description: str = "",
-    ):
-        if self.__provider.config.executor_type != "EMR" and file_path.startswith(
-            FilePrefix.S3.value
-        ):
+        return self.__registrar.register_primary_data(name=name,
+                                                      variant=variant,
+                                                      location=SQLTable(file_path),
+                                                      owner=owner,
+                                                      provider=self.name(),
+                                                      description=description,
+                                                      tags=tags,
+                                                      properties=properties)
+    
+    def register_parquet_file(self,
+                              name: str,
+                              file_path: str,
+                              variant: str = "default",
+                              owner: Union[str, UserRegistrar] = "",
+                              description: str = "", ):
+        if self.__provider.config.executor_type != "EMR" and file_path.startswith(FilePrefix.S3.value):
             file_path = file_path.replace(FilePrefix.S3.value, FilePrefix.S3A.value)
 
         return self.register_file(name, file_path, variant, owner, description)
 
-    def sql_transformation(
-        self,
-        variant: str,
-        owner: Union[str, UserRegistrar] = "",
-        name: str = "",
-        schedule: str = "",
-        description: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def sql_transformation(self,
+                           variant: str = "default",
+                           owner: Union[str, UserRegistrar] = "",
+                           name: str = "",
+                           schedule: str = "",
+                           description: str = "",
+                           tags: List[str] = [],
+                           properties: dict = {}):
         """
         Register a SQL transformation source. The spark.sql_transformation decorator takes the returned string in the
         following function and executes it as a SQL Query.
 
         The name of the function is the name of the resulting source.
 
         Sources for the transformation can be specified by adding the Name and Variant in brackets '{{ name.variant }}'.
@@ -252,123 +199,111 @@
             owner (Union[str, UserRegistrar]): Owner
             description (str): Description of primary data to be registered
 
 
         Returns:
             source (ColumnSourceRegistrar): Source
         """
-        return self.__registrar.sql_transformation(
-            name=name,
-            variant=variant,
-            owner=owner,
-            schedule=schedule,
-            provider=self.name(),
-            description=description,
-            tags=tags,
-            properties=properties,
-        )
-
-    def df_transformation(
-        self,
-        variant: str = "default",
-        owner: Union[str, UserRegistrar] = "",
-        name: str = "",
-        description: str = "",
-        inputs: list = [],
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+        return self.__registrar.sql_transformation(name=name,
+                                                   variant=variant,
+                                                   owner=owner,
+                                                   schedule=schedule,
+                                                   provider=self.name(),
+                                                   description=description,
+                                                   tags=tags,
+                                                   properties=properties)
+
+    def df_transformation(self,
+                          variant: str = "default",
+                          owner: Union[str, UserRegistrar] = "",
+                          name: str = "",
+                          description: str = "",
+                          inputs: list = [],
+                          tags: List[str] = [],
+                          properties: dict = {}):
         """
-        Register a Dataframe transformation source. The k8s_azure.df_transformation decorator takes the contents
+        Register a Dataframe transformation source. The spark.df_transformation decorator takes the contents
         of the following function and executes the code it contains at serving time.
 
         The name of the function is used as the name of the source when being registered.
 
         The specified inputs are loaded into dataframes that can be accessed using the function parameters.
 
         **Examples**:
         ``` py
-        @k8s_azure.df_transformation(inputs=[("source", "one")])        # Sources are added as inputs
+        @spark.df_transformation(inputs=[("source", "one")])        # Sources are added as inputs
         def average_user_transaction(df):                           # Sources can be manipulated by adding them as params
             return df
         ```
 
         Args:
             name (str): Name of source
             variant (str): Name of variant
             owner (Union[str, UserRegistrar]): Owner
             description (str): Description of primary data to be registered
             inputs (list[Tuple(str, str)]): A list of Source NameVariant Tuples to input into the transformation
 
         Returns:
             source (ColumnSourceRegistrar): Source
         """
-        return self.__registrar.df_transformation(
-            name=name,
-            variant=variant,
-            owner=owner,
-            provider=self.name(),
-            description=description,
-            inputs=inputs,
-            tags=tags,
-            properties=properties,
-        )
+        return self.__registrar.df_transformation(name=name,
+                                                  variant=variant,
+                                                  owner=owner,
+                                                  provider=self.name(),
+                                                  description=description,
+                                                  inputs=inputs,
+                                                  tags=tags,
+                                                  properties=properties)
 
 
 class OfflineK8sProvider(OfflineProvider):
     def __init__(self, registrar, provider):
         super().__init__(registrar, provider)
         self.__registrar = registrar
         self.__provider = provider
 
-    def register_file(
-        self,
-        name: str,
-        path: str,
-        variant: str = "default",
-        owner: Union[str, UserRegistrar] = "",
-        description: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_file(self,
+                      name: str,
+                      path: str,
+                      variant: str = "default",
+                      owner: Union[str, UserRegistrar] = "",
+                      description: str = "",
+                      tags: List[str] = [],
+                      properties: dict = {}):
         """Register a blob data source path as a primary data source.
 
         Args:
             name (str): Name of table to be registered
             variant (str): Name of variant to be registered
             path (str): The path to blob store file
             owner (Union[str, UserRegistrar]): Owner
             description (str): Description of table to be registered
 
         Returns:
             source (ColumnSourceRegistrar): source
         """
-        return self.__registrar.register_primary_data(
-            name=name,
-            variant=variant,
-            location=SQLTable(path),
-            owner=owner,
-            provider=self.name(),
-            description=description,
-            tags=tags,
-            properties=properties,
-        )
-
-    def sql_transformation(
-        self,
-        variant: str = "",
-        owner: Union[str, UserRegistrar] = "",
-        name: str = "",
-        schedule: str = "",
-        description: str = "",
-        docker_image: str = "",
-        resource_specs: Union[K8sResourceSpecs, None] = None,
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+        return self.__registrar.register_primary_data(name=name,
+                                                      variant=variant,
+                                                      location=SQLTable(path),
+                                                      owner=owner,
+                                                      provider=self.name(),
+                                                      description=description,
+                                                      tags=tags,
+                                                      properties=properties)
+
+    def sql_transformation(self,
+                           variant: str = "default",
+                           owner: Union[str, UserRegistrar] = "",
+                           name: str = "",
+                           schedule: str = "",
+                           description: str = "",
+                           docker_image: str = "",
+                           resource_specs: Union[K8sResourceSpecs, None] = None,
+                           tags: List[str] = [],
+                           properties: dict = {}):
         """
         Register a SQL transformation source. The k8s.sql_transformation decorator takes the returned string in the
         following function and executes it as a SQL Query.
 
         The name of the function is the name of the resulting source.
 
         Sources for the transformation can be specified by adding the Name and Variant in brackets '{{ name.variant }}'.
@@ -390,38 +325,34 @@
             docker_image (str): A custom Docker image to run the transformation
             resource_specs (K8sResourceSpecs): Custom resource requests and limits
 
 
         Returns:
             source (ColumnSourceRegistrar): Source
         """
-        return self.__registrar.sql_transformation(
-            name=name,
-            variant=variant,
-            owner=owner,
-            schedule=schedule,
-            provider=self.name(),
-            description=description,
-            args=K8sArgs(docker_image=docker_image, specs=resource_specs),
-            tags=tags,
-            properties=properties,
-        )
-
-    def df_transformation(
-        self,
-        variant: str = "default",
-        owner: Union[str, UserRegistrar] = "",
-        name: str = "",
-        description: str = "",
-        inputs: list = [],
-        docker_image: str = "",
-        resource_specs: Union[K8sResourceSpecs, None] = None,
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+        return self.__registrar.sql_transformation(name=name,
+                                                   variant=variant,
+                                                   owner=owner,
+                                                   schedule=schedule,
+                                                   provider=self.name(),
+                                                   description=description,
+                                                   args=K8sArgs(docker_image=docker_image, specs=resource_specs),
+                                                   tags=tags,
+                                                   properties=properties)
+
+    def df_transformation(self,
+                          variant: str = "default",
+                          owner: Union[str, UserRegistrar] = "",
+                          name: str = "",
+                          description: str = "",
+                          inputs: list = [],
+                          docker_image: str = "",
+                          resource_specs: Union[K8sResourceSpecs, None] = None,
+                          tags: List[str] = [],
+                          properties: dict = {}):
         """
         Register a Dataframe transformation source. The k8s_azure.df_transformation decorator takes the contents
         of the following function and executes the code it contains at serving time.
 
         The name of the function is used as the name of the source when being registered.
 
         The specified inputs are loaded into dataframes that can be accessed using the function parameters.
@@ -441,25 +372,23 @@
             inputs (list[Tuple(str, str)]): A list of Source NameVariant Tuples to input into the transformation
             docker_image (str): A custom Docker image to run the transformation
             resource_specs (K8sResourceSpecs): Custom resource requests and limits
 
         Returns:
             source (ColumnSourceRegistrar): Source
         """
-        return self.__registrar.df_transformation(
-            name=name,
-            variant=variant,
-            owner=owner,
-            provider=self.name(),
-            description=description,
-            inputs=inputs,
-            args=K8sArgs(docker_image=docker_image, specs=resource_specs),
-            tags=tags,
-            properties=properties,
-        )
+        return self.__registrar.df_transformation(name=name,
+                                                  variant=variant,
+                                                  owner=owner,
+                                                  provider=self.name(),
+                                                  description=description,
+                                                  inputs=inputs,
+                                                  args=K8sArgs(docker_image=docker_image, specs=resource_specs),
+                                                  tags=tags,
+                                                  properties=properties)
 
 
 class OnlineProvider:
     def __init__(self, registrar, provider):
         self.__registrar = registrar
         self.__provider = provider
 
@@ -507,16 +436,16 @@
 
     def name(self) -> str:
         return self.__provider.name
 
     def register_file(
         self,
         name,
-        description,
         path,
+        description="",
         variant="default",
         owner="",
         tags: List[str] = [],
         properties: dict = {},
     ):
         """Register a local file.
 
@@ -528,21 +457,28 @@
             description="A dataset of fraudulent transactions",
             path="transactions.csv"
         )
         ```
         Args:
             name (str): Name for how to reference the file later
             description (str): Description of the file
-            path (str): Path to the file
+            path (str): Path to the file (supported formats: csv, parquet)
             variant (str): File variant
             owner (str): Owner of the file
 
         Returns:
             source (LocalSource): source
         """
+        if not FileFormat.is_supported(path):
+            print(f"File format not supported: {path}")
+            raise Exception(
+                "File format not supported. Supported formats: {}".format(
+                    FileFormat.supported_formats()
+                )
+            )
         if owner == "":
             owner = self.__registrar.must_get_default_owner()
         # Store the file as a source
         self.__registrar.register_primary_data(
             name=name,
             variant=variant,
             location=SQLTable(path),
@@ -663,21 +599,25 @@
             description=description,
             tags=tags,
             properties=properties,
         )
 
 
 class SourceRegistrar:
+
     def __init__(self, registrar, source):
         self.__registrar = registrar
         self.__source = source
 
     def id(self) -> NameVariant:
         return self.__source.name, self.__source.variant
 
+    def name_variant(self) -> NameVariant:
+        return self.id()
+
     def registrar(self):
         return self.__registrar
 
 
 class ColumnMapping(dict):
     name: str
     variant: str
@@ -688,24 +628,22 @@
 
 
 class LocalSource:
     """
     LocalSource creates a reference to a source that can be accessed locally.
     """
 
-    def __init__(
-        self,
-        registrar,
-        name: str,
-        owner: str,
-        variant: str,
-        provider: str,
-        path: str,
-        description: str = "",
-    ):
+    def __init__(self,
+                 registrar,
+                 name: str,
+                 owner: str,
+                 variant: str,
+                 provider: str,
+                 path: str,
+                 description: str = ""):
         self.registrar = registrar
         self.name = name
         self.variant = variant
         self.owner = owner
         self.provider = provider
         self.path = path
         self.description = description
@@ -718,17 +656,17 @@
         self.__set_query(fn())
         fn.register_resources = self.register_resources
         return fn
 
     def __getitem__(self, columns: List[str]):
         col_len = len(columns)
         if col_len < 2:
-            raise Exception(
-                f"Expected 2 columns, but found {col_len}. Missing entity and/or source columns"
-            )
+            raise Exception(f"Expected 2 columns, but found {col_len}. Missing entity and/or source columns")
+        elif col_len > 3:
+            raise Exception(f"Found unrecognized columns {', '.join(columns[3:])}. Expected 2 required columns and an optional 3rd timestamp column")
         return (self.registrar, self.name_variant(), columns)
 
     def name_variant(self):
         return (self.name, self.variant)
 
     def pandas(self):
         """
@@ -736,22 +674,22 @@
 
         Returns:
         dataframe (pandas.Dataframe): A pandas Dataframe
         """
         return pd.read_csv(self.path)
 
     def register_resources(
-        self,
-        entity: Union[str, EntityRegistrar],
-        entity_column: str,
-        owner: Union[str, UserRegistrar] = "",
-        inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
-        features: List[ColumnMapping] = None,
-        labels: List[ColumnMapping] = None,
-        timestamp_column: str = "",
+            self,
+            entity: Union[str, EntityRegistrar],
+            entity_column: str,
+            owner: Union[str, UserRegistrar] = "",
+            inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
+            features: List[ColumnMapping] = None,
+            labels: List[ColumnMapping] = None,
+            timestamp_column: str = "",
     ):
         """
         Registers a features and/or labels that can be used in training sets or served.
 
         **Examples**:
         ``` py
         average_user_transaction.register_resources(
@@ -803,61 +741,54 @@
     feature = ff.Feature(average_user_transaction[["user_id", "avg_transaction_amt"]])
     ```
 
     Given the function type does not implement __getitem__ we need to wrap it in a class that 
     enables this behavior while still maintaining the original function signature and behavior.
     """
 
-    def __init__(
-        self,
-        fn,
-        registrar,
-        provider,
-        decorator_register_resources_method,
-        decorator_name_variant_method,
-    ):
+    def __init__(self, fn, registrar, provider, decorator_register_resources_method, decorator_name_variant_method):
         self.fn = fn
         self.registrar = registrar
         self.provider = provider
-        # Binds the register_resources and name_variant methods to the subscriptable_fn
-        # using the descriptor protocol. This allows us to call the methods on the
-        # subscriptable_fn instance. **NOTE** the MethodType could also be used to bind
-        # the methods to the subscriptable_fn instance; however, the descriptor protocol
-        # produces the same result while also being compatible with `classmethod`
-        # and `staticmethod`.
-        self.register_resources = decorator_register_resources_method.__get__(self)
-        self.name_variant = decorator_name_variant_method.__get__(self)
-        pass
+        # Previously, the descriptor protocol was used to apply methods from the decorator classes
+        # to instances of SubscriptableTransformation such that a user could call `fn.name_variant()`
+        # and receive a tuple of (name, variant) where name was the name of the wrapped function and
+        # variant was either the value passed to the decorator or the default value. This was achieved
+        # via the following syntax: `self.name_variant = decorator_name_variant_method.__get__(self)`
+        # For as-of-yet unknown reasons, this behavior was not working as expected in Python 3.11.2, so
+        # so the code has been reverted to the original syntax, which simply passes a reference to the
+        # the decorator methods to the SubscriptableTransformation class.
+        self.register_resources = decorator_register_resources_method
+        self.name_variant = decorator_name_variant_method
 
-    def __getitem__(self, columns):
+    def __getitem__(self, columns: List[str]):
         col_len = len(columns)
         if col_len < 2:
-            raise Exception(
-                f"Expected 2 columns, but found {col_len}. Missing entity and/or source columns"
-            )
+            raise Exception(f"Expected 2 columns, but found {col_len}. Missing entity and/or source columns")
+        elif col_len > 3:
+            raise Exception(f"Found unrecognized columns {', '.join(columns[3:])}. Expected 2 required columns and an optional 3rd timestamp column")
         return (self.registrar, self.name_variant(), columns)
 
     def __call__(self, *args, **kwds):
         return self.fn(*args, **kwds)
 
 
 class SQLTransformationDecorator:
-    def __init__(
-        self,
-        registrar,
-        owner: str,
-        provider: str,
-        tags: List[str],
-        properties: dict,
-        variant: str = "default",
-        name: str = "",
-        schedule: str = "",
-        description: str = "",
-        args: K8sArgs = None,
-    ):
+
+    def __init__(self,
+                 registrar,
+                 owner: str,
+                 provider: str,
+                 tags: List[str],
+                 properties: dict,
+                 variant: str = "default",
+                 name: str = "",
+                 schedule: str = "",
+                 description: str = "",
+                 args: K8sArgs = None):
         self.registrar = registrar
         self.name = name
         self.variant = variant
         self.owner = owner
         self.schedule = schedule
         self.provider = provider
         self.description = description
@@ -872,15 +803,15 @@
             self.name = fn.__name__
         self.__set_query(fn())
         return SubscriptableTransformation(
             fn,
             self.registrar,
             self.provider,
             self.register_resources,
-            self.name_variant,
+            self.name_variant
         )
 
     @typechecked
     def __set_query(self, query: str):
         if query == "":
             raise ValueError("Query cannot be an empty string")
         self.query = query
@@ -891,31 +822,31 @@
             variant=self.variant,
             definition=SQLTransformation(self.query, self.args),
             owner=self.owner,
             schedule=self.schedule,
             provider=self.provider,
             description=self.description,
             tags=self.tags,
-            properties=self.properties,
+            properties=self.properties
         )
 
     def name_variant(self):
         return (self.name, self.variant)
 
     def register_resources(
-        self,
-        entity: Union[str, EntityRegistrar],
-        entity_column: str,
-        owner: Union[str, UserRegistrar] = "",
-        inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
-        features: List[ColumnMapping] = None,
-        labels: List[ColumnMapping] = None,
-        timestamp_column: str = "",
-        description: str = "",
-        schedule: str = "",
+            self,
+            entity: Union[str, EntityRegistrar],
+            entity_column: str,
+            owner: Union[str, UserRegistrar] = "",
+            inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
+            features: List[ColumnMapping] = None,
+            labels: List[ColumnMapping] = None,
+            timestamp_column: str = "",
+            description: str = "",
+            schedule: str = "",
     ):
         return self.registrar.register_column_resources(
             source=(self.name, self.variant),
             entity=entity,
             entity_column=entity_column,
             owner=owner,
             inference_store=inference_store,
@@ -924,27 +855,26 @@
             timestamp_column=timestamp_column,
             description=description,
             schedule=schedule,
         )
 
 
 class DFTransformationDecorator:
-    def __init__(
-        self,
-        registrar,
-        owner: str,
-        provider: str,
-        tags: List[str],
-        properties: dict,
-        variant: str = "default",
-        name: str = "",
-        description: str = "",
-        inputs: list = [],
-        args: K8sArgs = None,
-    ):
+
+    def __init__(self,
+                 registrar,
+                 owner: str,
+                 provider: str,
+                 tags: List[str],
+                 properties: dict,
+                 variant: str = "default",
+                 name: str = "",
+                 description: str = "",
+                 inputs: list = [],
+                 args: K8sArgs = None):
         self.registrar = registrar
         self.name = name
         self.variant = variant
         self.owner = owner
         self.provider = provider
         self.description = description
         self.inputs = inputs
@@ -956,51 +886,49 @@
         if self.description == "" and fn.__doc__ is not None:
             self.description = fn.__doc__
         if self.name == "":
             self.name = fn.__name__
 
         for nv in self.inputs:
             if self.name is nv[0] and self.variant is nv[1]:
-                raise ValueError(
-                    f"Transformation cannot be input for itself: {self.name} {self.variant}"
-                )
+                raise ValueError(f"Transformation cannot be input for itself: {self.name} {self.variant}")
         self.query = dill.dumps(fn.__code__)
         return SubscriptableTransformation(
             fn,
             self.registrar,
             self.provider,
             self.register_resources,
-            self.name_variant,
+            self.name_variant
         )
 
     def to_source(self) -> Source:
         return Source(
             name=self.name,
             variant=self.variant,
             definition=DFTransformation(self.query, self.inputs, self.args),
             owner=self.owner,
             provider=self.provider,
             description=self.description,
             tags=self.tags,
-            properties=self.properties,
+            properties=self.properties
         )
 
     def name_variant(self):
         return (self.name, self.variant)
 
     def register_resources(
-        self,
-        entity: Union[str, EntityRegistrar],
-        entity_column: str,
-        owner: Union[str, UserRegistrar] = "",
-        inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
-        features: List[ColumnMapping] = None,
-        labels: List[ColumnMapping] = None,
-        timestamp_column: str = "",
-        description: str = "",
+            self,
+            entity: Union[str, EntityRegistrar],
+            entity_column: str,
+            owner: Union[str, UserRegistrar] = "",
+            inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
+            features: List[ColumnMapping] = None,
+            labels: List[ColumnMapping] = None,
+            timestamp_column: str = "",
+            description: str = ""
     ):
         return self.registrar.register_column_resources(
             source=(self.name, self.variant),
             entity=entity,
             entity_column=entity_column,
             owner=owner,
             inference_store=inference_store,
@@ -1008,33 +936,34 @@
             labels=labels,
             timestamp_column=timestamp_column,
             description=description,
         )
 
 
 class ColumnSourceRegistrar(SourceRegistrar):
+
     def __getitem__(self, columns: List[str]):
         col_len = len(columns)
         if col_len < 2:
-            raise Exception(
-                f"Expected 2 columns, but found {col_len}. Missing entity and/or source columns"
-            )
+            raise Exception(f"Expected 2 columns, but found {col_len}. Missing entity and/or source columns")
+        elif col_len > 3:
+            raise Exception(f"Found unrecognized columns {', '.join(columns[3:])}. Expected 2 required columns and an optional 3rd timestamp column")
         return (self.registrar(), self.id(), columns)
 
     def register_resources(
-        self,
-        entity: Union[str, EntityRegistrar],
-        entity_column: str,
-        owner: Union[str, UserRegistrar] = "",
-        inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
-        features: List[ColumnMapping] = None,
-        labels: List[ColumnMapping] = None,
-        timestamp_column: str = "",
-        description: str = "",
-        schedule: str = "",
+            self,
+            entity: Union[str, EntityRegistrar],
+            entity_column: str,
+            owner: Union[str, UserRegistrar] = "",
+            inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
+            features: List[ColumnMapping] = None,
+            labels: List[ColumnMapping] = None,
+            timestamp_column: str = "",
+            description: str = "",
+            schedule: str = "",
     ):
         """
         Registers a features and/or labels that can be used in training sets or served.
 
         **Examples**:
         ``` py
         average_user_transaction.register_resources(
@@ -1070,53 +999,51 @@
             timestamp_column=timestamp_column,
             description=description,
             schedule=schedule,
         )
 
 
 class ResourceRegistrar:
+
     def __init__(self, registrar, features, labels):
         self.__registrar = registrar
         self.__features = features
         self.__labels = labels
 
-    def create_training_set(
-        self,
-        name: str,
-        variant: str,
-        label: NameVariant = None,
-        schedule: str = "",
-        features: List[NameVariant] = None,
-        resources: List = None,
-        owner: Union[str, UserRegistrar] = "",
-        description: str = "",
-    ):
+    def create_training_set(self,
+                            name: str,
+                            variant: str = "default",
+                            label: NameVariant = None,
+                            schedule: str = "",
+                            features: List[NameVariant] = None,
+                            resources: List = None,
+                            owner: Union[str, UserRegistrar] = "",
+                            description: str = ""):
         if len(self.__labels) == 0:
             raise ValueError("A label must be included in a training set")
         if len(self.__features) == 0:
             raise ValueError("A feature must be included in a training set")
         if len(self.__labels) > 1 and label == None:
-            raise ValueError("Only one label may be specified in a TrainingSet.")
+            raise ValueError(
+                "Only one label may be specified in a TrainingSet.")
         if features is not None:
-            featureSet = set(
-                [(feature["name"], feature["variant"]) for feature in self.__features]
-            )
+            featureSet = set([(feature["name"], feature["variant"])
+                              for feature in self.__features])
             for feature in features:
                 if feature not in featureSet:
                     raise ValueError(f"Feature {feature} not found.")
         else:
-            features = [
-                (feature["name"], feature["variant"]) for feature in self.__features
-            ]
+            features = [(feature["name"], feature["variant"])
+                        for feature in self.__features]
         if label is None:
             label = (self.__labels[0]["name"], self.__labels[0]["variant"])
         else:
-            labelSet = set(
-                [(label["name"], label["variant"]) for label in self.__labels]
-            )
+            labelSet = set([
+                (label["name"], label["variant"]) for label in self.__labels
+            ])
             if label not in labelSet:
                 raise ValueError(f"Label {label} not found.")
         return self.__registrar.register_training_set(
             name=name,
             variant=variant,
             label=label,
             features=features,
@@ -1128,25 +1055,24 @@
 
     def features(self):
         return self.__features
 
     def label(self):
         if isinstance(self.__labels, list):
             if len(self.__labels) > 1:
-                raise ValueError(
-                    "A resource used has multiple labels. A training set can only have one label"
-                )
+                raise ValueError("A resource used has multiple labels. A training set can only have one label")
             elif len(self.__labels) == 1:
                 self.__labels = (self.__labels[0]["name"], self.__labels[0]["variant"])
             else:
                 self.__labels = ()
         return self.__labels
 
 
 class ModelRegistrar:
+
     def __init__(self, registrar, model):
         self.__registrar = registrar
         self.__model = model
 
     def name(self) -> str:
         return self.__model.name
 
@@ -1174,17 +1100,15 @@
 
     def add_resource(self, resource):
         self.__resources.append(resource)
 
     def get_resources(self):
         return self.__resources
 
-    def register_user(
-        self, name: str, tags: List[str] = [], properties: dict = {}
-    ) -> UserRegistrar:
+    def register_user(self, name: str, tags: List[str] = [], properties: dict = {}) -> UserRegistrar:
         """Register a user.
 
         Args:
             name (str): User to be registered.
 
         Returns:
             UserRegistrar: User
@@ -1203,15 +1127,16 @@
 
     def default_owner(self) -> str:
         return self.__default_owner
 
     def must_get_default_owner(self) -> str:
         owner = self.default_owner()
         if owner == "":
-            raise ValueError("Owner must be set or a default owner must be specified.")
+            raise ValueError(
+                "Owner must be set or a default owner must be specified.")
         return owner
 
     def get_source(self, name, variant, local=False):
         """Get a source. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1231,46 +1156,36 @@
 
         Returns:
             source (ColumnSourceRegistrar): Source
         """
         get = SourceReference(name=name, variant=variant, obj=None)
         self.__resources.append(get)
         if local:
-            return LocalSource(
-                self,
-                name=name,
-                owner="",
-                variant=variant,
-                provider="",
-                description="",
-                path="",
-            )
+            return LocalSource(self,
+                               name=name,
+                               owner="",
+                               variant=variant,
+                               provider="",
+                               description="",
+                               path="")
         else:
             fakeDefinition = PrimaryData(location=SQLTable(name=""))
-            fakeSource = Source(
-                name=name,
-                variant=variant,
-                definition=fakeDefinition,
-                owner="",
-                provider="",
-                description="",
-            )
+            fakeSource = Source(name=name,
+                                variant=variant,
+                                definition=fakeDefinition,
+                                owner="",
+                                provider="",
+                                description="")
             return ColumnSourceRegistrar(self, fakeSource)
 
     def get_local_provider(self, name="local-mode"):
         get = ProviderReference(name=name, provider_type="local", obj=None)
         self.__resources.append(get)
         fakeConfig = LocalConfig()
-        fakeProvider = Provider(
-            name=name,
-            function="LOCAL_ONLINE",
-            description="",
-            team="",
-            config=fakeConfig,
-        )
+        fakeProvider = Provider(name=name, function="LOCAL_ONLINE", description="", team="", config=fakeConfig)
         return LocalProvider(self, fakeProvider)
 
     def get_redis(self, name):
         """Get a Redis provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1290,17 +1205,15 @@
 
         Returns:
             redis (OnlineProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="redis", obj=None)
         self.__resources.append(get)
         fakeConfig = RedisConfig(host="", port=123, password="", db=123)
-        fakeProvider = Provider(
-            name=name, function="ONLINE", description="", team="", config=fakeConfig
-        )
+        fakeProvider = Provider(name=name, function="ONLINE", description="", team="", config=fakeConfig)
         return OnlineProvider(self, fakeProvider)
 
     def get_mongodb(self, name):
         """Get a MongoDB provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1320,17 +1233,15 @@
 
         Returns:
             mongodb (OnlineProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="mongodb", obj=None)
         self.__resources.append(get)
         mock_config = MongoDBConfig()
-        mock_provider = Provider(
-            name=name, function="ONLINE", description="", team="", config=mock_config
-        )
+        mock_provider = Provider(name=name, function="ONLINE", description="", team="", config=mock_config)
         return OnlineProvider(self, mock_provider)
 
     def get_blob_store(self, name):
         """Get a Azure Blob provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1349,23 +1260,17 @@
             name (str): Name of Azure blob provider to be retrieved
 
         Returns:
             azure_blob (FileStoreProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="AZURE", obj=None)
         self.__resources.append(get)
-        fake_azure_config = AzureFileStoreConfig(
-            account_name="", account_key="", container_name="", root_path=""
-        )
-        fake_config = OnlineBlobConfig(
-            store_type="AZURE", store_config=fake_azure_config.config()
-        )
-        fakeProvider = Provider(
-            name=name, function="ONLINE", description="", team="", config=fake_config
-        )
+        fake_azure_config = AzureFileStoreConfig(account_name="", account_key="", container_name="", root_path="")
+        fake_config = OnlineBlobConfig(store_type="AZURE", store_config=fake_azure_config.config())
+        fakeProvider = Provider(name=name, function="ONLINE", description="", team="", config=fake_config)
         return FileStoreProvider(self, fakeProvider, fake_config, "AZURE")
 
     def get_postgres(self, name):
         """Get a Postgres provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1382,17 +1287,15 @@
 
         Returns:
             postgres (OfflineSQLProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="postgres", obj=None)
         self.__resources.append(get)
         fakeConfig = PostgresConfig(host="", port="", database="", user="", password="")
-        fakeProvider = Provider(
-            name=name, function="OFFLINE", description="", team="", config=fakeConfig
-        )
+        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
         return OfflineSQLProvider(self, fakeProvider)
 
     def get_snowflake(self, name):
         """Get a Snowflake provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1408,25 +1311,42 @@
             name (str): Name of Snowflake provider to be retrieved
 
         Returns:
             snowflake (OfflineSQLProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="snowflake", obj=None)
         self.__resources.append(get)
-        fakeConfig = SnowflakeConfig(
-            account="",
-            database="",
-            organization="",
-            username="",
-            password="",
-            schema="",
-        )
-        fakeProvider = Provider(
-            name=name, function="OFFLINE", description="", team="", config=fakeConfig
+        fakeConfig = SnowflakeConfig(account="ff_fake", database="ff_fake", organization="ff_fake", username="ff_fake", password="ff_fake", schema="ff_fake")
+        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
+        return OfflineSQLProvider(self, fakeProvider)
+    
+    def get_snowflake_legacy(self, name: str):
+        """Get a Snowflake provider. The returned object can be used to register additional resources.
+
+        **Examples**:
+        ``` py
+        snowflake = ff.get_snowflake_legacy("snowflake-quickstart")
+        transactions = snowflake.register_table(
+            name="transactions",
+            variant="kaggle",
+            description="Fraud Dataset From Kaggle",
+            table="Transactions",  # This is the table's name in Postgres
         )
+        ```
+        Args:
+            name (str): Name of Snowflake provider to be retrieved
+
+        Returns:
+            snowflake_legacy (OfflineSQLProvider): Provider
+        """
+        get = ProviderReference(name=name, provider_type="snowflake", obj=None)
+        self.__resources.append(get)
+
+        fakeConfig = SnowflakeConfig(account_locator="ff_fake", database="ff_fake", username="ff_fake", password="ff_fake", schema="ff_fake", warehouse="ff_fake", role="ff_fake")
+        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
         return OfflineSQLProvider(self, fakeProvider)
 
     def get_redshift(self, name):
         """Get a Redshift provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1443,17 +1363,15 @@
 
         Returns:
             redshift (OfflineSQLProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="redshift", obj=None)
         self.__resources.append(get)
         fakeConfig = RedshiftConfig(host="", port="", database="", user="", password="")
-        fakeProvider = Provider(
-            name=name, function="OFFLINE", description="", team="", config=fakeConfig
-        )
+        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
         return OfflineSQLProvider(self, fakeProvider)
 
     def get_bigquery(self, name):
         """Get a BigQuery provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1470,17 +1388,15 @@
 
         Returns:
             bigquery (OfflineSQLProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="bigquery", obj=None)
         self.__resources.append(get)
         fakeConfig = BigQueryConfig(project_id="", dataset_id="", credentials_path="")
-        fakeProvider = Provider(
-            name=name, function="OFFLINE", description="", team="", config=fakeConfig
-        )
+        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
         return OfflineSQLProvider(self, fakeProvider)
 
     def get_spark(self, name):
         """Get a Spark provider. The returned object can be used to register additional resources.
         **Examples**:
         ``` py
         spark = ff.get_spark("spark-quickstart")
@@ -1494,20 +1410,16 @@
         Args:
             name (str): Name of Spark provider to be retrieved
         Returns:
             spark (OfflineSQLProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="spark", obj=None)
         self.__resources.append(get)
-        fakeConfig = SparkConfig(
-            executor_type="", executor_config={}, store_type="", store_config={}
-        )
-        fakeProvider = Provider(
-            name=name, function="OFFLINE", description="", team="", config=fakeConfig
-        )
+        fakeConfig = SparkConfig(executor_type="", executor_config={}, store_type="", store_config={})
+        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
         return OfflineSparkProvider(self, fakeProvider)
 
     def get_kubernetes(self, name):
         """
         Get a k8s Azure provider. The returned object can be used to register additional resources.
         **Examples**:
         ``` py
@@ -1525,17 +1437,15 @@
         Returns:
             k8s_azure (OfflineK8sProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="k8s-azure", obj=None)
         self.__resources.append(get)
 
         fakeConfig = K8sConfig(store_type="", store_config={})
-        fakeProvider = Provider(
-            name=name, function="OFFLINE", description="", team="", config=fakeConfig
-        )
+        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
         return OfflineK8sProvider(self, fakeProvider)
 
     def get_s3(self, name):
         """
         Get a S3 provider. The returned object can be used with other providers such as Spark and Databricks.
         **Examples**:
         ``` py
@@ -1554,43 +1464,35 @@
         Returns:
             s3 (FileStore): Provider
         """
         get = ProviderReference(name=name, provider_type="S3", obj=None)
         self.__resources.append(get)
 
         fake_creds = AWSCredentials("id", "secret")
-        fakeConfig = S3StoreConfig(
-            bucket_path="", bucket_region="", credentials=fake_creds
-        )
-        provider = Provider(
-            name=name,
-            function="OFFLINE",
-            description=description,
-            team=team,
-            config=s3_config,
-        )
+        fakeConfig = S3StoreConfig(bucket_path="", bucket_region="", credentials=fake_creds)
+        provider = Provider(name=name,
+                            function="OFFLINE",
+                            description=description,
+                            team=team,
+                            config=s3_config)
         return FileStoreProvider(provider, s3_config, s3_config.type())
-
+    
     def get_gcs(self, name):
         get = ProviderReference(name=name, provider_type="GCS", obj=None)
         self.__resources.append(get)
 
         filename = "fake_secrets.json"
         if not exists(filename):
             self._create_mock_creds_file(filename, {"test": "creds"})
 
         fake_creds = GCPCredentials("id", filename)
-        fakeConfig = GCSStoreConfig(
-            bucket_name="", bucket_path="", credentials=fake_creds
-        )
-        fakeProvider = Provider(
-            name=name, function="OFFLINE", description="", team="", config=fakeConfig
-        )
+        fakeConfig = GCSStoreConfig(bucket_name="", bucket_path="", credentials=fake_creds)
+        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
         return OfflineK8sProvider(self, fakeProvider)
-
+    
     def _create_mock_creds_file(self, filename, json_data):
         with open(filename, "w") as f:
             json.dumps(json_data, f)
 
     def get_entity(self, name, local=False):
         """Get an entity. The returned object can be used to register additional resources.
 
@@ -1613,26 +1515,24 @@
             entity (EntityRegistrar): Entity
         """
         get = EntityReference(name=name, obj=None)
         self.__resources.append(get)
         fakeEntity = Entity(name=name, description="")
         return EntityRegistrar(self, fakeEntity)
 
-    def register_redis(
-        self,
-        name: str,
-        description: str = "",
-        team: str = "",
-        host: str = "0.0.0.0",
-        port: int = 6379,
-        password: str = "",
-        db: int = 0,
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_redis(self,
+                       name: str,
+                       description: str = "",
+                       team: str = "",
+                       host: str = "0.0.0.0",
+                       port: int = 6379,
+                       password: str = "",
+                       db: int = 0,
+                       tags: List[str] = [],
+                       properties: dict = {}):
         """Register a Redis provider.
 
         **Examples**:
         ```
         redis = ff.register_redis(
             name="redis-quickstart",
             host="quickstart-redis",  # The internal dns name for redis
@@ -1651,51 +1551,48 @@
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             redis (OnlineProvider): Provider
         """
         config = RedisConfig(host=host, port=port, password=password, db=db)
-        provider = Provider(
-            name=name,
-            function="ONLINE",
-            description=description,
-            team=team,
-            config=config,
-            tags=tags,
-            properties=properties,
-        )
+        provider = Provider(name=name,
+                            function="ONLINE",
+                            description=description,
+                            team=team,
+                            config=config,
+                            tags=tags,
+                            properties=properties)
         self.__resources.append(provider)
         return OnlineProvider(self, provider)
 
-    def register_blob_store(
-        self,
-        name: str,
-        account_name: str,
-        account_key: str,
-        container_name: str,
-        root_path: str,
-        description: str = "",
-        team: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_blob_store(self,
+                            name: str,
+                            account_name: str,
+                            account_key: str,
+                            container_name: str,
+                            root_path: str,
+                            description: str = "",
+                            team: str = "",
+                            tags: List[str] = [],
+                            properties: dict = {}):
+
         """Register an azure blob store provider.
 
         This has the functionality of an online store and can be used as a parameter
         to a k8s or spark provider
 
         **Examples**:
         ```
         blob = ff.register_blob_store(
             name="azure-quickstart",
             container_name="my_company_container"
             root_path="custom/path/in/container"
             account_name=<azure_account_name>
-            account_key=<azure_account_key>
+            account_key=<azure_account_key> 
             description="An azure blob store provider to store offline and inference data"
         )
         ```
         Args:
             name (str): Name of Azure blob store to be registered
             container_name (str): Azure container name
             root_path (str): custom path in container to store data
@@ -1707,105 +1604,91 @@
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
         Returns:
             blob (StorageProvider): Provider
                 has all the functionality of OnlineProvider
         """
 
-        azure_config = AzureFileStoreConfig(
-            account_name=account_name,
-            account_key=account_key,
-            container_name=container_name,
-            root_path=root_path,
-        )
-        config = OnlineBlobConfig(
-            store_type="AZURE", store_config=azure_config.config()
-        )
-
-        provider = Provider(
-            name=name,
-            function="ONLINE",
-            description=description,
-            team=team,
-            config=config,
-            tags=tags,
-            properties=properties,
-        )
+        azure_config = AzureFileStoreConfig(account_name=account_name, account_key=account_key,
+                                            container_name=container_name, root_path=root_path)
+        config = OnlineBlobConfig(store_type="AZURE", store_config=azure_config.config())
+
+        provider = Provider(name=name,
+                            function="ONLINE",
+                            description=description,
+                            team=team,
+                            config=config,
+                            tags=tags,
+                            properties=properties)
         self.__resources.append(provider)
         return FileStoreProvider(self, provider, azure_config, "AZURE")
 
-    def register_s3(
-        self,
-        name: str,
-        credentials: AWSCredentials,
-        bucket_path: str,
-        bucket_region: str,
-        description: str = "",
-        team: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_s3(self,
+                    name: str,
+                    credentials: AWSCredentials,
+                    bucket_path: str,
+                    bucket_region: str,
+                    path: str = "",
+                    description: str = "",
+                    team: str = "",
+                    tags: List[str] = [],
+                    properties: dict = {}):
         """Register a S3 store provider.
 
         This has the functionality of an offline store and can be used as a parameter
         to a k8s or spark provider
 
         **Examples**:
         ```
         s3 = ff.register_s3(
             name="s3-quickstart",
             credentials=aws_creds,
-            bucket_path="bucket_name/path",
+            bucket_path="bucket_name",
             bucket_region=<bucket_region>,
+            path="path/to/store/featureform_files/in/",
             description="An s3 store provider to store offline"
         )
         ```
         Args:
             name (str): Name of S3 store to be registered
             credentials (AWSCredentials): AWS credentials to access the bucket
             bucket_path (str): custom path including the bucket name
             bucket_region (str): aws region the bucket is located in
+            path (str): the path used to store featureform files in
             description (str): Description of S3 provider to be registered
             team (str): the name of the team registering the filestore
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
         Returns:
             s3 (FileStoreProvider): Provider
                 has all the functionality of OfflineProvider
         """
 
-        s3_config = S3StoreConfig(
-            bucket_path=bucket_path,
-            bucket_region=bucket_region,
-            credentials=credentials,
-        )
+        s3_config = S3StoreConfig(bucket_path=bucket_path, bucket_region=bucket_region, credentials=credentials, path=path)
 
-        provider = Provider(
-            name=name,
-            function="OFFLINE",
-            description=description,
-            team=team,
-            config=s3_config,
-            tags=tags,
-            properties=properties,
-        )
+        provider = Provider(name=name,
+                            function="OFFLINE",
+                            description=description,
+                            team=team,
+                            config=s3_config,
+                            tags=tags,
+                            properties=properties)
         self.__resources.append(provider)
         return FileStoreProvider(self, provider, s3_config, s3_config.type())
 
-    def register_gcs(
-        self,
-        name: str,
-        credentials: GCPCredentials,
-        bucket_name: str,
-        bucket_path: str = "",
-        description: str = "",
-        team: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+
+    def register_gcs(self,
+                    name: str,
+                    credentials: GCPCredentials,
+                    bucket_name: str,
+                    bucket_path: str = "",
+                    description: str = "",
+                    team: str = "",
+                    tags: List[str] = [],
+                    properties: dict = {}):
         """Register a GCS store provider.
                 **Examples**:
         ```
         gcs = ff.register_gcs(
             name="gcs-quickstart",
             credentials=gcp_creds,
             bucket_name="bucket_name",
@@ -1823,41 +1706,33 @@
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
         Returns:
             gcs (FileStoreProvider): Provider
                 has all the functionality of OfflineProvider
         """
 
-        gcs_config = GCSFileStoreConfig(
-            bucket_name=bucket_name, bucket_path=bucket_path, credentials=credentials
-        )
-        provider = Provider(
-            name=name,
-            function="OFFLINE",
-            description=description,
-            team=team,
-            config=gcs_config,
-            tags=tags,
-            properties=properties,
-        )
+        gcs_config = GCSFileStoreConfig(bucket_name=bucket_name, bucket_path=bucket_path, credentials=credentials)
+        provider = Provider(name=name,
+                            function="OFFLINE",
+                            description=description,
+                            team=team,
+                            config=gcs_config,
+                            tags=tags,
+                            properties=properties)
         self.__resources.append(provider)
         return FileStoreProvider(self, provider, gcs_config, gcs_config.type())
 
-    def register_hdfs(
-        self,
-        name: str,
-        host: str,
-        port: str,
-        username: str = "",
-        path: str = "",
-        description: str = "",
-        team: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_hdfs(self,
+                      name: str,
+                      host: str,
+                      port: str,
+                      username: str = "",
+                      path: str = "",
+                      description: str = "",
+                      team: str = "", ):
         """Register a HDFS store provider.
 
         This has the functionality of an offline store and can be used as a parameter
         to a k8s or spark provider
 
         **Examples**:
         ```
@@ -1880,37 +1755,31 @@
             team (str): The name of the team registering HDFS
         Returns:
             hdfs (FileStoreProvider): Provider
         """
 
         hdfs_config = HDFSConfig(host=host, port=port, path=path, username=username)
 
-        provider = Provider(
-            name=name,
-            function="OFFLINE",
-            description=description,
-            team=team,
-            config=hdfs_config,
-            tags=tags,
-            properties=properties,
-        )
+        provider = Provider(name=name,
+                            function="OFFLINE",
+                            description=description,
+                            team=team,
+                            config=hdfs_config)
         self.__resources.append(provider)
         return FileStoreProvider(self, provider, hdfs_config, hdfs_config.type())
 
-    def register_firestore(
-        self,
-        name: str,
-        collection: str,
-        project_id: str,
-        credentials_path: str,
-        description: str = "",
-        team: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_firestore(self,
+                           name: str,
+                           collection: str,
+                           project_id: str,
+                           credentials_path: str,
+                           description: str = "",
+                           team: str = "",
+                           tags: List[str] = [],
+                           properties: dict = {}):
         """Register a Firestore provider.
 
         **Examples**:
         ```
         firestore = ff.register_firestore(
             name="firestore-quickstart",
             description="A Firestore deployment we created for the Featureform quickstart",
@@ -1926,46 +1795,38 @@
             collection (str): The Collection name in Firestore under the given project ID
             credentials_path (str): A path to a Google Credentials file with access permissions for Firestore
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
         Returns:
             firestore (OfflineSQLProvider): Provider
         """
-        config = FirestoreConfig(
-            collection=collection,
-            project_id=project_id,
-            credentials_path=credentials_path,
-        )
-        provider = Provider(
-            name=name,
-            function="ONLINE",
-            description=description,
-            team=team,
-            config=config,
-            tags=tags,
-            properties=properties,
-        )
+        config = FirestoreConfig(collection=collection, project_id=project_id, credentials_path=credentials_path)
+        provider = Provider(name=name,
+                            function="ONLINE",
+                            description=description,
+                            team=team,
+                            config=config,
+                            tags=tags,
+                            properties=properties)
         self.__resources.append(provider)
         return OnlineProvider(self, provider)
 
-    def register_cassandra(
-        self,
-        name: str,
-        description: str = "",
-        team: str = "",
-        host: str = "0.0.0.0",
-        port: int = 9042,
-        username: str = "cassandra",
-        password: str = "cassandra",
-        keyspace: str = "",
-        consistency: str = "THREE",
-        replication: int = 3,
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_cassandra(self,
+                           name: str,
+                           description: str = "",
+                           team: str = "",
+                           host: str = "0.0.0.0",
+                           port: int = 9042,
+                           username: str = "cassandra",
+                           password: str = "cassandra",
+                           keyspace: str = "",
+                           consistency: str = "THREE",
+                           replication: int = 3,
+                           tags: List[str] = [],
+                           properties: dict = {}):
         """Register a Cassandra provider.
 
         **Examples**:
         ```
         cassandra = ff.register_cassandra(
                 name = "cassandra",
                 description = "Example inference store",
@@ -1990,46 +1851,35 @@
             replication (int): Replication
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             cassandra (OnlineProvider): Provider
         """
-        config = CassandraConfig(
-            host=host,
-            port=port,
-            username=username,
-            password=password,
-            keyspace=keyspace,
-            consistency=consistency,
-            replication=replication,
-        )
-        provider = Provider(
-            name=name,
-            function="ONLINE",
-            description=description,
-            team=team,
-            config=config,
-            tags=tags,
-            properties=properties,
-        )
+        config = CassandraConfig(host=host, port=port, username=username, password=password, keyspace=keyspace,
+                                 consistency=consistency, replication=replication)
+        provider = Provider(name=name,
+                            function="ONLINE",
+                            description=description,
+                            team=team,
+                            config=config,
+                            tags=tags,
+                            properties=properties)
         self.__resources.append(provider)
         return OnlineProvider(self, provider)
 
-    def register_dynamodb(
-        self,
-        name: str,
-        description: str = "",
-        team: str = "",
-        access_key: str = None,
-        secret_key: str = None,
-        region: str = None,
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_dynamodb(self,
+                          name: str,
+                          description: str = "",
+                          team: str = "",
+                          access_key: str = None,
+                          secret_key: str = None,
+                          region: str = None,
+                          tags: List[str] = [],
+                          properties: dict = {}):
         """Register a DynamoDB provider.
 
         **Examples**:
         ```
         dynamodb = ff.register_dynamodb(
             name="dynamodb-quickstart",
             description="A Dynamodb deployment we created for the Featureform quickstart",
@@ -2047,43 +1897,38 @@
             region (str): Region
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             dynamodb (OnlineProvider): Provider
         """
-        config = DynamodbConfig(
-            access_key=access_key, secret_key=secret_key, region=region
-        )
-        provider = Provider(
-            name=name,
-            function="ONLINE",
-            description=description,
-            team=team,
-            config=config,
-            tags=tags,
-            properties=properties,
-        )
+        config = DynamodbConfig(access_key=access_key, secret_key=secret_key, region=region)
+        provider = Provider(name=name,
+                            function="ONLINE",
+                            description=description,
+                            team=team,
+                            config=config,
+                            tags=tags,
+                            properties=properties)
         self.__resources.append(provider)
         return OnlineProvider(self, provider)
 
-    def register_mongodb(
-        self,
-        name: str,
-        description: str = "",
-        team: str = "",
-        username: str = None,
-        password: str = None,
-        database: str = None,
-        host: str = None,
-        port: str = None,
-        throughput: int = 1000,
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_mongodb(self,
+                         name: str,
+                         description: str = "",
+                         team: str = "",
+                         username: str = None,
+                         password: str = None,
+                         database: str = None,
+                         host: str = None,
+                         port: str = None,
+                         throughput: int = 1000,
+                         tags: List[str] = [],
+                         properties: dict = {}
+                         ):
         """Register a MongoDB provider.
 
         **Examples**:
         ```
         mongodb = ff.register_mongodb(
             name="mongodb-quickstart",
             description="A MongoDB deployment",
@@ -2108,49 +1953,40 @@
             throughput (int): The maximum RU limit for autoscaling
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             mongodb (OnlineProvider): Provider
         """
-        config = MongoDBConfig(
-            username=username,
-            password=password,
-            host=host,
-            port=port,
-            database=database,
-            throughput=throughput,
-        )
-        provider = Provider(
-            name=name,
-            function="ONLINE",
-            description=description,
-            team=team,
-            config=config,
-            tags=tags,
-            properties=properties,
-        )
+        config = MongoDBConfig(username=username, password=password, host=host, port=port, database=database,
+                               throughput=throughput)
+        provider = Provider(name=name,
+                            function="ONLINE",
+                            description=description,
+                            team=team,
+                            config=config,
+                            tags=tags,
+                            properties=properties)
         self.__resources.append(provider)
         return OnlineProvider(self, provider)
 
     def register_snowflake_legacy(
-        self,
-        name: str,
-        username: str,
-        password: str,
-        account_locator: str,
-        database: str,
-        schema: str = "PUBLIC",
-        description: str = "",
-        team: str = "",
-        warehouse: str = "",
-        role: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+                self,
+                name: str,
+                username: str,
+                password: str,
+                account_locator: str,
+                database: str,
+                schema: str = "PUBLIC",
+                description: str = "",
+                team: str = "",
+                warehouse: str = "",
+                role: str = "",
+                tags: List[str] = [],
+                properties: dict = {}):
         """Register a Snowflake provider using legacy credentials.
 
         **Examples**:
         ```
         snowflake = ff.register_snowflake_legacy(
             name="snowflake-quickstart",
             username="snowflake",
@@ -2174,51 +2010,46 @@
             role (str): Specifies the role to use by default for accessing Snowflake objects in the client session
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             snowflake (OfflineSQLProvider): Provider
         """
-        config = SnowflakeConfig(
-            account_locator=account_locator,
-            database=database,
-            username=username,
-            password=password,
-            schema=schema,
-            warehouse=warehouse,
-            role=role,
-        )
-        provider = Provider(
-            name=name,
-            function="OFFLINE",
-            description=description,
-            team=team,
-            config=config,
-            tags=tags,
-            properties=properties,
-        )
+        config = SnowflakeConfig(account_locator=account_locator,
+                                 database=database,
+                                 username=username,
+                                 password=password,
+                                 schema=schema,
+                                 warehouse=warehouse,
+                                 role=role)
+        provider = Provider(name=name,
+                            function="OFFLINE",
+                            description=description,
+                            team=team,
+                            config=config,
+                            tags=tags,
+                            properties=properties)
         self.__resources.append(provider)
         return OfflineSQLProvider(self, provider)
 
     def register_snowflake(
-        self,
-        name: str,
-        username: str,
-        password: str,
-        account: str,
-        organization: str,
-        database: str,
-        schema: str = "PUBLIC",
-        description: str = "",
-        team: str = "",
-        warehouse: str = "",
-        role: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+            self,
+            name: str,
+            username: str,
+            password: str,
+            account: str,
+            organization: str,
+            database: str,
+            schema: str = "PUBLIC",
+            description: str = "",
+            team: str = "",
+            warehouse: str = "",
+            role: str = "",
+            tags: List[str] = [],
+            properties: dict = {}):
         """Register a Snowflake provider.
 
         **Examples**:
         ```
         snowflake = ff.register_snowflake(
             name="snowflake-quickstart",
             username="snowflake",
@@ -2244,49 +2075,43 @@
             role (str): Specifies the role to use by default for accessing Snowflake objects in the client session
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             snowflake (OfflineSQLProvider): Provider
         """
-        config = SnowflakeConfig(
-            account=account,
-            database=database,
-            organization=organization,
-            username=username,
-            password=password,
-            schema=schema,
-            warehouse=warehouse,
-            role=role,
-        )
-        provider = Provider(
-            name=name,
-            function="OFFLINE",
-            description=description,
-            team=team,
-            config=config,
-            tags=tags,
-            properties=properties,
-        )
+        config = SnowflakeConfig(account=account,
+                                 database=database,
+                                 organization=organization,
+                                 username=username,
+                                 password=password,
+                                 schema=schema,
+                                 warehouse=warehouse,
+                                 role=role)
+        provider = Provider(name=name,
+                            function="OFFLINE",
+                            description=description,
+                            team=team,
+                            config=config,
+                            tags=tags,
+                            properties=properties)
         self.__resources.append(provider)
         return OfflineSQLProvider(self, provider)
 
-    def register_postgres(
-        self,
-        name: str,
-        description: str = "",
-        team: str = "",
-        host: str = "0.0.0.0",
-        port: str = "5432",
-        user: str = "postgres",
-        password: str = "password",
-        database: str = "postgres",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_postgres(self,
+                          name: str,
+                          description: str = "",
+                          team: str = "",
+                          host: str = "0.0.0.0",
+                          port: str = "5432",
+                          user: str = "postgres",
+                          password: str = "password",
+                          database: str = "postgres",
+                          tags: List[str] = None,
+                          properties: dict = None):
         """Register a Postgres provider.
 
         **Examples**:
         ```
         postgres = ff.register_postgres(
             name="postgres-quickstart",
             description="A Postgres deployment we created for the Featureform quickstart",
@@ -2308,42 +2133,40 @@
             database (str): Database
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             postgres (OfflineSQLProvider): Provider
         """
-        config = PostgresConfig(
-            host=host, port=port, database=database, user=user, password=password
-        )
-        provider = Provider(
-            name=name,
-            function="OFFLINE",
-            description=description,
-            team=team,
-            config=config,
-            tags=tags,
-            properties=properties,
-        )
+        config = PostgresConfig(host=host,
+                                port=port,
+                                database=database,
+                                user=user,
+                                password=password)
+        provider = Provider(name=name,
+                            function="OFFLINE",
+                            description=description,
+                            team=team,
+                            config=config,
+                            tags=tags or [],
+                            properties=properties or {})
         self.__resources.append(provider)
         return OfflineSQLProvider(self, provider)
 
-    def register_redshift(
-        self,
-        name: str,
-        description: str = "",
-        team: str = "",
-        host: str = "",
-        port: int = 5432,
-        user: str = "redshift",
-        password: str = "password",
-        database: str = "dev",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_redshift(self,
+                          name: str,
+                          description: str = "",
+                          team: str = "",
+                          host: str = "",
+                          port: int = 5432,
+                          user: str = "redshift",
+                          password: str = "password",
+                          database: str = "dev",
+                          tags: List[str] = [],
+                          properties: dict = {}):
         """Register a Redshift provider.
 
         **Examples**:
         ```
         redshift = ff.register_redshift(
             name="redshift-quickstart",
             description="A Redshift deployment we created for the Featureform quickstart",
@@ -2365,40 +2188,38 @@
             database (str): Database
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             redshift (OfflineSQLProvider): Provider
         """
-        config = RedshiftConfig(
-            host=host, port=port, database=database, user=user, password=password
-        )
-        provider = Provider(
-            name=name,
-            function="OFFLINE",
-            description=description,
-            team=team,
-            config=config,
-            tags=tags,
-            properties=properties,
-        )
+        config = RedshiftConfig(host=host,
+                                port=port,
+                                database=database,
+                                user=user,
+                                password=password)
+        provider = Provider(name=name,
+                            function="OFFLINE",
+                            description=description,
+                            team=team,
+                            config=config,
+                            tags=tags,
+                            properties=properties)
         self.__resources.append(provider)
         return OfflineSQLProvider(self, provider)
 
-    def register_bigquery(
-        self,
-        name: str,
-        description: str = "",
-        team: str = "",
-        project_id: str = "",
-        dataset_id: str = "",
-        credentials_path: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_bigquery(self,
+                          name: str,
+                          description: str = "",
+                          team: str = "",
+                          project_id: str = "",
+                          dataset_id: str = "",
+                          credentials_path: str = "",
+                          tags: List[str] = [],
+                          properties: dict = {}):
         """Register a BigQuery provider.
 
         **Examples**:
         ```
         bigquery = ff.register_bigquery(
             name="bigquery-quickstart",
             description="A BigQuery deployment we created for the Featureform quickstart",
@@ -2415,41 +2236,35 @@
             credentials_path (str): A path to a Google Credentials file with access permissions for BigQuery
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             bigquery (OfflineSQLProvider): Provider
         """
-        config = BigQueryConfig(
-            project_id=project_id,
-            dataset_id=dataset_id,
-            credentials_path=credentials_path,
-        )
-        provider = Provider(
-            name=name,
-            function="OFFLINE",
-            description=description,
-            team=team,
-            config=config,
-            tags=tags,
-            properties=properties,
-        )
+        config = BigQueryConfig(project_id=project_id,
+                                dataset_id=dataset_id,
+                                credentials_path=credentials_path, )
+        provider = Provider(name=name,
+                            function="OFFLINE",
+                            description=description,
+                            team=team,
+                            config=config,
+                            tags=tags,
+                            properties=properties)
         self.__resources.append(provider)
         return OfflineSQLProvider(self, provider)
 
-    def register_spark(
-        self,
-        name: str,
-        executor: ExecutorCredentials,
-        filestore: FileStoreProvider,
-        description: str = "",
-        team: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_spark(self,
+                       name: str,
+                       executor: ExecutorCredentials,
+                       filestore: FileStoreProvider,
+                       description: str = "",
+                       team: str = "",
+                       tags: List[str] = [],
+                       properties: dict = {}):
         """Register a Spark on Executor provider.
         **Examples**:
         ```
         spark = ff.register_spark(
             name="spark-quickstart",
             description="A Spark deployment we created for the Featureform quickstart",
             team="featureform-team",
@@ -2470,42 +2285,37 @@
             spark (OfflineSparkProvider): Provider
         """
 
         config = SparkConfig(
             executor_type=executor.type(),
             executor_config=executor.config(),
             store_type=filestore.store_type(),
-            store_config=filestore.config(),
-        )
+            store_config=filestore.config())
 
-        provider = Provider(
-            name=name,
-            function="OFFLINE",
-            description=description,
-            team=team,
-            config=config,
-            tags=tags,
-            properties=properties,
-        )
+        provider = Provider(name=name,
+                            function="OFFLINE",
+                            description=description,
+                            team=team,
+                            config=config,
+                            tags=tags,
+                            properties=properties)
         self.__resources.append(provider)
         return OfflineSparkProvider(self, provider)
 
-    def register_k8s(
-        self,
-        name: str,
-        store: FileStoreProvider,
-        description: str = "",
-        team: str = "",
-        docker_image: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_k8s(self,
+                     name: str,
+                     store: FileStoreProvider,
+                     description: str = "",
+                     team: str = "",
+                     docker_image: str = "",
+                     tags: List[str] = [],
+                     properties: dict = {}):
         """
         Register an offline store provider to run on featureform's own k8s deployment
-
+        
         Args:
             name (str): Name of provider
             store (FileStoreProvider): Reference to registered file store provider
             description (str): Description of primary data to be registered
             team (str): A string parameter describing the team that owns the provider
             docker_image (str): A custom docker image using the base image featureformcom/k8s_runner
             tags (List[str]): Optional grouping mechanism for resources
@@ -2520,65 +2330,59 @@
             docker_image="my-repo/image:version"
         )
         ```
         """
         config = K8sConfig(
             store_type=store.store_type(),
             store_config=store.config(),
-            docker_image=docker_image,
+            docker_image=docker_image
         )
 
-        provider = Provider(
-            name=name,
-            function="OFFLINE",
-            description=description,
-            team=team,
-            config=config,
-            tags=tags,
-            properties=properties,
-        )
+        provider = Provider(name=name,
+                            function="OFFLINE",
+                            description=description,
+                            team=team,
+                            config=config,
+                            tags=tags,
+                            properties=properties)
         self.__resources.append(provider)
         return OfflineK8sProvider(self, provider)
 
     def register_local(self):
         """Register a Local provider.
 
         **Examples**:
         ```
             local = register_local()
         ```
         Returns:
             local (LocalProvider): Provider
         """
         config = LocalConfig()
-        provider = Provider(
-            name="local-mode",
-            function="LOCAL_ONLINE",
-            description="This is local mode",
-            team="team",
-            config=config,
-            tags=["local-mode"],
-            properties={"resource_type": "Provider"},
-        )
+        provider = Provider(name="local-mode",
+                            function="LOCAL_ONLINE",
+                            description="This is local mode",
+                            team="team",
+                            config=config,
+                            tags=['local-mode'],
+                            properties={"resource_type": "Provider"})
         self.__resources.append(provider)
         local_provider = LocalProvider(self, provider)
         local_provider.insert_provider()
         return local_provider
 
-    def register_primary_data(
-        self,
-        name: str,
-        variant: str,
-        location: Location,
-        provider: Union[str, OfflineProvider],
-        tags: List[str],
-        properties: dict,
-        owner: Union[str, UserRegistrar] = "",
-        description: str = "",
-    ):
+    def register_primary_data(self,
+                              name: str,
+                              variant: str,
+                              location: Location,
+                              provider: Union[str, OfflineProvider],
+                              tags: List[str],
+                              properties: dict,
+                              owner: Union[str, UserRegistrar] = "",
+                              description: str = ""):
         """Register a primary data source.
 
         Args:
             name (str): Name of source
             variant (str): Name of variant
             location (Location): Location of primary data
             provider (Union[str, OfflineProvider]): Provider
@@ -2590,40 +2394,36 @@
         """
         if not isinstance(owner, str):
             owner = owner.name()
         if owner == "":
             owner = self.must_get_default_owner()
         if not isinstance(provider, str):
             provider = provider.name()
-        source = Source(
-            name=name,
-            variant=variant,
-            definition=PrimaryData(location=location),
-            owner=owner,
-            provider=provider,
-            description=description,
-            tags=tags,
-            properties=properties,
-        )
+        source = Source(name=name,
+                        variant=variant,
+                        definition=PrimaryData(location=location),
+                        owner=owner,
+                        provider=provider,
+                        description=description,
+                        tags=tags,
+                        properties=properties)
         self.__resources.append(source)
         return ColumnSourceRegistrar(self, source)
 
-    def register_sql_transformation(
-        self,
-        name: str,
-        variant: str,
-        query: str,
-        provider: Union[str, OfflineProvider],
-        owner: Union[str, UserRegistrar] = "",
-        description: str = "",
-        schedule: str = "",
-        args: K8sArgs = None,
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_sql_transformation(self,
+                                    name: str,
+                                    query: str,
+                                    provider: Union[str, OfflineProvider],
+                                    variant: str = "default",
+                                    owner: Union[str, UserRegistrar] = "",
+                                    description: str = "",
+                                    schedule: str = "",
+                                    args: K8sArgs = None,
+                                    tags: List[str] = [],
+                                    properties: dict = {}):
         """Register a SQL transformation source.
 
         Args:
             name (str): Name of source
             variant (str): Name of variant
             query (str): SQL query
             provider (Union[str, OfflineProvider]): Provider
@@ -2648,31 +2448,29 @@
             variant=variant,
             definition=SQLTransformation(query, args),
             owner=owner,
             schedule=schedule,
             provider=provider,
             description=description,
             tags=tags,
-            properties=properties,
+            properties=properties
         )
         self.__resources.append(source)
         return ColumnSourceRegistrar(self, source)
 
-    def sql_transformation(
-        self,
-        variant: str,
-        provider: Union[str, OfflineProvider],
-        name: str = "",
-        schedule: str = "",
-        owner: Union[str, UserRegistrar] = "",
-        description: str = "",
-        args: K8sArgs = None,
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def sql_transformation(self,
+                           provider: Union[str, OfflineProvider],
+                           variant: str = "default",
+                           name: str = "",
+                           schedule: str = "",
+                           owner: Union[str, UserRegistrar] = "",
+                           description: str = "",
+                           args: K8sArgs = None,
+                           tags: List[str] = [],
+                           properties: dict = {}):
         """SQL transformation decorator.
 
         Args:
             variant (str): Name of variant
             provider (Union[str, OfflineProvider]): Provider
             name (str): Name of source
             schedule (str): Kubernetes CronJob schedule string ("* * * * *")
@@ -2697,33 +2495,31 @@
             variant=variant,
             provider=provider,
             schedule=schedule,
             owner=owner,
             description=description,
             args=args,
             tags=tags,
-            properties=properties,
+            properties=properties
         )
         self.__resources.append(decorator)
         return decorator
 
-    def register_df_transformation(
-        self,
-        name: str,
-        query: str,
-        provider: Union[str, OfflineProvider],
-        variant: str = "default",
-        owner: Union[str, UserRegistrar] = "",
-        description: str = "",
-        inputs: list = [],
-        schedule: str = "",
-        args: K8sArgs = None,
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_df_transformation(self,
+                                   name: str,
+                                   query: str,
+                                   provider: Union[str, OfflineProvider],
+                                   variant: str = "default",
+                                   owner: Union[str, UserRegistrar] = "",
+                                   description: str = "",
+                                   inputs: list = [],
+                                   schedule: str = "",
+                                   args: K8sArgs = None,
+                                   tags: List[str] = [],
+                                   properties: dict = {}):
         """Register a Dataframe transformation source.
 
         Args:
             name (str): Name of source
             variant (str): Name of variant
             query (str): SQL query
             provider (Union[str, OfflineProvider]): Provider
@@ -2753,31 +2549,30 @@
             variant=variant,
             definition=DFTransformation(query, inputs, args),
             owner=owner,
             schedule=schedule,
             provider=provider,
             description=description,
             tags=tags,
-            properties=properties,
+            properties=properties
         )
         self.__resources.append(source)
         return ColumnSourceRegistrar(self, source)
 
-    def df_transformation(
-        self,
-        provider: Union[str, OfflineProvider],
-        tags: List[str],
-        properties: dict,
-        variant: str = "default",
-        name: str = "",
-        owner: Union[str, UserRegistrar] = "",
-        description: str = "",
-        inputs: list = [],
-        args: K8sArgs = None,
-    ):
+    def df_transformation(self,
+                          provider: Union[str, OfflineProvider],
+                          tags: List[str],
+                          properties: dict,
+                          variant: str = "default",
+                          name: str = "",
+                          owner: Union[str, UserRegistrar] = "",
+                          description: str = "",
+                          inputs: list = [],
+                          args: K8sArgs = None
+                          ):
         """Dataframe transformation decorator.
 
         Args:
             variant (str): Name of variant
             provider (Union[str, OfflineProvider]): Provider
             name (str): Name of source
             owner (Union[str, UserRegistrar]): Owner
@@ -2806,49 +2601,87 @@
             variant=variant,
             provider=provider,
             owner=owner,
             description=description,
             inputs=inputs,
             args=args,
             tags=tags,
-            properties=properties,
+            properties=properties
         )
         self.__resources.append(decorator)
         return decorator
 
+    def ondemand_feature(self, 
+                          fn=None, *,
+                          tags: List[str] = None,
+                          properties: dict = None,
+                          variant: str = "default",
+                          name: str = "",
+                          owner: Union[str, UserRegistrar] = "",
+                          description: str = "",
+                          ):
+        """On Demand Feature decorator.
+
+        Args:
+            variant (str): Name of variant
+            name (str): Name of source
+            owner (Union[str, UserRegistrar]): Owner
+            description (str): Description of on demand feature
+            tags (List[str]): Optional grouping mechanism for resources
+            properties (dict): Optional grouping mechanism for resources
+
+        Returns:
+            decorator (OnDemandFeature): decorator
+
+        **Examples**
+        ```python
+        @ff.ondemand_feature()
+        def avg_user_transactions():
+            pass
+        ```
+        """
+
+        if not isinstance(owner, str):
+            owner = owner.name()
+        if owner == "":
+            owner = self.must_get_default_owner()
+    
+        decorator = OnDemandFeature(
+            name=name,
+            variant=variant,
+            owner=owner,
+            description=description,
+            tags=tags or [],
+            properties=properties or {},
+        )
+        self.__resources.append(decorator)
+        
+        if fn is None:
+            return decorator
+        else:
+            return decorator(fn)
+
     def state(self):
         for resource in self.__resources:
             try:
-                if isinstance(resource, SQLTransformationDecorator) or isinstance(
-                    resource, DFTransformationDecorator
-                ):
+                if isinstance(resource, SQLTransformationDecorator) or isinstance(resource, DFTransformationDecorator):
                     resource = resource.to_source()
                 self.__state.add(resource)
             except ResourceRedefinedError:
                 raise
             except Exception as e:
-                resource_variant = (
-                    f" ({resource.variant})" if hasattr(resource, "variant") else ""
-                )
-                raise Exception(
-                    f"Could not add apply {resource.name}{resource_variant}: {e}"
-                )
+                resource_variant = f" ({resource.variant})" if hasattr(resource, 'variant') else ""
+                raise Exception(f"Could not add apply {resource.name}{resource_variant}: {e}")
         self.__resources = []
         return self.__state
 
     def clear_state(self):
         self.__state = ResourceState()
 
-    def register_entity(
-        self,
-        name: str,
-        description: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_entity(self, name: str, description: str = "", tags: List[str] = [], properties: dict = {}):
         """Register an entity.
 
         **Examples**:
         ``` py
             user = ff.register_entity("user")
         ```
         Args:
@@ -2856,33 +2689,30 @@
             description (str): Description of entity to be registered
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             entity (EntityRegistrar): Entity
         """
-        entity = Entity(
-            name=name, description=description, tags=tags, properties=properties
-        )
+        entity = Entity(name=name, description=description, tags=tags, properties=properties)
         self.__resources.append(entity)
         return EntityRegistrar(self, entity)
 
     def register_column_resources(
-        self,
-        source: Union[NameVariant, SourceRegistrar, SQLTransformationDecorator],
-        entity: Union[str, EntityRegistrar],
-        entity_column: str,
-        owner: Union[str, UserRegistrar] = "",
-        inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
-        features: List[ColumnMapping] = None,
-        labels: List[ColumnMapping] = None,
-        timestamp_column: str = "",
-        description: str = "",
-        schedule: str = "",
-    ):
+            self,
+            source: Union[NameVariant, SourceRegistrar, SQLTransformationDecorator],
+            entity: Union[str, EntityRegistrar],
+            entity_column: str,
+            owner: Union[str, UserRegistrar] = "",
+            inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
+            features: List[ColumnMapping] = None,
+            labels: List[ColumnMapping] = None,
+            timestamp_column: str = "",
+            description: str = "",
+            schedule: str = "",):
         """Create features and labels from a source. Used in the register_resources function.
 
         Args:
             source (Union[NameVariant, SourceRegistrar, SQLTransformationDecorator]): Source of features, labels, entity
             entity (Union[str, EntityRegistrar]): Entity
             entity_column (str): Column of entity in source
             owner (Union[str, UserRegistrar]): Owner
@@ -2894,36 +2724,32 @@
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             resource (ResourceRegistrar): resource
         """
 
-        if (
-            type(inference_store) == FileStoreProvider
-            and inference_store.store_type() in NON_INFERENCE_STORES
-        ):
-            raise Exception(
-                f"cannot use '{inference_store.store_type()}' as an inference store."
-            )
+        if type(inference_store) == FileStoreProvider and inference_store.store_type() in NON_INFERENCE_STORES:
+            raise Exception(f"cannot use '{inference_store.store_type()}' as an inference store.")
 
         if features is None:
             features = []
         if labels is None:
             labels = []
         if len(features) == 0 and len(labels) == 0:
             raise ValueError("No features or labels set")
         if not isinstance(source, tuple):
             source = source.id()
         if not isinstance(entity, str):
             entity = entity.name()
         if not isinstance(inference_store, str):
             inference_store = inference_store.name()
         if len(features) > 0 and inference_store == "":
-            raise ValueError("Inference store must be set when defining features")
+            raise ValueError(
+                "Inference store must be set when defining features")
         if not isinstance(owner, str):
             owner = owner.name()
         if owner == "":
             owner = self.must_get_default_owner()
         feature_resources = []
         label_resources = []
         for feature in features:
@@ -2943,15 +2769,15 @@
                 schedule=schedule,
                 location=ResourceColumnMapping(
                     entity=entity_column,
                     value=feature["column"],
                     timestamp=timestamp_column,
                 ),
                 tags=feature_tags,
-                properties=feature_properties,
+                properties=feature_properties
             )
             self.__resources.append(resource)
             feature_resources.append(resource)
 
         for label in labels:
             variant = label.get("variant", "default")
             desc = label.get("description", "")
@@ -2968,15 +2794,15 @@
                 description=desc,
                 location=ResourceColumnMapping(
                     entity=entity_column,
                     value=label["column"],
                     timestamp=timestamp_column,
                 ),
                 tags=label_tags,
-                properties=label_properties,
+                properties=label_properties
             )
             self.__resources.append(resource)
             label_resources.append(resource)
         return ResourceRegistrar(self, features, labels)
 
     def __get_feature_nv(self, features):
         feature_nv_list = []
@@ -2986,35 +2812,28 @@
                 feature_nv = (feature, "default")
                 feature_nv_list.append(feature_nv)
             elif isinstance(feature, dict):
                 lag = feature.get("lag")
                 if lag:
                     required_lag_keys = set(["lag", "feature", "variant"])
                     received_lag_keys = set(feature.keys())
-                    if (
-                        required_lag_keys.intersection(received_lag_keys)
-                        != required_lag_keys
-                    ):
+                    if required_lag_keys.intersection(received_lag_keys) != required_lag_keys:
                         raise ValueError(
-                            f"feature lags require 'lag', 'feature', 'variant' fields. Received: {feature.keys()}"
-                        )
+                            f"feature lags require 'lag', 'feature', 'variant' fields. Received: {feature.keys()}")
 
                     if not isinstance(lag, timedelta):
                         raise ValueError(
-                            f"the lag, '{lag}', needs to be of type 'datetime.timedelta'. Received: {type(lag)}."
-                        )
+                            f"the lag, '{lag}', needs to be of type 'datetime.timedelta'. Received: {type(lag)}.")
 
                     feature_name_variant = (feature["feature"], feature["variant"])
                     if feature_name_variant not in feature_nv_list:
                         feature_nv_list.append(feature_name_variant)
 
                     lag_name = f"{feature['feature']}_{feature['variant']}_lag_{lag}"
-                    sanitized_lag_name = (
-                        lag_name.replace(" ", "").replace(",", "_").replace(":", "_")
-                    )
+                    sanitized_lag_name = lag_name.replace(" ", "").replace(",", "_").replace(":", "_")
                     feature["name"] = feature.get("name", sanitized_lag_name)
 
                     feature_lags.append(feature)
                 else:
                     feature_nv = (feature["name"], feature["variant"])
                     feature_nv_list.append(feature_nv)
             elif isinstance(feature, list):
@@ -3025,27 +2844,25 @@
                 if len(feature_lags_list) != 0:
                     feature_lags.extend(feature_lags_list)
             else:
                 feature_nv_list.append(feature)
 
         return feature_nv_list, feature_lags
 
-    def register_training_set(
-        self,
-        name: str,
-        variant: str = "default",
-        features: list = [],
-        label: NameVariant = (),
-        resources: list = [],
-        owner: Union[str, UserRegistrar] = "",
-        description: str = "",
-        schedule: str = "",
-        tags: List[str] = [],
-        properties: dict = {},
-    ):
+    def register_training_set(self,
+                              name: str,
+                              variant: str = "default",
+                              features: list = [],
+                              label: NameVariant = (),
+                              resources: list = [],
+                              owner: Union[str, UserRegistrar] = "",
+                              description: str = "",
+                              schedule: str = "",
+                              tags: List[str] = [],
+                              properties: dict = {}):
         """Register a training set.
 
         Args:
             name (str): Name of training set to be registered
             variant (str): Name of variant to be registered
             label (NameVariant): Label of training set
             features (List[NameVariant]): Features of training set
@@ -3100,17 +2917,15 @@
             features=features,
             feature_lags=feature_lags,
             tags=tags,
             properties=properties,
         )
         self.__resources.append(resource)
 
-    def register_model(
-        self, name: str, tags: List[str] = [], properties: dict = {}
-    ) -> Model:
+    def register_model(self, name: str, tags: List[str] = [], properties: dict = {}) -> Model:
         """Register a model.
 
         Args:
             name (str): Model to be registered
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
@@ -3118,75 +2933,91 @@
             ModelRegistrar: Model
         """
         model = Model(name, tags=tags, properties=properties)
         self.__resources.append(model)
         return model
 
 
-class ResourceClient(Registrar):
+class ResourceClient:
     """The resource client is used to retrieve information on specific resources (entities, providers, features, labels, training sets, models, users). If retrieved resources are needed to register additional resources (e.g. registering a feature from a source), use the [Client](client.md) functions instead.
 
     **Using the Resource Client:**
     ``` py title="definitions.py"
     import featureform as ff
     from featureform import ResourceClient
 
     rc = ResourceClient("localhost:8000")
 
     # example query:
     redis = rc.get_provider("redis-quickstart")
     ```
     """
 
-    def __init__(
-        self, host=None, local=False, insecure=False, cert_path=None, dry_run=False
-    ):
+    def __init__(self, host=None, local=False, insecure=False, cert_path=None, dry_run=False):
         """Initialise a Resource Client object.
 
         Args:
             host (str): The hostname of the Featureform instance. Exclude if using Localmode.
             local (bool): True if using Localmode.
             insecure (bool): True if connecting to an insecure Featureform endpoint. False if using a self-signed or public TLS certificate
             cert_path (str): The path to a public certificate if using a self-signed certificate.
         """
-        super().__init__()
+        # This line ensures that the warning is only raised if ResourceClient is instantiated directly
+        # TODO: Remove this check once ServingClient is deprecated
+        is_instantiated_directed = inspect.stack()[1].function != "__init__"
+        if is_instantiated_directed:
+            warnings.warn(
+                "ResourceClient is deprecated and will be removed in future versions; use Client instead.",
+                PendingDeprecationWarning,
+            )
         self._dry_run = dry_run
         self._stub = None
         self.local = local
 
         if dry_run:
             return
 
         if local and host:
             raise ValueError("Cannot be local and have a host")
         elif not local:
-            host = host or os.getenv("FEATUREFORM_HOST")
+            host = host or os.getenv('FEATUREFORM_HOST')
             if host is None:
                 raise RuntimeError(
-                    "If not in local mode then `host` must be passed or the environment"
-                    " variable FEATUREFORM_HOST must be set."
+                    'If not in local mode then `host` must be passed or the environment'
+                    ' variable FEATUREFORM_HOST must be set.'
                 )
             if insecure:
                 channel = insecure_channel(host)
             else:
                 channel = secure_channel(host, cert_path)
             self._stub = ff_grpc.ApiStub(channel)
             self._host = host
 
-    def apply(self):
-        """Apply all definitions, creating and retrieving all specified resources."""
+    def apply(self, asynchronous=True):
+        """
+        Apply all definitions, creating and retrieving all specified resources.
 
+        @param asynchronous: Wait for all resources to be ready before returning.
+        """
+        resource_state = state()
         if self._dry_run:
-            print(state().sorted_list())
+            print(resource_state.sorted_list())
             return
 
         if self.local:
-            state().create_all_local()
+            resource_state.create_all_local()
         else:
-            state().create_all(self._stub)
+            resource_state.create_all(self._stub)
+
+        if not asynchronous and self._stub:
+            resources = resource_state.sorted_list()
+            display_statuses(self._stub, resources)
+
+        clear_state()
+
 
     def get_user(self, name, local=False):
         """Get a user. Prints out name of user, and all resources associated with the user.
 
         **Examples:**
 
         ``` py title="Input"
@@ -3410,15 +3241,15 @@
             source=(feature.source.name, feature.source.variant),
             value_type=feature.type,
             entity=feature.entity,
             owner=feature.owner,
             provider=feature.provider,
             location=ResourceColumnMapping("", "", ""),
             description=feature.description,
-            status=feature.status.Status._enum_type.values[feature.status.status].name,
+            status=feature.status.Status._enum_type.values[feature.status.status].name
         )
 
     def print_feature(self, name, variant=None, local=False):
         """Get a feature. Prints out information on feature, and all variants associated with the feature. If variant is included, print information on that specific variant and all resources associated with it.
 
         **Examples:**
 
@@ -3533,15 +3364,15 @@
             source=(label.source.name, label.source.variant),
             value_type=label.type,
             entity=label.entity,
             owner=label.owner,
             provider=label.provider,
             location=ResourceColumnMapping("", "", ""),
             description=label.description,
-            status=label.status.Status._enum_type.values[label.status.status].name,
+            status=label.status.Status._enum_type.values[label.status.status].name
         )
 
     def print_label(self, name, variant=None, local=False):
         """Get a label. Prints out information on label, and all variants associated with the label. If variant is included, print information on that specific variant and all resources associated with it.
 
         **Examples:**
 
@@ -3773,33 +3604,39 @@
             name=source.name,
             definition=definition,
             owner=source.owner,
             provider=source.provider,
             description=source.description,
             variant=source.variant,
             status=source.status.Status._enum_type.values[source.status.status].name,
+            tags=[],
+            properties={}
         )
 
     def _get_source_definition(self, source):
         if source.primaryData.table.name:
-            return PrimaryData(Location(source.primaryData.table.name))
+            return PrimaryData(
+                Location(source.primaryData.table.name)
+            )
         elif source.transformation:
             return self._get_transformation_definition(source)
         else:
             raise Exception(f"Invalid source type {source}")
 
     def _get_transformation_definition(self, source):
         if source.transformation.DFTransformation.query != bytes():
             transformation = source.transformation.DFTransformation
             return DFTransformation(
                 query=transformation.query,
-                inputs=[(input.name, input.variant) for input in transformation.inputs],
+                inputs=[(input.name, input.variant) for input in transformation.inputs]
             )
         elif source.transformation.SQLTransformation.query != "":
-            return SQLTransformation(source.transformation.SQLTransformation.query)
+            return SQLTransformation(
+                source.transformation.SQLTransformation.query
+            )
         else:
             raise Exception(f"Invalid transformation type {source}")
 
     def print_source(self, name, variant=None, local=False):
         """Get a source. Prints out information on source, and all variants associated with the source. If variant is included, print information on that specific variant and all resources associated with it.
 
         **Examples:**
@@ -3947,17 +3784,15 @@
         ]
         ```
 
         Returns:
             features (List[Feature]): List of Feature Objects
         """
         if local:
-            return list_local(
-                "feature", [ColumnName.NAME, ColumnName.VARIANT, ColumnName.STATUS]
-            )
+            return list_local("feature", [ColumnName.NAME, ColumnName.VARIANT, ColumnName.STATUS])
         return list_name_variant_status(self._stub, "feature")
 
     def list_labels(self, local=False):
         """List all labels.
 
         **Examples:**
         ``` py title="Input"
@@ -3990,17 +3825,15 @@
         ]
         ```
 
         Returns:
             labels (List[Label]): List of Label Objects
         """
         if local:
-            return list_local(
-                "label", [ColumnName.NAME, ColumnName.VARIANT, ColumnName.STATUS]
-            )
+            return list_local("label", [ColumnName.NAME, ColumnName.VARIANT, ColumnName.STATUS])
         return list_name_variant_status(self._stub, "label")
 
     def list_users(self, local=False):
         """List all users. Prints a list of all users.
 
         **Examples:**
         ``` py title="Input"
@@ -4154,23 +3987,16 @@
         ]
         ```
 
         Returns:
             sources (List[Source]): List of Source Objects
         """
         if local:
-            return list_local(
-                "source",
-                [
-                    ColumnName.NAME,
-                    ColumnName.VARIANT,
-                    ColumnName.STATUS,
-                    ColumnName.DESCRIPTION,
-                ],
-            )
+            return list_local("source",
+                              [ColumnName.NAME, ColumnName.VARIANT, ColumnName.STATUS, ColumnName.DESCRIPTION])
         return list_name_variant_status_desc(self._stub, "source")
 
     def list_training_sets(self, local=False):
         """List all training sets. Prints a list of all training sets.
 
         **Examples:**
         ``` py title="Input"
@@ -4202,17 +4028,15 @@
         ]
         ```
 
         Returns:
             training_sets (List[TrainingSet]): List of TrainingSet Objects
         """
         if local:
-            return list_local(
-                "training-set", [ColumnName.NAME, ColumnName.VARIANT, ColumnName.STATUS]
-            )
+            return list_local("training-set", [ColumnName.NAME, ColumnName.VARIANT, ColumnName.STATUS])
         return list_name_variant_status_desc(self._stub, "training-set")
 
     def list_models(self, local=False) -> List[Model]:
         """List all models. Prints a list of all models.
 
         Returns:
             models (List[Model]): List of Model Objects
@@ -4220,17 +4044,15 @@
         models = []
         if local:
             rows = list_local("model", [ColumnName.NAME])
             models = [Model(row["name"], tags=[], properties={}) for row in rows]
         else:
             model_protos = list_name(self._stub, "model")
             # TODO: apply values from proto
-            models = [
-                Model(proto.name, tags=[], properties={}) for proto in model_protos
-            ]
+            models = [Model(proto.name, tags=[], properties={}) for proto in model_protos]
 
         return models
 
     def list_providers(self, local=False):
         """List all providers. Prints a list of all providers.
 
         **Examples:**
@@ -4294,17 +4116,15 @@
         ]
         ```
 
         Returns:
             providers (List[Provider]): List of Provider Objects
         """
         if local:
-            return list_local(
-                "provider", [ColumnName.NAME, ColumnName.STATUS, ColumnName.DESCRIPTION]
-            )
+            return list_local("provider", [ColumnName.NAME, ColumnName.STATUS, ColumnName.DESCRIPTION])
         return list_name_status_desc(self._stub, "provider")
 
     def search(self, raw_query, local=False):
         """Search for registered resources. Prints a list of results.
 
         **Examples:**
         ``` py title="Input"
@@ -4316,15 +4136,15 @@
 
         NAME                           VARIANT            TYPE
         avg_transactions               default            Source
         ```
         """
         if type(raw_query) != str or len(raw_query) == 0:
             raise Exception("query must be string and cannot be empty")
-        processed_query = raw_query.translate({ord(i): None for i in ".,-@!*#"})
+        processed_query = raw_query.translate({ ord(i): None for i in '.,-@!*#'})
         if local:
             return search_local(processed_query)
         else:
             return search(processed_query, self._host)
 
 
 class ColumnResource:
@@ -4332,15 +4152,14 @@
     Base class for all column resources. This class is not meant to be instantiated directly.
     In the original syntax, features and labels were registered using the `register_resources`
     method on the sources (e.g. SQL/DF transformation or tables sources); however, in the new
     Class API syntax, features and labels can now be declared as class attributes on an entity
     class. This means that all possible params for either resource must be passed into this base
     class prior to calling `register_column_resources` on the registrar.
     """
-
     def __init__(
         self,
         transformation_args: tuple,
         type: Union[ColumnTypes, str],
         resource_type: str,
         entity: Union[Entity, str],
         variant: str,
@@ -4359,15 +4178,20 @@
         self.entity_column = columns[0]
         self.source_column = columns[1]
         self.resource_type = resource_type
         self.entity = entity
         self.variant = variant
         self.owner = owner
         self.inference_store = inference_store
-        self.timestamp_column = timestamp_column
+        if not timestamp_column and len(columns) == 3:
+            self.timestamp_column = columns[2]
+        elif timestamp_column and len(columns) == 3:
+            raise Exception("Timestamp column specified twice.")
+        else:
+            self.timestamp_column = timestamp_column
         self.description = description
         self.schedule = schedule
         self.tags = tags
         self.properties = properties
 
     def register(self):
         features, labels = self.features_and_labels()
@@ -4379,27 +4203,25 @@
             owner=self.owner,
             inference_store=self.inference_store,
             features=features,
             labels=labels,
             timestamp_column=self.timestamp_column,
             schedule=self.schedule,
         )
-
+    
     def features_and_labels(self) -> Tuple[List[ColumnMapping], List[ColumnMapping]]:
-        resources = [
-            {
-                "name": self.name,
-                "variant": self.variant,
-                "column": self.source_column,
-                "type": self.type,
-                "description": self.description,
-                "tags": self.tags,
-                "properties": self.properties,
-            }
-        ]
+        resources = [{
+            "name": self.name,
+            "variant": self.variant,
+            "column": self.source_column,
+            "type": self.type,
+            "description": self.description,
+            "tags": self.tags,
+            "properties": self.properties,
+        }]
         if self.resource_type == "feature":
             features = resources
             labels = []
         elif self.resource_type == "label":
             features = []
             labels = resources
         else:
@@ -4410,86 +4232,78 @@
 class Variants:
     def __init__(self, resources: Dict[str, ColumnResource]):
         self.resources = resources
         self.validate_variant_names()
 
     def validate_variant_names(self):
         for variant_key, resource in self.resources.items():
-            if resource.variant is "default":
+            if resource.variant == "default":
                 resource.variant = variant_key
             if resource.variant != variant_key:
                 raise ValueError(
                     f"Variant name {variant_key} does not match resource variant name {resource.variant}"
                 )
 
     def register(self):
         for resource in self.resources.values():
             resource.register()
 
 
 class FeatureColumnResource(ColumnResource):
-    def __init__(
-        self,
-        transformation_args: tuple,
-        type: Union[ColumnTypes, str],
-        entity: Union[Entity, str] = "",
-        variant="default",
-        owner: str = "",
-        inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
-        timestamp_column: str = "",
-        description: str = "",
-        schedule: str = "",
-        tags: List[str] = [],
-        properties: Dict[str, str] = {},
-    ):
-        super().__init__(
-            transformation_args=transformation_args,
-            type=type,
-            resource_type="feature",
-            entity=entity,
-            variant=variant,
-            owner=owner,
-            inference_store=inference_store,
-            timestamp_column=timestamp_column,
-            description=description,
-            schedule=schedule,
-            tags=tags,
-            properties=properties,
-        )
+    def __init__(self,
+                 transformation_args: tuple,
+                 type: Union[ColumnTypes, str],
+                 entity: Union[Entity, str] = "",
+                 variant="default",
+                 owner: str = "",
+                 inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
+                 timestamp_column: str = "",
+                 description: str = "",
+                 schedule: str = "",
+                 tags: List[str] = [],
+                 properties: Dict[str, str] = {}):
+        super().__init__(transformation_args=transformation_args,
+                            type=type,
+                            resource_type="feature",
+                            entity=entity,
+                            variant=variant,
+                            owner=owner,
+                            inference_store=inference_store,
+                            timestamp_column=timestamp_column,
+                            description=description,
+                            schedule=schedule,
+                            tags=tags,
+                            properties=properties)
 
 
 class LabelColumnResource(ColumnResource):
-    def __init__(
-        self,
-        transformation_args: tuple,
-        type: Union[ColumnTypes, str],
-        entity: Union[Entity, str] = "",
-        variant="default",
-        owner: str = "",
-        inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
-        timestamp_column: str = "",
-        description: str = "",
-        schedule: str = "",
-        tags: List[str] = [],
-        properties: Dict[str, str] = {},
-    ):
-        super().__init__(
-            transformation_args=transformation_args,
-            type=type,
-            resource_type="label",
-            entity=entity,
-            variant=variant,
-            owner=owner,
-            inference_store=inference_store,
-            timestamp_column=timestamp_column,
-            description=description,
-            schedule=schedule,
-            tags=tags,
-            properties=properties,
-        )
+    def __init__(self,
+                 transformation_args: tuple,
+                 type: Union[ColumnTypes, str],
+                 entity: Union[Entity, str] = "",
+                 variant="default",
+                 owner: str = "",
+                 inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
+                 timestamp_column: str = "",
+                 description: str = "",
+                 schedule: str = "",
+                 tags: List[str] = [],
+                 properties: Dict[str, str] = {}):
+        super().__init__(transformation_args=transformation_args,
+                            type=type,
+                            resource_type="label",
+                            entity=entity,
+                            variant=variant,
+                            owner=owner,
+                            inference_store=inference_store,
+                            timestamp_column=timestamp_column,
+                            description=description,
+                            schedule=schedule,
+                            tags=tags,
+                            properties=properties)
 
 
 def entity(cls):
     """
     Class decorator for registering entities and their associated features and labels.
 
     **Examples**
@@ -4556,21 +4370,23 @@
 get_entity = global_registrar.get_entity
 get_source = global_registrar.get_source
 get_local_provider = global_registrar.get_local_provider
 get_redis = global_registrar.get_redis
 get_postgres = global_registrar.get_postgres
 get_mongodb = global_registrar.get_mongodb
 get_snowflake = global_registrar.get_snowflake
+get_snowflake_legacy = global_registrar.get_snowflake_legacy
 get_redshift = global_registrar.get_redshift
 get_bigquery = global_registrar.get_bigquery
 get_spark = global_registrar.get_spark
 get_kubernetes = global_registrar.get_kubernetes
 get_blob_store = global_registrar.get_blob_store
 get_s3 = global_registrar.get_s3
 get_gcs = global_registrar.get_gcs
+ondemand_feature = global_registrar.ondemand_feature
 ResourceStatus = ResourceStatus
 
 
 Nil = ColumnTypes.NIL
 String = ColumnTypes.STRING
 Int = ColumnTypes.INT
 Int32 = ColumnTypes.INT32
```

### Comparing `featureform-1.7.3rc5/src/featureform/register_test.py` & `featureform-1.7.4/src/featureform/register_test.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/resources.py` & `featureform-1.7.4/src/featureform/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,36 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import sys
 import json
 import time
-import datetime
+import base64
 from enum import Enum
 from typeguard import typechecked
-from typing import List, Tuple, Union
+from typing import List, Tuple, Union, Optional
 
+import dill
 import grpc
 from .sqlite_metadata import SQLiteMetadata
 from google.protobuf.duration_pb2 import Duration
 
 from featureform.proto import metadata_pb2 as pb
 from dataclasses import dataclass, field
 from .version import check_up_to_date
+from .exceptions import *
+from .enums import *
 
 NameVariant = Tuple[str, str]
 
 
 # Constants for Pyspark Versions
 MAJOR_VERSION = "3"
-MINOR_VERSIONS = ["7", "8", "9", "10"]
-
-
-class ColumnTypes(Enum):
-    NIL = ""
-    INT = "int"
-    INT32 = "int32"
-    INT64 = "int64"
-    FLOAT32 = "float32"
-    FLOAT64 = "float64"
-    STRING = "string"
-    BOOL = "bool"
-    DATETIME = "datetime"
-
-
-class ResourceStatus(Enum):
-    NO_STATUS = "NO_STATUS"
-    CREATED = "CREATED"
-    PENDING = "PENDING"
-    READY = "READY"
-    FAILED = "FAILED"
-
-
-@typechecked
-@dataclass
-class OperationType(Enum):
-    GET = 0
-    CREATE = 1
-
-
-@typechecked
-@dataclass
-class SourceType(Enum):
-    PRIMARY_SOURCE = "PRIMARY"
-    DF_TRANSFORMATION = "DF"
-    SQL_TRANSFORMATION = "SQL"
-
-
-@typechecked
-@dataclass
-class FilePrefix(Enum):
-    S3 = "s3://"
-    S3A = "s3a://"
+MINOR_VERSIONS = ["7", "8", "9", "10", "11"]
 
 
 @typechecked
 def valid_name_variant(nvar: NameVariant) -> bool:
     return nvar[0] != "" and nvar[1] != ""
 
 
@@ -86,20 +47,16 @@
         return OperationType.CREATE
 
     def type(self) -> str:
         return "schedule"
 
     def _create(self, stub) -> None:
         serialized = pb.SetScheduleChangeRequest(
-            resource=pb.ResourceId(
-                pb.NameVariant(name=self.name, variant=self.variant),
-                resource_type=self.resource_type,
-            ),
-            schedule=self.schedule_string,
-        )
+            resource=pb.ResourceId(pb.NameVariant(name=self.name, variant=self.variant),
+                                   resource_type=self.resource_type), schedule=self.schedule_string)
         stub.RequestScheduleChange(serialized)
 
 
 @typechecked
 @dataclass
 class RedisConfig:
     host: str
@@ -121,24 +78,20 @@
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class AWSCredentials:
-    def __init__(
-        self,
-        aws_access_key_id: str = "",
-        aws_secret_access_key: str = "",
-    ):
+    def __init__(self,
+                 aws_access_key_id: str = "",
+                 aws_secret_access_key: str = "",):
         empty_strings = aws_access_key_id == "" or aws_secret_access_key == ""
         if empty_strings:
-            raise Exception(
-                "'AWSCredentials' requires all parameters: 'aws_access_key_id', 'aws_secret_access_key'"
-            )
+            raise Exception("'AWSCredentials' requires all parameters: 'aws_access_key_id', 'aws_secret_access_key'")
 
         self.aws_access_key_id = aws_access_key_id
         self.aws_secret_access_key = aws_secret_access_key
 
     def type(self):
         return "AWS_CREDENTIALS"
 
@@ -148,19 +101,18 @@
             "AWSSecretKey": self.aws_secret_access_key,
         }
 
 
 @typechecked
 @dataclass
 class GCPCredentials:
-    def __init__(
-        self,
-        project_id: str,
-        credentials_path: str,
-    ):
+    def __init__(self,
+                 project_id: str,
+                 credentials_path: str,):
+
         self.project_id = project_id
         self.credentials = json.load(open(credentials_path))
 
     def type(self):
         return "GCPCredentials"
 
     def config(self):
@@ -236,55 +188,58 @@
     def store_type(self):
         return self.type()
 
 
 @typechecked
 @dataclass
 class S3StoreConfig:
-    def __init__(
-        self, bucket_path: str, bucket_region: str, credentials: AWSCredentials
-    ):
+    def __init__(self, 
+                 bucket_path: str,
+                 bucket_region: str,
+                 credentials: AWSCredentials,
+                 path: str = ""):
         bucket_path_ends_with_slash = len(bucket_path) != 0 and bucket_path[-1] == "/"
 
         if bucket_path_ends_with_slash:
             raise Exception("The 'bucket_path' cannot end with '/'.")
-
+                 
         self.bucket_path = bucket_path
         self.bucket_region = bucket_region
         self.credentials = credentials
+        self.path = path
 
     def software(self) -> str:
         return "S3"
 
     def type(self) -> str:
         return "S3"
 
     def serialize(self) -> bytes:
-        config = {
-            "Credentials": self.credentials.config(),
-            "BucketRegion": self.bucket_region,
-            "BucketPath": self.bucket_path,
-        }
+        config = self.config()
         return bytes(json.dumps(config), "utf-8")
 
     def config(self):
         return {
             "Credentials": self.credentials.config(),
             "BucketRegion": self.bucket_region,
             "BucketPath": self.bucket_path,
+            "Path": self.path,
         }
-
+    
     def store_type(self):
         return self.type()
 
-
 @typechecked
 @dataclass
 class HDFSConfig:
-    def __init__(self, host: str, port: str, path: str, username: str):
+    def __init__(self,
+                 host: str,
+                 port: str,
+                 path: str,
+                 username: str):
         bucket_path_ends_with_slash = len(path) != 0 and path[-1] == "/"
 
         if bucket_path_ends_with_slash:
             raise Exception("The 'bucket_path' cannot end with '/'.")
 
         self.path = path
         self.host = host
@@ -298,24 +253,24 @@
         return "HDFS"
 
     def serialize(self) -> bytes:
         config = {
             "Host": self.host,
             "Port": self.port,
             "Path": self.path,
-            "Username": self.username,
+            "Username": self.username
         }
         return bytes(json.dumps(config), "utf-8")
 
     def config(self):
         return {
             "Host": self.host,
             "Port": self.port,
             "Path": self.path,
-            "Username": self.username,
+            "Username": self.username
         }
 
     def store_type(self):
         return self.type()
 
 
 @typechecked
@@ -383,15 +338,15 @@
     def serialize(self) -> bytes:
         config = {
             "Keyspace": self.keyspace,
             "Addr": f"{self.host}:{self.port}",
             "Username": self.username,
             "Password": self.password,
             "Consistency": self.consistency,
-            "Replication": self.replication,
+            "Replication": self.replication
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class DynamodbConfig:
@@ -405,15 +360,15 @@
     def type(self) -> str:
         return "DYNAMODB_ONLINE"
 
     def serialize(self) -> bytes:
         config = {
             "Region": self.region,
             "AccessKey": self.access_key,
-            "SecretKey": self.secret_key,
+            "SecretKey": self.secret_key
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class MongoDBConfig:
@@ -433,30 +388,32 @@
     def serialize(self) -> bytes:
         config = {
             "Username": self.username,
             "Password": self.password,
             "Host": self.host,
             "Port": self.port,
             "Database": self.database,
-            "Throughput": self.throughput,
+            "Throughput": self.throughput
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class LocalConfig:
+
     def software(self) -> str:
         return "localmode"
 
     def type(self) -> str:
         return "LOCAL_ONLINE"
 
     def serialize(self) -> bytes:
-        config = {}
+        config = {
+        }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class SnowflakeConfig:
     username: str
@@ -467,28 +424,24 @@
     database: str = ""
     account_locator: str = ""
     warehouse: str = ""
     role: str = ""
 
     def __post_init__(self):
         if self.__has_legacy_credentials() and self.__has_current_credentials():
-            raise ValueError(
-                "Cannot create configure Snowflake with both current and legacy credentials"
-            )
+            raise ValueError("Cannot create configure Snowflake with both current and legacy credentials")
 
         if not self.__has_legacy_credentials() and not self.__has_current_credentials():
             raise ValueError("Cannot create configure Snowflake without credentials")
 
     def __has_legacy_credentials(self) -> bool:
         return self.account_locator != ""
 
     def __has_current_credentials(self) -> bool:
-        if (self.account != "" and self.organization == "") or (
-            self.account == "" and self.organization != ""
-        ):
+        if (self.account != "" and self.organization == "") or (self.account == "" and self.organization != ""):
             raise ValueError("Both Snowflake organization and account must be included")
         elif self.account != "" and self.organization != "":
             return True
         else:
             return False
 
     def software(self) -> str:
@@ -503,15 +456,15 @@
             "Password": self.password,
             "Organization": self.organization,
             "AccountLocator": self.account_locator,
             "Account": self.account,
             "Schema": self.schema,
             "Database": self.database,
             "Warehouse": self.warehouse,
-            "Role": self.role,
+            "Role": self.role
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class PostgresConfig:
@@ -605,38 +558,34 @@
             "ExecutorType": self.executor_type,
             "StoreType": self.store_type,
             "ExecutorConfig": self.executor_config,
             "StoreConfig": self.store_config,
         }
         return bytes(json.dumps(config), "utf-8")
 
-
 @typechecked
 @dataclass
 class K8sResourceSpecs:
     cpu_request: str = ""
     cpu_limit: str = ""
     memory_request: str = ""
     memory_limit: str = ""
 
-
 @typechecked
 @dataclass
 class K8sArgs:
     docker_image: str
     specs: Union[K8sResourceSpecs, None] = None
 
     def apply(self, transformation: pb.Transformation):
         transformation.kubernetes_args.docker_image = self.docker_image
         if self.specs is not None:
             transformation.kubernetes_args.specs.cpu_request = self.specs.cpu_request
             transformation.kubernetes_args.specs.cpu_limit = self.specs.cpu_limit
-            transformation.kubernetes_args.specs.memory_request = (
-                self.specs.memory_request
-            )
+            transformation.kubernetes_args.specs.memory_request = self.specs.memory_request
             transformation.kubernetes_args.specs.memory_limit = self.specs.memory_limit
         return transformation
 
 
 @typechecked
 @dataclass
 class K8sConfig:
@@ -649,40 +598,42 @@
 
     def type(self) -> str:
         return "K8S_OFFLINE"
 
     def serialize(self) -> bytes:
         config = {
             "ExecutorType": "K8S",
-            "ExecutorConfig": {"docker_image": self.docker_image},
+            "ExecutorConfig": {
+                "docker_image": self.docker_image
+            },
             "StoreType": self.store_type,
             "StoreConfig": self.store_config,
         }
         return bytes(json.dumps(config), "utf-8")
 
 
+@typechecked
+@dataclass
+class EmptyConfig:
+    def software(self) -> str:
+        return ""
+
+    def type(self) -> str:
+        return ""
+
+    def serialize(self) -> bytes:
+        return bytes("", "utf-8")
+
+
 Config = Union[
-    RedisConfig,
-    SnowflakeConfig,
-    PostgresConfig,
-    RedshiftConfig,
-    LocalConfig,
-    BigQueryConfig,
-    FirestoreConfig,
-    SparkConfig,
-    OnlineBlobConfig,
-    AzureFileStoreConfig,
-    S3StoreConfig,
-    K8sConfig,
-    MongoDBConfig,
-    GCSFileStoreConfig,
-    HDFSConfig,
+    RedisConfig, SnowflakeConfig, PostgresConfig, RedshiftConfig, LocalConfig, BigQueryConfig,
+    FirestoreConfig, SparkConfig, OnlineBlobConfig, AzureFileStoreConfig, S3StoreConfig, K8sConfig,
+    MongoDBConfig, GCSFileStoreConfig, EmptyConfig
 ]
 
-
 @typechecked
 @dataclass
 class Properties:
     properties: dict
 
     def __post_init__(self):
         self.serialized = pb.Properties()
@@ -690,64 +641,79 @@
             self.serialized.property[key].string_value = val
 
 
 @typechecked
 @dataclass
 class Provider:
     name: str
-    function: str
-    config: Config
     description: str
     team: str
-    tags: list
-    properties: dict
+    config: Config
+    function: str
+    status: str = "NO_STATUS"
+    tags: list = None
+    properties: dict = None
+    error: Optional[str] = None
 
     def __post_init__(self):
-        self.software = self.config.software()
+        self.software = self.config.software() if self.config is not None else None
 
     @staticmethod
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     @staticmethod
     def type() -> str:
         return "provider"
 
+    def get(self, stub) -> 'Provider':
+        name = pb.Name(name=self.name)
+        provider = next(stub.GetProviders(iter([name])))
+
+        return Provider(
+            name=provider.name,
+            description=provider.description,
+            function=provider.type,
+            team=provider.team,
+            config=EmptyConfig(),  # TODO add deserializer to configs
+            tags=list(provider.tags.tag),
+            properties={k: v for k, v in provider.properties.property.items()},
+            status=provider.status.Status._enum_type.values[provider.status.status].name,
+            error=provider.status.error_message
+        )
+
     def _create(self, stub) -> None:
         serialized = pb.Provider(
             name=self.name,
             description=self.description,
             type=self.config.type(),
             software=self.config.software(),
             team=self.team,
             serialized_config=self.config.serialize(),
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateProvider(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert(
-            "providers",
-            self.name,
-            "Provider",
-            self.description,
-            self.config.type(),
-            self.config.software(),
-            self.team,
-            "sources",
-            "ready",
-            str(self.config.serialize(), "utf-8"),
-        )
+        db.insert("providers",
+                  self.name,
+                  "Provider",
+                  self.description,
+                  self.config.type(),
+                  self.config.software(),
+                  self.team,
+                  "sources",
+                  "ready",
+                  str(self.config.serialize(), 'utf-8')
+                  )
         if len(self.tags):
             db.upsert("tags", self.name, "", "providers", json.dumps(self.tags))
         if len(self.properties):
-            db.upsert(
-                "properties", self.name, "", "providers", json.dumps(self.properties)
-            )
+            db.upsert("properties", self.name, "", "providers", json.dumps(self.properties))
 
     def __eq__(self, other):
         for attribute in vars(self):
             if getattr(self, attribute) != getattr(other, attribute):
                 return False
         return True
 
@@ -771,15 +737,19 @@
             name=self.name,
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateUser(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert("users", self.name, "User", "ready")
+        db.insert("users",
+                  self.name,
+                  "User",
+                  "ready"
+                  )
         if len(self.tags):
             db.upsert("tags", self.name, "", "users", json.dumps(self.tags))
         if len(self.properties):
             db.upsert("properties", self.name, "", "users", json.dumps(self.properties))
 
     def __eq__(self, other):
         for attribute in vars(self):
@@ -800,19 +770,17 @@
 @typechecked
 @dataclass
 class PrimaryData:
     location: Location
 
     def kwargs(self):
         return {
-            "primaryData": pb.PrimaryData(
-                table=pb.PrimarySQLTable(
-                    name=self.location.name,
-                ),
-            ),
+            "primaryData":
+                pb.PrimaryData(table=pb.PrimarySQLTable(
+                    name=self.location.name, ), ),
         }
 
     def name(self):
         return self.location.name
 
 
 class Transformation:
@@ -834,15 +802,17 @@
                 query=self.query,
             )
         )
 
         if self.args is not None:
             transformation = self.args.apply(transformation)
 
-        return {"transformation": transformation}
+        return {
+            "transformation": transformation
+        }
 
 
 @typechecked
 @dataclass
 class DFTransformation(Transformation):
     query: bytes
     inputs: list
@@ -851,22 +821,24 @@
     def type(self):
         return SourceType.DF_TRANSFORMATION.value
 
     def kwargs(self):
         transformation = pb.Transformation(
             DFTransformation=pb.DFTransformation(
                 query=self.query,
-                inputs=[pb.NameVariant(name=v[0], variant=v[1]) for v in self.inputs],
+                inputs=[pb.NameVariant(name=v[0], variant=v[1]) for v in self.inputs]
             )
         )
-
+        
         if self.args is not None:
             transformation = self.args.apply(transformation)
 
-        return {"transformation": transformation}
+        return {
+            "transformation": transformation
+        }
 
 
 SourceDefinition = Union[PrimaryData, Transformation]
 
 
 @typechecked
 @dataclass
@@ -874,38 +846,76 @@
     name: str
     definition: SourceDefinition
     owner: str
     provider: str
     description: str
     tags: list
     properties: dict
+    status: str = "NO_STATUS"
     variant: str = "default"
     schedule: str = ""
     schedule_obj: Schedule = None
     is_transformation = SourceType.PRIMARY_SOURCE.value
-    inputs = ([],)
-    status: str = "NO_STATUS"
+    inputs = [],
+    error: Optional[str] = None
 
     def update_schedule(self, schedule) -> None:
-        self.schedule_obj = Schedule(
-            name=self.name,
-            variant=self.variant,
-            resource_type=7,
-            schedule_string=schedule,
-        )
+        self.schedule_obj = Schedule(name=self.name, variant=self.variant, resource_type=7, schedule_string=schedule)
         self.schedule = schedule
 
     @staticmethod
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     @staticmethod
     def type() -> str:
         return "source"
 
+    def get(self, stub):
+        name_variant = pb.NameVariant(name=self.name, variant=self.variant)
+        source = next(stub.GetSourceVariants(iter([name_variant])))
+        definition = self._get_source_definition(source)
+
+        return Source(
+            name=source.name,
+            definition=definition,
+            owner=source.owner,
+            provider=source.provider,
+            description=source.description,
+            variant=source.variant,
+            tags=list(source.tags.tag),
+            properties={k: v for k, v in source.properties.property.items()},
+            status=source.status.Status._enum_type.values[source.status.status].name,
+            error=source.status.error_message,
+        )
+
+    def _get_source_definition(self, source):
+        if source.primaryData.table.name:
+            return PrimaryData(
+                Location(source.primaryData.table.name)
+            )
+        elif source.transformation:
+            return self._get_transformation_definition(source)
+        else:
+            raise Exception(f"Invalid source type {source}")
+
+    def _get_transformation_definition(self, source):
+        if source.transformation.DFTransformation.query != bytes():
+            transformation = source.transformation.DFTransformation
+            return DFTransformation(
+                query=transformation.query,
+                inputs=[(input.name, input.variant) for input in transformation.inputs]
+            )
+        elif source.transformation.SQLTransformation.query != "":
+            return SQLTransformation(
+                source.transformation.SQLTransformation.query
+            )
+        else:
+            raise Exception(f"Invalid transformation type {source}")
+
     def _create(self, stub) -> None:
         defArgs = self.definition.kwargs()
         serialized = pb.SourceVariant(
             name=self.name,
             variant=self.variant,
             owner=self.owner,
             description=self.description,
@@ -924,44 +934,40 @@
             self.definition = self.definition.query
         elif type(self.definition) == SQLTransformation:
             self.is_transformation = SourceType.SQL_TRANSFORMATION.value
             self.definition = self.definition.query
         elif type(self.definition) == PrimaryData:
             self.definition = self.definition.name()
             self.is_transformation = SourceType.PRIMARY_SOURCE.value
-        db.insert_source(
-            "source_variant",
-            str(time.time()),
-            self.description,
-            self.name,
-            "Source",
-            self.owner,
-            self.provider,
-            self.variant,
-            "ready",
-            self.is_transformation,
-            json.dumps(self.inputs),
-            self.definition,
-        )
+        db.insert_source("source_variant",
+                         str(time.time()),
+                         self.description,
+                         self.name,
+                         "Source",
+                         self.owner,
+                         self.provider,
+                         self.variant,
+                         "ready",
+                         self.is_transformation,
+                         json.dumps(self.inputs),
+                         self.definition
+                         )
         if len(self.tags):
-            db.upsert(
-                "tags", self.name, self.variant, "source_variant", json.dumps(self.tags)
-            )
+            db.upsert("tags", self.name, self.variant, "source_variant", json.dumps(self.tags))
         if len(self.properties):
-            db.upsert(
-                "properties",
-                self.name,
-                self.variant,
-                "source_variant",
-                json.dumps(self.properties),
-            )
+            db.upsert("properties", self.name, self.variant, "source_variant", json.dumps(self.properties))
         self._create_source_resource(db)
 
     def _create_source_resource(self, db) -> None:
-        db.insert("sources", "Source", self.variant, self.name)
+        db.insert(
+            "sources",
+            "Source",
+            self.variant,
+            self.name
+        )
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_ready(self):
         return self.status == ResourceStatus.READY.value
 
@@ -994,21 +1000,24 @@
             description=self.description,
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateEntity(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert("entities", self.name, "Entity", self.description, "ready")
+        db.insert("entities",
+                  self.name,
+                  "Entity",
+                  self.description,
+                  "ready"
+                  )
         if len(self.tags):
             db.upsert("tags", self.name, "", "entities", json.dumps(self.tags))
         if len(self.properties):
-            db.upsert(
-                "properties", self.name, "", "entities", json.dumps(self.properties)
-            )
+            db.upsert("properties", self.name, "", "entities", json.dumps(self.properties))
 
     def __eq__(self, other):
         for attribute in vars(self):
             if getattr(self, attribute) != getattr(other, attribute):
                 return False
         return True
 
@@ -1038,45 +1047,59 @@
     source: NameVariant
     value_type: str
     entity: str
     owner: str
     provider: str
     location: ResourceLocation
     description: str
-    tags: list
-    properties: dict
+    tags: list = None
+    properties: dict = None
     variant: str = "default"
     schedule: str = ""
     schedule_obj: Schedule = None
     status: str = "NO_STATUS"
+    error: Optional[str] = None
 
     def __post_init__(self):
         col_types = [member.value for member in ColumnTypes]
         if self.value_type not in col_types:
-            raise ValueError(
-                f"Invalid feature type ({self.value_type}) must be one of: {col_types}"
-            )
+            raise ValueError(f"Invalid feature type ({self.value_type}) must be one of: {col_types}")
 
     def update_schedule(self, schedule) -> None:
-        self.schedule_obj = Schedule(
-            name=self.name,
-            variant=self.variant,
-            resource_type=4,
-            schedule_string=schedule,
-        )
+        self.schedule_obj = Schedule(name=self.name, variant=self.variant, resource_type=4, schedule_string=schedule)
         self.schedule = schedule
 
     @staticmethod
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     @staticmethod
     def type() -> str:
         return "feature"
 
+    def get(self, stub) -> "Feature":
+        name_variant = pb.NameVariant(name=self.name, variant=self.variant)
+        feature = next(stub.GetFeatureVariants(iter([name_variant])))
+
+        return Feature(
+            name=feature.name,
+            variant=feature.variant,
+            source=(feature.source.name, feature.source.variant),
+            value_type=feature.type,
+            entity=feature.entity,
+            owner=feature.owner,
+            provider=feature.provider,
+            location=ResourceColumnMapping("", "", ""),
+            description=feature.description,
+            tags=list(feature.tags.tag),
+            properties={k: v for k, v in feature.properties.property.items()},
+            status=feature.status.Status._enum_type.values[feature.status.status].name,
+            error=feature.status.error_message,
+        )
+
     def _create(self, stub) -> None:
         serialized = pb.FeatureVariant(
             name=self.name,
             variant=self.variant,
             source=pb.NameVariant(
                 name=self.source[0],
                 variant=self.source[1],
@@ -1084,57 +1107,170 @@
             type=self.value_type,
             entity=self.entity,
             owner=self.owner,
             description=self.description,
             schedule=self.schedule,
             provider=self.provider,
             columns=self.location.proto(),
+            mode=ComputationMode.PRECOMPUTED.proto(),
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateFeatureVariant(serialized)
 
     def _create_local(self, db) -> None:
+        db.insert("feature_variant",
+                  str(time.time()),
+                  self.description,
+                  self.entity,
+                  self.name,
+                  self.owner,
+                  self.provider,
+                  self.value_type,
+                  self.variant,
+                  "ready",
+                  self.location.entity,
+                  self.location.timestamp,
+                  self.location.value,
+                  self.source[0],
+                  self.source[1]
+                  )
+        if len(self.tags):
+            db.upsert("tags", self.name, self.variant, "feature_variant", json.dumps(self.tags))
+        if len(self.properties):
+            db.upsert("properties", self.name, self.variant, "feature_variant", json.dumps(self.properties))
+
+        self._write_feature_variant_and_mode(db)
+
+    def _write_feature_variant_and_mode(self, db) -> None:
         db.insert(
-            "feature_variant",
-            str(time.time()),
-            self.description,
-            self.entity,
+            "features",
             self.name,
-            self.owner,
-            self.provider,
+            self.variant,
             self.value_type,
+        )
+        is_on_demand = 0
+        db.insert(
+            "feature_computation_mode",
+            self.name,
             self.variant,
-            "ready",
-            self.location.entity,
-            self.location.timestamp,
-            self.location.value,
-            self.source[0],
-            self.source[1],
+            ComputationMode.PRECOMPUTED.value,
+            is_on_demand,
         )
-        if len(self.tags):
-            db.upsert(
-                "tags",
-                self.name,
-                self.variant,
-                "feature_variant",
-                json.dumps(self.tags),
-            )
+
+    def get_status(self):
+        return ResourceStatus(self.status)
+
+    def is_ready(self):
+        return self.status == ResourceStatus.READY.value
+
+    def __eq__(self, other):
+        for attribute in vars(self):
+            if getattr(self, attribute) != getattr(other, attribute):
+                return False
+        return True
+
+@typechecked
+@dataclass
+class OnDemandFeature:
+    owner: str
+    tags: List[str] = field(default_factory=list)
+    properties: dict = field(default_factory=dict)
+    variant: str = "default"
+    name: str = ""
+    description: str = ""
+    status: str = "READY"
+    error: Optional[str] = None
+
+    def __call__(self, fn):
+        if self.description == "" and fn.__doc__ is not None:
+            self.description = fn.__doc__
+        if self.name == "":
+            self.name = fn.__name__
+
+        self.query = dill.dumps(fn.__code__)
+        fn.name_variant = self.name_variant
+        fn.query = self.query
+        return fn
+
+    def name_variant(self):
+        return (self.name, self.variant)
+
+    @staticmethod
+    def operation_type() -> OperationType:
+        return OperationType.CREATE
+
+    @staticmethod
+    def type() -> str:
+        return "ondemand_feature"
+
+    def _create(self, stub) -> None:
+        serialized = pb.FeatureVariant(
+            name=self.name,
+            variant=self.variant,
+            owner=self.owner,
+            description=self.description,
+            function=pb.PythonFunction(query=self.query),
+            mode=ComputationMode.CLIENT_COMPUTED.proto(),
+            tags=pb.Tags(tag=self.tags),
+            properties=Properties(self.properties).serialized,
+            status=pb.ResourceStatus(status=pb.ResourceStatus.READY),
+        )
+        stub.CreateFeatureVariant(serialized)
+
+    def _create_local(self, db) -> None:
+        decode_query = base64.b64encode(self.query).decode("ascii")
+
+        db.insert("ondemand_feature_variant",
+                  str(time.time()),
+                  self.description,
+                  self.name,
+                  self.owner,
+                  self.variant,
+                  "ready",
+                  decode_query,
+                  )
+        if self.tags and len(self.tags):
+            db.upsert("tags", self.name, self.variant, "feature_variant", json.dumps(self.tags))
         if len(self.properties):
-            db.upsert(
-                "properties",
-                self.name,
-                self.variant,
-                "feature_variant",
-                json.dumps(self.properties),
-            )
-        self._create_feature_resource(db)
+            db.upsert("properties", self.name, self.variant, "feature_variant", json.dumps(self.properties))
+
+        self._write_feature_variant_and_mode(db)
 
-    def _create_feature_resource(self, db) -> None:
-        db.insert("features", self.name, self.variant, self.value_type)
+    def _write_feature_variant_and_mode(self, db) -> None:
+        db.insert(
+            "features",
+            self.name,
+            self.variant,
+            "tbd",
+        )
+        is_on_demand = 1
+
+        db.insert(
+            "feature_computation_mode",
+            self.name,
+            self.variant,
+            ComputationMode.CLIENT_COMPUTED.value,
+            is_on_demand,
+        )
+    
+    def get(self, stub) -> "OnDemandFeature":
+        name_variant = pb.NameVariant(name=self.name, variant=self.variant)
+        ondemand_feature = next(stub.GetFeatureVariants(iter([name_variant])))
+
+        return OnDemandFeature(
+            name=ondemand_feature.name,
+            variant=ondemand_feature.variant,
+            owner=ondemand_feature.owner,
+            description=ondemand_feature.description,
+            tags=list(ondemand_feature.tags.tag),
+            properties={k: v for k, v in ondemand_feature.properties.property.items()},
+            status=ondemand_feature.status.Status._enum_type.values[ondemand_feature.status.status].name,
+            error=ondemand_feature.status.error_message,
+        )
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_ready(self):
         return self.status == ResourceStatus.READY.value
 
@@ -1154,32 +1290,51 @@
     entity: str
     owner: str
     provider: str
     description: str
     tags: list
     properties: dict
     location: ResourceLocation
-    variant: str = "default"
     status: str = "NO_STATUS"
+    variant: str = "default"
+    error: Optional[str] = None
 
     def __post_init__(self):
         col_types = [member.value for member in ColumnTypes]
         if self.value_type not in col_types:
-            raise ValueError(
-                f"Invalid label type ({self.value_type}) must be one of: {col_types}"
-            )
+            raise ValueError(f"Invalid label type ({self.value_type}) must be one of: {col_types}")
 
     @staticmethod
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     @staticmethod
     def type() -> str:
         return "label"
 
+    def get(self, stub) -> "Label":
+        name_variant = pb.NameVariant(name=self.name, variant=self.variant)
+        label = next(stub.GetLabelVariants(iter([name_variant])))
+
+        return Label(
+            name=label.name,
+            variant=label.variant,
+            source=(label.source.name, label.source.variant),
+            value_type=label.type,
+            entity=label.entity,
+            owner=label.owner,
+            provider=label.provider,
+            location=ResourceColumnMapping("", "", ""),
+            description=label.description,
+            tags=list(label.tags.tag),
+            properties={k: v for k, v in label.properties.property.items()},
+            status=label.status.Status._enum_type.values[label.status.status].name,
+            error=label.status.error_message
+        )
+
     def _create(self, stub) -> None:
         serialized = pb.LabelVariant(
             name=self.name,
             variant=self.variant,
             source=pb.NameVariant(
                 name=self.source[0],
                 variant=self.source[1],
@@ -1191,47 +1346,43 @@
             columns=self.location.proto(),
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateLabelVariant(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert(
-            "label_variant",
-            str(time.time()),
-            self.description,
-            self.entity,
-            self.name,
-            self.owner,
-            self.provider,
-            self.value_type,
-            self.variant,
-            self.location.entity,
-            self.location.timestamp,
-            self.location.value,
-            "ready",
-            self.source[0],
-            self.source[1],
-        )
+        db.insert("label_variant",
+                  str(time.time()),
+                  self.description,
+                  self.entity,
+                  self.name,
+                  self.owner,
+                  self.provider,
+                  self.value_type,
+                  self.variant,
+                  self.location.entity,
+                  self.location.timestamp,
+                  self.location.value,
+                  "ready",
+                  self.source[0],
+                  self.source[1]
+                  )
         if len(self.tags):
-            db.upsert(
-                "tags", self.name, self.variant, "label_variant", json.dumps(self.tags)
-            )
+            db.upsert("tags", self.name, self.variant, "label_variant", json.dumps(self.tags))
         if len(self.properties):
-            db.upsert(
-                "properties",
-                self.name,
-                self.variant,
-                "label_variant",
-                json.dumps(self.properties),
-            )
+            db.upsert("properties", self.name, self.variant, "label_variant", json.dumps(self.properties))
         self._create_label_resource(db)
 
     def _create_label_resource(self, db) -> None:
-        db.insert("labels", self.value_type, self.variant, self.name)
+        db.insert(
+            "labels",
+            self.value_type,
+            self.variant,
+            self.name
+        )
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_ready(self):
         return self.status == ResourceStatus.READY.value
 
@@ -1288,17 +1439,15 @@
 
     def _get(self, stub):
         providerList = stub.GetProviders(iter([pb.Name(name=self.name)]))
         try:
             for provider in providerList:
                 self.obj = provider
         except grpc._channel._MultiThreadedRendezvous:
-            raise ValueError(
-                f"Provider {self.name} of type {self.provider_type} not found."
-            )
+            raise ValueError(f"Provider {self.name} of type {self.provider_type} not found.")
 
     def _get_local(self, db):
         local_provider = db.query_resource("providers", "name", self.name)
         if local_provider == []:
             raise ValueError("Local mode provider not found.")
         self.obj = local_provider
 
@@ -1315,17 +1464,15 @@
         return OperationType.GET
 
     @staticmethod
     def type() -> str:
         return "source"
 
     def _get(self, stub):
-        sourceList = stub.GetSourceVariants(
-            iter([pb.NameVariant(name=self.name, variant=self.variant)])
-        )
+        sourceList = stub.GetSourceVariants(iter([pb.NameVariant(name=self.name, variant=self.variant)]))
         try:
             for source in sourceList:
                 self.obj = source
         except grpc._channel._MultiThreadedRendezvous:
             raise ValueError(f"Source {self.name}, variant {self.variant} not found.")
 
     def _get_local(self, db):
@@ -1339,30 +1486,26 @@
 @dataclass
 class TrainingSet:
     name: str
     owner: str
     label: NameVariant
     features: List[NameVariant]
     description: str
-    tags: list
-    properties: dict
     feature_lags: list = field(default_factory=list)
-    status: str = "NO_STATUS"
+    tags: list = None
+    properties: dict = None
     variant: str = "default"
     schedule: str = ""
     schedule_obj: Schedule = None
     provider: str = ""
+    status: str = "NO_STATUS"
+    error: Optional[str] = None
 
     def update_schedule(self, schedule) -> None:
-        self.schedule_obj = Schedule(
-            name=self.name,
-            variant=self.variant,
-            resource_type=6,
-            schedule_string=schedule,
-        )
+        self.schedule_obj = Schedule(name=self.name, variant=self.variant, resource_type=6, schedule_string=schedule)
         self.schedule = schedule
 
     def __post_init__(self):
         if not valid_name_variant(self.label):
             raise ValueError("Label must be set")
         if len(self.features) == 0:
             raise ValueError("A training-set must have atleast one feature")
@@ -1374,14 +1517,33 @@
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     @staticmethod
     def type() -> str:
         return "training-set"
 
+    def get(self, stub):
+        name_variant = pb.NameVariant(name=self.name, variant=self.variant)
+        ts = next(stub.GetTrainingSetVariants(iter([name_variant])))
+
+        return TrainingSet(
+            name=ts.name,
+            variant=ts.variant,
+            owner=ts.owner,
+            description=ts.description,
+            status=ts.status.Status._enum_type.values[ts.status.status].name,
+            label=(ts.label.name, ts.label.variant),
+            features=[(f.name, f.variant) for f in ts.features],
+            feature_lags=[],
+            provider=ts.provider,
+            tags=list(ts.tags.tag),
+            properties={k: v for k, v in ts.properties.property.items()},
+            error=ts.status.error_message,
+        )
+
     def _create(self, stub) -> None:
         feature_lags = []
         for lag in self.feature_lags:
             lag_duration = Duration()
             _ = lag_duration.FromTimedelta(lag["lag"])
             feature_lag = pb.FeatureLag(
                 feature=lag["feature"],
@@ -1393,71 +1555,65 @@
 
         serialized = pb.TrainingSetVariant(
             name=self.name,
             variant=self.variant,
             description=self.description,
             schedule=self.schedule,
             owner=self.owner,
-            features=[pb.NameVariant(name=v[0], variant=v[1]) for v in self.features],
+            features=[
+                pb.NameVariant(name=v[0], variant=v[1]) for v in self.features
+            ],
             label=pb.NameVariant(name=self.label[0], variant=self.label[1]),
             feature_lags=feature_lags,
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateTrainingSetVariant(serialized)
 
     def _create_local(self, db) -> None:
         self._check_insert_training_set_resources(db)
-        db.insert(
-            "training_set_variant",
-            str(time.time()),
-            self.description,
-            self.name,
-            self.owner,
-            self.variant,
-            self.label[0],
-            self.label[1],
-            "ready",
-        )
+        db.insert("training_set_variant",
+                  str(time.time()),
+                  self.description,
+                  self.name,
+                  self.owner,
+                  self.variant,
+                  self.label[0],
+                  self.label[1],
+                  "ready"
+                  )
         if len(self.tags):
-            db.upsert(
-                "tags",
-                self.name,
-                self.variant,
-                "training_set_variant",
-                json.dumps(self.tags),
-            )
+            db.upsert("tags", self.name, self.variant, "training_set_variant", json.dumps(self.tags))
         if len(self.properties):
-            db.upsert(
-                "properties",
-                self.name,
-                self.variant,
-                "training_set_variant",
-                json.dumps(self.properties),
-            )
+            db.upsert("properties", self.name, self.variant, "training_set_variant", json.dumps(self.properties))
         self._create_training_set_resource(db)
 
     def _create_training_set_resource(self, db) -> None:
-        db.insert("training_sets", "TrainingSet", self.variant, self.name)
+        db.insert(
+            "training_sets",
+            "TrainingSet",
+            self.variant,
+            self.name
+        )
 
     def _check_insert_training_set_resources(self, db) -> None:
         try:
             db.get_label_variant(self.label[0], self.label[1])
         except ValueError:
-            raise ValueError(
-                f"{self.label[0]} does not exist. Failed to register training set"
-            )
+            raise ValueError(f"{self.label[0]} does not exist. Failed to register training set")
 
         for feature_name, feature_variant in self.features:
             try:
-                db.get_feature_variant(feature_name, feature_variant)
+                is_on_demand = db.get_feature_variant_on_demand(feature_name, feature_variant)
+                if is_on_demand:
+                    raise InvalidTrainingSetFeatureComputationMode(feature_name, feature_variant)
+            except InvalidTrainingSetFeatureComputationMode as e:
+                raise e
             except Exception as e:
-                raise Exception(
-                    f"{feature_name} does not exist. Failed to register training set. Error: {e}"
-                )
+                raise Exception(f"{feature_name}:{feature_variant} does not exist. Failed to register training set. Error: {e}")
 
             db.insert(
                 "training_set_features",
                 self.name,
                 self.variant,
                 feature_name,  # feature name
                 feature_variant,  # feature variant
@@ -1468,26 +1624,24 @@
             feature_variant = feature["variant"]
             feature_new_name = feature["name"]
             feature_lag = feature["lag"].total_seconds()
 
             try:
                 db.get_feature_variant(feature_name, feature_variant)
             except Exception as e:
-                raise Exception(
-                    f"{feature_name} does not exist. Failed to register training set. Error: {e}"
-                )
+                raise Exception(f"{feature_name} does not exist. Failed to register training set. Error: {e}")
 
             db.insert(
                 "training_set_lag_features",
                 self.name,
                 self.variant,
                 feature_name,  # feature name
                 feature_variant,  # feature variant
                 feature_new_name,  # feature new name
-                feature_lag,  # feature_lag
+                feature_lag  # feature_lag
             )
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_ready(self):
         return self.status == ResourceStatus.READY.value
@@ -1510,257 +1664,221 @@
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     def type(self) -> str:
         return "model"
 
     def _create(self, stub) -> None:
-        properties = pb.Properties(property=self.properties)
+        properties = pb.Properties(
+            property=self.properties
+        )
         serialized = pb.Model(
             name=self.name,
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateModel(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert(
-            "models",
-            self.name,
-            "Model",
-        )
+        db.insert("models",
+                  self.name,
+                  "Model",
+                  )
         if len(self.tags):
             db.upsert("tags", self.name, "", "models", json.dumps(self.tags))
         if len(self.properties):
-            db.upsert(
-                "properties", self.name, "", "models", json.dumps(self.properties)
-            )
+            db.upsert("properties", self.name, "", "models", json.dumps(self.properties))
 
     def __eq__(self, other):
         for attribute in vars(self):
             if getattr(self, attribute) != getattr(other, attribute):
                 return False
         return True
 
 
-Resource = Union[
-    PrimaryData,
-    Provider,
-    Entity,
-    User,
-    Feature,
-    Label,
-    TrainingSet,
-    Source,
-    Schedule,
-    ProviderReference,
-    SourceReference,
-    EntityReference,
-    Model,
-]
+Resource = Union[PrimaryData, Provider, Entity, User, Feature, Label,
+                 TrainingSet, Source, Schedule, ProviderReference, SourceReference, EntityReference, Model, OnDemandFeature]
 
 
 class ResourceRedefinedError(Exception):
     @typechecked
     def __init__(self, resource: Resource):
-        variantStr = (
-            f" variant {resource.variant}" if hasattr(resource, "variant") else ""
-        )
+        variantStr = f" variant {resource.variant}" if hasattr(
+            resource, 'variant') else ""
         resourceId = f"{resource.name}{variantStr}"
         super().__init__(
             f"{resource.type()} resource {resourceId} defined in multiple places"
         )
 
 
 class ResourceState:
+
     def __init__(self):
         self.__state = {}
-        self.__create_list = []
 
     @typechecked
     def add(self, resource: Resource) -> None:
-        if hasattr(resource, "variant"):
-            key = (
-                resource.operation_type().name,
-                resource.type(),
-                resource.name,
-                resource.variant,
-            )
+        if hasattr(resource, 'variant'):
+            key = (resource.operation_type().name, resource.type(), resource.name, resource.variant)
         else:
             key = (resource.operation_type().name, resource.type(), resource.name)
         if key in self.__state:
             if resource == self.__state[key]:
                 print(f"Resource {resource.type()} already registered.")
                 return
             raise ResourceRedefinedError(resource)
         self.__state[key] = resource
-        self.__create_list.append(resource)
-        if hasattr(resource, "schedule_obj") and resource.schedule_obj != None:
+        if hasattr(resource, 'schedule_obj') and resource.schedule_obj != None:
             my_schedule = resource.schedule_obj
             key = (my_schedule.type(), my_schedule.name)
             self.__state[key] = my_schedule
-            self.__create_list.append(my_schedule)
 
     def sorted_list(self) -> List[Resource]:
         resource_order = {
             "user": 0,
             "provider": 1,
             "source": 2,
             "entity": 3,
             "feature": 4,
-            "label": 5,
-            "training-set": 6,
-            "schedule": 7,
+            "ondemand_feature": 5,
+            "label": 6,
+            "training-set": 7,
+            "schedule": 8,
+            "model": 9
         }
 
         def to_sort_key(res):
             resource_num = resource_order[res.type()]
             variant = res.variant if hasattr(res, "variant") else ""
             return (resource_num, res.name, variant)
 
         return sorted(self.__state.values(), key=to_sort_key)
 
     def create_all_dryrun(self) -> None:
-        for resource in self.__create_list:
+        for resource in self.sorted_list():
             if resource.operation_type() is OperationType.GET:
                 print("Getting", resource.type(), resource.name)
             if resource.operation_type() is OperationType.CREATE:
                 print("Creating", resource.type(), resource.name)
 
     def create_all_local(self) -> None:
         db = SQLiteMetadata()
         check_up_to_date(True, "register")
-        for resource in self.__create_list:
+        for resource in self.sorted_list():
             if resource.operation_type() is OperationType.GET:
                 print("Getting", resource.type(), resource.name)
                 resource._get_local(db)
             if resource.operation_type() is OperationType.CREATE:
                 print("Creating", resource.type(), resource.name)
                 resource._create_local(db)
         db.close()
         return
 
     def create_all(self, stub) -> None:
         check_up_to_date(False, "register")
-        for resource in self.__create_list:
+        for resource in self.sorted_list():
             if resource.type() == "provider" and resource.name == "local-mode":
                 continue
             try:
+                # NOTE: There is an extra space before the variant name to better handle the case
+                # where a resource has no variant; ultimately, we should separate data access and
+                # logging/CLI output to avoid this unnecessary coupling.
+                resource_variant = f" {resource.variant}" if hasattr(resource, "variant") else ""
                 if resource.operation_type() is OperationType.GET:
-                    print("Getting", resource.type(), resource.name)
+                    print(f"Getting {resource.type()} {resource.name}{resource_variant}")
                     resource._get(stub)
                 if resource.operation_type() is OperationType.CREATE:
-                    print("Creating", resource.type(), resource.name)
+                    print(f"Creating {resource.type()} {resource.name}{resource_variant}")
                     resource._create(stub)
             except grpc.RpcError as e:
                 if e.code() == grpc.StatusCode.ALREADY_EXISTS:
-                    print(resource.name, "already exists.")
+                    print(f"{resource.name}{resource_variant} already exists.")
                     continue
 
                 raise e
 
 
 ## Executor Providers
 @typechecked
 class DatabricksCredentials:
-    def __init__(
-        self,
-        username: str = "",
-        password: str = "",
-        host: str = "",
-        token: str = "",
-        cluster_id: str = "",
-    ):
+    def __init__(self,
+                 username: str = "",
+                 password: str = "",
+                 host: str = "",
+                 token: str = "",
+                 cluster_id: str = ""):
         self.username = username
         self.password = password
         self.host = host
         self.token = token
         self.cluster_id = cluster_id
 
-        host_token_provided = (
-            username == "" and password == "" and host != "" and token != ""
-        )
-        username_password_provided = (
-            username != "" and password != "" and host == "" and token == ""
-        )
+        host_token_provided = username == "" and password == "" and host != "" and token != ""
+        username_password_provided = username != "" and password != "" and host == "" and token == ""
 
-        if (
-            not host_token_provided
-            and not username_password_provided
-            or host_token_provided
-            and username_password_provided
-        ):
+        if not host_token_provided and not username_password_provided or host_token_provided and username_password_provided:
             raise Exception(
-                "The DatabricksCredentials requires only one credentials set ('username' and 'password' or 'host' and 'token' set.)"
-            )
+                "The DatabricksCredentials requires only one credentials set ('username' and 'password' or 'host' and 'token' set.)")
 
         if not cluster_id:
             raise Exception("Cluster_id of existing cluster must be provided")
 
     def type(self):
         return "DATABRICKS"
 
     def config(self):
         return {
             "Username": self.username,
             "Password": self.password,
             "Host": self.host,
             "Token": self.token,
-            "Cluster": self.cluster_id,
+            "Cluster": self.cluster_id
         }
 
 
+
 @typechecked
 @dataclass
 class EMRCredentials:
-    def __init__(
-        self, emr_cluster_id: str, emr_cluster_region: str, credentials: AWSCredentials
-    ):
+    def __init__(self,
+                 emr_cluster_id: str,
+                 emr_cluster_region: str,
+                 credentials: AWSCredentials):
+        
         self.emr_cluster_id = emr_cluster_id
         self.emr_cluster_region = emr_cluster_region
         self.credentials = credentials
 
     def type(self):
         return "EMR"
 
     def config(self):
         return {
             "ClusterName": self.emr_cluster_id,
             "ClusterRegion": self.emr_cluster_region,
             "Credentials": self.credentials.config(),
         }
 
-
 @typechecked
 @dataclass
 class SparkCredentials:
-    def __init__(
-        self,
-        master: str,
-        deploy_mode: str,
-        python_version: str = "",
-        core_site_path: str = "",
-        yarn_site_path: str = "",
-    ):
+    def __init__(self,
+                 master: str,
+                 deploy_mode: str,
+                 python_version: str = "",
+                ):
+        
         self.master = master.lower()
         self.deploy_mode = deploy_mode.lower()
-        self.core_site_path = core_site_path
-        self.yarn_site_path = yarn_site_path
 
         if self.deploy_mode != "cluster" and self.deploy_mode != "client":
-            raise Exception(
-                f"Spark does not support '{self.deploy_mode}' deploy mode. It only supports 'cluster' and 'client'."
-            )
-
-        self.python_version = self._verify_python_version(
-            self.deploy_mode, python_version
-        )
-
-        self._verify_yarn_config()
+            raise Exception(f"Spark does not support '{self.deploy_mode}' deploy mode. It only supports 'cluster' and 'client'.")
 
+        self.python_version = self._verify_python_version(self.deploy_mode, python_version)
+    
     def _verify_python_version(self, deploy_mode, version):
         if deploy_mode == "cluster" and version == "":
             client_python_version = sys.version_info
             client_major = str(client_python_version.major)
             client_minor = str(client_python_version.minor)
 
             if client_major != MAJOR_VERSION:
@@ -1769,53 +1887,38 @@
                 client_minor = "7"
 
             version = f"{client_major}.{client_minor}"
 
         if version.count(".") == 2:
             major, minor, _ = version.split(".")
         elif version.count(".") == 1:
-            major, minor = version.split(".")
+            major, minor = version.split(".")    
         else:
-            raise Exception(
-                "Please specify your Python version on the Spark cluster. Accepted formats: Major.Minor or Major.Minor.Patch; ex. '3.7' or '3.7.16"
-            )
+            raise Exception("Please specify your Python version on the Spark cluster. Accepted formats: Major.Minor or Major.Minor.Patch; ex. '3.7' or '3.7.16")
 
         if major != MAJOR_VERSION or minor not in MINOR_VERSIONS:
-            raise Exception(
-                f"The Python version {version} is not supported. Currently, supported versions are 3.7-3.10."
-            )
-
+            raise Exception(f"The Python version {version} is not supported. Currently, supported versions are 3.7-3.10.")
+        
         """
-        The Python versions on the Docker image are 3.7.16, 3.8.16, 3.9.16, and 3.10.10. 
+        The Python versions on the Docker image are 3.7.16, 3.8.16, 3.9.16, 3.10.10, and 3.11.2.
         This conditional statement sets the patch number based on the minor version. 
         """
         if minor == "10":
             patch = "10"
+        elif minor == "11":
+            patch = "2"
         else:
             patch = "16"
-
+        
         return f"{major}.{minor}.{patch}"
 
-    def _verify_yarn_config(self):
-        if self.master == "yarn" and (
-            self.core_site_path == "" or self.yarn_site_path == ""
-        ):
-            raise Exception(
-                "Yarn requires core-site.xml and yarn-site.xml files."
-                "Please copy these files from your Spark instance to local, then provide the local path in "
-                "core_site_path and yarn_site_path. "
-            )
-
     def type(self):
         return "SPARK"
 
     def config(self):
         return {
             "Master": self.master,
             "DeployMode": self.deploy_mode,
-            "PythonVersion": self.python_version,
-            "CoreSite": open(self.core_site_path, "r").read(),
-            "YarnSite": open(self.yarn_site_path, "r").read(),
+            "PythonVersion": self.python_version
         }
 
-
 ExecutorCredentials = Union[EMRCredentials, DatabricksCredentials, SparkCredentials]
```

### Comparing `featureform-1.7.3rc5/src/featureform/search.py` & `featureform-1.7.4/src/featureform/search.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/serving.py` & `featureform-1.7.4/src/featureform/serving.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,45 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
+import inspect
 import os
-import re
 from typing import Union
+import warnings
 import dill
 import json
 import math
 import types
+import base64
 import random
 
 import numpy as np
 import pandas as pd
+from pandas.core.generic import NDFrame
 from pandasql import sqldf
 from featureform.proto import serving_pb2
+
+from .local_cache import LocalCache
+from .local_utils import (
+    get_sql_transformation_sources,
+    feature_df_with_entity,
+    list_to_combined_df,
+    get_features_for_entity,
+    feature_df_from_csv,
+    label_df_from_csv,
+    merge_feature_into_ts,
+)
 from .sqlite_metadata import SQLiteMetadata
 from featureform.proto import serving_pb2_grpc
 
-from .resources import Model, SourceType
+from .resources import Model, SourceType, ComputationMode
 from .tls import insecure_channel, secure_channel
 from .version import check_up_to_date
+from .enums import FileFormat
 
 
 def check_feature_type(features):
     checked_features = []
     for feature in features:
         if isinstance(feature, tuple):
             checked_features.append(feature)
@@ -50,29 +65,43 @@
     training_dataset = dataset.repeat(10).shuffle(1000).batch(8)
     for feature_batch in training_dataset:
         # Train model
     ```
     """
 
     def __init__(self, host=None, local=False, insecure=False, cert_path=None):
+        # This line ensures that the warning is only raised if ServingClient is instantiated directly
+        # TODO: Remove this check once ServingClient is deprecated
+        is_instantiated_directed = inspect.stack()[1].function != "__init__"
+        if is_instantiated_directed:
+            warnings.warn(
+                "ServingClient is deprecated and will be removed in future versions; use Client instead.",
+                PendingDeprecationWarning,
+            )
         """
         Args:
             host (str): The hostname of the Featureform instance. Exclude if using Localmode.
             local (bool): True if using Localmode.
             insecure (bool): True if connecting to an insecure Featureform endpoint. False if using a self-signed or public TLS certificate
             cert_path (str): The path to a public certificate if using a self-signed certificate.
         """
         if local and host:
             raise ValueError("Host and local cannot both be set")
         if local:
             self.impl = LocalClientImpl()
         else:
             self.impl = HostedClientImpl(host, insecure, cert_path)
 
-    def training_set(self, name, variant="default", include_label_timestamp=False, model: Union[str, Model] = None):
+    def training_set(
+        self,
+        name,
+        variant="default",
+        include_label_timestamp=False,
+        model: Union[str, Model] = None,
+    ):
         """Return an iterator that iterates through the specified training set.
 
         **Examples**:
         ``` py
             client = ff.ServingClient()
             dataset = client.training_set("fraud_training", "quickstart")
             training_dataset = dataset.repeat(10).shuffle(1000).batch(8)
@@ -106,399 +135,533 @@
         """
         features = check_feature_type(features)
         return self.impl.features(features, entities, model)
 
 
 class HostedClientImpl:
     def __init__(self, host=None, insecure=False, cert_path=None):
-        host = host or os.getenv('FEATUREFORM_HOST')
+        host = host or os.getenv("FEATUREFORM_HOST")
         if host is None:
             raise ValueError(
-                'If not in local mode then `host` must be passed or the environment'
-                ' variable FEATUREFORM_HOST must be set.'
+                "If not in local mode then `host` must be passed or the environment"
+                " variable FEATUREFORM_HOST must be set."
             )
         check_up_to_date(False, "serving")
         channel = self._create_channel(host, insecure, cert_path)
         self._stub = serving_pb2_grpc.FeatureStub(channel)
 
     def _create_channel(self, host, insecure, cert_path):
         if insecure:
             return insecure_channel(host)
         else:
             return secure_channel(host, cert_path)
 
-    def training_set(self, name, variation, include_label_timestamp, model: Union[str, Model] = None):
+    def training_set(
+        self, name, variation, include_label_timestamp, model: Union[str, Model] = None
+    ):
         return Dataset(self._stub).from_stub(name, variation, model)
 
-    def features(self, features, entities, model: Union[str, Model] = None):
+    def features(
+        self, features, entities, model: Union[str, Model] = None, params: list = None
+    ):
         req = serving_pb2.FeatureServeRequest()
         for name, value in entities.items():
             entity_proto = req.entities.add()
             entity_proto.name = name
             entity_proto.value = value
-        for (name, variation) in features:
+        for name, variation in features:
             feature_id = req.features.add()
             feature_id.name = name
             feature_id.version = variation
         if model is not None:
             req.model.name = model if isinstance(model, str) else model.name
         resp = self._stub.FeatureServe(req)
-        return [parse_proto_value(val) for val in resp.values]
+
+        feature_values = []
+        for val in resp.values:
+            parsed_value = parse_proto_value(val)
+
+            is_ondemand_feature = type(parsed_value) == bytes
+            if is_ondemand_feature:
+                code = dill.loads(bytearray(parsed_value))
+                func = types.FunctionType(code, globals(), "transformation")
+                parsed_value = func(self, params, entities)
+
+            feature_values.append(parsed_value)
+
+        return feature_values
+
+    def get_source_as_df(self, name, variant):
+        warnings.warn(
+            "Computing dataframes on sources in hosted mode is not yet supported."
+        )
+        return pd.DataFrame()
 
 
 class LocalClientImpl:
     def __init__(self):
         self.db = SQLiteMetadata()
+        self.local_cache = LocalCache(self.db)
         check_up_to_date(True, "serving")
 
-    def training_set(self, training_set_name, training_set_variant, include_label_timestamp, model: Union[str, Model] = None):
-        training_set = self.db.get_training_set_variant(training_set_name, training_set_variant)
+    def get_training_set_dataframe(
+        self, label, label_df, training_set_name, training_set_variant
+    ) -> NDFrame:
+        def get() -> pd.DataFrame:
+            feature_columns = []
+
+            # We will build the training set DF by merging each feature one by one into it.
+            training_set_df = label_df
+            features = self.db.get_training_set_features(
+                training_set_name, training_set_variant
+            )
+            for feature in features:
+                feature_variant = self.db.get_feature_variant(
+                    feature["feature_name"], feature["feature_variant"]
+                )
+                feature_df = self.get_feature_dataframe(feature_variant)
+                training_set_df = merge_feature_into_ts(
+                    feature_variant, label, feature_df, training_set_df
+                )
+                feature_columns.append(
+                    f"{feature['feature_name']}.{feature['feature_variant']}"
+                )
+
+            lag_features = self.db.get_training_set_lag_features(
+                training_set_name, training_set_variant
+            )
+            if len(lag_features) > 0:
+                timestamp_column = label["source_timestamp"]
+                entity_column = label["source_entity"]
+                label_column = "label"
+                lag_sql_query = self.get_lag_features_sql_query(
+                    lag_features,
+                    feature_columns,
+                    entity_column,
+                    label_column,
+                    timestamp_column,
+                )
+
+                globals()["source_0"] = training_set_df
+                mysql = lambda q: sqldf(q, globals())
+                training_set_df = mysql(lag_sql_query)
+
+            return training_set_df
+
+        return self.local_cache.get_or_put_training_set(
+            training_set_name=training_set_name,
+            training_set_variant=training_set_variant,
+            func=get,
+        )
+
+    def training_set(
+        self,
+        training_set_name,
+        training_set_variant,
+        include_label_timestamp,
+        model: Union[str, Model] = None,
+    ):
+        training_set = self.db.get_training_set_variant(
+            training_set_name, training_set_variant
+        )
+
+        label = self.db.get_label_variant(
+            training_set["label_name"], training_set["label_variant"]
+        )
+        label_df = self.get_label_dataframe(label)
 
         if model is not None:
             self._register_model(
                 model,
                 look_up_table="model_training_sets",
                 association_name=training_set_name,
-                association_variant=training_set_variant
+                association_variant=training_set_variant,
             )
 
-        label = self.db.get_label_variant(training_set['label_name'], training_set['label_variant'])
-        label_df = self.get_label_dataframe(label)
-
-        feature_columns = []
-
-        # We will build the training set DF by merging each feature one by one into it.
-        trainingset_df = label_df
-        features = self.db.get_training_set_features(training_set_name, training_set_variant)
-        for feature_variant in features:
-            feature = self.db.get_feature_variant(feature_variant['feature_name'], feature_variant['feature_variant'])
-            feature_df = self.get_feature_dataframe(feature)
-            trainingset_df = self.merge_feature_into_ts(feature, label, feature_df, trainingset_df)
-
-            feature_columns.append(f"{feature_variant['feature_name']}.{feature_variant['feature_variant']}")
-
-        lag_features = self.db.get_training_set_lag_features(training_set_name, training_set_variant)
-        if len(lag_features) > 0:
-            timestamp_column = label["source_timestamp"]
-            entity_column = label["source_entity"]
-            label_column = "label"
-            lag_sql_query = self.get_lag_features_sql_query(lag_features, feature_columns, entity_column, label_column, timestamp_column)
-
-            globals()["source_0"] = trainingset_df
-            mysql = lambda q: sqldf(q, globals())
-            trainingset_df = mysql(lag_sql_query)
-        
-        return self.convert_ts_df_to_dataset(label, trainingset_df, include_label_timestamp)
-
-
-    def get_lag_features_sql_query(self, lag_features, feature_columns, entity, label, ts):
+        training_set_df = self.get_training_set_dataframe(
+            label, label_df, training_set_name, training_set_variant
+        )
+
+        return self.convert_ts_df_to_dataset(
+            label, training_set_df, include_label_timestamp
+        )
+
+    def get_lag_features_sql_query(
+        self, lag_features, feature_columns, entity, label, ts
+    ):
         """
-        Returns the SQL query to compute the lag features. 
+        Returns the SQL query to compute the lag features.
         Input:
         - lag_features: dict
-        
+
         Returns:
         - sql_query: string
         """
 
         if len(lag_features) == 0:
             return "SELECT * FROM source_0"
 
-        
         features = ""
         for f in feature_columns:
-            features = f"{features}, \"{f}\"" if features != "" else f"\"{f}\""
-    
+            features = f'{features}, "{f}"' if features != "" else f'"{f}"'
+
         MAIN_SELECT = f"SELECT {entity}, {ts}, {features}"
         SUBQUERY = "FROM (SELECT * FROM (SELECT *, row_number FROM ("
         INNER_QUERY = "FROM (( SELECT * FROM source_0 )"
         CLOSING_QUERY = f") tt ) WHERE row_number=1 ORDER BY {ts} ASC ))"
 
         lag_columns = []
         lag_timestamps = []
 
         LAG_QUERIES = ""
         for i, lag_feature in enumerate(lag_features):
-            feature_column_name = f"{lag_feature['feature_name']}.{lag_feature['feature_variant']}"
+            feature_column_name = (
+                f"{lag_feature['feature_name']}.{lag_feature['feature_variant']}"
+            )
             lag_feature_column_name = lag_feature["feature_new_name"]
             lag = lag_feature["feature_lag"]
 
             lag_query = f"""
                          LEFT OUTER JOIN ( SELECT * FROM ( SELECT {entity} AS t{i}_entity, \"{feature_column_name}\" AS \"{lag_feature_column_name}\", {ts} AS t{i}_ts
                          FROM source_0) 
                          ORDER BY t{i}_ts ASC) t{i}
                          ON (t{i}_entity = {entity} AND DATETIME(t{i}_ts, \"+{lag} seconds\") <= {ts})
                         """
-            
-            LAG_QUERIES = f"{LAG_QUERIES} {lag_query}" if LAG_QUERIES != "" else lag_query
-            MAIN_SELECT = f"{MAIN_SELECT}, \"{lag_feature_column_name}\""
-            
-            lag_columns.append(f"\"{lag_feature_column_name}\"")
-            lag_timestamps.append(f"t{i}_ts")
 
+            LAG_QUERIES = (
+                f"{LAG_QUERIES} {lag_query}" if LAG_QUERIES != "" else lag_query
+            )
+            MAIN_SELECT = f'{MAIN_SELECT}, "{lag_feature_column_name}"'
+
+            lag_columns.append(f'"{lag_feature_column_name}"')
+            lag_timestamps.append(f"t{i}_ts")
 
         lag_columns = ", ".join(lag_columns)
         lag_timestamps = " DESC, ".join(lag_timestamps)
 
         INNER_SELECT = f"SELECT {entity}, {ts}, {label}, {features}, {lag_columns}, ROW_NUMBER() over (PARTITION BY {entity}, {label}, {ts} ORDER BY {ts} DESC, {lag_timestamps} DESC) as row_number"
         FULL_QUERY = f"{MAIN_SELECT}, {label} {SUBQUERY} {INNER_SELECT} {INNER_QUERY} {LAG_QUERIES} {CLOSING_QUERY}"
 
         return FULL_QUERY
 
-
     def get_input_df(self, source_name, source_variant):
-        if self.db.is_transformation(source_name, source_variant) == SourceType.PRIMARY_SOURCE.value:
+        if (
+            self.db.is_transformation(source_name, source_variant)
+            == SourceType.PRIMARY_SOURCE
+        ):
             source = self.db.get_source_variant(source_name, source_variant)
-            df = pd.read_csv(str(source['definition']))
+            file_path = source["definition"]
+            if FileFormat.get_format(file_path) == FileFormat.CSV:
+                df = pd.read_csv(file_path)
+            elif FileFormat.get_format(file_path) == FileFormat.PARQUET:
+                df = pd.read_parquet(file_path)
+            else:
+                raise ValueError(f"Unsupported file format for {file_path}")
+            return df
         else:
             df = self.process_transformation(source_name, source_variant)
         return df
 
     def sql_transformation(self, query):
-        # Use regex to parse query inputs in double curly braces {{ }} and store in a list
-        inputs = re.findall("(?={{).*?(?<=}})", query)
-        for i, input in enumerate(inputs):
-            # Trim curly braces before and after to get name.variant from {{name.variant}}
-            name_variant = input[2:-2].split(".")
-            source_name, source_variant = name_variant[0], name_variant[1]
+        transformation_sources = get_sql_transformation_sources(query)
+        for i, (source_name, source_variant) in enumerate(transformation_sources):
             # Creates a variable called dataframes_i which stores the corresponding df for each input
             df_variable = f"dataframes_{i}"
             # globals()[df_variable]:
             # 1. Converts a string "dataframes_i" to a variable name
             # 2. Assigns a global scope to the variable, to access it outside the loop
             globals()[df_variable] = self.get_input_df(source_name, source_variant)
-            query = query.replace(input, df_variable)
+
+            # using '+' signs for readability
+            query_source_to_replace = "{{" + f"{source_name}.{source_variant}" + "}}"
+            query = query.replace(query_source_to_replace, df_variable)
 
         return sqldf(query, globals())
 
     def process_transformation(self, name, variant):
-        source = self.db.get_source_variant(name, variant)
-        if self.db.is_transformation(name, variant) == SourceType.SQL_TRANSFORMATION.value:
-            query = source['definition']
-            new_data = self.sql_transformation(query)
-        else:
-            code = dill.loads(bytearray(source['definition']))
-            inputs = json.loads(source['inputs'])
-            dataframes = []
-            for input in inputs:
-                source_name, source_variant = input[0], input[1],
-                dataframes.append(self.get_input_df(source_name, source_variant))
-            func = types.FunctionType(code, globals(), "transformation")
-            new_data = func(*dataframes)
-
-        return new_data
-
-    def get_label_dataframe(self, label):
-        transform_type = self.db.is_transformation(label['source_name'], label['source_variant'])
-        if transform_type == SourceType.SQL_TRANSFORMATION.value or transform_type == SourceType.DF_TRANSFORMATION.value:
-            label_df = self.label_df_from_transformation(label)
-        else:
-            label_source = self.db.get_source_variant(label['source_name'], label['source_variant'])
-            label_df = self.label_df_from_csv(label, label_source['definition'])
-        label_df.rename(columns={label['source_value']: 'label'}, inplace=True)
-        return label_df
+        def get():
+            source = self.db.get_source_variant(name, variant)
+            if (
+                self.db.is_transformation(name, variant)
+                == SourceType.SQL_TRANSFORMATION.value
+            ):
+                query = source["definition"]
+                new_data = self.sql_transformation(query)
+            else:
+                code = dill.loads(bytearray(source["definition"]))
+                inputs = json.loads(source["inputs"])
+                dataframes = []
+                for input in inputs:
+                    source_name, source_variant = (
+                        input[0],
+                        input[1],
+                    )
+                    dataframes.append(self.get_input_df(source_name, source_variant))
+                func = types.FunctionType(code, globals(), "transformation")
+                new_data = func(*dataframes)
+            return new_data
+
+        return self.local_cache.get_or_put(
+            resource_type="transformation",
+            resource_name=name,
+            resource_variant=variant,
+            source_name=name,
+            source_variant=variant,
+            func=get,
+        )
+
+    def get_label_dataframe(self, label) -> NDFrame:
+        def get() -> pd.DataFrame:
+            transform_type = self.db.is_transformation(
+                label["source_name"], label["source_variant"]
+            )
+            if (
+                transform_type == SourceType.SQL_TRANSFORMATION.value
+                or transform_type == SourceType.DF_TRANSFORMATION.value
+            ):
+                label_df = self.label_df_from_transformation(label)
+            else:
+                label_source = self.db.get_source_variant(
+                    label["source_name"], label["source_variant"]
+                )
+                label_df = label_df_from_csv(label, label_source["definition"])
+            label_df.rename(columns={label["source_value"]: "label"}, inplace=True)
+            return label_df
+
+        return self.local_cache.get_or_put(
+            resource_type="label",
+            resource_name=label["name"],
+            resource_variant=label["variant"],
+            source_name=label["source_name"],
+            source_variant=label["source_variant"],
+            func=get,
+        )
 
     def label_df_from_transformation(self, label):
-        df = self.process_transformation(label['source_name'], label['source_variant'])
-        if label['source_timestamp'] != "":
-            df = df[[label['source_entity'], label['source_value'], label['source_timestamp']]]
-            df[label['source_timestamp']] = pd.to_datetime(df[label['source_timestamp']])
+        df = self.process_transformation(label["source_name"], label["source_variant"])
+        if label["source_timestamp"] != "":
+            df = df[
+                [
+                    label["source_entity"],
+                    label["source_value"],
+                    label["source_timestamp"],
+                ]
+            ]
+            df[label["source_timestamp"]] = pd.to_datetime(
+                df[label["source_timestamp"]]
+            )
         else:
-            df = df[[label['source_entity'], label['source_value']]]
-        df.set_index(label['source_entity'])
+            df = df[[label["source_entity"], label["source_value"]]]
+        df.set_index(label["source_entity"])
         return df
 
-    def label_df_from_csv(self, label, file_name):
-        df = pd.read_csv(file_name)
-        self.check_missing_values(label, df)
-        if label['source_timestamp'] != "":
-            df = df[[label['source_entity'], label['source_value'], label['source_timestamp']]]
-            df[label['source_timestamp']] = pd.to_datetime(df[label['source_timestamp']])
-            df.sort_values(by=label['source_timestamp'], inplace=True)
-            df.drop_duplicates(subset=[label['source_entity'], label['source_timestamp']], keep="last", inplace=True)
-        else:
-            df = df[[label['source_entity'], label['source_value']]]
-        df.set_index(label['source_entity'], inplace=True)
-        return df
+    def get_feature_dataframe(self, feature) -> NDFrame:
+        def get() -> pd.DataFrame:
+            name_variant = feature["name"] + "." + feature["variant"]
+            transform_type = self.db.is_transformation(
+                feature["source_name"], feature["source_variant"]
+            )
+            if (
+                transform_type == SourceType.SQL_TRANSFORMATION.value
+                or transform_type == SourceType.DF_TRANSFORMATION.value
+            ):
+                feature_df = self.feature_df_from_transformation(feature)
+            else:
+                source = self.db.get_source_variant(
+                    feature["source_name"], feature["source_variant"]
+                )
+                feature_df = feature_df_from_csv(feature, source["definition"])
+            feature_df.set_index(feature["source_entity"])
+            feature_df.rename(
+                columns={feature["source_value"]: name_variant}, inplace=True
+            )
+            return feature_df
 
-    def get_feature_dataframe(self, feature):
-        name_variant = feature['name'] + "." + feature['variant']
-        transform_type = self.db.is_transformation(feature['source_name'], feature['source_variant'])
-        if transform_type == SourceType.SQL_TRANSFORMATION.value or transform_type == SourceType.DF_TRANSFORMATION.value:
-            feature_df = self.feature_df_from_transformation(feature)
-        else:
-            source = self.db.get_source_variant(feature['source_name'], feature['source_variant'])
-            feature_df = self.feature_df_from_csv(feature, source['definition'])
-        feature_df.set_index(feature['source_entity'])
-        feature_df.rename(columns={feature['source_value']: name_variant}, inplace=True)
-        return feature_df
+        return self.local_cache.get_or_put(
+            resource_type="feature",
+            resource_name=feature["name"],
+            resource_variant=feature["variant"],
+            source_name=feature["source_name"],
+            source_variant=feature["source_variant"],
+            func=get,
+        )
 
     def feature_df_from_transformation(self, feature):
-        df = self.process_transformation(feature['source_name'], feature['source_variant'])
+        df = self.process_transformation(
+            feature["source_name"], feature["source_variant"]
+        )
         if isinstance(df, pd.Series):
             df = df.to_frame()
             df.reset_index(inplace=True)
-        if feature['source_timestamp'] != "":
-            df = df[[feature['source_entity'], feature['source_value'], feature['source_timestamp']]]
-            df[feature['source_timestamp']] = pd.to_datetime(df[feature['source_timestamp']])
-        else:
-            df = df[[feature['source_entity'], feature['source_value']]]
-        return df
-
-    def feature_df_from_csv(self, feature, filename):
-        df = pd.read_csv(str(filename))
-        self.check_missing_values(feature, df)
-        if feature['source_timestamp'] != "":
-            df = df[[feature['source_entity'], feature['source_value'], feature['source_timestamp']]]
-            df[feature['source_timestamp']] = pd.to_datetime(df[feature['source_timestamp']])
-            df = df.sort_values(by=feature['source_timestamp'], ascending=True)
+        if feature["source_timestamp"] != "":
+            df = df[
+                [
+                    feature["source_entity"],
+                    feature["source_value"],
+                    feature["source_timestamp"],
+                ]
+            ]
+            df[feature["source_timestamp"]] = pd.to_datetime(
+                df[feature["source_timestamp"]]
+            )
         else:
-            df = df[[feature['source_entity'], feature['source_value']]]
+            df = df[[feature["source_entity"], feature["source_value"]]]
         return df
 
-    def merge_feature_into_ts(self, feature_row, label_row, df, trainingset_df):
-        if feature_row['source_timestamp'] != "":
-            trainingset_df = pd.merge_asof(trainingset_df, df.sort_values(feature_row['source_timestamp']),
-                                           direction='backward',
-                                           left_on=label_row['source_timestamp'],
-                                           right_on=feature_row['source_timestamp'], left_by=label_row['source_entity'],
-                                           right_by=feature_row['source_entity'])
-            if feature_row['source_timestamp'] != label_row['source_timestamp']:
-                trainingset_df.drop(columns=feature_row['source_timestamp'], inplace=True)
-        else:
-            df.drop_duplicates(subset=[feature_row['source_entity']], keep="last", inplace=True)
-            trainingset_df.reset_index(inplace=True)
-            trainingset_df[label_row['source_entity']] = trainingset_df[label_row['source_entity']].astype('string')
-            df[label_row['source_entity']] = df[label_row['source_entity']].astype('string')
-            trainingset_df = trainingset_df.join(df.set_index(label_row['source_entity']), how="left",
-                                                 on=label_row['source_entity'],
-                                                 lsuffix="_left")
-            if "index" in trainingset_df.columns:
-                trainingset_df.drop(columns='index', inplace=True)
-        return trainingset_df
-
-    def convert_ts_df_to_dataset(self, label_row, trainingset_df, include_label_timestamp): 
-        if label_row['source_timestamp'] != "" and include_label_timestamp != True:
-            trainingset_df.drop(columns=label_row['source_timestamp'], inplace=True)
-        elif label_row['source_timestamp'] != "" and include_label_timestamp:
-            source_timestamp_col = trainingset_df.pop(label_row['source_timestamp'])
-            trainingset_df = trainingset_df.assign(label_timestamp=source_timestamp_col)
-        trainingset_df.drop(columns=label_row['source_entity'], inplace=True)
-            
-        label_col = trainingset_df.pop('label')
-        trainingset_df = trainingset_df.assign(label=label_col)
-        return Dataset.from_dataframe(trainingset_df, include_label_timestamp)
-
-    def features(self, feature_variant_list, entities, model: Union[str, Model] = None):
+    def features(
+        self,
+        feature_variant_list,
+        entities,
+        model: Union[str, Model] = None,
+        params: list = None,
+    ):
         if len(feature_variant_list) == 0:
             raise Exception("No features provided")
+
+        self.entities = entities
+        self.params = params if params else []
+
         # This code assumes that the entities dictionary only has one entity
         entity_id = list(entities.keys())[0]
         entity_value = entities[entity_id]
-        all_features_list = self.add_feature_dfs_to_list(feature_variant_list, entity_id)
-        all_features_df = self.list_to_combined_df(all_features_list, entity_id)
-        features = self.get_features_for_entity(entity_id, entity_value, all_features_df)
+        all_features_list = self.add_feature_dfs_to_list(
+            feature_variant_list, entity_id
+        )
+        all_features_df = list_to_combined_df(all_features_list, entity_id)
+        features = get_features_for_entity(entity_id, entity_value, all_features_df)
 
         if model is not None:
             for feature_name, feature_variant in feature_variant_list:
                 self._register_model(
                     model,
                     look_up_table="model_features",
                     association_name=feature_name,
-                    association_variant=feature_variant
+                    association_variant=feature_variant,
                 )
 
         return features
 
     def add_feature_dfs_to_list(self, feature_variant_list, entity_id):
         feature_df_list = []
+
         for feature_variant in feature_variant_list:
-            feature = self.db.get_feature_variant(feature_variant[0], feature_variant[1])
-            name_variant = f"{feature['name']}.{feature['variant']}"
-            source_name, source_variant = feature['source_name'], feature['source_variant']
-            if feature["entity"] != entity_id:
-                raise ValueError(
-                    f"Invalid entity {entity_id} for feature {source_name}-{source_variant}")
-            if self.db.is_transformation(source_name, source_variant) != SourceType.PRIMARY_SOURCE.value:
-                feature_df = self.process_transformation(source_name, source_variant)
-                if isinstance(feature_df, pd.Series):
-                    feature_df = feature_df.to_frame()
-                    feature_df.reset_index(inplace=True)
-                if not feature["source_entity"] in feature_df.columns:
-                    raise ValueError(
-                        f"Could not set entity column. No column name {feature['source_entity']} exists in {source_name}-{source_variant}")
-                if not feature['source_value'] in feature_df.columns:
-                    raise ValueError(
-                        f"Could not access feature value column. No column name {feature['source_value']} exists in {source_name}-{source_variant}")
-                feature_df = feature_df[[feature['source_entity'], feature['source_value']]]
-                feature_df.rename(columns={feature['source_entity']: entity_id, feature['source_value']: name_variant}, inplace=True)
-                feature_df.drop_duplicates(subset=[entity_id], keep="last", inplace=True)
-                feature_df.set_index(entity_id)
+            f_name = feature_variant[0]
+            f_variant = feature_variant[1]
+            f_mode = self.db.get_feature_variant_mode(f_name, f_variant)
+
+            if f_mode == ComputationMode.CLIENT_COMPUTED:
+                feature_df = self.calculate_ondemand_feature(
+                    f_name, f_variant, entity_id
+                )
             else:
-                source = self.db.get_source_variant(source_name, source_variant)
-                feature_df = self.feature_df_with_entity(source['definition'], entity_id, feature)
+                feature_df = self.get_precomputed_feature(f_name, f_variant, entity_id)
+
             feature_df_list.append(feature_df)
 
         return feature_df_list
 
-    def list_to_combined_df(self, features_list, entity_id):
-        all_feature_df = None
-        try:
-            for feature in features_list:
-                if all_feature_df is None:
-                    all_feature_df = feature
-                else:
-                    all_feature_df = all_feature_df.join(feature.set_index(entity_id), on=entity_id,
-                                                         lsuffix='_left')
-            return all_feature_df
-        except TypeError:
-            print("Set is empty")
-
-    def get_features_for_entity(self, entity_id, entity_value, all_feature_df):
-        entity = all_feature_df.loc[all_feature_df[entity_id] == entity_value].copy()
-        entity.drop(columns=entity_id, inplace=True)
-        if len(entity.values) > 0:
-            return entity.values[0]
+    def get_precomputed_feature(self, f_name, f_variant, entity_id):
+        feature = self.db.get_feature_variant(f_name, f_variant)
+        source_name, source_variant = feature["source_name"], feature["source_variant"]
+        if feature["entity"] != entity_id:
+            raise ValueError(
+                f"Invalid entity {entity_id} for feature {source_name}-{source_variant}"
+            )
+        if (
+            self.db.is_transformation(source_name, source_variant)
+            != SourceType.PRIMARY_SOURCE.value
+        ):
+            feature_df = self.process_non_primary_df_transformation(
+                feature, source_name, source_variant, entity_id
+            )
         else:
-            raise Exception(f"No matching entities for {entity_id}: {entity_value}")
+            source = self.db.get_source_variant(source_name, source_variant)
+            feature_df = feature_df_with_entity(
+                source["definition"], entity_id, feature
+            )
 
-    def feature_df_with_entity(self, source_path, entity_id, feature):
+        return feature_df
+
+    def process_non_primary_df_transformation(
+        self, feature, source_name, source_variant, entity_id
+    ):
         name_variant = f"{feature['name']}.{feature['variant']}"
-        df = pd.read_csv(str(source_path))
-        self.check_missing_values(feature, df)
-        if feature['source_timestamp'] != "":
-            df = df[[feature['source_entity'], feature['source_value'], feature['source_timestamp']]]
-            df = df.sort_values(by=feature['source_timestamp'], ascending=True)
-            df = df.drop(columns=feature['source_timestamp'])
-        else:
-            df = df[[feature['source_entity'], feature['source_value']]]
-        df.set_index(feature['source_entity'])
-        df.rename(columns={feature['source_entity']: entity_id, feature['source_value']: name_variant}, inplace=True)
-        df.drop_duplicates(subset=[entity_id], keep="last", inplace=True)
+        feature_df = self.process_transformation(source_name, source_variant)
+        if isinstance(feature_df, pd.Series):
+            feature_df = feature_df.to_frame()
+            feature_df.reset_index(inplace=True)
+        if not feature["source_entity"] in feature_df.columns:
+            raise ValueError(
+                f"Could not set entity column. No column name {feature['source_entity']} exists in {source_name}-{source_variant}"
+            )
+        if not feature["source_value"] in feature_df.columns:
+            raise ValueError(
+                f"Could not access feature value column. No column name {feature['source_value']} exists in {source_name}-{source_variant}"
+            )
+        feature_df = feature_df[[feature["source_entity"], feature["source_value"]]]
+        feature_df.rename(
+            columns={
+                feature["source_entity"]: entity_id,
+                feature["source_value"]: name_variant,
+            },
+            inplace=True,
+        )
+        feature_df.drop_duplicates(subset=[entity_id], keep="last", inplace=True)
+        feature_df.set_index(entity_id)
+        return feature_df
+
+    def calculate_ondemand_feature(self, f_name, f_variant, entity_id):
+        query = self.db.get_ondemand_feature_query(f_name, f_variant)
+        base64_bytes = query.encode("ascii")
+        query = base64.b64decode(base64_bytes)
+
+        code = dill.loads(bytearray(query))
+        func = types.FunctionType(code, globals(), "transformation")
+        output_value = func(self, self.params, self.entities)
+
+        feature_col_name = f"{f_name}.{f_variant}"
+        df = pd.DataFrame.from_dict(
+            {
+                entity_id: [self.entities.get(entity_id, "")],
+                feature_col_name: [output_value],
+            }
+        )
         return df
 
-    def check_missing_values(self, resource, df):
-        if resource['source_entity'] not in df.columns:
-            raise KeyError(f"Entity column does not exist: {resource['source_entity']}")
-        if resource['source_value'] not in df.columns:
-            raise KeyError(f"Value column does not exist: {resource['source_value']}")
-        if resource['source_timestamp'] not in df.columns and resource['source_timestamp'] != "":
-            raise KeyError(f"Timestamp column does not exist: {resource['source_timestamp']}")
+    @staticmethod
+    def convert_ts_df_to_dataset(label_row, trainingset_df, include_label_timestamp):
+        if label_row["source_timestamp"] != "" and include_label_timestamp != True:
+            trainingset_df.drop(columns=label_row["source_timestamp"], inplace=True)
+        elif label_row["source_timestamp"] != "" and include_label_timestamp:
+            source_timestamp_col = trainingset_df.pop(label_row["source_timestamp"])
+            trainingset_df = trainingset_df.assign(label_timestamp=source_timestamp_col)
+        trainingset_df.drop(columns=label_row["source_entity"], inplace=True)
 
+        label_col = trainingset_df.pop("label")
+        trainingset_df = trainingset_df.assign(label=label_col)
+        return Dataset.from_dataframe(trainingset_df, include_label_timestamp)
 
-    def _register_model(self, model: Union[str, Model], look_up_table: str, association_name: str, association_variant: str):
+    def _register_model(
+        self,
+        model: Union[str, Model],
+        look_up_table: str,
+        association_name: str,
+        association_variant: str,
+    ):
         name = model if isinstance(model, str) else model.name
         type = "Model" if isinstance(model, str) else model.type()
 
         self.db.insert("models", name, type)
         self.db.insert(look_up_table, name, association_name, association_variant)
 
+    def get_source_as_df(self, name, variant):
+        return self.get_input_df(name, variant)
 
-class Stream:
 
+class Stream:
     def __init__(self, stub, name, version, model: Union[str, Model] = None):
         req = serving_pb2.TrainingDataRequest()
         req.id.name = name
         req.id.version = version
         if model is not None:
             req.model.name = model if isinstance(model, str) else model.name
         self.name = name
@@ -514,15 +677,14 @@
         return Row(next(self._iter))
 
     def restart(self):
         self._iter = self._stub.TrainingData(self._req)
 
 
 class LocalStream:
-
     def __init__(self, datalist, include_label_timestamp):
         self._datalist = datalist
         self._iter = iter(datalist)
         self._include_label_timestamp = include_label_timestamp
 
     def __iter__(self):
         return iter(self._iter)
@@ -531,15 +693,14 @@
         return LocalRow(next(self._iter), self._include_label_timestamp)
 
     def restart(self):
         self._iter = iter(self._datalist)
 
 
 class Repeat:
-
     def __init__(self, repeat_num, stream):
         self.repeat_num = repeat_num
         self._stream = stream
 
     def __iter__(self):
         return self
 
@@ -554,15 +715,14 @@
             else:
                 raise
 
         return next_val
 
 
 class Shuffle:
-
     def __init__(self, buffer_size, stream):
         self.buffer_size = buffer_size
         self._shuffled_data_list = []
         self._stream = stream
         self.__setup_buffer()
 
     def __setup_buffer(self):
@@ -590,15 +750,14 @@
         except StopIteration:
             pass
 
         return next_row
 
 
 class Batch:
-
     def __init__(self, batch_size, stream):
         self.batch_size = batch_size
         self._stream = stream
 
     def restart(self):
         self._stream.restart()
 
@@ -615,15 +774,14 @@
                 if len(rows) == 0:
                     raise
                 return rows
         return rows
 
 
 class Dataset:
-
     def __init__(self, stream, dataframe=None):
         """Repeats the Dataset for the specified number of times
 
         Args:
             stream (Iterator): An iterable object.
 
         Returns:
@@ -631,15 +789,15 @@
         """
         self._stream = stream
         self._dataframe = dataframe
 
     def from_stub(self, name, version, model: Union[str, Model] = None):
         stream = Stream(self._stream, name, version, model)
         return Dataset(stream)
-    
+
     def from_dataframe(dataframe, include_label_timestamp):
         stream = LocalStream(dataframe.values.tolist(), include_label_timestamp)
         return Dataset(stream, dataframe)
 
     def pandas(self):
         return self._dataframe
 
@@ -686,15 +844,15 @@
         Returns:
             self (Dataset): Returns the current Dataset
         """
         if buffer_size <= 0:
             raise Exception("Buffer size must be greater than or equal to 1")
         self._stream = Shuffle(buffer_size, self._stream)
         if self._dataframe is not None:
-            self._dataframe = self._dataframe.sample(frac=1) 
+            self._dataframe = self._dataframe.sample(frac=1)
         return self
 
     def batch(self, batch_size):
         """Creates a batch row in the Dataset.
 
         **Examples**:
         ``` py
@@ -710,51 +868,52 @@
         Returns:
             self (Dataset): Returns the current Dataset
         """
         if batch_size <= 0:
             raise Exception("Batch size must be greater than or equal to 1")
         self._stream = Batch(batch_size, self._stream)
         if self._dataframe is not None:
-            self._dataframe = np.array_split(self._dataframe, math.ceil(len(self._dataframe) // batch_size))
+            self._dataframe = np.array_split(
+                self._dataframe, math.ceil(len(self._dataframe) // batch_size)
+            )
         return self
 
     def __iter__(self):
         return self
 
     def __next__(self):
         next_val = next(self._stream)
         return next_val
 
 
 class Row:
-
     def __init__(self, proto_row):
         features = np.array(
-            [parse_proto_value(feature) for feature in proto_row.features])
+            [parse_proto_value(feature) for feature in proto_row.features]
+        )
         self._label = parse_proto_value(proto_row.label)
         self._row = np.append(features, self._label)
 
     def features(self):
         return [self._row[:-1]]
 
     def label(self):
         return [self._label]
 
     def to_numpy(self):
-        return self._row()
+        return self._row
 
     def __repr__(self):
         return "Features: {} , Label: {}".format(self.features(), self.label())
 
 
 class LocalRow:
-
     def __init__(self, row_list, include_label_timestamp):
         """
-        If include_label_timestamp is true then we want the label to equal to the 
+        If include_label_timestamp is true then we want the label to equal to the
         last two columns in the list. Otherwise, just the label will be the last column only.
         """
 
         self._features = row_list[:-2] if include_label_timestamp else row_list[:-1]
         self._row = row_list
         self._label = row_list[-2:] if include_label_timestamp else row_list[-1]
 
@@ -768,15 +927,14 @@
         return np.array(self._row)
 
     def __repr__(self):
         return "Features: {} , Label: {}".format(self.features(), self.label())
 
 
 class BatchRow:
-
     def __init__(self, rows=None):
         self._features = []
         self._labels = []
         if rows is None:
             rows = []
         self._rows = rows
         for row in rows:
@@ -797,10 +955,9 @@
         return self._rows
 
     def __len__(self):
         return len(self._rows)
 
 
 def parse_proto_value(value):
-    """ parse_proto_value is used to parse the one of Value message
-	"""
+    """parse_proto_value is used to parse the one of Value message"""
     return getattr(value, value.WhichOneof("value"))
```

### Comparing `featureform-1.7.3rc5/src/featureform/sqlite_metadata.py` & `featureform-1.7.4/src/featureform/sqlite_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,22 +60,45 @@
 
           PRIMARY KEY(name, variant),
 
           FOREIGN KEY(name) REFERENCES features(name),
           FOREIGN KEY(entity) REFERENCES entities(name),
           FOREIGN KEY(provider) REFERENCES providers(name),
           FOREIGN KEY(source_name) REFERENCES sources(name))''')
+      
+        # OnDemand Features variant table
+        self.__conn.execute('''CREATE TABLE IF NOT EXISTS ondemand_feature_variant(
+          created text,
+          description text,
+          name text NOT NULL,
+          owner text,
+          variant text NOT NULL,
+          status text,
+          query text,
+
+          PRIMARY KEY(name, variant),
+
+          FOREIGN KEY(name) REFERENCES features(name))''')
 
         # Features table
         self.__conn.execute('''CREATE TABLE IF NOT EXISTS features(
           name text NOT NULL,
           default_variant text NOT NULL,
           type text,
           PRIMARY KEY (name));''')
 
+        # features type table
+        # this is used to determine if it is a pre-calculated or client-calculated feature
+        self.__conn.execute('''CREATE TABLE IF NOT EXISTS feature_computation_mode (
+          name text NOT NULL,
+          variant text NOT NULL,
+          mode text,
+          is_on_demand integer,
+          PRIMARY KEY (name, variant));''')
+
         # training set variant
         self.__conn.execute('''CREATE TABLE IF NOT EXISTS training_set_variant(
           created text,
           description text,            
           name text NOT NULL,
           owner text,
           variant text,
@@ -198,14 +221,25 @@
           provider_type     text,
           software         text,
           team             text,
           sources          text,
           status           text,
           serialized_config text)''')
 
+        # source files for a resource
+        # tracks the source files that have been used to create a resource and contains the files last_updated
+        # this is used to determined if caches need to be invalidated
+        self.__conn.execute('''CREATE TABLE IF NOT EXISTS resource_source_files(
+            resource_type text NOT NULL,
+            name text NOT NULL,
+            variant text NOT NULL,
+            file_path text NOT NULL,
+            updated_at text NOT NULL,
+            PRIMARY KEY(resource_type, name, variant, file_path))''')
+
         # full-text search table
         self.__conn.execute('''CREATE VIRTUAL TABLE IF NOT EXISTS resources_fts USING fts5(
           resource_type, -- an "enum" column to filter with (e.g. feature, training_set, source, provider, entity, label, model, user)
           name,
           variant,
           description,
           status,
@@ -346,27 +380,27 @@
       return self.query_resource("users", "name", name, should_fetch_tags_properties)[0]
 
     def get_entity(self, name, should_fetch_tags_properties):
       return self.query_resource("entities", "name", name, should_fetch_tags_properties)[0]
 
     def get_feature(self, name, should_fetch_tags_properties):
       return self.query_resource("features", "name", name, should_fetch_tags_properties)[0]
-    
+
     def get_label(self, name, should_fetch_tags_properties):
       return self.query_resource("labels", "name", name, should_fetch_tags_properties)[0]
-    
+
     def get_source(self, name, should_fetch_tags_properties):
       return self.query_resource("sources", "name", name, should_fetch_tags_properties)[0]
 
     def get_training_set(self, name, should_fetch_tags_properties):
       return self.query_resource("training_sets", "name", name, should_fetch_tags_properties)[0]
-    
+
     def get_model(self, name, should_fetch_tags_properties):
       return self.query_resource("models", "name", name, should_fetch_tags_properties)[0]
-    
+
     def get_provider(self, name, should_fetch_tags_properties):
       return self.query_resource("providers", "name", name, should_fetch_tags_properties)[0]
 
     def get_feature_variant(self, name, variant):
         query = '''SELECT fv.*, t.tag_list as tags, p.property_list as properties
         FROM feature_variant fv
         LEFT JOIN tags t ON t.name = fv.name AND t.variant = fv.variant
@@ -383,14 +417,26 @@
         LEFT JOIN tags t ON t.name = fv.name AND t.variant = fv.variant
         LEFT JOIN properties p ON p.name = fv.name AND p.variant = fv.variant
         WHERE fv.source_name = '{0}' AND fv.source_variant = '{1}';'''.format(name, variant)
         return self.fetch_data_safe(query, "feature_variant", name, variant)
 
     def get_feature_variants_from_feature(self, name):
       return self.query_resource_variant("feature_variant", "name", name)
+    
+    def get_feature_variant_mode(self, name, variant):
+      query = f"SELECT mode FROM feature_computation_mode WHERE name='{name}' AND variant='{variant}'"
+      return self.fetch_data_safe(query, "feature_computation_mode", name, variant)[0]["mode"]
+    
+    def get_feature_variant_on_demand(self, name, variant):
+      query = f"SELECT is_on_demand FROM feature_computation_mode WHERE name='{name}' AND variant='{variant}'"
+      return bool(self.fetch_data_safe(query, "feature_computation_mode", name, variant)[0]["is_on_demand"])
+
+    def get_ondemand_feature_query(self, name, variant):
+      query = f"SELECT query FROM ondemand_feature_variant WHERE name='{name}' AND variant='{variant}'"
+      return self.fetch_data_safe(query, "ondemand_feature_variant", name, variant)[0]["query"]
 
     def get_training_set_variant(self, name, variant):
         query = f"SELECT * FROM training_set_variant WHERE name = '{name}' AND variant = '{variant}';"
         query = '''SELECT v.*, t.tag_list as tags, p.property_list as properties
         FROM training_set_variant v
         LEFT JOIN tags t ON t.name = v.name AND t.variant = v.variant
         LEFT JOIN properties p ON p.name = v.name AND p.variant = v.variant
@@ -496,27 +542,51 @@
         transformation = self.__conn.execute(query)
         self.__conn.commit()
         t = transformation.fetchall()
         if len(t) == 0:
             return 0
         return t[0][0]
 
+    def get_source_files_for_resource(self, resource_type, name, variant):
+        query = f"SELECT * FROM resource_source_files WHERE resource_type='{resource_type}' and name='{name}' and variant='{variant}';"
+        result = self.__conn.execute(query)
+        self.__conn.commit()
+        return result.fetchall()
+
+    def get_source_file_last_updated(self, resource_type, name, variant, file_path):
+        query = f"SELECT * FROM resource_source_files WHERE resource_type='{resource_type}' and name='{name}' and variant='{variant}' and file_path='{file_path}';"
+        result = self.__conn.execute(query)
+        self.__conn.commit()
+        res = result.fetchone()
+        return res[0] if res else None
+
     def insert_source(self, tablename, *args):
         stmt = f"INSERT OR IGNORE INTO {tablename} VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)"
         self.__conn.execute_stmt(stmt, args)
         self.__conn.commit()
 
     def insert(self, tablename, *args):
         query = f"INSERT OR IGNORE INTO {tablename} VALUES {str(args)}"
         self.__conn.execute(query)
         self.__conn.commit()
 
+    def insert_or_update(self, tablename, keys, cols, *args):
+        """
+        Upserts a row into the table. `keys` indicate columns that are unique
+        and `cols` are the columns that are updated.
+        """
+        query = (
+            f"INSERT INTO {tablename} VALUES {str(args)} "
+            f"ON CONFLICT ({','.join(keys)}) DO UPDATE SET {','.join([f'{col}=excluded.{col}' for col in cols])}"
+        )
+        self.__conn.execute(query)
+        self.__conn.commit()
+
+    # TODO get something generic working, possibly consider using the above insert or update
     def upsert(self, tablename, *args):
-        query = ""
-        is_update = False
         if tablename == "tags" or tablename == "properties":
            query, is_update = self.upsert_tags_properties(tablename, *args)
         else:
            raise NotImplementedError(f"UPSERT not implemented for table {tablename}")
 
         if is_update:
           self.__conn.execute(query)
```

### Comparing `featureform-1.7.3rc5/src/featureform/type_objects.py` & `featureform-1.7.4/src/featureform/type_objects.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform/version.py` & `featureform-1.7.4/src/featureform/version.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/src/featureform.egg-info/PKG-INFO` & `featureform-1.7.4/src/featureform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform
-Version: 1.7.3rc5
+Version: 1.7.4
 Summary: Package for the Featureform Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/embeddinghub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `featureform-1.7.3rc5/src/featureform.egg-info/SOURCES.txt` & `featureform-1.7.4/src/featureform.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,29 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 src/featureform/__init__.py
 src/featureform/__main__.py
 src/featureform/cli.py
+src/featureform/client.py
 src/featureform/dashboard_metadata.py
+src/featureform/enums.py
+src/featureform/exceptions.py
 src/featureform/format.py
 src/featureform/get.py
 src/featureform/get_local.py
 src/featureform/get_test.py
 src/featureform/list.py
 src/featureform/list_local.py
 src/featureform/list_test.py
 src/featureform/local.py
+src/featureform/local_cache.py
 src/featureform/local_dash_test.py
+src/featureform/local_utils.py
 src/featureform/register.py
 src/featureform/register_test.py
 src/featureform/resources.py
 src/featureform/search.py
 src/featureform/search_local.py
 src/featureform/serving.py
 src/featureform/serving_test.py
@@ -37,14 +42,16 @@
 src/featureform/dashboard/out/[type].html
 src/featureform/dashboard/out/connections.html
 src/featureform/dashboard/out/index.html
 src/featureform/dashboard/out/robots.txt
 src/featureform/dashboard/out/search.html
 src/featureform/dashboard/out/site.webmanifest
 src/featureform/dashboard/out/[type]/[entity].html
+src/featureform/dashboard/out/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js
+src/featureform/dashboard/out/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
 src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js
 src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js
 src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js
 src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js
 src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js
@@ -272,25 +279,23 @@
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.28bbfbd268843c68.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js
 src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js
 src/featureform/dashboard/out/_next/static/chunks/pages/404-baaca4b2f4acc755.js
 src/featureform/dashboard/out/_next/static/chunks/pages/[type]-751a928da9d524e9.js
-src/featureform/dashboard/out/_next/static/chunks/pages/_app-01b1894ee40506d5.js
+src/featureform/dashboard/out/_next/static/chunks/pages/_app-a764893ff9420ec0.js
 src/featureform/dashboard/out/_next/static/chunks/pages/_error-3f70f2d61eb8c6dd.js
 src/featureform/dashboard/out/_next/static/chunks/pages/connections-1d67ba61869dece6.js
 src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js
 src/featureform/dashboard/out/_next/static/chunks/pages/search-175858e61ba25631.js
 src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-b07f3c4463890639.js
 src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js
 src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
 src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
-src/featureform/dashboard/out/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_buildManifest.js
-src/featureform/dashboard/out/_next/static/tM9MEYWwbsEHYQ8l3Xl7G/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
 src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
 src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
 src/featureform/dashboard/out/static/Apache_Spark_logo.svg
 src/featureform/dashboard/out/static/Capital_One_logo.svg
 src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
@@ -322,14 +327,18 @@
 src/featureform/proto/serving.proto
 src/featureform/proto/serving_pb2.py
 src/featureform/proto/serving_pb2_grpc.py
 tests/test_class_api.py
 tests/test_cli.py
 tests/test_executor_resources.py
 tests/test_getting_model.py
+tests/test_localmode_caching.py
 tests/test_localmode_include_label_ts.py
 tests/test_localmode_lag_features.py
+tests/test_ondemand_features.py
+tests/test_resource_registration.py
 tests/test_search.py
 tests/test_serving_model.py
+tests/test_source_dataframe.py
 tests/test_spark_provider.py
 tests/test_tags_and_properties.py
 tests/test_updating_provider.py
```

### Comparing `featureform-1.7.3rc5/tests/test_cli.py` & `featureform-1.7.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/tests/test_executor_resources.py` & `featureform-1.7.4/tests/test_executor_resources.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/tests/test_getting_model.py` & `featureform-1.7.4/tests/test_getting_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,10 +64,10 @@
     setup_teardown()
     yield
     setup_teardown()
 
 def arrange_resources(model_name, is_local, is_insecure):
     ff.register_model(model_name)
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
-    resource_client.apply()
+    resource_client.apply(asynchronous=True)
 
     return resource_client
```

### Comparing `featureform-1.7.3rc5/tests/test_localmode_include_label_ts.py` & `featureform-1.7.4/tests/test_localmode_include_label_ts.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,41 +14,26 @@
 
     @local.df_transformation(variant="quickstart",
                                 inputs=[("transactions", "quickstart")])
     def average_user_transaction(transactions):
         """the average transaction amount for a user """
         return transactions.groupby("CustomerID")["TransactionAmount"].mean()
 
-    @local.sql_transformation(variant="quickstart")
-    def sql_average_user_transaction():
-        """the average transaction amount for a user """
-        return "SELECT CustomerID as user_id, avg(TransactionAmount) " \
-            "as avg_transaction_amt from {{transactions.kaggle}} GROUP BY user_id"
-
     user = ff.register_entity("user")
 
     # Register a column from our transformation as a feature
     average_user_transaction.register_resources(
         entity=user,
         entity_column="CustomerID",
         inference_store=local,
         features=[
             {"name": "avg_transactions", "variant": "quickstart", "column": "TransactionAmount", "type": "float32"},
         ],
     )
 
-    sql_average_user_transaction.register_resources(
-        entity=user,
-        entity_column="CustomerID",
-        inference_store=local,
-        features=[
-            {"name": "avg_transactions", "variant": "sql", "column": "TransactionAmount", "type": "float32"},
-        ],
-    )
-
     # Register label from our base Transactions table
     transactions.register_resources(
         entity=user,
         entity_column="CustomerID",
         timestamp_column="Timestamp",
         labels=[
             {"name": "fraudulent", "variant": "quickstart", "column": "IsFraud", "type": "bool"},
```

### Comparing `featureform-1.7.3rc5/tests/test_localmode_lag_features.py` & `featureform-1.7.4/tests/test_localmode_lag_features.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/tests/test_search.py` & `featureform-1.7.4/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/tests/test_serving_model.py` & `featureform-1.7.4/tests/test_serving_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import time
 import featureform as ff
 from featureform.resources import Model
 import pytest
 
+
 @pytest.mark.parametrize(
     "provider_source_fxt,serving_client_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", "serving_client", True, True, marks=pytest.mark.local),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, False, marks=pytest.mark.hosted),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, True, marks=pytest.mark.docker),
     ]
@@ -21,14 +22,18 @@
 
     fts = serving_client.features([("avg_transactions", "quickstart")], {"user": "C1410926"})
 
     models = resource_client.list_models(is_local)
 
     assert len(models) == 0
 
+    # TODO: Shouldn't have to do this
+    if is_local:
+        serving_client.impl.db.close()
+
 
 @pytest.mark.parametrize(
     "provider_source_fxt,serving_client_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", "serving_client", True, True, marks=pytest.mark.local),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, False, marks=pytest.mark.hosted),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, True, marks=pytest.mark.docker),
@@ -47,14 +52,17 @@
     ts = serving_client.training_set("fraud_training", "quickstart", model=model_name_a)
     next(ts)
 
     model = resource_client.get_model(model_name_a, is_local)
 
     assert isinstance(model, Model) and model.name == model_name_a and model.type() == "model"
 
+    if is_local:
+        serving_client.impl.db.close()
+
 
 @pytest.mark.parametrize(
     "provider_source_fxt,serving_client_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", "serving_client", True, True, marks=pytest.mark.local),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, False, marks=pytest.mark.hosted),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, True, marks=pytest.mark.docker),
@@ -80,14 +88,17 @@
     models_names = [model.name for model in models]
 
     contains_expected_names = all(expected_name in models_names for expected_name in [model_name_b, model_name_c])
     are_models_instances = all([isinstance(model, Model) for model in models])
 
     assert contains_expected_names and are_models_instances
 
+    if is_local:
+        serving_client.impl.db.close()
+
 
 @pytest.mark.parametrize(
     "provider_source_fxt,serving_client_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", "serving_client", True, True, marks=pytest.mark.local),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, False, marks=pytest.mark.hosted),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, True, marks=pytest.mark.docker),
@@ -109,14 +120,17 @@
     next(ts_2)
 
     models = resource_client.list_models(is_local)
     expected = [model.name for model in models if model.name == model_name_d]
 
     assert model_name_d in expected and len(expected) == 1 and all([isinstance(model, Model) for model in models])
 
+    if is_local:
+        serving_client.impl.db.close()
+
 
 @pytest.mark.parametrize(
     "provider_source_fxt,serving_client_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", "serving_client", True, True, marks=pytest.mark.local),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, False, marks=pytest.mark.hosted),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, True, marks=pytest.mark.docker),
@@ -134,14 +148,17 @@
 
     fts = serving_client.features([("avg_transactions", "quickstart")], {"user": "C1410926"}, model=model_name_e)
 
     model = resource_client.get_model(model_name_e, is_local)
 
     assert isinstance(model, Model) and model.name == model_name_e and model.type() == "model"
 
+    if is_local:
+        serving_client.impl.db.close()
+
 
 @pytest.mark.parametrize(
     "provider_source_fxt,serving_client_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", "serving_client", True, True, marks=pytest.mark.local),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, False, marks=pytest.mark.hosted),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, True, marks=pytest.mark.docker),
@@ -165,14 +182,17 @@
     models_names = [model.name for model in models]
 
     contains_expected_names = all(expected_name in models_names for expected_name in [model_name_f, model_name_g])
     are_models_instances = all([isinstance(model, Model) for model in models])
 
     assert contains_expected_names and are_models_instances
 
+    if is_local:
+        serving_client.impl.db.close()
+
 
 @pytest.mark.parametrize(
     "provider_source_fxt,serving_client_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", "serving_client", True, True, marks=pytest.mark.local),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, False, marks=pytest.mark.hosted),
         pytest.param("hosted_sql_provider_and_source","serving_client", False, True, marks=pytest.mark.docker),
@@ -192,14 +212,17 @@
     fts_2 = serving_client.features([("avg_transactions", "quickstart")], {"user": "C1410926"}, model=model_name_h)
 
     models = resource_client.list_models(is_local)
     expected = [model.name for model in models if model.name == model_name_h]
 
     assert model_name_h in expected and len(expected) == 1 and all([isinstance(model, Model) for model in models])
 
+    if is_local:
+        serving_client.impl.db.close()
+
 
 @pytest.fixture(autouse=True)
 def before_and_after_each(setup_teardown):
     setup_teardown()
     yield
     setup_teardown()
 
@@ -242,15 +265,15 @@
     ff.register_training_set(
         training_set_name, training_set_variant,
         label=("fraudulent", "quickstart"),
         features=[("avg_transactions", "quickstart")],
     )
 
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
-    resource_client.apply()
+    resource_client.apply(asynchronous=True)
 
     if not is_local:
         start = time.time()
         while True:
             time.sleep(3)
             ts = resource_client.get_training_set(training_set_name, training_set_variant)
             elapsed_wait = time.time() - start
```

### Comparing `featureform-1.7.3rc5/tests/test_spark_provider.py` & `featureform-1.7.4/tests/test_spark_provider.py`

 * *Files 18% similar despite different names*

```diff
@@ -83,33 +83,62 @@
         description="doc string",
         tags=[],
         properties={}
     )
 
 
 @pytest.mark.parametrize(
-    "name,variant,transformation",
+    "sql",
     [
-        ("test_name", "test_variant","avg_user_transaction"),
+        ("SELECT * FROM {{test_name.test_variant}}"),
     ]
 )
-def test_df_transformation(name, variant, transformation, spark_provider, request):
+def test_sql_transformation_without_variant(sql, spark_provider):
+    def transformation():
+        """doc string"""
+        return sql
+
+    decorator = spark_provider.sql_transformation()
+    decorator(transformation)
+
+    assert decorator.to_source() == Source(
+        name=transformation.__name__,
+        variant="default",
+        definition=SQLTransformation(query=sql),
+        owner="tester",
+        provider="spark",
+        description="doc string",
+        tags=[],
+        properties={}
+    )
+
+
+@pytest.mark.parametrize(
+    "name,variant,inputs,transformation",
+    [
+        ("test_input", "primary_dataset", "primary_dataset", "avg_user_transaction"),
+        ("test_input", "df_transformation", "df_transformation_src", "avg_user_transaction"),
+        ("test_input", "sql_transformation", "sql_transformation_src", "avg_user_transaction"),
+        ("test_input", "tuples", "tuple_inputs", "avg_user_transaction"),
+    ]
+)
+def test_df_transformation(name, variant, inputs, transformation, spark_provider, request):
     df_transformation = request.getfixturevalue(transformation)
+    inputs = request.getfixturevalue(inputs)
 
-    src_variant = f"{variant}_src"
-    decorator = spark_provider.df_transformation(name=name, variant=variant, inputs=[(name, src_variant)])
+    decorator = spark_provider.df_transformation(name=name, variant=variant, inputs=inputs)
     decorator(df_transformation)
 
     query = dill.dumps(df_transformation.__code__)
 
     decorator_src = decorator.to_source()
     expected_src = Source(
         name=name,
         variant=variant,
-        definition=DFTransformation(query=query, inputs=[(name, src_variant)]),
+        definition=DFTransformation(query=query, inputs=inputs),
         owner="tester",
         provider="spark",
         description="doc string",
         tags=[],
         properties={}
     )
     
@@ -160,14 +189,15 @@
         ("3.9","3.9.16"),
         ("3.10","3.10.10"),
         ("3.7.10","3.7.16"),
         ("3.7.1","3.7.16"),
         ("3.8.16","3.8.16"),
         ("3.9.11","3.9.16"),
         ("3.10.10","3.10.10"),
+        ("3.11.2","3.11.2"),
         pytest.param("3","", marks=pytest.mark.xfail),
         pytest.param("3.","", marks=pytest.mark.xfail),
         pytest.param("2.10","", marks=pytest.mark.xfail),
         pytest.param("3.10.10.0","", marks=pytest.mark.xfail),
     ]
 )
 def test__verify_python_version(version, expected_version):
```

### Comparing `featureform-1.7.3rc5/tests/test_tags_and_properties.py` & `featureform-1.7.4/tests/test_tags_and_properties.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.3rc5/tests/test_updating_provider.py` & `featureform-1.7.4/tests/test_updating_provider.py`

 * *Files identical despite different names*

