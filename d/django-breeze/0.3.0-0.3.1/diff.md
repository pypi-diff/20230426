# Comparing `tmp/django_breeze-0.3.0.tar.gz` & `tmp/django_breeze-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_breeze-0.3.0.tar", max compression
+gzip compressed data, was "django_breeze-0.3.1.tar", max compression
```

## Comparing `django_breeze-0.3.0.tar` & `django_breeze-0.3.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1066 2023-04-25 13:49:15.054522 django_breeze-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     4814 2023-04-25 13:49:15.054522 django_breeze-0.3.0/README.md
--rw-r--r--   0        0        0       61 2023-04-25 13:49:15.054522 django_breeze-0.3.0/django_breeze/__init__.py
--rw-r--r--   0        0        0      222 2023-04-25 13:49:15.054522 django_breeze-0.3.0/django_breeze/__main__.py
--rw-r--r--   0        0        0      814 2023-04-25 13:49:15.054522 django_breeze-0.3.0/django_breeze/apps.py
--rw-r--r--   0        0        0        0 2023-04-25 13:49:15.054522 django_breeze-0.3.0/django_breeze/core/__init__.py
--rw-r--r--   0        0        0     4100 2023-04-25 13:49:15.054522 django_breeze-0.3.0/django_breeze/core/management/__init__.py
--rw-r--r--   0        0        0      719 2023-04-25 13:49:15.054522 django_breeze-0.3.0/django_breeze/middleware.py
--rw-r--r--   0        0        0      232 2023-04-25 13:49:15.054522 django_breeze-0.3.0/django_breeze/scripts/django_breeze.py
--rw-r--r--   0        0        0     3145 2023-04-25 13:49:15.054522 django_breeze-0.3.0/django_breeze/settings.py
--rw-r--r--   0        0        0   129342 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/static/django_breeze/django-breeze-logo.jpg
--rw-r--r--   0        0        0   211529 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/static/django_breeze/django-breeze-logo.png
--rw-r--r--   0        0        0      322 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react/.gitignore
--rw-r--r--   0        0        0      561 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react/package.json
--rw-r--r--   0        0        0       80 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react/postcss.config.js
--rw-r--r--   0        0        0      115 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react/src/Layout/SiteLayout.jsx
--rw-r--r--   0        0        0     4126 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react/src/assets/react.svg
--rw-r--r--   0        0        0       58 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react/src/index.css
--rw-r--r--   0        0        0      416 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react/src/index.html
--rw-r--r--   0        0        0      544 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react/src/main.jsx
--rw-r--r--   0        0        0      983 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react/src/pages/index.jsx
--rw-r--r--   0        0        0      174 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react/tailwind.config.js
--rw-r--r--   0        0        0      814 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react/vite.config.js
--rw-r--r--   0        0        0      322 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react_typescript/.gitignore
--rw-r--r--   0        0        0      577 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react_typescript/package.json
--rw-r--r--   0        0        0       80 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react_typescript/postcss.config.js
--rw-r--r--   0        0        0     1497 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react_typescript/public/vite.svg
--rw-r--r--   0        0        0      115 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react_typescript/src/Layout/SiteLayout.tsx
--rw-r--r--   0        0        0     4126 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react_typescript/src/assets/react.svg
--rw-r--r--   0        0        0       59 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react_typescript/src/index.css
--rw-r--r--   0        0        0      417 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react_typescript/src/index.html
--rw-r--r--   0        0        0      544 2023-04-25 13:49:15.058522 django_breeze-0.3.0/django_breeze/templates/react_typescript/src/main.tsx
--rw-r--r--   0        0        0     1024 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/react_typescript/src/pages/index.tsx
--rw-r--r--   0        0        0       38 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/react_typescript/src/vite-env.d.ts
--rw-r--r--   0        0        0      174 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/react_typescript/tailwind.config.js
--rw-r--r--   0        0        0      559 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/react_typescript/tsconfig.json
--rw-r--r--   0        0        0      184 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/react_typescript/tsconfig.node.json
--rw-r--r--   0        0        0      814 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/react_typescript/vite.config.ts
--rw-r--r--   0        0        0      253 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3/.gitignore
--rw-r--r--   0        0        0      429 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3/package.json
--rw-r--r--   0        0        0       80 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3/postcss.config.js
--rw-r--r--   0        0        0      496 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3/src/assets/vue.svg
--rw-r--r--   0        0        0      282 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3/src/components/Framwork.vue
--rw-r--r--   0        0        0       58 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3/src/index.css
--rw-r--r--   0        0        0      422 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3/src/index.html
--rw-r--r--   0        0        0      441 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3/src/main.jsx
--rw-r--r--   0        0        0      824 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3/src/pages/index.vue
--rw-r--r--   0        0        0     1497 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3/src/public/vite.svg
--rw-r--r--   0        0        0      178 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3/tailwind.config.js
--rw-r--r--   0        0        0      768 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3/vite.config.js
--rw-r--r--   0        0        0      253 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3_typescript/.gitignore
--rw-r--r--   0        0        0      504 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3_typescript/package.json
--rw-r--r--   0        0        0       80 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3_typescript/postcss.config.js
--rw-r--r--   0        0        0      496 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3_typescript/src/assets/vue.svg
--rw-r--r--   0        0        0      282 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3_typescript/src/components/Framwork.vue
--rw-r--r--   0        0        0       58 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3_typescript/src/index.css
--rw-r--r--   0        0        0      433 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3_typescript/src/index.html
--rw-r--r--   0        0        0      441 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3_typescript/src/main.tsx
--rw-r--r--   0        0        0      824 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3_typescript/src/pages/index.vue
--rw-r--r--   0        0        0     1497 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3_typescript/src/public/vite.svg
--rw-r--r--   0        0        0       38 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3_typescript/src/vite-env.d.ts
--rw-r--r--   0        0        0      178 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3_typescript/tailwind.config.js
--rw-r--r--   0        0        0      661 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3_typescript/tsconfig.json
--rw-r--r--   0        0        0      213 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3_typescript/tsconfig.node.json
--rw-r--r--   0        0        0      768 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templates/vue3_typescript/vite.config.ts
--rw-r--r--   0        0        0        0 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templatetags/__init__.py
--rw-r--r--   0        0        0       51 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/templatetags/django_vite.py
--rw-r--r--   0        0        0      130 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/urls.py
--rw-r--r--   0        0        0      354 2023-04-25 13:49:15.062522 django_breeze-0.3.0/django_breeze/views.py
--rw-r--r--   0        0        0      804 2023-04-25 13:49:15.062522 django_breeze-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5647 1970-01-01 00:00:00.000000 django_breeze-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-25 16:41:13.257732 django_breeze-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0     4814 2023-04-25 16:41:13.257732 django_breeze-0.3.1/README.md
+-rw-r--r--   0        0        0       61 2023-04-25 16:41:13.257732 django_breeze-0.3.1/django_breeze/__init__.py
+-rw-r--r--   0        0        0      222 2023-04-25 16:41:13.257732 django_breeze-0.3.1/django_breeze/__main__.py
+-rw-r--r--   0        0        0      814 2023-04-25 16:41:13.257732 django_breeze-0.3.1/django_breeze/apps.py
+-rw-r--r--   0        0        0        0 2023-04-25 16:41:13.257732 django_breeze-0.3.1/django_breeze/core/__init__.py
+-rw-r--r--   0        0        0     4100 2023-04-25 16:41:13.257732 django_breeze-0.3.1/django_breeze/core/management/__init__.py
+-rw-r--r--   0        0        0      719 2023-04-25 16:41:13.257732 django_breeze-0.3.1/django_breeze/middleware.py
+-rw-r--r--   0        0        0      232 2023-04-25 16:41:13.257732 django_breeze-0.3.1/django_breeze/scripts/django_breeze.py
+-rw-r--r--   0        0        0     3145 2023-04-25 16:41:13.257732 django_breeze-0.3.1/django_breeze/settings.py
+-rw-r--r--   0        0        0   129342 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/static/django_breeze/django-breeze-logo.jpg
+-rw-r--r--   0        0        0   211529 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/static/django_breeze/django-breeze-logo.png
+-rw-r--r--   0        0        0      322 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react/.gitignore
+-rw-r--r--   0        0        0      561 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react/package.json
+-rw-r--r--   0        0        0       80 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react/postcss.config.js
+-rw-r--r--   0        0        0      115 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react/src/Layout/SiteLayout.jsx
+-rw-r--r--   0        0        0     4126 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react/src/assets/react.svg
+-rw-r--r--   0        0        0       58 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react/src/index.css
+-rw-r--r--   0        0        0      416 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react/src/index.html
+-rw-r--r--   0        0        0      544 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react/src/main.jsx
+-rw-r--r--   0        0        0      964 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react/src/pages/index.jsx
+-rw-r--r--   0        0        0      174 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react/tailwind.config.js
+-rw-r--r--   0        0        0      814 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react/vite.config.js
+-rw-r--r--   0        0        0      322 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react_typescript/.gitignore
+-rw-r--r--   0        0        0      577 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react_typescript/package.json
+-rw-r--r--   0        0        0       80 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react_typescript/postcss.config.js
+-rw-r--r--   0        0        0     1497 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react_typescript/public/vite.svg
+-rw-r--r--   0        0        0      115 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react_typescript/src/Layout/SiteLayout.tsx
+-rw-r--r--   0        0        0     4126 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react_typescript/src/assets/react.svg
+-rw-r--r--   0        0        0       59 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react_typescript/src/index.css
+-rw-r--r--   0        0        0      417 2023-04-25 16:41:13.261733 django_breeze-0.3.1/django_breeze/templates/react_typescript/src/index.html
+-rw-r--r--   0        0        0      544 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/react_typescript/src/main.tsx
+-rw-r--r--   0        0        0     1005 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/react_typescript/src/pages/index.tsx
+-rw-r--r--   0        0        0       38 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/react_typescript/src/vite-env.d.ts
+-rw-r--r--   0        0        0      174 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/react_typescript/tailwind.config.js
+-rw-r--r--   0        0        0      559 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/react_typescript/tsconfig.json
+-rw-r--r--   0        0        0      184 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/react_typescript/tsconfig.node.json
+-rw-r--r--   0        0        0      814 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/react_typescript/vite.config.ts
+-rw-r--r--   0        0        0      253 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3/.gitignore
+-rw-r--r--   0        0        0      429 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3/package.json
+-rw-r--r--   0        0        0       80 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3/postcss.config.js
+-rw-r--r--   0        0        0      496 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3/src/assets/vue.svg
+-rw-r--r--   0        0        0      282 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3/src/components/Framwork.vue
+-rw-r--r--   0        0        0       58 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3/src/index.css
+-rw-r--r--   0        0        0      422 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3/src/index.html
+-rw-r--r--   0        0        0      441 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3/src/main.jsx
+-rw-r--r--   0        0        0      809 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3/src/pages/index.vue
+-rw-r--r--   0        0        0     1497 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3/src/public/vite.svg
+-rw-r--r--   0        0        0      178 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3/tailwind.config.js
+-rw-r--r--   0        0        0      768 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3/vite.config.js
+-rw-r--r--   0        0        0      253 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3_typescript/.gitignore
+-rw-r--r--   0        0        0      504 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3_typescript/package.json
+-rw-r--r--   0        0        0       80 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3_typescript/postcss.config.js
+-rw-r--r--   0        0        0      496 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3_typescript/src/assets/vue.svg
+-rw-r--r--   0        0        0      282 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3_typescript/src/components/Framwork.vue
+-rw-r--r--   0        0        0       58 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3_typescript/src/index.css
+-rw-r--r--   0        0        0      433 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3_typescript/src/index.html
+-rw-r--r--   0        0        0      441 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3_typescript/src/main.tsx
+-rw-r--r--   0        0        0      809 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3_typescript/src/pages/index.vue
+-rw-r--r--   0        0        0     1497 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3_typescript/src/public/vite.svg
+-rw-r--r--   0        0        0       38 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3_typescript/src/vite-env.d.ts
+-rw-r--r--   0        0        0      178 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3_typescript/tailwind.config.js
+-rw-r--r--   0        0        0      661 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3_typescript/tsconfig.json
+-rw-r--r--   0        0        0      213 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3_typescript/tsconfig.node.json
+-rw-r--r--   0        0        0      768 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templates/vue3_typescript/vite.config.ts
+-rw-r--r--   0        0        0        0 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templatetags/__init__.py
+-rw-r--r--   0        0        0       51 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/templatetags/django_vite.py
+-rw-r--r--   0        0        0      130 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/urls.py
+-rw-r--r--   0        0        0      354 2023-04-25 16:41:13.265733 django_breeze-0.3.1/django_breeze/views.py
+-rw-r--r--   0        0        0      804 2023-04-25 16:41:13.265733 django_breeze-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5647 1970-01-01 00:00:00.000000 django_breeze-0.3.1/PKG-INFO
```

### Comparing `django_breeze-0.3.0/LICENSE.md` & `django_breeze-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/README.md` & `django_breeze-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/apps.py` & `django_breeze-0.3.1/django_breeze/apps.py`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/core/management/__init__.py` & `django_breeze-0.3.1/django_breeze/core/management/__init__.py`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/middleware.py` & `django_breeze-0.3.1/django_breeze/middleware.py`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/settings.py` & `django_breeze-0.3.1/django_breeze/settings.py`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/static/django_breeze/django-breeze-logo.jpg` & `django_breeze-0.3.1/django_breeze/static/django_breeze/django-breeze-logo.jpg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/static/django_breeze/django-breeze-logo.png` & `django_breeze-0.3.1/django_breeze/static/django_breeze/django-breeze-logo.png`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/templates/react/package.json` & `django_breeze-0.3.1/django_breeze/templates/react/package.json`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/templates/react/src/assets/react.svg` & `django_breeze-0.3.1/django_breeze/templates/react/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/templates/react/src/main.jsx` & `django_breeze-0.3.1/django_breeze/templates/react/src/main.jsx`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/templates/react/src/pages/index.jsx` & `django_breeze-0.3.1/django_breeze/templates/react/src/pages/index.jsx`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,15 @@
     <div className="text-center h-screen flex justify-center flex-col items-center p-4">
       <img
         className="w-full lg:w-[60%]"
         src="/static/django_breeze/django-breeze-logo.jpg"
         alt=""
       />
       <h1 className="text-3xl font-bold">Welcome, Django Breeze</h1>
