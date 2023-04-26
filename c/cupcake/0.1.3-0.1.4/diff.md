# Comparing `tmp/cupcake-0.1.3.tar.gz` & `tmp/cupcake-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cupcake-0.1.3.tar", max compression
+gzip compressed data, was "cupcake-0.1.4.tar", max compression
```

## Comparing `cupcake-0.1.3.tar` & `cupcake-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-0.1.3/LICENSE
--rw-r--r--   0        0        0      549 2023-04-16 13:36:58.104474 cupcake-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-0.1.3/src/cupcake/__init__.py
--rw-r--r--   0        0        0     4023 2023-03-13 20:49:00.721516 cupcake-0.1.3/src/cupcake/cascade.py
--rw-r--r--   0        0        0     2345 2023-03-24 13:54:18.178294 cupcake-0.1.3/src/cupcake/confee.py
--rw-r--r--   0        0        0       35 2023-03-08 23:12:26.626449 cupcake-0.1.3/src/cupcake/data/new/.gitignore
--rw-r--r--   0        0        0      446 2023-04-05 14:08:12.001491 cupcake-0.1.3/src/cupcake/data/new/CMakeLists.txt
--rw-r--r--   0        0        0     1534 2023-04-04 16:25:50.085034 cupcake-0.1.3/src/cupcake/data/new/conanfile.py
--rw-r--r--   0        0        0      177 2022-04-07 22:23:03.400195 cupcake-0.1.3/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
--rw-r--r--   0        0        0       87 2022-04-07 22:23:55.073837 cupcake-0.1.3/src/cupcake/data/new/src/lib{{name}}.cpp
--rw-r--r--   0        0        0      143 2022-04-07 22:49:53.297481 cupcake-0.1.3/src/cupcake/data/new/src/{{name}}.cpp
--rw-r--r--   0        0        0      177 2023-03-10 21:15:53.093370 cupcake-0.1.3/src/cupcake/data/new/tests/CMakeLists.txt
--rw-r--r--   0        0        0      169 2022-04-07 22:20:24.683135 cupcake-0.1.3/src/cupcake/data/new/tests/{{name}}.cpp
--rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-0.1.3/src/cupcake/data/query/CMakeLists.txt
--rw-r--r--   0        0        0    27445 2023-04-16 01:37:02.469659 cupcake-0.1.3/src/cupcake/main.py
--rw-r--r--   0        0        0     6725 2023-03-08 20:46:34.258683 cupcake-0.1.3/src/cupcake/scratch.py
--rw-r--r--   0        0        0     1004 2023-04-16 13:37:27.791882 cupcake-0.1.3/setup.py
--rw-r--r--   0        0        0      578 2023-04-16 13:37:27.792074 cupcake-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-0.1.4/LICENSE
+-rw-r--r--   0        0        0      549 2023-04-26 15:54:10.021402 cupcake-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-0.1.4/src/cupcake/__init__.py
+-rw-r--r--   0        0        0     4023 2023-03-13 20:49:00.721516 cupcake-0.1.4/src/cupcake/cascade.py
+-rw-r--r--   0        0        0     2345 2023-03-24 13:54:18.178294 cupcake-0.1.4/src/cupcake/confee.py
+-rw-r--r--   0        0        0      650 2023-04-17 16:48:12.052154 cupcake-0.1.4/src/cupcake/data/cmake_file_name.py
+-rw-r--r--   0        0        0       35 2023-03-08 23:12:26.626449 cupcake-0.1.4/src/cupcake/data/new/.gitignore
+-rw-r--r--   0        0        0      457 2023-04-17 16:32:26.489411 cupcake-0.1.4/src/cupcake/data/new/CMakeLists.txt
+-rw-r--r--   0        0        0     1534 2023-04-04 16:25:50.085034 cupcake-0.1.4/src/cupcake/data/new/conanfile.py
+-rw-r--r--   0        0        0      215 2023-04-18 03:25:43.426297 cupcake-0.1.4/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
+-rw-r--r--   0        0        0       87 2022-04-07 22:23:55.073837 cupcake-0.1.4/src/cupcake/data/new/src/lib{{name}}.cpp
+-rw-r--r--   0        0        0      143 2022-04-07 22:49:53.297481 cupcake-0.1.4/src/cupcake/data/new/src/{{name}}.cpp
+-rw-r--r--   0        0        0      187 2023-04-17 16:32:36.189898 cupcake-0.1.4/src/cupcake/data/new/tests/CMakeLists.txt
+-rw-r--r--   0        0        0      169 2022-04-07 22:20:24.683135 cupcake-0.1.4/src/cupcake/data/new/tests/{{name}}.cpp
+-rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-0.1.4/src/cupcake/data/query/CMakeLists.txt
+-rw-r--r--   0        0        0    32755 2023-04-26 15:52:37.305011 cupcake-0.1.4/src/cupcake/main.py
+-rw-r--r--   0        0        0     6725 2023-03-08 20:46:34.258683 cupcake-0.1.4/src/cupcake/scratch.py
+-rw-r--r--   0        0        0     1033 2023-04-26 15:54:47.661366 cupcake-0.1.4/setup.py
+-rw-r--r--   0        0        0      578 2023-04-26 15:54:47.661583 cupcake-0.1.4/PKG-INFO
```

### Comparing `cupcake-0.1.3/LICENSE` & `cupcake-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.3/pyproject.toml` & `cupcake-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cupcake"
-version = "0.1.3"
+version = "0.1.4"
 description = "Make C++ a piece of cake."
 authors = ["John Freeman <jfreeman08@gmail.com>"]
 packages = [{include = "cupcake", from = "src"}]
 
 [tool.poetry.scripts]
 cupcake = 'cupcake.main:main'
