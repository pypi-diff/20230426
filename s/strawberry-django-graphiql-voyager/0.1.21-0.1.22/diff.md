# Comparing `tmp/strawberry_django_graphiql_voyager-0.1.21.tar.gz` & `tmp/strawberry_django_graphiql_voyager-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_graphiql_voyager-0.1.21.tar", last modified: Wed Apr 26 16:05:51 2023, max compression
+gzip compressed data, was "strawberry_django_graphiql_voyager-0.1.22.tar", last modified: Wed Apr 26 17:07:00 2023, max compression
```

## Comparing `strawberry_django_graphiql_voyager-0.1.21.tar` & `strawberry_django_graphiql_voyager-0.1.22.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 16:05:51.042214 strawberry_django_graphiql_voyager-0.1.21/
--rw-r--r--   0 mdizon     (501) staff       (20)     1070 2022-07-27 16:26:09.000000 strawberry_django_graphiql_voyager-0.1.21/LICENSE
--rw-r--r--   0 mdizon     (501) staff       (20)      160 2022-07-27 17:00:14.000000 strawberry_django_graphiql_voyager-0.1.21/MANIFEST.in
--rw-r--r--   0 mdizon     (501) staff       (20)      969 2023-04-26 16:05:51.042369 strawberry_django_graphiql_voyager-0.1.21/PKG-INFO
--rw-r--r--   0 mdizon     (501) staff       (20)       37 2022-07-27 16:25:56.000000 strawberry_django_graphiql_voyager-0.1.21/README.md
--rw-r--r--   0 mdizon     (501) staff       (20)      945 2023-04-26 16:05:51.044784 strawberry_django_graphiql_voyager-0.1.21/setup.cfg
--rw-r--r--   0 mdizon     (501) staff       (20)       38 2022-07-27 15:52:06.000000 strawberry_django_graphiql_voyager-0.1.21/setup.py
-drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 16:05:50.967558 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/
--rw-r--r--   0 mdizon     (501) staff       (20)        0 2022-07-27 15:52:06.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/__init__.py
-drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 16:05:50.965361 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/
-drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 16:05:50.965627 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/
-drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 16:05:50.965547 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/
-drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 16:05:50.971234 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/
--rw-r--r--   0 mdizon     (501) staff       (20)    33027 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/11.66866c8b.chunk.css
--rw-r--r--   0 mdizon     (501) staff       (20)    52338 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/11.66866c8b.chunk.css.map
--rw-r--r--   0 mdizon     (501) staff       (20)      389 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/main.d0b1e8f9.chunk.css
--rw-r--r--   0 mdizon     (501) staff       (20)      679 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/main.d0b1e8f9.chunk.css.map
-drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 16:05:51.023567 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/
--rw-r--r--   0 mdizon     (501) staff       (20)   183825 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/0.d69ee02e.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)   703219 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/0.d69ee02e.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)    53368 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/1.d76c06cc.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)   171605 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/1.d76c06cc.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)   720327 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/11.8fdec039.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)  2599509 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/11.8fdec039.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)    32522 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/12.a9526db5.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)   119573 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/12.a9526db5.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     9468 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/13.2ac64509.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    32711 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/13.2ac64509.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     9779 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/14.d5d84371.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    37491 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/14.d5d84371.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     6431 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/15.812c88f9.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    21743 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/15.812c88f9.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     6142 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/16.ce8357ac.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    24306 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/16.ce8357ac.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     3632 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/17.e84c62d5.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    13648 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/17.e84c62d5.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     4100 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/18.9d20f18a.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    14584 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/18.9d20f18a.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     5109 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/19.8e86fbfa.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    16860 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/19.8e86fbfa.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)    16024 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/2.591f5756.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    60169 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/2.591f5756.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     5293 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/20.3b18185a.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    17415 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/20.3b18185a.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     4409 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/21.41f21244.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    16899 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/21.41f21244.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     4767 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/22.8fbf3b0e.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    18823 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/22.8fbf3b0e.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     2761 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/23.6098cda7.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)     9363 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/23.6098cda7.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)    20001 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/24.d76a1f43.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    79418 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/24.d76a1f43.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     6077 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/25.53cfe552.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    21986 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/25.53cfe552.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     3896 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/26.5a70ef0a.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    14204 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/26.5a70ef0a.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)    11642 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/27.c2a642ff.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    39909 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/27.c2a642ff.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)    26167 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/3.be05d828.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    93074 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/3.be05d828.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     4806 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/4.6c088241.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    16894 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/4.6c088241.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     2884 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/5.2f6c7945.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    11659 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/5.2f6c7945.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     3066 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/6.c7c77fbb.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    11293 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/6.c7c77fbb.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     5948 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/7.b605e08f.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    21799 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/7.b605e08f.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     6305 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/8.32bdc3c7.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    25710 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/8.32bdc3c7.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     5731 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/main.0d12cfba.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)    20718 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/main.0d12cfba.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     2591 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/runtime~main.75c1c0e5.js
--rw-r--r--   0 mdizon     (501) staff       (20)    12794 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/runtime~main.75c1c0e5.js.map
-drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 16:05:50.965764 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/
-drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 16:05:51.025959 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/css/
--rw-r--r--   0 mdizon     (501) staff       (20)      344 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/css/main.34de6062.chunk.css
--rw-r--r--   0 mdizon     (501) staff       (20)      579 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/css/main.34de6062.chunk.css.map
-drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 16:05:51.035692 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/
--rw-r--r--   0 mdizon     (501) staff       (20)   800098 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/2.30b5ba40.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)  3417792 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/2.30b5ba40.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)      868 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/main.6d24c0c6.chunk.js
--rw-r--r--   0 mdizon     (501) staff       (20)     6929 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/main.6d24c0c6.chunk.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)     1502 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/runtime~main.a8a9905a.js
--rw-r--r--   0 mdizon     (501) staff       (20)     7996 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/runtime~main.a8a9905a.js.map
--rw-r--r--   0 mdizon     (501) staff       (20)  1979770 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/voyager.worker.js
-drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 16:05:50.965911 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/templates/
-drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 16:05:51.041854 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/templates/strawberry_django_graphiql_voyager/
--rw-r--r--   0 mdizon     (501) staff       (20)     6595 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/templates/strawberry_django_graphiql_voyager/graphiql.html
--rw-r--r--   0 mdizon     (501) staff       (20)     4273 2022-08-03 12:39:37.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/templates/strawberry_django_graphiql_voyager/voyager.html
--rw-r--r--   0 mdizon     (501) staff       (20)     1948 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/views.py
-drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 16:05:50.969471 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager.egg-info/
--rw-r--r--   0 mdizon     (501) staff       (20)      969 2023-04-26 16:05:50.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager.egg-info/PKG-INFO
--rw-r--r--   0 mdizon     (501) staff       (20)     8296 2023-04-26 16:05:50.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager.egg-info/SOURCES.txt
--rw-r--r--   0 mdizon     (501) staff       (20)        1 2023-04-26 16:05:50.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager.egg-info/dependency_links.txt
--rw-r--r--   0 mdizon     (501) staff       (20)       35 2023-04-26 16:05:50.000000 strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager.egg-info/top_level.txt
+drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 17:07:00.828408 strawberry_django_graphiql_voyager-0.1.22/
+-rw-r--r--   0 mdizon     (501) staff       (20)     1070 2022-07-27 16:26:09.000000 strawberry_django_graphiql_voyager-0.1.22/LICENSE
+-rw-r--r--   0 mdizon     (501) staff       (20)      160 2022-07-27 17:00:14.000000 strawberry_django_graphiql_voyager-0.1.22/MANIFEST.in
+-rw-r--r--   0 mdizon     (501) staff       (20)      969 2023-04-26 17:07:00.828527 strawberry_django_graphiql_voyager-0.1.22/PKG-INFO
+-rw-r--r--   0 mdizon     (501) staff       (20)       37 2022-07-27 16:25:56.000000 strawberry_django_graphiql_voyager-0.1.22/README.md
+-rw-r--r--   0 mdizon     (501) staff       (20)      945 2023-04-26 17:07:00.828933 strawberry_django_graphiql_voyager-0.1.22/setup.cfg
+-rw-r--r--   0 mdizon     (501) staff       (20)       38 2022-07-27 15:52:06.000000 strawberry_django_graphiql_voyager-0.1.22/setup.py
+drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 17:07:00.761865 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/
+-rw-r--r--   0 mdizon     (501) staff       (20)        0 2022-07-27 15:52:06.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/__init__.py
+drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 17:07:00.759694 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/
+drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 17:07:00.759967 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/
+drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 17:07:00.759886 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/
+drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 17:07:00.767183 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/
+-rw-r--r--   0 mdizon     (501) staff       (20)    33027 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/11.66866c8b.chunk.css
+-rw-r--r--   0 mdizon     (501) staff       (20)    52338 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/11.66866c8b.chunk.css.map
+-rw-r--r--   0 mdizon     (501) staff       (20)      389 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/main.d0b1e8f9.chunk.css
+-rw-r--r--   0 mdizon     (501) staff       (20)      679 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/main.d0b1e8f9.chunk.css.map
+drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 17:07:00.813579 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/
+-rw-r--r--   0 mdizon     (501) staff       (20)   183825 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/0.d69ee02e.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)   703219 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/0.d69ee02e.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)    53368 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/1.d76c06cc.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)   171605 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/1.d76c06cc.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)   720327 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/11.8fdec039.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)  2599509 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/11.8fdec039.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)    32522 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/12.a9526db5.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)   119573 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/12.a9526db5.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     9468 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/13.2ac64509.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    32711 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/13.2ac64509.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     9779 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/14.d5d84371.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    37491 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/14.d5d84371.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     6431 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/15.812c88f9.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    21743 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/15.812c88f9.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     6142 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/16.ce8357ac.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    24306 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/16.ce8357ac.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     3632 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/17.e84c62d5.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    13648 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/17.e84c62d5.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     4100 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/18.9d20f18a.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    14584 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/18.9d20f18a.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     5109 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/19.8e86fbfa.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    16860 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/19.8e86fbfa.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)    16024 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/2.591f5756.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    60169 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/2.591f5756.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     5293 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/20.3b18185a.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    17415 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/20.3b18185a.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     4409 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/21.41f21244.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    16899 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/21.41f21244.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     4767 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/22.8fbf3b0e.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    18823 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/22.8fbf3b0e.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     2761 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/23.6098cda7.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)     9363 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/23.6098cda7.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)    20001 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/24.d76a1f43.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    79418 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/24.d76a1f43.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     6077 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/25.53cfe552.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    21986 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/25.53cfe552.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     3896 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/26.5a70ef0a.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    14204 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/26.5a70ef0a.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)    11642 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/27.c2a642ff.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    39909 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/27.c2a642ff.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)    26167 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/3.be05d828.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    93074 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/3.be05d828.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     4806 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/4.6c088241.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    16894 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/4.6c088241.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     2884 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/5.2f6c7945.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    11659 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/5.2f6c7945.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     3066 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/6.c7c77fbb.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    11293 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/6.c7c77fbb.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     5948 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/7.b605e08f.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    21799 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/7.b605e08f.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     6305 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/8.32bdc3c7.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    25710 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/8.32bdc3c7.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     5731 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/main.0d12cfba.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    20718 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/main.0d12cfba.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     2591 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/runtime~main.75c1c0e5.js
+-rw-r--r--   0 mdizon     (501) staff       (20)    12794 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/runtime~main.75c1c0e5.js.map
+drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 17:07:00.760093 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/
+drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 17:07:00.814266 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/css/
+-rw-r--r--   0 mdizon     (501) staff       (20)      344 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/css/main.34de6062.chunk.css
+-rw-r--r--   0 mdizon     (501) staff       (20)      579 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/css/main.34de6062.chunk.css.map
+drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 17:07:00.825018 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/
+-rw-r--r--   0 mdizon     (501) staff       (20)   800098 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/2.30b5ba40.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)  3417792 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/2.30b5ba40.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)      868 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/main.6d24c0c6.chunk.js
+-rw-r--r--   0 mdizon     (501) staff       (20)     6929 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/main.6d24c0c6.chunk.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)     1502 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/runtime~main.a8a9905a.js
+-rw-r--r--   0 mdizon     (501) staff       (20)     7996 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/runtime~main.a8a9905a.js.map
+-rw-r--r--   0 mdizon     (501) staff       (20)  1979770 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/voyager.worker.js
+drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 17:07:00.760223 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/templates/
+drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 17:07:00.828068 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/templates/strawberry_django_graphiql_voyager/
+-rw-r--r--   0 mdizon     (501) staff       (20)     6595 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/templates/strawberry_django_graphiql_voyager/graphiql.html
+-rw-r--r--   0 mdizon     (501) staff       (20)     4273 2022-08-03 12:39:37.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/templates/strawberry_django_graphiql_voyager/voyager.html
+-rw-r--r--   0 mdizon     (501) staff       (20)     1948 2022-08-01 14:47:31.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/views.py
+drwxr-xr-x   0 mdizon     (501) staff       (20)        0 2023-04-26 17:07:00.762726 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager.egg-info/
+-rw-r--r--   0 mdizon     (501) staff       (20)      969 2023-04-26 17:07:00.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager.egg-info/PKG-INFO
+-rw-r--r--   0 mdizon     (501) staff       (20)     8296 2023-04-26 17:07:00.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager.egg-info/SOURCES.txt
+-rw-r--r--   0 mdizon     (501) staff       (20)        1 2023-04-26 17:07:00.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager.egg-info/dependency_links.txt
+-rw-r--r--   0 mdizon     (501) staff       (20)       35 2023-04-26 17:07:00.000000 strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager.egg-info/top_level.txt
```

### Comparing `strawberry_django_graphiql_voyager-0.1.21/LICENSE` & `strawberry_django_graphiql_voyager-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/PKG-INFO` & `strawberry_django_graphiql_voyager-0.1.22/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry_django_graphiql_voyager
-Version: 0.1.21
+Version: 0.1.22
 Summary: A Strawberry Django app that adds GraphiQL and Voyager to the graphql view
 Home-page: https://github.com/mikedizon/strawberry-django-graphiql-voyager
 Author: mikedizon
 Author-email: mdizon@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `strawberry_django_graphiql_voyager-0.1.21/setup.cfg` & `strawberry_django_graphiql_voyager-0.1.22/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = strawberry_django_graphiql_voyager
-version = 0.1.21
+version = 0.1.22
 description = A Strawberry Django app that adds GraphiQL and Voyager to the graphql view
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mikedizon/strawberry-django-graphiql-voyager
 author = mikedizon
 author_email = mdizon@gmail.com
 license = MIT
```

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/11.66866c8b.chunk.css` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/11.66866c8b.chunk.css`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/11.66866c8b.chunk.css.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/11.66866c8b.chunk.css.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/main.d0b1e8f9.chunk.css.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/css/main.d0b1e8f9.chunk.css.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/0.d69ee02e.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/0.d69ee02e.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/0.d69ee02e.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/0.d69ee02e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/1.d76c06cc.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/1.d76c06cc.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/1.d76c06cc.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/1.d76c06cc.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/11.8fdec039.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/11.8fdec039.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/11.8fdec039.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/11.8fdec039.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/12.a9526db5.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/12.a9526db5.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/12.a9526db5.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/12.a9526db5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/13.2ac64509.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/13.2ac64509.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/13.2ac64509.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/13.2ac64509.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/14.d5d84371.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/14.d5d84371.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/14.d5d84371.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/14.d5d84371.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/15.812c88f9.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/15.812c88f9.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/15.812c88f9.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/15.812c88f9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/16.ce8357ac.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/16.ce8357ac.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/16.ce8357ac.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/16.ce8357ac.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/17.e84c62d5.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/17.e84c62d5.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/17.e84c62d5.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/17.e84c62d5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/18.9d20f18a.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/18.9d20f18a.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/18.9d20f18a.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/18.9d20f18a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/19.8e86fbfa.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/19.8e86fbfa.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/19.8e86fbfa.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/19.8e86fbfa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/2.591f5756.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/2.591f5756.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/2.591f5756.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/2.591f5756.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/20.3b18185a.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/20.3b18185a.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/20.3b18185a.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/20.3b18185a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/21.41f21244.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/21.41f21244.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/21.41f21244.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/21.41f21244.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/22.8fbf3b0e.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/22.8fbf3b0e.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/22.8fbf3b0e.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/22.8fbf3b0e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/23.6098cda7.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/23.6098cda7.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/23.6098cda7.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/23.6098cda7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/24.d76a1f43.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/24.d76a1f43.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/24.d76a1f43.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/24.d76a1f43.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/25.53cfe552.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/25.53cfe552.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/25.53cfe552.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/25.53cfe552.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/26.5a70ef0a.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/26.5a70ef0a.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/26.5a70ef0a.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/26.5a70ef0a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/27.c2a642ff.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/27.c2a642ff.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/27.c2a642ff.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/27.c2a642ff.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/3.be05d828.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/3.be05d828.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/3.be05d828.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/3.be05d828.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/4.6c088241.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/4.6c088241.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/4.6c088241.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/4.6c088241.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/5.2f6c7945.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/5.2f6c7945.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/5.2f6c7945.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/5.2f6c7945.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/6.c7c77fbb.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/6.c7c77fbb.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/6.c7c77fbb.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/6.c7c77fbb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/7.b605e08f.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/7.b605e08f.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/7.b605e08f.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/7.b605e08f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/8.32bdc3c7.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/8.32bdc3c7.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/8.32bdc3c7.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/8.32bdc3c7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/main.0d12cfba.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/main.0d12cfba.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/main.0d12cfba.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/main.0d12cfba.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/runtime~main.75c1c0e5.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/runtime~main.75c1c0e5.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/runtime~main.75c1c0e5.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/graphiql/js/runtime~main.75c1c0e5.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/css/main.34de6062.chunk.css.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/css/main.34de6062.chunk.css.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/2.30b5ba40.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/2.30b5ba40.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/2.30b5ba40.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/2.30b5ba40.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/main.6d24c0c6.chunk.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/main.6d24c0c6.chunk.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/main.6d24c0c6.chunk.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/main.6d24c0c6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/runtime~main.a8a9905a.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/runtime~main.a8a9905a.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/runtime~main.a8a9905a.js.map` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/runtime~main.a8a9905a.js.map`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/voyager.worker.js` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/static/strawberry_django_graphiql_voyager/voyager/js/voyager.worker.js`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/templates/strawberry_django_graphiql_voyager/graphiql.html` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/templates/strawberry_django_graphiql_voyager/graphiql.html`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/templates/strawberry_django_graphiql_voyager/voyager.html` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/templates/strawberry_django_graphiql_voyager/voyager.html`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager/views.py` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager/views.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager.egg-info/PKG-INFO` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-graphiql-voyager
-Version: 0.1.21
+Version: 0.1.22
 Summary: A Strawberry Django app that adds GraphiQL and Voyager to the graphql view
 Home-page: https://github.com/mikedizon/strawberry-django-graphiql-voyager
 Author: mikedizon
 Author-email: mdizon@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `strawberry_django_graphiql_voyager-0.1.21/strawberry_django_graphiql_voyager.egg-info/SOURCES.txt` & `strawberry_django_graphiql_voyager-0.1.22/strawberry_django_graphiql_voyager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