-      <p className="text-green-600 mb-5">
-        Your project is setup is successfully!
-      </p>
+      <p className="text-green-600 mb-5">Your project is setup successfully!</p>
       <h3 className="text-slate-500">Powered by:</h3>
       <div className="lg:flex space-y-2 lg:space-y-0 lg:space-x-3 mt-3">
         {props.packages.map((framework, i) => (
           <PackageCard key={i} framework={framework} />
         ))}
       </div>
     </div>
```

### Comparing `django_breeze-0.3.0/django_breeze/templates/react/vite.config.js` & `django_breeze-0.3.1/django_breeze/templates/react/vite.config.js`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/templates/react_typescript/package.json` & `django_breeze-0.3.1/django_breeze/templates/react_typescript/package.json`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/templates/react_typescript/public/vite.svg` & `django_breeze-0.3.1/django_breeze/templates/react_typescript/public/vite.svg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/templates/react_typescript/src/assets/react.svg` & `django_breeze-0.3.1/django_breeze/templates/react_typescript/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/templates/react_typescript/src/main.tsx` & `django_breeze-0.3.1/django_breeze/templates/react_typescript/src/main.tsx`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/templates/react_typescript/src/pages/index.tsx` & `django_breeze-0.3.1/django_breeze/templates/react_typescript/src/pages/index.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,15 @@
     <div className="text-center h-screen flex justify-center flex-col items-center p-4">
       <img
         className="w-full lg:w-[60%]"
         src="/static/django_breeze/django-breeze-logo.jpg"
         alt=""
       />
       <h1 className="text-3xl font-bold">Welcome, Django Breeze</h1>
-      <p className="text-green-600 mb-5">
-        Your project is setup is successfully!
-      </p>
+      <p className="text-green-600 mb-5">Your project is setup successfully!</p>
       <h3 className="text-slate-500">Powered by:</h3>
       <div className="lg:flex space-y-2 lg:space-y-0 lg:space-x-3 mt-3">
         {props.packages.map((framework, i) => (
           <PackageCard key={i} framework={framework} />
         ))}
       </div>
     </div>
```

