# Comparing `tmp/insteon-frontend-home-assistant-0.3.4.tar.gz` & `tmp/insteon-frontend-home-assistant-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insteon-frontend-home-assistant-0.3.4.tar", last modified: Fri Mar 17 19:00:53 2023, max compression
+gzip compressed data, was "insteon-frontend-home-assistant-0.3.5.tar", last modified: Tue Apr 25 22:18:49 2023, max compression
```

## Comparing `insteon-frontend-home-assistant-0.3.4.tar` & `insteon-frontend-home-assistant-0.3.5.tar`

### file list

```diff
@@ -1,695 +1,15 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-17 19:00:53.419075 insteon-frontend-home-assistant-0.3.4/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1070 2023-02-10 18:38:22.000000 insteon-frontend-home-assistant-0.3.4/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)       48 2023-02-10 18:38:22.000000 insteon-frontend-home-assistant-0.3.4/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)      573 2023-03-17 19:00:53.419075 insteon-frontend-home-assistant-0.3.4/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      120 2023-02-10 18:38:22.000000 insteon-frontend-home-assistant-0.3.4/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-17 19:00:53.319075 insteon-frontend-home-assistant-0.3.4/insteon_frontend/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      279 2023-03-17 18:19:59.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       24 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/constants.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      405 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/entrypoint-fbe0ce27.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      278 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/entrypoint-fbe0ce27.js.gz
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-17 19:00:53.367075 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11153 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/02dded1b.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3409 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/02dded1b.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10626 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/04bf09eb.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3338 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/04bf09eb.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    19492 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/06a3a94e.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5198 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/06a3a94e.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)   975803 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/0739ce8b.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/0739ce8b.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)   104802 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/0739ce8b.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    29068 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/079df134.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6597 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/079df134.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23662 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/106f07ea.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/106f07ea.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6869 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/106f07ea.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    95400 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/17d2139d.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2579 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/17d2139d.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    20358 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/17d2139d.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    21794 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/18102fc2.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      177 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/18102fc2.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4911 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/18102fc2.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    29923 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/19e7fd8e.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/19e7fd8e.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8406 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/19e7fd8e.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11829 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/1ddc3c7d.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3714 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/1ddc3c7d.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14102 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/1ef53e88.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4307 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/1ef53e88.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    27785 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/22783b06.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5526 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/22783b06.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    27751 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/24b9a66d.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10422 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/24b9a66d.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    18693 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2a6f87d3.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5579 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2a6f87d3.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    60433 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2c4b2ad6.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2c4b2ad6.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10559 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2c4b2ad6.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    16046 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2c61c109.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      327 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2c61c109.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4976 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2c61c109.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    41437 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2dbd9372.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2dbd9372.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8036 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2dbd9372.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26497 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2e568b1b.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2e568b1b.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7509 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2e568b1b.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    25802 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2ef4f4ba.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2ef4f4ba.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7324 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/2ef4f4ba.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    36122 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/330b53d2.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8025 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/330b53d2.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22727 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/38cfe62d.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/38cfe62d.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6965 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/38cfe62d.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    36344 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/3a446539.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5602 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/3a446539.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23407 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/3a5dd0b5.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      240 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/3a5dd0b5.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5161 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/3a5dd0b5.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26259 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/3ac95a0d.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5087 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/3ac95a0d.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11288 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/3de3c5b6.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1023 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/3de3c5b6.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3361 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/3de3c5b6.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22357 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/3f406ec6.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4127 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/3f406ec6.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    47104 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/4055672a.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14394 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/4055672a.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3322 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/4503c4ca.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1554 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/4503c4ca.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    79102 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/459a7d5b.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1023 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/459a7d5b.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14385 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/459a7d5b.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    39308 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/47bd7637.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)       68 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/47bd7637.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12597 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/47bd7637.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    30927 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/47e19a4d.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      177 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/47e19a4d.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6219 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/47e19a4d.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    29872 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/484c5423.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5664 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/484c5423.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    29835 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/49677277.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5681 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/49677277.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11058 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/4c42dfa0.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3371 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/4c42dfa0.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    47956 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/4ec4cded.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/4ec4cded.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9885 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/4ec4cded.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12235 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/5097dc28.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3738 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/5097dc28.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11861 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/50b08eaf.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3652 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/50b08eaf.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11075 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/52f5e102.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)       88 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/52f5e102.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3961 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/52f5e102.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12093 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/547ab9cc.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3710 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/547ab9cc.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13237 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/54d85da0.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4047 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/54d85da0.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    78084 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/54dd3db4.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      240 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/54dd3db4.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17394 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/54dd3db4.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)   400364 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/54ea107d.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)   111302 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/54ea107d.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8925 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/5a896b13.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      824 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/5a896b13.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2844 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/5a896b13.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23276 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/5b67570a.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4368 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/5b67570a.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12245 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/5f251f1d.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3706 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/5f251f1d.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    39927 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/604a17db.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      266 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/604a17db.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7511 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/604a17db.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    32301 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/629b9c21.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4502 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/629b9c21.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)   148415 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/63634fc5.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      153 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/63634fc5.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    40921 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/63634fc5.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)   117737 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/6419e8c2.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      661 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/6419e8c2.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    18918 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/6419e8c2.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23395 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/66b8b86d.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/66b8b86d.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6649 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/66b8b86d.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)   100001 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/69bdcbb6.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/69bdcbb6.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15519 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/69bdcbb6.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    56460 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/6c3c48ee.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/6c3c48ee.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9549 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/6c3c48ee.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    29166 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/75481fb2.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      268 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/75481fb2.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6405 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/75481fb2.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    19344 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/76ffb990.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/76ffb990.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6083 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/76ffb990.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12224 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/7716551e.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3831 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/7716551e.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23335 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/7b23ac34.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/7b23ac34.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7264 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/7b23ac34.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    21538 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/7bef76ff.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5464 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/7bef76ff.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    55120 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/7e755d19.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/7e755d19.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10769 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/7e755d19.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22307 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/80df3fc2.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3985 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/80df3fc2.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13687 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8125d779.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      416 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8125d779.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4204 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8125d779.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    79198 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8249a85c.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8249a85c.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10098 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8249a85c.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    38788 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/828b60d6.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      511 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/828b60d6.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6132 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/828b60d6.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3322 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8380d187.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1554 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8380d187.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    31112 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8413919e.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8413919e.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7519 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8413919e.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)      199 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8489119e.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      158 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8489119e.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    55666 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/855c0068.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/855c0068.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9017 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/855c0068.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)   103431 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8665aeea.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8665aeea.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17454 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8665aeea.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11390 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/870501ac.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3506 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/870501ac.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13414 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/87a5709e.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)       88 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/87a5709e.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3721 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/87a5709e.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7660 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/89c99c47.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      511 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/89c99c47.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2568 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/89c99c47.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)   164601 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8af0b086.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1868 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8af0b086.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    29420 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8af0b086.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12140 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8c149918.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3748 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8c149918.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)   169161 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8dca7fc9.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8dca7fc9.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23664 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/8dca7fc9.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12133 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/906ecb5c.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3741 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/906ecb5c.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    39863 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/9190ed84.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1021 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/9190ed84.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10650 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/9190ed84.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12170 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/9443b1fe.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      331 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/9443b1fe.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4029 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/9443b1fe.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    56862 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/945424fe.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      331 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/945424fe.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11848 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/945424fe.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)   146680 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/9a09d164.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      598 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/9a09d164.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    24344 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/9a09d164.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    29710 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/a02336a2.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/a02336a2.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8725 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/a02336a2.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    45557 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/a1c8cda8.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/a1c8cda8.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9172 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/a1c8cda8.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    85868 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/a791c512.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/a791c512.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    16229 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/a791c512.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    84942 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/a7bf2a23.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      327 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/a7bf2a23.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15705 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/a7bf2a23.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14000 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/ac25eba9.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4439 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/ac25eba9.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    35415 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/b045888f.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6620 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/b045888f.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14050 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/b60b88b2.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)       90 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/b60b88b2.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3865 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/b60b88b2.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    21791 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/bb0466a6.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4025 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/bb0466a6.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2168 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/bc35e642.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      895 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/bc35e642.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)      202 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c366ac3c.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      167 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c366ac3c.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    53419 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c4d6bf84.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1173 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c4d6bf84.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12624 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c4d6bf84.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    25330 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c52f8a9d.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c52f8a9d.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7278 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c52f8a9d.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    49392 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c61390ea.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1933 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c61390ea.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11483 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c61390ea.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11942 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c71b5316.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3739 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c71b5316.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    25757 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c74b217e.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8171 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c74b217e.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12491 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c77eaecd.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)       88 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c77eaecd.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4075 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c77eaecd.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22360 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c9e9e1d9.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c9e9e1d9.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6709 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/c9e9e1d9.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10979 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/cccc9947.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3345 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/cccc9947.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    20410 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/cd84453d.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/cd84453d.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6347 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/cd84453d.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)      148 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/d005cf0b.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11662 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/d0b5e763.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3551 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/d0b5e763.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    16282 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/d20f3e47.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)       88 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/d20f3e47.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4875 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/d20f3e47.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15477 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/d3fd159f.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5210 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/d3fd159f.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23223 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/d461fe25.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/d461fe25.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7015 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/d461fe25.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10406 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/d5de4242.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      511 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/d5de4242.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2375 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/d5de4242.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10885 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/da3aa6c1.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3376 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/da3aa6c1.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11557 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/db65e312.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      177 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/db65e312.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3359 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/db65e312.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    33077 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/e0ae7386.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/e0ae7386.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7449 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/e0ae7386.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    67542 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/e7047a2f.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13681 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/e7047a2f.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    29082 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/e88d8a00.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5269 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/e88d8a00.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6422 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/e93344f8.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1932 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/e93344f8.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    43834 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/ec565ff6.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/ec565ff6.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10116 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/ec565ff6.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    43963 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/ece4cd77.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/ece4cd77.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10155 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/ece4cd77.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    38511 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/ef49476d.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/ef49476d.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8482 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/ef49476d.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)  2513055 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/entrypoint-acae4cac.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4845 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/entrypoint-acae4cac.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)   445282 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/entrypoint-acae4cac.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    35717 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f3b6bab0.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      125 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f3b6bab0.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11913 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f3b6bab0.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11524 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f3c0d644.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f3c0d644.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3975 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f3c0d644.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12880 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f620a2cd.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3805 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f620a2cd.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23652 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f677bac4.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      177 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f677bac4.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4200 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f677bac4.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    47573 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f6da9109.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f6da9109.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11136 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f6da9109.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    21424 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f6f7e806.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f6f7e806.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6660 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f6f7e806.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11579 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f8894f3f.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3552 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/f8894f3f.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11573 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/fd27dfba.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3606 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/fd27dfba.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)       76 2023-03-17 18:17:15.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_es5/manifest.json
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-17 19:00:53.419075 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    32232 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0282887a.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6235 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0282887a.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23392 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0282887a.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9386 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/03f89fa1.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2995 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/03f89fa1.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2115 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/03f89fa1.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    24226 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/048ff6ae.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5798 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/048ff6ae.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7818 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/048ff6ae.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    44853 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/076b68ec.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)       90 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/076b68ec.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9335 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/076b68ec.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9042 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/076b68ec.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    19687 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0ba17776.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      960 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0ba17776.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6600 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0ba17776.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10620 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0ba17776.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9910 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0ca0b87f.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3103 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0ca0b87f.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2797 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0ca0b87f.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    69304 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0cbded7c.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10622 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0cbded7c.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    48781 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0cbded7c.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    44188 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0d99baf8.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7872 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0d99baf8.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26197 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0d99baf8.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6096 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0ddf5491.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1912 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/0ddf5491.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14572 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/122cc134.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4559 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/122cc134.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3512 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/122cc134.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23955 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/132aedec.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      177 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/132aedec.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5294 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/132aedec.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10398 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/132aedec.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15254 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/14021133.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4392 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/14021133.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13752 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/14021133.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26310 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/152db136.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5539 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/152db136.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10143 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/152db136.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9673 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/15506ccb.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3050 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/15506ccb.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2298 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/15506ccb.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    33161 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/17469f49.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      871 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/17469f49.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8134 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/17469f49.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    24641 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/17469f49.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11058 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/178593e9.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      511 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/178593e9.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2564 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/178593e9.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23124 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/178593e9.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9759 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/17a6b9ea.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3121 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/17a6b9ea.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11917 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/17fb3582.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3918 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/17fb3582.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17915 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1972789a.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5498 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1972789a.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9711 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1972789a.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    42209 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1b20b003.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1933 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1b20b003.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9717 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1b20b003.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15678 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1b20b003.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    50823 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1bb7914c.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2429 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1bb7914c.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12332 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1bb7914c.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    39115 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1bb7914c.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    20684 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1cd037c9.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4258 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1cd037c9.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5596 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1cd037c9.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    46902 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1eb39258.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14287 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/1eb39258.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    25916 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/233360ae.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5373 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/233360ae.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10730 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/233360ae.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10040 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/2370abfe.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3135 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/2370abfe.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2580 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/2370abfe.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    93804 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/24065ffe.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13060 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/24065ffe.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    51232 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/24065ffe.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    18076 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/26a1be3f.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1112 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/26a1be3f.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4925 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/26a1be3f.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    20250 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/26a1be3f.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8939 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/28c04b81.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2772 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/28c04b81.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1482 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/28c04b81.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)   148366 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/2ab920ab.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      153 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/2ab920ab.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    40935 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/2ab920ab.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    20654 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/2e1351a2.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      177 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/2e1351a2.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3216 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/2e1351a2.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5310 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/2e1351a2.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    27987 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/2f2b2cbb.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4116 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/2f2b2cbb.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5866 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/2f2b2cbb.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    29095 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/30d95ca2.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11079 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/30d95ca2.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)  1362667 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/328b24df.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)   179304 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/328b24df.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14437 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/345ace8f.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3469 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/345ace8f.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    47691 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/350ef536.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      266 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/350ef536.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7278 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/350ef536.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    18686 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/350ef536.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    25846 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/36f999eb.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5569 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/36f999eb.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9298 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/36f999eb.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14553 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/4286abe5.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4229 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/4286abe5.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5632 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/4286abe5.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8936 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/476b67bc.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      824 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/476b67bc.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2857 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/476b67bc.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8960 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/4a55d6ce.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2829 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/4a55d6ce.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1362 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/4a55d6ce.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    64087 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/4eb438cb.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    19481 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/4eb438cb.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    27923 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/512ebcab.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4170 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/512ebcab.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6040 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/512ebcab.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6639 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5719e9ca.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2293 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5719e9ca.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9773 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5a20a8b4.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3135 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5a20a8b4.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3129 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5a20a8b4.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23922 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5bcf33be.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4743 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5bcf33be.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9535 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5bcf33be.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    33690 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5d6e59a2.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5273 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5d6e59a2.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    16385 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5d6e59a2.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23818 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5dbecaa4.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4944 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5dbecaa4.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10208 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5dbecaa4.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    24381 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5df6d3c4.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5160 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5df6d3c4.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13938 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5df6d3c4.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    28315 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5e7b8eb4.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      511 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5e7b8eb4.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4761 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5e7b8eb4.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    20250 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5e7b8eb4.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    30186 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5fca4c55.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10309 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/5fca4c55.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8497 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6112141b.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2721 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6112141b.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1125 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6112141b.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    60324 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6238c6aa.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      511 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6238c6aa.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13389 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6238c6aa.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)   111941 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6238c6aa.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    39042 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6353c82b.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)       68 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6353c82b.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12498 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6353c82b.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4671 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/64b90405.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)       88 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/64b90405.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2015 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/64b90405.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    41497 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/695f3a70.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11740 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/695f3a70.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    25736 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/69e24e3a.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5163 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/69e24e3a.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10308 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/69e24e3a.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)   109546 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6a2185b4.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      448 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6a2185b4.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17026 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6a2185b4.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    35969 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6a2185b4.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    39732 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6bdb6d31.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      511 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6bdb6d31.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7370 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6bdb6d31.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    19767 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6bdb6d31.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    20020 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6d7c0101.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4008 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6d7c0101.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5962 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6d7c0101.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    35357 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6e9252f8.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4229 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6e9252f8.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6061 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/6e9252f8.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13759 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/73236200.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4239 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/73236200.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8725 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/73236200.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4671 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/73e6b166.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)       88 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/73e6b166.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2014 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/73e6b166.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17845 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/73f8c857.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      689 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/73f8c857.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4099 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/73f8c857.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15164 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/73f8c857.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)   147319 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/74ec5c13.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    18007 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/74ec5c13.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    78420 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/74ec5c13.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      139 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/752aa587.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9230 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/76107771.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2911 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/76107771.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2309 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/76107771.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11733 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/7648f7a6.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3837 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/7648f7a6.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4405 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/7648f7a6.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    21662 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/77957770.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4348 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/77957770.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6277 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/77957770.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7778 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/7a713077.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2472 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/7a713077.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26581 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/7f3fd3a8.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      778 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/7f3fd3a8.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5700 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/7f3fd3a8.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    24257 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/7f3fd3a8.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22886 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/8494aceb.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4640 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/8494aceb.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8640 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/8494aceb.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11323 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/862f816a.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3536 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/862f816a.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    92133 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/871ce0b0.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1868 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/871ce0b0.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22225 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/871ce0b0.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    72999 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/871ce0b0.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    35768 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/8bd369ba.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)       90 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/8bd369ba.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10352 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/8bd369ba.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    39914 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/8bd369ba.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13834 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/8d33a7df.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3936 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/8d33a7df.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11396 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/8d33a7df.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22752 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/8e38fd26.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7437 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/8e38fd26.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10197 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/8e38fd26.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26055 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/91f6510a.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5497 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/91f6510a.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9377 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/91f6510a.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14218 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/928a876c.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4298 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/928a876c.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4528 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/928a876c.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    35694 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/92b91621.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      125 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/92b91621.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11919 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/92b91621.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    34166 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/95433b5f.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5319 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/95433b5f.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13501 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/95433b5f.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22773 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/96276335.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4608 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/96276335.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5044 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/96276335.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    19313 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/9bf37f60.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3744 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/9bf37f60.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4552 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/9bf37f60.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    30687 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/9c79a124.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4743 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/9c79a124.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10252 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/9c79a124.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    21315 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/9caaf2c0.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      181 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/9caaf2c0.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6069 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/9caaf2c0.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11257 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/9f1e6a4e.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3527 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/9f1e6a4e.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    57810 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/a49460ca.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8371 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/a49460ca.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    29386 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/a49460ca.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    25061 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/a9681d55.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4829 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/a9681d55.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12686 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/a9681d55.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10892 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/a9ef605d.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1023 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/a9ef605d.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3237 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/a9ef605d.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    20679 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/a9ef605d.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    68217 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/add81c96.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6947 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/add81c96.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    19014 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/add81c96.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    28919 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/af18a7f9.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4406 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/af18a7f9.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6896 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/af18a7f9.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    71172 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/b03c1460.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      177 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/b03c1460.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11557 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/b03c1460.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    27783 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/b03c1460.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14654 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/b4b217af.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)       90 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/b4b217af.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3665 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/b4b217af.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    39750 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/b8b77466.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      266 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/b8b77466.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6788 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/b8b77466.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13826 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/b8b77466.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14017 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/b959cea2.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      177 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/b959cea2.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3503 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/b959cea2.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9159 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/b959cea2.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11914 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/ba14f601.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3801 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/ba14f601.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6577 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/ba14f601.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    41460 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/ba8431b2.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      177 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/ba8431b2.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7109 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/ba8431b2.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17909 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/ba8431b2.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14822 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/babdf89e.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      177 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/babdf89e.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4329 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/babdf89e.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4913 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/babdf89e.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    24102 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/c3815531.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4857 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/c3815531.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9085 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/c3815531.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      176 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/c3a2462a.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/c3a2462a.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    39379 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/c5ca155a.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)       90 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/c5ca155a.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7455 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/c5ca155a.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9694 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/c5ca155a.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    16354 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/c7e9ce9f.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5503 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/c7e9ce9f.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3157 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/c7e9ce9f.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26636 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/c80b298e.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5386 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/c80b298e.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13351 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/c80b298e.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    19122 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/cf6983d5.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      266 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/cf6983d5.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4920 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/cf6983d5.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8375 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/cf6983d5.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23976 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/d28fe432.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4777 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/d28fe432.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9755 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/d28fe432.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    43114 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/d4b858c8.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      266 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/d4b858c8.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8600 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/d4b858c8.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    18892 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/d4b858c8.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9027 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/d6ae8c81.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2810 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/d6ae8c81.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1628 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/d6ae8c81.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      518 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/da6c1d69.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      316 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/da6c1d69.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    49015 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/db32589b.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7563 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/db32589b.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26083 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/db32589b.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)   311709 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/dc6d4fd6.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    95516 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/dc6d4fd6.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7584 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/dc6fe1ff.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      511 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/dc6fe1ff.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2564 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/dc6fe1ff.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12745 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/e59c1d38.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3808 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/e59c1d38.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10250 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/e59c1d38.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    21038 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/e6e89675.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4341 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/e6e89675.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6299 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/e6e89675.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)   721641 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/e7022f34.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    64947 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/e7022f34.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)   289697 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/e7022f34.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)   443461 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/entrypoint-fbe0ce27.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5695 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/entrypoint-fbe0ce27.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)    96192 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/entrypoint-fbe0ce27.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    85494 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/entrypoint-fbe0ce27.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      215 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/f3d474c3.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      177 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/f3d474c3.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    67309 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/f645ea33.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13602 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/f645ea33.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17423 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/fa6c0e88.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3316 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/fa6c0e88.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2671 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/fa6c0e88.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    42576 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/fcc81ea9.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6791 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/fcc81ea9.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26078 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/fcc81ea9.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    19338 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/fea404af.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3517 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/fea404af.js.gz
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4999 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/fea404af.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)       79 2023-03-17 18:16:58.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend/frontend_latest/manifest.json
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-17 19:00:53.419075 insteon-frontend-home-assistant-0.3.4/insteon_frontend_git/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       19 2023-03-07 05:24:46.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend_git/constants.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-17 19:00:53.419075 insteon-frontend-home-assistant-0.3.4/insteon_frontend_home_assistant.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      573 2023-03-17 19:00:52.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend_home_assistant.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)    32276 2023-03-17 19:00:53.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend_home_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-03-17 19:00:52.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend_home_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-03-07 18:21:22.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend_home_assistant.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-03-17 19:00:53.000000 insteon-frontend-home-assistant-0.3.4/insteon_frontend_home_assistant.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      640 2023-03-17 18:45:32.000000 insteon-frontend-home-assistant-0.3.4/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      626 2023-03-17 19:00:53.419075 insteon-frontend-home-assistant-0.3.4/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 22:18:49.109751 insteon-frontend-home-assistant-0.3.5/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1070 2023-02-10 18:38:22.000000 insteon-frontend-home-assistant-0.3.5/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       48 2023-02-10 18:38:22.000000 insteon-frontend-home-assistant-0.3.5/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      573 2023-04-25 22:18:49.109751 insteon-frontend-home-assistant-0.3.5/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      120 2023-02-10 18:38:22.000000 insteon-frontend-home-assistant-0.3.5/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 22:18:49.109751 insteon-frontend-home-assistant-0.3.5/insteon_frontend_git/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       19 2023-03-07 05:24:46.000000 insteon-frontend-home-assistant-0.3.5/insteon_frontend_git/constants.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 22:18:49.109751 insteon-frontend-home-assistant-0.3.5/insteon_frontend_home_assistant.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      573 2023-04-25 22:18:48.000000 insteon-frontend-home-assistant-0.3.5/insteon_frontend_home_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      362 2023-04-25 22:18:49.000000 insteon-frontend-home-assistant-0.3.5/insteon_frontend_home_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-25 22:18:48.000000 insteon-frontend-home-assistant-0.3.5/insteon_frontend_home_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-25 22:18:46.000000 insteon-frontend-home-assistant-0.3.5/insteon_frontend_home_assistant.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       21 2023-04-25 22:18:48.000000 insteon-frontend-home-assistant-0.3.5/insteon_frontend_home_assistant.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      640 2023-04-25 22:18:09.000000 insteon-frontend-home-assistant-0.3.5/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      626 2023-04-25 22:18:49.109751 insteon-frontend-home-assistant-0.3.5/setup.cfg
```

### Comparing `insteon-frontend-home-assistant-0.3.4/LICENSE` & `insteon-frontend-home-assistant-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `insteon-frontend-home-assistant-0.3.4/PKG-INFO` & `insteon-frontend-home-assistant-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insteon-frontend-home-assistant
-Version: 0.3.4
+Version: 0.3.5
 Summary: The Insteon frontend for Home Assistant
 Home-page: https://github.com/home-assistant/frontend
 Author: The pyinsteon development team
 Author-email: Tom Harris <pyinsteon@harrisnj.net>
 License: MIT License
 Project-URL: Homepage, https://github.com/pyinsteon/insteon-panel
 Platform: any
```