```

### Comparing `cupcake-0.1.3/src/cupcake/cascade.py` & `cupcake-0.1.4/src/cupcake/cascade.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.3/src/cupcake/confee.py` & `cupcake-0.1.4/src/cupcake/confee.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.3/src/cupcake/data/new/conanfile.py` & `cupcake-0.1.4/src/cupcake/data/new/conanfile.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.3/src/cupcake/main.py` & `cupcake-0.1.4/src/cupcake/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,27 +12,43 @@
 import operator
 import os
 import pathlib
 import re
 import shlex
 import shutil
 import subprocess
+import sys
 import tempfile
 import urllib.parse
 
 from cupcake import cascade, confee
 
 def run(command, *args, **kwargs):
     # TODO: Print this in a special color.
     print(' '.join(shlex.quote(str(arg)) for arg in command), flush=True)
     proc = subprocess.run(command, *args, **kwargs)
     if proc.returncode != 0:
         raise SystemExit(proc.returncode)
     return proc
 
+def tee(command, *args, log, **kwargs):
+    proc = subprocess.Popen(
+        command, *args,
+        stdout=subprocess.PIPE, stderr=subprocess.STDOUT, **kwargs
+    )
+    with open(log, 'wb') as logf:
+        line = ' '.join(shlex.quote(str(arg)) for arg in command).encode()
+        logf.write(line)
+        sys.stdout.buffer.write(line)
+        for line in proc.stdout:
+            logf.write(line)
+            sys.stdout.buffer.write(line)
+    if proc.wait() != 0:
+        raise SystemExit(proc.returncode)
+
 def hash_file(path):
     return hashlib.sha256(path.read_bytes()).hexdigest()
 
 def max_by(compare):
     def function(x, y):
         return y if compare(x, y) < 0 else x
     return function
@@ -236,14 +252,52 @@
         }
         args = [f'-D{name}={value}' for name, value in variables.items()]
         args = [*args, source_dir]
         if generator is not None:
             args = ['-G', generator, *args]
         run([self.CMAKE, *args], cwd=build_dir)
 