### Comparing `django_breeze-0.3.0/django_breeze/templates/react_typescript/tsconfig.json` & `django_breeze-0.3.1/django_breeze/templates/react_typescript/tsconfig.json`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/templates/react_typescript/vite.config.ts` & `django_breeze-0.3.1/django_breeze/templates/react_typescript/vite.config.ts`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/templates/vue3/src/pages/index.vue` & `django_breeze-0.3.1/django_breeze/templates/vue3/src/pages/index.vue`

 * *Files 15% similar despite different names*

```diff
@@ -13,17 +13,15 @@
   >
     <img
       className="w-full lg:w-[60%]"
       src="/static/django_breeze/django-breeze-logo.jpg"
       alt=""
     />
     <h1 className="text-3xl font-bold">Welcome, Django Breeze</h1>
-    <p className="text-green-600 mb-5">
-      Your project is setup is successfully!
-    </p>
+    <p className="text-green-600 mb-5">Your project is setup successfully!</p>
     <h3 className="text-slate-500">Powered by:</h3>
     <div className="lg:flex space-y-2 lg:space-y-0 lg:space-x-3 mt-3">
       <div v-for="framework in packages">
         <Framework :framework="framework" />
       </div>
     </div>
   </div>
```

### Comparing `django_breeze-0.3.0/django_breeze/templates/vue3/src/public/vite.svg` & `django_breeze-0.3.1/django_breeze/templates/vue3/src/public/vite.svg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/templates/vue3/vite.config.js` & `django_breeze-0.3.1/django_breeze/templates/vue3/vite.config.js`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/templates/vue3_typescript/src/pages/index.vue` & `django_breeze-0.3.1/django_breeze/templates/vue3_typescript/src/pages/index.vue`

 * *Files 15% similar despite different names*