### Comparing `insteon-frontend-home-assistant-0.3.4/insteon_frontend_home_assistant.egg-info/PKG-INFO` & `insteon-frontend-home-assistant-0.3.5/insteon_frontend_home_assistant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insteon-frontend-home-assistant
-Version: 0.3.4
+Version: 0.3.5
 Summary: The Insteon frontend for Home Assistant
 Home-page: https://github.com/home-assistant/frontend
 Author: The pyinsteon development team
 Author-email: Tom Harris <pyinsteon@harrisnj.net>
 License: MIT License
 Project-URL: Homepage, https://github.com/pyinsteon/insteon-panel
 Platform: any
```

### Comparing `insteon-frontend-home-assistant-0.3.4/pyproject.toml` & `insteon-frontend-home-assistant-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name         = "insteon-frontend-home-assistant"
-version      = "0.3.4"
+version      = "0.3.5"
 license      = {text = "MIT License"}
 description  = "The Insteon frontend for Home Assistant"
 readme       = "README.md"
 authors      = [
     {name = "Tom Harris", email = "pyinsteon@harrisnj.net"}
 ]
 requires-python = ">=3.4.0"
```

### Comparing `insteon-frontend-home-assistant-0.3.4/setup.cfg` & `insteon-frontend-home-assistant-0.3.5/setup.cfg`

 * *Files identical despite different names*