+class CMakeLists:
+    def __init__(self, path):
+        self.path = path
+
+    def import_(self, package, version):
+        MODE_FIND = 0
+        MODE_INSERT = 1
+        MODE_FINISH = 2
+
+        added_line = f'cupcake_find_package({package} {version})\n'
+        with tempfile.NamedTemporaryFile(mode='w') as cml_out:
+            with self.path.open('r') as cml_in:
+                mode = MODE_FIND
+                for line in cml_in:
+                    if mode == MODE_FIND and re.match(r'^# imports$', line):
+                        mode = MODE_INSERT
+                    elif mode == MODE_INSERT:
+                        is_comment = re.match(r'^#', line)
+                        match = re.match(r'^cupcake_find_package\((\w+)', line)
+                        skip = (
+                            is_comment or
+                            (match and match.group(1) < package)
+                        )
+                        # Would love to have goto for this situation.
+                        if match and match.group(1) == package:
+                            mode = MODE_FINISH
+                        elif not skip:
+                            cml_out.write(added_line)
+                            mode = MODE_FINISH
+                    cml_out.write(line)
+            if mode == MODE_INSERT:
+                cml_out.write(added_line)
+            elif mode == MODE_FIND:
+                print(f'nowhere to insert call to `find_package` in {cml}')
+                return
+            cml_out.flush()
+            shutil.copy(cml_out.name, self.path)
+
 test_template = """
 {{ cmake }} --build {{ cmakeDir }}
 {% if multiConfig %} --config {{ flavor }} {% endif %}
 --target {% if multiConfig %} RUN_TESTS {% else %} test {% endif %}
 """
 
 def cstNewLine(indent=''):
@@ -377,14 +431,20 @@
         """
         :param build_dir: pretty format of build directory
         """
         build_dir_path_.mkdir(parents=True, exist_ok=True)
         return build_dir_path_
 
     @cascade.value()