```diff
@@ -13,17 +13,15 @@
   >
     <img
       className="w-full lg:w-[60%]"
       src="/static/django_breeze/django-breeze-logo.jpg"
       alt=""
     />
     <h1 className="text-3xl font-bold">Welcome, Django Breeze</h1>
-    <p className="text-green-600 mb-5">
-      Your project is setup is successfully!
-    </p>
+    <p className="text-green-600 mb-5">Your project is setup successfully!</p>
     <h3 className="text-slate-500">Powered by:</h3>
     <div className="lg:flex space-y-2 lg:space-y-0 lg:space-x-3 mt-3">
       <div v-for="framework in packages">
         <Framework :framework="framework" />
       </div>
     </div>
   </div>
```

### Comparing `django_breeze-0.3.0/django_breeze/templates/vue3_typescript/src/public/vite.svg` & `django_breeze-0.3.1/django_breeze/templates/vue3_typescript/src/public/vite.svg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/templates/vue3_typescript/tsconfig.json` & `django_breeze-0.3.1/django_breeze/templates/vue3_typescript/tsconfig.json`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/django_breeze/templates/vue3_typescript/vite.config.ts` & `django_breeze-0.3.1/django_breeze/templates/vue3_typescript/vite.config.ts`

 * *Files identical despite different names*

### Comparing `django_breeze-0.3.0/pyproject.toml` & `django_breeze-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-breeze"
-version =  "0.3.0"
+version =  "0.3.1"
 description = "Django Breeze provides a minimal and simple starting point for building a Django application with Inertia and Vite with minimal or no configuration. Styled with Tailwind CSS."
 keywords = ["react", "django", "vue", "inertia", "vite"]
 authors = ["louxsdon <louisayivi.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Louxsdon/django-breeze"
 packages = [{include = "django_breeze"}]
```

### Comparing `django_breeze-0.3.0/PKG-INFO` & `django_breeze-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-breeze
-Version: 0.3.0
+Version: 0.3.1
 Summary: Django Breeze provides a minimal and simple starting point for building a Django application with Inertia and Vite with minimal or no configuration. Styled with Tailwind CSS.
 Home-page: https://github.com/Louxsdon/django-breeze
 License: MIT
 Keywords: react,django,vue,inertia,vite
 Author: louxsdon
 Author-email: louisayivi.dev@gmail.com
 Requires-Python: >=3.10,<4.0
```