+    def log_dir_(self, build_dir_) -> pathlib.Path:
+        log_dir_path_ = build_dir_ / 'logs'
+        log_dir_path_.mkdir(exist_ok=True)
+        return log_dir_path_
+
+    @cascade.value()
     def state_(self, build_dir_):
         path = build_dir_ / 'cupcake.toml'
         return confee.read(path)
 
     @cascade.value()
     @cascade.option(
         '--flavor',
@@ -421,14 +481,15 @@
     @cascade.option('--profile', help='Name of Conan profile.')
     # TODO: Add option to configure shared linkage.
     def conan(
         self,
         source_dir_,
         conanfile_path_,
         build_dir_,
+        log_dir_,
         config_,
         CONAN,
         state_,
         flavor_,
         profile,
     ):
         """Configure Conan."""
@@ -457,16 +518,17 @@
         conan_dir.mkdir(parents=True, exist_ok=True)
         base_command = [
             CONAN, 'install', source_dir_, '--build', 'missing',
             '--output-folder', conan_dir,
             '--profile:build', profile, '--profile:host', profile,
         ]
         for flavor in diff_flavors:
-            run(
+            tee(
                 [*base_command, '--settings', f'build_type={FLAVORS[flavor_]}'],
+                log=log_dir_ / 'conan',
                 cwd=conan_dir,
             )
         state_.conan.id = id
         state_.conan.flavors = new_flavors
         # TODO: Find layout. How?
         toolchain = conan_dir / 'conan_toolchain.cmake'
         if not toolchain.exists():
@@ -492,30 +554,62 @@
         default=None,
     )
     @cascade.option(
         '-P', 'prefixes',
         help='Prefix to search for installed packages. Repeatable.',
         multiple=True,
     )
+    @cascade.option(
+        '-D', 'variables',
+        help='CMake variables to set. Repeatable.',
+        multiple=True,
+    )
+    @cascade.option(
+        '-U', 'unvariables',
+        help='CMake variables to unset. Repeatable.',
+        multiple=True,
+    )
     def cmake(
         self,
         source_dir_,
         config_,
         CMAKE,
         build_dir_,
         state_,
         flavor_,
         prefix_,
         conan,
         generator,
         shared,
         with_tests,
         prefixes,
+        variables,
+        unvariables,
     ):
         """Configure CMake."""
+        # Variables are a little unique.
+        # We must start with `config.cmake.variables` (default `{}`),
+        # override with `variables`,
+        # remove `unvariables`,
+        # and then write the result to `config.cmake.variables`.
+        cvars = config_.cmake.variables({})
+        for variable in variables:
+            match = re.match(r'^([^=]+)(?:=(.+))?$', variable)
+            if not match:
+                raise SystemExit(f'bad variable: `{variable}`')
+            name = match.group(1)
+            value = match.group(2)
+            if value is None:
+                value = 'TRUE'
+            cvars[name] = value
+        for name in unvariables:
+            cvars.pop(name, None)
+        if cvars:
+            config_.cmake.variables = cvars
+
         generator = confee.resolve(generator, config_.cmake.generator, None)
         shared = confee.resolve(shared, config_.cmake.shared, False)
         with_tests = confee.resolve(with_tests, config_.cmake.tests, True)
         prefixes = confee.resolve(prefixes or None, config_.cmake.prefixes, [])
         # TODO: Convenience API for hashing identities.
         m = hashlib.sha256()
         if conan is not None:
@@ -526,14 +620,17 @@
             m.update(generator.encode())
         if shared:
             m.update(b'shared')
         if with_tests:
             m.update(b'tests')
         for p in prefixes:
             m.update(p.encode())
+        for name, value in cvars.items():
+            m.update(name.encode())
+            m.update(value.encode())
         id = m.hexdigest()
         # We need to know what flavors are configured in CMake after this
         # step.
         # If we find that the generator is single-config and the CMake state
         # ID is the same, then we can add the new flavor to the existing
         # CMake state flavors.
         # If we find that the generator is multi-config, then we'll use all
@@ -576,14 +673,17 @@
         if prefixes:
             cmake_args['CMAKE_PREFIX_PATH'] = ';'.join(prefixes)
         if multiConfig:
             new_flavors = config_.flavors()
             cmake_args['CMAKE_CONFIGURATION_TYPES'] = ';'.join(new_flavors)
         else:
             cmake_args['CMAKE_BUILD_TYPE'] = FLAVORS[flavor_]
+        # Add these last to let callers override anything.
+        for name, value in cvars.items():
+            cmake_args[name] = value
         CMake(CMAKE).configure(
             cmake_dir, source_dir_, generator, cmake_args
         )
         state_.cmake.id = id
         state_.cmake.multiConfig = multiConfig
         state_.cmake.flavors = new_flavors
         confee.write(config_)
@@ -597,26 +697,40 @@
             build_dir_ /= flavor_
         return build_dir_
 
     @cascade.command()
     @cascade.option(
         '--jobs', '-j', help='Maximum number of simultaneous jobs.'
     )
-    def build(self, CMAKE, cmake_dir_, flavor_, cmake, jobs):
+    def build(self, CMAKE, build_dir_, log_dir_, cmake_dir_, flavor_, cmake, jobs):
         """Build the selected flavor."""
-        args = ['--verbose']
+        command = [CMAKE, '--build', cmake_dir_, '--verbose']
         if cmake.multiConfig():
-            args.extend(['--config', FLAVORS[flavor_]])
-        args.append('--parallel')
+            command.extend(['--config', FLAVORS[flavor_]])
+        command.append('--parallel')
         if jobs is not None:
-            args.append(jobs)
-        run([CMAKE, '--build', cmake_dir_, *args])
+            command.append(jobs)
+        tee(command, log=log_dir_ / 'build')
         return cmake
 
     @cascade.command()
+    @cascade.argument('executable', required=False)
+    @cascade.argument('arguments', nargs=-1)
+    def exe(self, CMAKE, cmake_dir_, flavor_, cmake, executable, arguments):
+        target = 'execute'
+        if executable is not None:
+            target += '-' + executable
+        command = [CMAKE, '--build', cmake_dir_, '--target', target]
+        if cmake.multiConfig():
+            command.extend(['--config', FLAVORS[flavor_]])
+        env = os.environ.copy()
+        env['CUPCAKE_EXE_ARGUMENTS'] = ' '.join(map(shlex.quote, arguments))
+        run(command, env=env)
+
+    @cascade.command()
     def install(self, CMAKE, cmake_dir_, flavor_, build, prefix_):
         """Install the selected flavor."""
         run([
             CMAKE,
             '--install',
             cmake_dir_,
             '--config',
@@ -722,15 +836,15 @@
 
     @cascade.command()
     # TODO: Mutually exclusive option group for category.
     @cascade.option(
         '--test', '-T', 'as_test', is_flag=True, help='As a test requirement.',
     )
     @cascade.argument('package')
-    def add(self, CONAN, conanfile_path_, as_test, package):
+    def add(self, CONAN, source_dir_, conanfile_path_, as_test, package):
         """Add a requirement."""
         # TODO: Support conanfile.txt.
         if conanfile_path_.name != 'conanfile.py':
             raise SystemExit('missing conanfile.py')
         results = Conan(CONAN).search(package)
         if len(results) < 1:
             raise SystemExit('no matches found')
@@ -741,14 +855,39 @@
             tree = tree.visit(AddRequirement(
                 'test_requires' if as_test else 'requires', package, version,
             ))
             recipe_out.write(tree.code)
             recipe_out.flush()
             shutil.copy(recipe_out.name, conanfile_path_)
 
+        # Have to jump through some hoops to get the `cmake_file_name`
+        # that we must pass to `find_package`.
+        loader = jinja2.PackageLoader('cupcake', 'data')
+        env = jinja2.Environment(
+            loader=loader,
+            keep_trailing_newline=True,
+            trim_blocks=True,
+            lstrip_blocks=True,
+        )
+        template = env.get_template('cmake_file_name.py')
+        with tempfile.TemporaryDirectory() as tmp:
+            cwd = pathlib.Path(tmp)
+            stream = template.stream(dict(ref=f'{package}/{version}'))
+            with (cwd / 'conanfile.py').open('w') as file:
+                stream.dump(file)
+            run([CONAN, 'install', '.', '--build', 'missing'], cwd=cwd)
+            cmake_file_name = (cwd / 'cmake_file_name.txt').read_text()
+
+        # Add an import.
+        cml = source_dir_
+        if as_test:
+            cml /= 'tests'
+        cml /= 'CMakeLists.txt'
+        CMakeLists(cml).import_(cmake_file_name, version)
+
     @cascade.command()
     @cascade.argument('package')
     def remove(self, conanfile_path_, package):
         """Remove a requirement."""
         # TODO: Support conanfile.txt.
         if conanfile_path_.name != 'conanfile.py':
             raise SystemExit('missing conanfile.py')
```

### Comparing `cupcake-0.1.3/src/cupcake/scratch.py` & `cupcake-0.1.4/src/cupcake/scratch.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.3/setup.py` & `cupcake-0.1.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['cupcake', 'cupcake.data.new']
+['cupcake', 'cupcake.data', 'cupcake.data.new']
 
 package_data = \
 {'': ['*'],
- 'cupcake': ['data/query/*'],
+ 'cupcake.data': ['query/CMakeLists.txt'],
  'cupcake.data.new': ['include/{{name}}/*', 'src/*', 'tests/*']}
 
 install_requires = \
 ['click-option-group>=0.5.3,<0.6.0',
  'click>=8.0.4,<9.0.0',
  'jinja2>=3.1.1,<4.0.0',
  'libcst>=0.4.9,<0.5.0',
  'tomlkit>=0.10.1,<0.11.0']
 
 entry_points = \
 {'console_scripts': ['cupcake = cupcake.main:main']}
 
 setup_kwargs = {
     'name': 'cupcake',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Make C++ a piece of cake.',
     'long_description': None,
     'author': 'John Freeman',
     'author_email': 'jfreeman08@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `cupcake-0.1.3/PKG-INFO` & `cupcake-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cupcake
-Version: 0.1.3
+Version: 0.1.4
 Summary: Make C++ a piece of cake.
 Author: John Freeman
 Author-email: jfreeman08@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

