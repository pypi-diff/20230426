# Comparing `tmp/hypofuzz-22.7.1.tar.gz` & `tmp/hypofuzz-23.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypofuzz-22.7.1.tar", last modified: Mon Jul 11 16:43:26 2022, max compression
+gzip compressed data, was "hypofuzz-23.4.1.tar", last modified: Wed Apr 26 00:18:40 2023, max compression
```

## Comparing `hypofuzz-22.7.1.tar` & `hypofuzz-23.4.1.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 16:43:26.001019 hypofuzz-22.7.1/
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-07-11 16:43:26.001019 hypofuzz-22.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-07-11 16:43:18.000000 hypofuzz-22.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-11 16:43:26.001019 hypofuzz-22.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-07-11 16:43:18.000000 hypofuzz-22.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 16:43:25.997019 hypofuzz-22.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 16:43:26.001019 hypofuzz-22.7.1/src/hypofuzz/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-07-11 16:43:18.000000 hypofuzz-22.7.1/src/hypofuzz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15726 2022-07-11 16:43:18.000000 hypofuzz-22.7.1/src/hypofuzz/corpus.py
--rw-r--r--   0 runner    (1001) docker     (121)     4686 2022-07-11 16:43:18.000000 hypofuzz-22.7.1/src/hypofuzz/cov.py
--rw-r--r--   0 runner    (1001) docker     (121)     8516 2022-07-11 16:43:18.000000 hypofuzz-22.7.1/src/hypofuzz/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-07-11 16:43:18.000000 hypofuzz-22.7.1/src/hypofuzz/debugger.py
--rw-r--r--   0 runner    (1001) docker     (121)     2961 2022-07-11 16:43:18.000000 hypofuzz-22.7.1/src/hypofuzz/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (121)    16282 2022-07-11 16:43:18.000000 hypofuzz-22.7.1/src/hypofuzz/hy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3260 2022-07-11 16:43:18.000000 hypofuzz-22.7.1/src/hypofuzz/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-11 16:43:18.000000 hypofuzz-22.7.1/src/hypofuzz/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 16:43:26.001019 hypofuzz-22.7.1/src/hypofuzz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-07-11 16:43:25.000000 hypofuzz-22.7.1/src/hypofuzz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-07-11 16:43:25.000000 hypofuzz-22.7.1/src/hypofuzz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-11 16:43:25.000000 hypofuzz-22.7.1/src/hypofuzz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-07-11 16:43:25.000000 hypofuzz-22.7.1/src/hypofuzz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-11 16:43:25.000000 hypofuzz-22.7.1/src/hypofuzz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-07-11 16:43:25.000000 hypofuzz-22.7.1/src/hypofuzz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-11 16:43:25.000000 hypofuzz-22.7.1/src/hypofuzz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:40.243405 hypofuzz-23.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-26 00:18:40.243405 hypofuzz-23.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 00:18:40.243405 hypofuzz-23.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:40.239405 hypofuzz-23.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:40.239405 hypofuzz-23.4.1/src/hypofuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17170 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/hy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/src/hypofuzz/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:40.243405 hypofuzz-23.4.1/src/hypofuzz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-26 00:18:40.000000 hypofuzz-23.4.1/src/hypofuzz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-26 00:18:40.000000 hypofuzz-23.4.1/src/hypofuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:18:40.000000 hypofuzz-23.4.1/src/hypofuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 00:18:40.000000 hypofuzz-23.4.1/src/hypofuzz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:18:40.000000 hypofuzz-23.4.1/src/hypofuzz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-26 00:18:40.000000 hypofuzz-23.4.1/src/hypofuzz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 00:18:40.000000 hypofuzz-23.4.1/src/hypofuzz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:18:40.243405 hypofuzz-23.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/tests/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/tests/test_coverage_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/tests/test_fuzz_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-26 00:18:21.000000 hypofuzz-23.4.1/tests/test_version.py
```

### Comparing `hypofuzz-22.7.1/PKG-INFO` & `hypofuzz-23.4.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,63 @@
 Metadata-Version: 2.1
 Name: hypofuzz
-Version: 22.7.1
+Version: 23.4.1
 Summary: Adaptive fuzzing for property-based tests
 Home-page: https://hypofuzz.com/
 Author: Zac Hatfield-Dodds
 Author-email: zac@hypofuzz.com
-License: Proprietary License
-Project-URL: Funding, https://hypofuzz.com/pricing/
+License: AGPL-3.0
 Project-URL: Documentation, https://hypofuzz.com/docs/
 Project-URL: Changelog, https://hypofuzz.com/docs/changelog.html
 Keywords: python testing fuzzing property-based-testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Hypothesis
 Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Testing
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pytrace
+License-File: LICENSE
 
 # [HypoFuzz](https://hypofuzz.com/)
 
 *Adaptive fuzzing of [Hypothesis](https://hypothesis.readthedocs.io) tests.*
 
 
 Property-based approaches help you to write better tests which find more bugs,
 but don't have great ways to exchange much more CPU time for more bugs.
 The goal of this project is to bring togther the best parts of fuzzing and PBT.
 
 
 ## Motivation
 
 You can [run a traditional fuzzer](https://hypothesis.readthedocs.io/en/latest/details.html#use-with-external-fuzzers)
-like AFL on Hypothesis tests to get basic coverage guidance.
-
-- This does actually work, which is pretty cool
-- It's very slow though, and often fails to parse the bytes into an example
-- Installing, configuring, and connecting all the parts is a pain
-- Also assumes one fuzz target per core, which doesn't scale very far
+like AFL on Hypothesis tests to get basic coverage guidance.  This works OK, but there's
+a lot of performance overhead.  Installing, configuring, and connecting all the parts is
+a pain, and because it assumes one fuzz target per core you probably can't scale up far
+enough to fuzz your whole test suite.
 
 Alternatively, you can just run Hypothesis with a large `max_examples` setting.
-This also works pretty well, but doesn't get the benefits of coverage guidance
-(i.e. avoiding the exponential scaling cliff by learning from feedback) and
-also occupies one fuzz target per core.
-
-(turns out that you can [emulate coverage guidance](https://engineering.backtrace.io/posts/2020-03-11-how-hard-is-it-to-guide-test-case-generators-with-branch-coverage-feedback/)
-with `hypothesis.target()`, which appears to work well enough as a starting point)
-
-(also Hypothesis used to have coverage guidance built in, but we took it back out
-because of performance and ecosystem integration problems - as a rule of thumb it's
-just not worth the trouble for less than a thousand inputs.
-[see here](https://github.com/HypothesisWorks/hypothesis/pulls?q=is%3Amerged+use_coverage).)
+This also works pretty well, but doesn't get the benefits of coverage guidance and
+you have to guess how long it'll take to run the tests - each gets the same budget.
+
+HypoFuzz solves all of these problems, and more!
 
 
 ## Features
 
 - Interleave execution of many test functions
 - Prioritise functions where we expect to make progress
 - Coverage-guided exploration of your system-under-test
-- Seamless python-native and CLI integrations
+- Seamless python-native and CLI integrations (replaces the `pytest` command)
 - Web-based time-travel debugging with [PyTrace](https://pytrace.com/)
   (automatic if you `pip install hypofuzz[pytrace]`)
 
-
-## Changelog
-
-Patch notes [can be found in `CHANGELOG.md`](https://github.com/Zac-HD/hypofuzz/blob/master/CHANGELOG.md).
-
-
-## License
-
-This is an active research project as part of my (Zac Hatfield-Dodds) PhD.
-
-Unlike Hypothesis, it is *not* open source and I am not seeking external contributions.
-
-As a complement to users of free, world-class PBT tools, I'm planning to sell
-licenses in order to fund ongoing work on both this project and Hypothesis itself.
-Please [contact me](mailto:sales@hypofuzz.com) if you are interested.
+Read more about HypoFuzz at https://hypofuzz.com/docs/, including
+[the changelog](https://hypofuzz.com/docs/changelog.html).
```

### Comparing `hypofuzz-22.7.1/setup.py` & `hypofuzz-23.4.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,69 @@
-import os
-
-import setuptools
-
-
-def local_file(name: str) -> str:
-    """Interpret filename as relative to this file."""
-    return os.path.relpath(os.path.join(os.path.dirname(__file__), name))
-
-
-SOURCE = local_file("src")
-README = local_file("README.md")
-
-with open(local_file("src/hypofuzz/__init__.py")) as o:
-    for line in o:
-        if line.startswith("__version__"):
-            _, __version__, _ = line.split('"')
-
-
-setuptools.setup(
-    name="hypofuzz",
-    version=__version__,
-    author="Zac Hatfield-Dodds",
-    author_email="zac@hypofuzz.com",
-    packages=setuptools.find_packages(SOURCE),
-    package_dir={"": SOURCE},
-    package_data={"": ["py.typed"]},
-    url="https://hypofuzz.com/",
-    project_urls={
-        "Funding": "https://hypofuzz.com/pricing/",
-        "Documentation": "https://hypofuzz.com/docs/",
-        "Changelog": "https://hypofuzz.com/docs/changelog.html",
-    },
-    license="Proprietary License",
-    description="Adaptive fuzzing for property-based tests",
-    zip_safe=False,
-    install_requires=[
-        "coverage >= 5.2.1",
-        "dash >= 2.0.0",
-        "hypothesis[cli] >= 6.50.1",
-        "pandas >= 1.0.0",
-        "psutil >= 3.0.0",
-        "pytest >= 6.0.1",
-        "requests >= 2.24.0",
-    ],
-    extras_require={
-        "pytrace": [
-            "flask-cors >= 3.0.10",
-            "pycrunch-trace >= 0.1.6",
-        ],
-    },
-    python_requires=">=3.7",
-    classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Framework :: Hypothesis",
-        "Intended Audience :: Developers",
-        "License :: Other/Proprietary License",  # Get in touch if you're interested!
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Topic :: Software Development :: Testing",
-        "Typing :: Typed",
-    ],
-    entry_points={"hypothesis": ["_ = hypofuzz.entrypoint"]},
-    long_description=open(README).read(),
-    long_description_content_type="text/markdown",
-    keywords="python testing fuzzing property-based-testing",
-)
+import os
+
+import setuptools
+
+
+def local_file(name: str) -> str:
+    """Interpret filename as relative to this file."""
+    return os.path.relpath(os.path.join(os.path.dirname(__file__), name))
+
+
+SOURCE = local_file("src")
+README = local_file("README.md")
+
+with open(local_file("src/hypofuzz/__init__.py")) as o:
+    for line in o:
+        if line.startswith("__version__"):
+            _, __version__, _ = line.split('"')
+
+
+setuptools.setup(
+    name="hypofuzz",
+    version=__version__,
+    author="Zac Hatfield-Dodds",
+    author_email="zac@hypofuzz.com",
+    packages=setuptools.find_packages(SOURCE),
+    package_dir={"": SOURCE},
+    package_data={"": ["py.typed"]},
+    url="https://hypofuzz.com/",
+    project_urls={
+        "Documentation": "https://hypofuzz.com/docs/",
+        "Changelog": "https://hypofuzz.com/docs/changelog.html",
+    },
+    license="AGPL-3.0",
+    description="Adaptive fuzzing for property-based tests",
+    zip_safe=False,
+    install_requires=[
+        "coverage >= 5.2.1",
+        "dash >= 2.0.0",
+        "hypothesis[cli] >= 6.50.1",
+        "pandas >= 1.0.0",
+        "psutil >= 3.0.0",
+        "pytest >= 6.0.1",
+        "requests >= 2.24.0",
+    ],
+    extras_require={
+        "pytrace": [
+            "flask-cors >= 3.0.10",
+            "pycrunch-trace >= 0.1.6",
+        ],
+    },
+    python_requires=">=3.8",
+    classifiers=[
+        "Development Status :: 3 - Alpha",
+        "Framework :: Hypothesis",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: GNU Affero General Public License v3",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Software Development :: Testing",
+        "Typing :: Typed",
+    ],
+    entry_points={"hypothesis": ["_ = hypofuzz.entrypoint"]},
+    long_description=open(README).read(),
+    long_description_content_type="text/markdown",
+    keywords="python testing fuzzing property-based-testing",
+)
```

### Comparing `hypofuzz-22.7.1/src/hypofuzz/corpus.py` & `hypofuzz-23.4.1/src/hypofuzz/corpus.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,387 +1,388 @@
-"""Adaptive fuzzing for property-based tests using Hypothesis."""
-
-import abc
-import enum
-from random import Random
-from typing import (
-    Callable,
-    Counter,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Set,
-    Tuple,
-    Type,
-    Union,
-)
-
-from hypothesis import __version__ as hypothesis_version
-from hypothesis.core import encode_failure
-from hypothesis.database import ExampleDatabase
-from hypothesis.internal.conjecture.data import (
-    ConjectureData,
-    ConjectureResult,
-    Overrun,
-    Status,
-)
-from hypothesis.internal.conjecture.shrinker import Shrinker
-from sortedcontainers import SortedDict
-
-from .cov import Arc
-
-
-class HowGenerated(enum.Enum):
-    blackbox = "blackbox"
-    mutation = "mutation"
-    shrinking = "shrinking"
-
-
-def sort_key(buffer: Union[bytes, ConjectureResult]) -> Tuple[int, bytes]:
-    """Sort our buffers in shortlex order.
-
-    See `hypothesis.internal.conjecture.shrinker.sort_key` for details on why we
-    use shortlex order in particular.  This tweaked version is identical except
-    for handling ConjectureResult objects too.
-    """
-    if isinstance(buffer, ConjectureResult):
-        buffer = buffer.buffer
-    return (len(buffer), buffer)
-
-
-def reproduction_decorator(buffer: bytes) -> str:
-    """Return `@reproduce_failure` decorator for the given buffer."""
-    return f"@reproduce_failure({hypothesis_version!r}, {encode_failure(buffer)!r})"
-
-
-class EngineStub:
-    """A knock-off ConjectureEngine, just large enough to run a shrinker."""
-
-    def __init__(
-        self, test_fn: Callable[[bytes], ConjectureData], random: Random
-    ) -> None:
-        self.cached_test_function = test_fn
-        self.random = random
-        self.call_count = 0
-        self.report_debug_info = False
-
-    def debug(self, msg: str) -> None:
-        """Unimplemented stub."""
-
-    def explain_next_call_as(self, msg: str) -> None:
-        """Unimplemented stub."""
-
-    def clear_call_explanation(self) -> None:
-        """Unimplemented stub."""
-
-
-class Pool:
-    """Manage the seed pool for a fuzz target.
-
-    The class tracks the minimal valid example which covers each known arc.
-    """
-
-    def __init__(self, database: ExampleDatabase, key: bytes) -> None:
-        # The database and our database key are the stable identifiers for a corpus.
-        # Everything else is reconstructed each run, and tracked only in memory.
-        self._database = database
-        self._key = key
-
-        # Our sorted pool of covering examples, ready to be sampled from.
-        # TODO: One suggestion to reduce effective pool size/redundancy is to skip
-        #       over earlier inputs whose coverage is a subset of later inputs.
-        self.results: Dict[bytes, ConjectureResult] = SortedDict(sort_key)
-
-        # For each arc, what's the minimal covering example?
-        self.covering_buffers: Dict[Arc, bytes] = {}
-        # How many times have we seen each arc since discovering our latest arc?
-        self.arc_counts: Counter[Arc] = Counter()
-
-        # And various internal attributes and metadata
-        self.interesting_examples: Dict[
-            Tuple[Type[BaseException], str, int], Tuple[ConjectureResult, List[str]]
-        ] = {}
-        self._loaded_from_database: Set[bytes] = set()
-        self.__shrunk_to_buffers: Set[bytes] = set()
-
-        # To show the current state of the pool in the dashboard
-        self.json_report: List[List[str]] = []
-        self._in_distill_phase = False
-
-    def __repr__(self) -> str:
-        rs = {b: r.extra_information.branches for b, r in self.results.items()}
-        return (
-            f"<Pool\n    results={rs}\n    arc_counts={self.arc_counts}\n    "
-            f"covering_buffers={self.covering_buffers}\n>"
-        )
-
-    def _check_invariants(self) -> None:
-        """Check all invariants of the structure."""
-        seen: Set[Arc] = set()
-        for res in self.results.values():
-            # Each result in our ordered buffer covers at least one arc not covered
-            # by any more-minimal result.
-            not_previously_covered = res.extra_information.branches - seen
-            assert not_previously_covered
-            # And our covering_buffers map points back the correct (minimal) buffer
-            for arc in not_previously_covered:
-                assert self.covering_buffers[arc] == res.buffer
-            seen.update(res.extra_information.branches)
-
-        # And the union of those branches is exactly covered by our counters.
-        assert seen == set(self.covering_buffers), seen.symmetric_difference(
-            self.covering_buffers
-        )
-        assert seen == set(self.covering_buffers), seen.symmetric_difference(
-            self.arc_counts
-        )
-
-        # Every covering buffer was either read from the database, or saved to it.
-        assert self._loaded_from_database.issuperset(self.covering_buffers.values())
-
-    @property
-    def _fuzz_key(self) -> bytes:
-        return self._key + b".fuzz"
-
-    def add(self, result: ConjectureResult, source: HowGenerated) -> Optional[bool]:
-        """Update the corpus with the result of running a test.
-
-        Returns None for invalid examples, False if no change, True if changed.
-        """
-        assert result is Overrun or isinstance(result, ConjectureResult), result
-        if result.status < Status.VALID:
-            return None
-
-        # We now know that we have a ConjectureResult representing a valid test
-        # execution, either passing or possibly failing.
-        branches = result.extra_information.branches
-        buf = result.buffer
-
-        # If the example is "interesting", i.e. the test failed, add the buffer to
-        # the database under Hypothesis' default key so it will be reproduced.
-        if result.status == Status.INTERESTING:
-            origin = result.interesting_origin
-            if origin not in self.interesting_examples or sort_key(result) < sort_key(
-                self.interesting_examples[origin]
-            ):
-                self.interesting_examples[origin] = (
-                    result,
-                    [
-                        result.extra_information.call_repr,
-                        result.extra_information.reports,
-                        reproduction_decorator(result.buffer),
-                        result.extra_information.traceback,
-                    ],
-                )
-                return True
-
-        # If we haven't just discovered new branches and our example is larger than the
-        # current largest minimal example, we can skip the expensive calculation.
-        if (not branches.issubset(self.arc_counts)) or (
-            self.results
-            and sort_key(result.buffer)
-            < sort_key(self.results.keys()[-1])  # type: ignore
-            and any(
-                sort_key(buf) < sort_key(known_buf)
-                for arc, known_buf in self.covering_buffers.items()
-                if arc in branches
-            )
-        ):
-            # We do this the stupid-but-obviously-correct way: add the new buffer to
-            # our tracked corpus, and then run a distillation step.
-            self.results[result.buffer] = result
-            self._database.save(self._fuzz_key, buf)
-            self._loaded_from_database.add(buf)
-            # Clear out any redundant entries
-            seen_branches: Set[Arc] = set()
-            self.covering_buffers = {}
-            for res in list(self.results.values()):
-                covers = res.extra_information.branches - seen_branches
-                seen_branches.update(res.extra_information.branches)
-                if not covers:
-                    del self.results[res.buffer]
-                    self._database.delete(self._fuzz_key, res.buffer)
-                else:
-                    for arc in covers:
-                        self.covering_buffers[arc] = res.buffer
-            # We add newly-discovered branches to the counter later; so here our only
-            # unseen branches should be the newly discovered branches.
-            assert seen_branches - set(self.arc_counts) == branches - set(
-                self.arc_counts
-            )
-            self.json_report = [
-                [
-                    reproduction_decorator(res.buffer),
-                    res.extra_information.call_repr,
-                    res.extra_information.reports,
-                ]
-                for res in self.results.values()
-            ]
-
-        # Either update the arc counts so we can prioritize rarer branches in future,
-        # or save an example with new coverage and reset the counter because we'll
-        # have a different distribution with a new seed pool.
-        if branches.issubset(self.arc_counts):
-            self.arc_counts.update(branches)
-        else:
-            # Reset our seen arc counts.  This is essential because changing our
-            # seed pool alters the probability of seeing each arc in future.
-            # For details see AFL-fast, esp. the markov-chain trick.
-            self.arc_counts = Counter(branches.union(self.arc_counts))
-
-            # Save this buffer as our minimal-known covering example for each new arc.
-            if result.buffer not in self.results:
-                self.results[result.buffer] = result
-            self._database.save(self._fuzz_key, buf)
-            for arc in branches - set(self.covering_buffers):
-                self.covering_buffers[arc] = buf
-
-            # We've just finished making some tricky changes, so this is a good time
-            # to assert that all our invariants have been upheld.
-            self._check_invariants()
-            return True
-
-        return False
-
-    def fetch(self) -> Iterable[bytes]:
-        """Yield all buffers from the database which have not been loaded before.
-
-        For the purposes of this method, a buffer which we saved to the database
-        counts as having been loaded - the idea is to avoid duplicate executions.
-        """
-        saved = sorted(
-            set(self._database.fetch(self._key)) - self._loaded_from_database,
-            key=sort_key,
-            reverse=True,
-        )
-        self._loaded_from_database.update(saved)
-        for idx in (0, -1):
-            if saved:
-                yield saved.pop(idx)
-        seeds = sorted(
-            set(self._database.fetch(self._key + b".fuzz"))
-            - self._loaded_from_database,
-            key=sort_key,
-            reverse=True,
-        )
-        self._loaded_from_database.update(seeds)
-        yield from seeds
-        yield from saved
-        self._check_invariants()
-
-    def distill(self, fn: Callable[[bytes], ConjectureData], random: Random) -> None:
-        """Shrink to a pool of *minimal* covering examples.
-
-        We have a couple of unusual structures here.
-
-        1. We exploit the fact that each successful shrink calls self.add(result)
-           to let us skip a lot of work.  Because any "fully shrunk" example is
-           a local fixpoint of all our reduction passes, there's no point trying
-           to shrink a buffer for arc A if it's already minimal for arc B.
-           (because we'd have updated the best known for A while shrinking for B)
-        2. All of the loops are designed to make some amount of progress, and then
-           try again if they did not reach a fixpoint.  Almost all of the structures
-           we're using can be mutated in the process, so it can get strange.
-        """
-        self._in_distill_phase = True
-        self._check_invariants()
-        minimal_branches = {
-            arc
-            for arc, buf in self.covering_buffers.items()
-            if buf in self.__shrunk_to_buffers
-        }
-        while set(self.covering_buffers) - minimal_branches:
-            # The "largest first" shrinking order is designed to maximise the rate
-            # of incidental progress, where shrinking hard problems stumbles over
-            # smaller starting points for the easy ones.
-            arc_to_shrink = max(
-                set(self.covering_buffers) - minimal_branches,
-                key=lambda a: sort_key(self.covering_buffers[a]),
-            )
-            shrinker = Shrinker(
-                EngineStub(fn, random),
-                self.results[self.covering_buffers[arc_to_shrink]],
-                predicate=lambda d, a=arc_to_shrink: a in d.extra_information.branches,
-                allow_transition=None,
-            )
-            shrinker.shrink()
-            self.__shrunk_to_buffers.add(shrinker.shrink_target.buffer)
-            minimal_branches |= {
-                arc
-                for arc, buf in self.covering_buffers.items()
-                if buf == shrinker.shrink_target.buffer
-            }
-            self._check_invariants()
-        self._in_distill_phase = False
-
-
-class Mutator(abc.ABC):
-    def __init__(self, pool: Pool, random: Random) -> None:
-        self.pool = pool
-        self.random = random
-
-    def _random_bytes(self, n: int) -> bytes:
-        return bytes(self.random.randint(0, 255) for _ in range(n))
-
-    @abc.abstractmethod
-    def generate_buffer(self) -> bytes:
-        """Generate a buffer, usually by choosing and mutating examples from pool."""
-        raise NotImplementedError
-
-
-class BlackBoxMutator(Mutator):
-    def generate_buffer(self) -> bytes:
-        """Return an empty prefix, triggering blackbox random generation.
-
-        This 'null mutator' is sometimes useful because - doing no work - it's very
-        fast, and it provides a good baseline for comparisons.
-        """
-        return b""
-
-
-class CrossOverMutator(Mutator):
-    def _get_weights(self) -> List[float]:
-        # (1 / rarest_arc_count) each item in self.results
-        # This is related to the AFL-fast trick, but doesn't track the transition
-        # probabilities - just node densities in the markov chain.
-        weights = [
-            1 / min(self.pool.arc_counts[arc] for arc in res.extra_information.branches)
-            for res in self.pool.results.values()
-        ]
-        total = sum(weights)
-        return [x / total for x in weights]
-
-    def generate_buffer(self) -> bytes:
-        """Splice together two known valid buffers with some random infill.
-
-        This is a pretty poor mutator, and not structure-aware, but works better than
-        the blackbox one already.
-        """
-        if not self.pool.results:
-            return b""
-        # Choose two previously-seen buffers to form a prefix and postfix,
-        # plus some random bytes in the middle to pad it out a bit.
-        # TODO: exploit the .examples tracking for structured mutation.
-        prefix, postfix = self.random.choices(  # type: ignore
-            self.pool.results.keys(), weights=self._get_weights(), k=2  # type: ignore
-        )
-        # TODO: structure-aware slicing - we want to align the crossover points
-        # with a `start_example()` boundary.  This is tricky to get out of Hypothesis
-        # at the moment though, and we don't have any facilities (beyond luck!)
-        # to line up the postfix boundary correctly.  Requires upstream changes.
-        buffer = (
-            prefix[: self.random.randint(0, len(prefix))]
-            + self._random_bytes(self.random.randint(0, 9))
-            + postfix[: self.random.randint(0, len(postfix))]
-        )
-        assert isinstance(buffer, bytes)
-        return buffer
-
-
-class RadamsaMutator(Mutator):
-    # TODO: based on https://github.com/tsundokul/pyradamsa
-    # I *expect* this to be useful mostly for evaluation, and I'd rather not
-    # have the dependency, but I guess it could surprise me.
-    # (expectation/evaluation is to quantify the advantages of structure-aware
-    # mutation given Hypothesis' designed-for-that IR format)
-    pass
+"""Adaptive fuzzing for property-based tests using Hypothesis."""
+
+import abc
+import enum
+from random import Random
+from typing import (
+    Callable,
+    Counter,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    Type,
+    Union,
+)
+
+from hypothesis import __version__ as hypothesis_version
+from hypothesis.core import encode_failure
+from hypothesis.database import ExampleDatabase
+from hypothesis.internal.conjecture.data import (
+    ConjectureData,
+    ConjectureResult,
+    Overrun,
+    Status,
+)
+from hypothesis.internal.conjecture.shrinker import Shrinker
+from sortedcontainers import SortedDict
+
+from .cov import Arc
+
+
+class HowGenerated(enum.Enum):
+    blackbox = "blackbox"
+    mutation = "mutation"
+    shrinking = "shrinking"
+
+
+def sort_key(buffer: Union[bytes, ConjectureResult]) -> Tuple[int, bytes]:
+    """Sort our buffers in shortlex order.
+
+    See `hypothesis.internal.conjecture.shrinker.sort_key` for details on why we
+    use shortlex order in particular.  This tweaked version is identical except
+    for handling ConjectureResult objects too.
+    """
+    if isinstance(buffer, ConjectureResult):
+        buffer = buffer.buffer
+    return (len(buffer), buffer)
+
+
+def reproduction_decorator(buffer: bytes) -> str:
+    """Return `@reproduce_failure` decorator for the given buffer."""
+    return f"@reproduce_failure({hypothesis_version!r}, {encode_failure(buffer)!r})"
+
+
+class EngineStub:
+    """A knock-off ConjectureEngine, just large enough to run a shrinker."""
+
+    def __init__(
+        self, test_fn: Callable[[bytes], ConjectureData], random: Random
+    ) -> None:
+        self.cached_test_function = test_fn
+        self.random = random
+        self.call_count = 0
+        self.report_debug_info = False
+
+    def debug(self, msg: str) -> None:
+        """Unimplemented stub."""
+
+    def explain_next_call_as(self, msg: str) -> None:
+        """Unimplemented stub."""
+
+    def clear_call_explanation(self) -> None:
+        """Unimplemented stub."""
+
+
+class Pool:
+    """Manage the seed pool for a fuzz target.
+
+    The class tracks the minimal valid example which covers each known arc.
+    """
+
+    def __init__(self, database: ExampleDatabase, key: bytes) -> None:
+        # The database and our database key are the stable identifiers for a corpus.
+        # Everything else is reconstructed each run, and tracked only in memory.
+        self._database = database
+        self._key = key
+
+        # Our sorted pool of covering examples, ready to be sampled from.
+        # TODO: One suggestion to reduce effective pool size/redundancy is to skip
+        #       over earlier inputs whose coverage is a subset of later inputs.
+        self.results: Dict[bytes, ConjectureResult] = SortedDict(sort_key)
+
+        # For each arc, what's the minimal covering example?
+        self.covering_buffers: Dict[Arc, bytes] = {}
+        # How many times have we seen each arc since discovering our latest arc?
+        self.arc_counts: Counter[Arc] = Counter()
+
+        # And various internal attributes and metadata
+        self.interesting_examples: Dict[
+            Tuple[Type[BaseException], str, int], Tuple[ConjectureResult, List[str]]
+        ] = {}
+        self._loaded_from_database: Set[bytes] = set()
+        self.__shrunk_to_buffers: Set[bytes] = set()
+
+        # To show the current state of the pool in the dashboard
+        self.json_report: List[List[str]] = []
+        self._in_distill_phase = False
+
+    def __repr__(self) -> str:
+        rs = {b: r.extra_information.branches for b, r in self.results.items()}
+        return (
+            f"<Pool\n    results={rs}\n    arc_counts={self.arc_counts}\n    "
+            f"covering_buffers={self.covering_buffers}\n>"
+        )
+
+    def _check_invariants(self) -> None:
+        """Check all invariants of the structure."""
+        seen: Set[Arc] = set()
+        for res in self.results.values():
+            # Each result in our ordered buffer covers at least one arc not covered
+            # by any more-minimal result.
+            not_previously_covered = res.extra_information.branches - seen
+            assert not_previously_covered
+            # And our covering_buffers map points back the correct (minimal) buffer
+            for arc in not_previously_covered:
+                assert self.covering_buffers[arc] == res.buffer
+            seen.update(res.extra_information.branches)
+
+        # And the union of those branches is exactly covered by our counters.
+        assert seen == set(self.covering_buffers), seen.symmetric_difference(
+            self.covering_buffers
+        )
+        assert seen == set(self.covering_buffers), seen.symmetric_difference(
+            self.arc_counts
+        )
+
+        # Every covering buffer was either read from the database, or saved to it.
+        assert self._loaded_from_database.issuperset(self.covering_buffers.values())
+
+    @property
+    def _fuzz_key(self) -> bytes:
+        return self._key + b".fuzz"
+
+    def add(self, result: ConjectureResult, source: HowGenerated) -> Optional[bool]:
+        """Update the corpus with the result of running a test.
+
+        Returns None for invalid examples, False if no change, True if changed.
+        """
+        assert result is Overrun or isinstance(result, ConjectureResult), result
+        if result.status < Status.VALID:
+            return None
+
+        # We now know that we have a ConjectureResult representing a valid test
+        # execution, either passing or possibly failing.
+        branches = result.extra_information.branches
+        buf = result.buffer
+
+        # If the example is "interesting", i.e. the test failed, add the buffer to
+        # the database under Hypothesis' default key so it will be reproduced.
+        if result.status == Status.INTERESTING:
+            origin = result.interesting_origin
+            if origin not in self.interesting_examples or sort_key(result) < sort_key(
+                self.interesting_examples[origin]
+            ):
+                self._database.save(self._key, result.buffer)
+                self.interesting_examples[origin] = (
+                    result,
+                    [
+                        result.extra_information.call_repr,
+                        result.extra_information.reports,
+                        reproduction_decorator(result.buffer),
+                        result.extra_information.traceback,
+                    ],
+                )
+                return True
+
+        # If we haven't just discovered new branches and our example is larger than the
+        # current largest minimal example, we can skip the expensive calculation.
+        if (not branches.issubset(self.arc_counts)) or (
+            self.results
+            and sort_key(result.buffer)
+            < sort_key(self.results.keys()[-1])  # type: ignore
+            and any(
+                sort_key(buf) < sort_key(known_buf)
+                for arc, known_buf in self.covering_buffers.items()
+                if arc in branches
+            )
+        ):
+            # We do this the stupid-but-obviously-correct way: add the new buffer to
+            # our tracked corpus, and then run a distillation step.
+            self.results[result.buffer] = result
+            self._database.save(self._fuzz_key, buf)
+            self._loaded_from_database.add(buf)
+            # Clear out any redundant entries
+            seen_branches: Set[Arc] = set()
+            self.covering_buffers = {}
+            for res in list(self.results.values()):
+                covers = res.extra_information.branches - seen_branches
+                seen_branches.update(res.extra_information.branches)
+                if not covers:
+                    del self.results[res.buffer]
+                    self._database.delete(self._fuzz_key, res.buffer)
+                else:
+                    for arc in covers:
+                        self.covering_buffers[arc] = res.buffer
+            # We add newly-discovered branches to the counter later; so here our only
+            # unseen branches should be the newly discovered branches.
+            assert seen_branches - set(self.arc_counts) == branches - set(
+                self.arc_counts
+            )
+            self.json_report = [
+                [
+                    reproduction_decorator(res.buffer),
+                    res.extra_information.call_repr,
+                    res.extra_information.reports,
+                ]
+                for res in self.results.values()
+            ]
+
+        # Either update the arc counts so we can prioritize rarer branches in future,
+        # or save an example with new coverage and reset the counter because we'll
+        # have a different distribution with a new seed pool.
+        if branches.issubset(self.arc_counts):
+            self.arc_counts.update(branches)
+        else:
+            # Reset our seen arc counts.  This is essential because changing our
+            # seed pool alters the probability of seeing each arc in future.
+            # For details see AFL-fast, esp. the markov-chain trick.
+            self.arc_counts = Counter(branches.union(self.arc_counts))
+
+            # Save this buffer as our minimal-known covering example for each new arc.
+            if result.buffer not in self.results:
+                self.results[result.buffer] = result
+            self._database.save(self._fuzz_key, buf)
+            for arc in branches - set(self.covering_buffers):
+                self.covering_buffers[arc] = buf
+
+            # We've just finished making some tricky changes, so this is a good time
+            # to assert that all our invariants have been upheld.
+            self._check_invariants()
+            return True
+
+        return False
+
+    def fetch(self) -> Iterable[bytes]:
+        """Yield all buffers from the database which have not been loaded before.
+
+        For the purposes of this method, a buffer which we saved to the database
+        counts as having been loaded - the idea is to avoid duplicate executions.
+        """
+        saved = sorted(
+            set(self._database.fetch(self._key)) - self._loaded_from_database,
+            key=sort_key,
+            reverse=True,
+        )
+        self._loaded_from_database.update(saved)
+        for idx in (0, -1):
+            if saved:
+                yield saved.pop(idx)
+        seeds = sorted(
+            set(self._database.fetch(self._key + b".fuzz"))
+            - self._loaded_from_database,
+            key=sort_key,
+            reverse=True,
+        )
+        self._loaded_from_database.update(seeds)
+        yield from seeds
+        yield from saved
+        self._check_invariants()
+
+    def distill(self, fn: Callable[[bytes], ConjectureData], random: Random) -> None:
+        """Shrink to a pool of *minimal* covering examples.
+
+        We have a couple of unusual structures here.
+
+        1. We exploit the fact that each successful shrink calls self.add(result)
+           to let us skip a lot of work.  Because any "fully shrunk" example is
+           a local fixpoint of all our reduction passes, there's no point trying
+           to shrink a buffer for arc A if it's already minimal for arc B.
+           (because we'd have updated the best known for A while shrinking for B)
+        2. All of the loops are designed to make some amount of progress, and then
+           try again if they did not reach a fixpoint.  Almost all of the structures
+           we're using can be mutated in the process, so it can get strange.
+        """
+        self._in_distill_phase = True
+        self._check_invariants()
+        minimal_branches = {
+            arc
+            for arc, buf in self.covering_buffers.items()
+            if buf in self.__shrunk_to_buffers
+        }
+        while set(self.covering_buffers) - minimal_branches:
+            # The "largest first" shrinking order is designed to maximise the rate
+            # of incidental progress, where shrinking hard problems stumbles over
+            # smaller starting points for the easy ones.
+            arc_to_shrink = max(
+                set(self.covering_buffers) - minimal_branches,
+                key=lambda a: sort_key(self.covering_buffers[a]),
+            )
+            shrinker = Shrinker(
+                EngineStub(fn, random),
+                self.results[self.covering_buffers[arc_to_shrink]],
+                predicate=lambda d, a=arc_to_shrink: a in d.extra_information.branches,
+                allow_transition=None,
+            )
+            shrinker.shrink()
+            self.__shrunk_to_buffers.add(shrinker.shrink_target.buffer)
+            minimal_branches |= {
+                arc
+                for arc, buf in self.covering_buffers.items()
+                if buf == shrinker.shrink_target.buffer
+            }
+            self._check_invariants()
+        self._in_distill_phase = False
+
+
+class Mutator(abc.ABC):
+    def __init__(self, pool: Pool, random: Random) -> None:
+        self.pool = pool
+        self.random = random
+
+    def _random_bytes(self, n: int) -> bytes:
+        return bytes(self.random.randint(0, 255) for _ in range(n))
+
+    @abc.abstractmethod
+    def generate_buffer(self) -> bytes:
+        """Generate a buffer, usually by choosing and mutating examples from pool."""
+        raise NotImplementedError
+
+
+class BlackBoxMutator(Mutator):
+    def generate_buffer(self) -> bytes:
+        """Return an empty prefix, triggering blackbox random generation.
+
+        This 'null mutator' is sometimes useful because - doing no work - it's very
+        fast, and it provides a good baseline for comparisons.
+        """
+        return b""
+
+
+class CrossOverMutator(Mutator):
+    def _get_weights(self) -> List[float]:
+        # (1 / rarest_arc_count) each item in self.results
+        # This is related to the AFL-fast trick, but doesn't track the transition
+        # probabilities - just node densities in the markov chain.
+        weights = [
+            1 / min(self.pool.arc_counts[arc] for arc in res.extra_information.branches)
+            for res in self.pool.results.values()
+        ]
+        total = sum(weights)
+        return [x / total for x in weights]
+
+    def generate_buffer(self) -> bytes:
+        """Splice together two known valid buffers with some random infill.
+
+        This is a pretty poor mutator, and not structure-aware, but works better than
+        the blackbox one already.
+        """
+        if not self.pool.results:
+            return b""
+        # Choose two previously-seen buffers to form a prefix and postfix,
+        # plus some random bytes in the middle to pad it out a bit.
+        # TODO: exploit the .examples tracking for structured mutation.
+        prefix, postfix = self.random.choices(  # type: ignore
+            self.pool.results.keys(), weights=self._get_weights(), k=2  # type: ignore
+        )
+        # TODO: structure-aware slicing - we want to align the crossover points
+        # with a `start_example()` boundary.  This is tricky to get out of Hypothesis
+        # at the moment though, and we don't have any facilities (beyond luck!)
+        # to line up the postfix boundary correctly.  Requires upstream changes.
+        buffer = (
+            prefix[: self.random.randint(0, len(prefix))]
+            + self._random_bytes(self.random.randint(0, 9))
+            + postfix[: self.random.randint(0, len(postfix))]
+        )
+        assert isinstance(buffer, bytes)
+        return buffer
+
+
+class RadamsaMutator(Mutator):
+    # TODO: based on https://github.com/tsundokul/pyradamsa
+    # I *expect* this to be useful mostly for evaluation, and I'd rather not
+    # have the dependency, but I guess it could surprise me.
+    # (expectation/evaluation is to quantify the advantages of structure-aware
+    # mutation given Hypothesis' designed-for-that IR format)
+    pass
```

### Comparing `hypofuzz-22.7.1/src/hypofuzz/cov.py` & `hypofuzz-23.4.1/src/hypofuzz/cov.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-"""Adaptive fuzzing for property-based tests using Hypothesis."""
-
-import sys
-from typing import Any, Dict, FrozenSet, Optional, Set
-
-import attr
-import coverage
-from hypothesis.internal.escalation import is_hypothesis_file
-
-# The upstream notion of an arc is (int, int) with an implicit filename,
-# but HypoFuzz uses an explicit filename as part of the arc.
-_ARC_CACHE: Dict[str, Dict[int, Dict[int, "Arc"]]] = {}
-
-
-@attr.s(frozen=True, slots=True)
-class Arc:
-    fname: str = attr.ib()
-    start_line: int = attr.ib()
-    end_line: int = attr.ib()
-
-    @staticmethod
-    def make(fname: str, start: int, end: int) -> "Arc":
-        try:
-            return _ARC_CACHE[fname][start][end]
-        except KeyError:
-            self = Arc(fname, start, end)
-            _ARC_CACHE.setdefault(fname, {}).setdefault(start, {})[end] = self
-            return self
-
-
-_POSSIBLE_ARCS: Dict[str, FrozenSet[Arc]] = {}
-
-
-def get_coverage_instance(**kwargs: Any) -> coverage.Coverage:
-    # See https://coverage.readthedocs.io/en/latest/api_coverage.html
-    c = coverage.Coverage(
-        data_file=None,  # write nothing to disk
-        cover_pylib=True,  # measure stdlib and package code too
-        branch=True,  # branch coverage
-        config_file=False,  # ignore any config files
-        **kwargs,
-    )
-    c._init()
-    return c
-
-
-def get_possible_branches(cov: coverage.CoverageData, fname: str) -> FrozenSet[Arc]:
-    """Return a list of possible branches for the given file."""
-    try:
-        return _POSSIBLE_ARCS[fname]
-    except KeyError:
-        fr = coverage.python.PythonFileReporter(fname, coverage=cov)
-        _POSSIBLE_ARCS[fname] = frozenset(
-            Arc.make(fname, src, dst) for src, dst in fr.arcs()
-        )
-        return _POSSIBLE_ARCS[fname]
-
-
-class CollectionContext:
-    """Collect coverage data as a context manager.
-
-    The context manager can be reused; each use updates the ``.branches``
-    attribute which will be reset on next use.
-
-    TODO: excluding Hypothesis (and fuzz) files from tracing as well
-            as results would be a small performance upgrade.
-    """
-
-    def __init__(self, cov: coverage.CoverageData = None) -> None:
-        self.cov = cov or get_coverage_instance()
-        self.branches: Set[Arc] = set()
-
-    def __enter__(self) -> None:
-        self.branches = set()
-        self.cov.erase()
-        self.cov.start()
-
-    def __exit__(self, _type: Exception, _value: object, _traceback: object) -> None:
-        # The `stop()` line shows up as uncovered because we are always running under
-        # our *internal* coverage, not *selftest* coverage, here and we don't yet have
-        # a way to pass the data back out without breaking pytest-cov's reporting.
-        self.cov.stop()  # pragma: no cover
-        self.cov.save()
-        for f in self.cov._data.measured_files():
-            if not is_hypothesis_file(f):
-                self.branches.update(
-                    Arc.make(f, src, dst) for src, dst in self.cov._data.branches(f)
-                )
-                # For later: we may want to generalise our notion of an arc to include
-                # coverage contexts, for easy Nezha-style differential fuzzing.
-                # See `CoverageData.contexts_by_lineno()` for this.
-
-        # If coverage was already running, e.g. for HypoFuzz' self-tests,
-        # update that previous instance with the data we just collected.
-        # *except* that this pollutes the report with way to much extra data...
-        # This would also need to handle the not-under-coverage case, for both
-        # correctness and performance.
-        # coverage.Coverage.current()._data.update(self.cov._data)
-
-
-class CustomCollectionContext:
-    """Collect coverage data as a context manager.
-
-    The context manager can be reused; each use updates the ``.branches``
-    attribute which will be reset on next use.
-
-    TODO: excluding Hypothesis (and fuzz) files from tracing as well
-            as results would be a small performance upgrade.
-    """
-
-    last: Optional[tuple]
-
-    def trace(self, frame: Any, event: Any, arg: Any) -> Any:
-        if event == "line":
-            fname = frame.f_code.co_filename
-            if not is_hypothesis_file(fname):
-                this = (fname, frame.f_lineno)
-                self.branches.add((self.last, this))
-                self.last = this
-        return self.trace
-
-    def __enter__(self) -> None:
-        self.last = None
-        self.branches: Set[tuple] = set()
-        self.prev_trace = sys.gettrace()
-        sys.settrace(self.trace)
-
-    def __exit__(self, _type: Exception, _value: object, _traceback: object) -> None:
-        sys.settrace(self.prev_trace)
+"""Adaptive fuzzing for property-based tests using Hypothesis."""
+
+import sys
+from typing import Any, Dict, FrozenSet, Optional, Set
+
+import attr
+import coverage
+from hypothesis.internal.escalation import is_hypothesis_file
+
+# The upstream notion of an arc is (int, int) with an implicit filename,
+# but HypoFuzz uses an explicit filename as part of the arc.
+_ARC_CACHE: Dict[str, Dict[int, Dict[int, "Arc"]]] = {}
+
+
+@attr.s(frozen=True, slots=True)
+class Arc:
+    fname: str = attr.ib()
+    start_line: int = attr.ib()
+    end_line: int = attr.ib()
+
+    @staticmethod
+    def make(fname: str, start: int, end: int) -> "Arc":
+        try:
+            return _ARC_CACHE[fname][start][end]
+        except KeyError:
+            self = Arc(fname, start, end)
+            _ARC_CACHE.setdefault(fname, {}).setdefault(start, {})[end] = self
+            return self
+
+
+_POSSIBLE_ARCS: Dict[str, FrozenSet[Arc]] = {}
+
+
+def get_coverage_instance(**kwargs: Any) -> coverage.Coverage:
+    # See https://coverage.readthedocs.io/en/latest/api_coverage.html
+    c = coverage.Coverage(
+        data_file=None,  # write nothing to disk
+        cover_pylib=True,  # measure stdlib and package code too
+        branch=True,  # branch coverage
+        config_file=False,  # ignore any config files
+        **kwargs,
+    )
+    c._init()
+    return c
+
+
+def get_possible_branches(cov: coverage.CoverageData, fname: str) -> FrozenSet[Arc]:
+    """Return a list of possible branches for the given file."""
+    try:
+        return _POSSIBLE_ARCS[fname]
+    except KeyError:
+        fr = coverage.python.PythonFileReporter(fname, coverage=cov)
+        _POSSIBLE_ARCS[fname] = frozenset(
+            Arc.make(fname, src, dst) for src, dst in fr.arcs()
+        )
+        return _POSSIBLE_ARCS[fname]
+
+
+class CollectionContext:
+    """Collect coverage data as a context manager.
+
+    The context manager can be reused; each use updates the ``.branches``
+    attribute which will be reset on next use.
+
+    TODO: excluding Hypothesis (and fuzz) files from tracing as well
+            as results would be a small performance upgrade.
+    """
+
+    def __init__(self, cov: coverage.CoverageData = None) -> None:
+        self.cov = cov or get_coverage_instance()
+        self.branches: Set[Arc] = set()
+
+    def __enter__(self) -> None:
+        self.branches = set()
+        self.cov.erase()
+        self.cov.start()
+
+    def __exit__(self, _type: Exception, _value: object, _traceback: object) -> None:
+        # The `stop()` line shows up as uncovered because we are always running under
+        # our *internal* coverage, not *selftest* coverage, here and we don't yet have
+        # a way to pass the data back out without breaking pytest-cov's reporting.
+        self.cov.stop()  # pragma: no cover
+        self.cov.save()
+        for f in self.cov._data.measured_files():
+            if not is_hypothesis_file(f):
+                self.branches.update(
+                    Arc.make(f, src, dst) for src, dst in self.cov._data.branches(f)
+                )
+                # For later: we may want to generalise our notion of an arc to include
+                # coverage contexts, for easy Nezha-style differential fuzzing.
+                # See `CoverageData.contexts_by_lineno()` for this.
+
+        # If coverage was already running, e.g. for HypoFuzz' self-tests,
+        # update that previous instance with the data we just collected.
+        # *except* that this pollutes the report with way to much extra data...
+        # This would also need to handle the not-under-coverage case, for both
+        # correctness and performance.
+        # coverage.Coverage.current()._data.update(self.cov._data)
+
+
+class CustomCollectionContext:
+    """Collect coverage data as a context manager.
+
+    The context manager can be reused; each use updates the ``.branches``
+    attribute which will be reset on next use.
+
+    TODO: excluding Hypothesis (and fuzz) files from tracing as well
+            as results would be a small performance upgrade.
+    """
+
+    last: Optional[tuple]
+
+    def trace(self, frame: Any, event: Any, arg: Any) -> Any:
+        if event == "line":
+            fname = frame.f_code.co_filename
+            if not is_hypothesis_file(fname):
+                this = (fname, frame.f_lineno)
+                self.branches.add((self.last, this))
+                self.last = this
+        return self.trace
+
+    def __enter__(self) -> None:
+        self.last = None
+        self.branches: Set[tuple] = set()
+        self.prev_trace = sys.gettrace()
+        sys.settrace(self.trace)
+
+    def __exit__(self, _type: Exception, _value: object, _traceback: object) -> None:
+        sys.settrace(self.prev_trace)
```

### Comparing `hypofuzz-22.7.1/src/hypofuzz/dashboard.py` & `hypofuzz-23.4.1/src/hypofuzz/dashboard.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,269 +1,276 @@
-"""Live web dashboard for a fuzzing run."""
-import datetime
-import os
-from typing import List, Tuple
-
-import black
-import dash
-import flask
-import plotly.express as px
-import plotly.graph_objects as go
-from dash import dcc, html
-from dash.dependencies import Input, Output
-
-DATA_TO_PLOT = [{"nodeid": "", "elapsed_time": 0, "ninputs": 0, "branches": 0}]
-LAST_UPDATE: dict = {}
-
-headings = ["nodeid", "elapsed time", "ninputs", "since new cov", "branches", "note"]
-app = flask.Flask(__name__, static_folder=os.path.abspath("pycrunch-recordings"))
-
-try:
-    import flask_cors
-    from pycrunch_trace.oop.safe_filename import SafeFilename
-except ImportError:
-    SafeFilename = None
-else:
-    flask_cors.CORS(app)
-
-
-@app.route("/", methods=["POST"])  # type: ignore
-def recv_data() -> Tuple[str, int]:
-    data = flask.request.json
-    if not isinstance(data, list):
-        data = [data]
-    for d in data:
-        add_data(d)
-    return "", 200
-
-
-def add_data(d: dict) -> None:
-    if not LAST_UPDATE:
-        del DATA_TO_PLOT[0]
-    DATA_TO_PLOT.append(
-        {k: d[k] for k in ["nodeid", "elapsed_time", "ninputs", "branches"] if k in d}
-    )
-    LAST_UPDATE[d["nodeid"]] = d
-
-
-external_stylesheets = ["https://codepen.io/chriddyp/pen/bWLwgP.css"]
-board = dash.Dash(__name__, server=app, external_stylesheets=external_stylesheets)
-board.layout = html.Div(
-    children=[
-        # represents the URL bar, doesn't render anything
-        dcc.Location(id="url", refresh=False),
-        html.H1(
-            children=[
-                html.A("HypoFuzz", href="https://hypofuzz.com"),
-                " Live Dashboard",
-            ]
-        ),
-        html.Div(id="page-content"),
-        dcc.Interval(id="interval-component", interval=5000),  # time in millis
-    ]
-)
-
-
-def row_for(data: dict, include_link: bool = True, *extra: object) -> html.Tr:
-    parts = []
-    if include_link:
-        parts.append(
-            dcc.Link(data["nodeid"], href="/" + data["nodeid"].replace("/", "_"))
-        )
-    if "elapsed_time" in data:
-        parts.append(str(datetime.timedelta(seconds=int(data["elapsed_time"]))))
-    else:
-        parts.append("")
-    for key in headings[2:]:
-        parts.append(data.get(key, ""))
-    return html.Tr([html.Td(p) for p in parts + [str(e) for e in extra]])
-
-
-def try_format(code: str) -> str:
-    try:
-        return black.format_str(code, mode=black.FileMode())
-    except Exception:
-        return code
-
-
-@board.callback(  # type: ignore
-    Output("page-content", "children"),
-    [Input("url", "pathname")],
-)
-def display_page(pathname: str) -> html.Div:
-    # Main page
-    if pathname == "/" or pathname is None:
-        return html.Div(
-            children=[
-                html.Div("Total branch coverage for each test."),
-                dcc.Graph(id="live-update-graph"),
-                html.Button("Toggle log-xaxis", id="xaxis-state", n_clicks=0),
-                html.Div(html.Table(id="summary-table-rows")),
-                html.Div("Estimated number of inputs to discover new coverage or bugs"),
-                html.Div(html.Table(id="estimators-table-rows")),
-            ]
-        )
-
-    # Target-specific subpages
-    nodeid = pathname[1:]
-    trace = [
-        d
-        for d in DATA_TO_PLOT
-        if d["nodeid"].replace("/", "_") == nodeid  # type: ignore
-    ]
-    fig1 = px.line(
-        trace, x="ninputs", y="branches", line_shape="hv", hover_data=["elapsed_time"]
-    )
-    fig2 = px.line(
-        trace, x="elapsed_time", y="branches", line_shape="hv", hover_data=["ninputs"]
-    )
-    last_update = LAST_UPDATE[trace[-1]["nodeid"]]
-    add: List[str] = []
-    if "failures" in last_update:
-        for failures in last_update["failures"]:
-            failures[0] = try_format(failures[0])
-            add.extend(html.Pre(children=[html.Code(children=[x])]) for x in failures)
-        if SafeFilename:
-            url = f"http://{flask.request.host}/pycrunch-recordings/{SafeFilename(nodeid)}/session.chunked"
-            link = dcc.Link(
-                "Debug failing example online with pytrace",
-                href=f"https://app.pytrace.com/?open={url}",
-            )
-            add.append(html.Pre(children=[link]))
-    return html.Div(
-        children=[
-            dcc.Link("Back to main dashboard", href="/"),
-            html.P(
-                children=[
-                    "Example count by status: ",
-                    str(last_update.get("status_counts", "???")),
-                ]
-            ),
-            html.Table(
-                children=[
-                    html.Tr(
-                        [html.Th(h) for h in headings[1:]] + [html.Th(["seed count"])]
-                    ),
-                    row_for(last_update, False, len(last_update.get("seed_pool", []))),
-                ]
-            ),
-            *add,
-            dcc.Graph(id=f"graph-of-{pathname}-1", figure=fig1),
-            dcc.Graph(id=f"graph-of-{pathname}-2", figure=fig2),
-            html.H3(["Minimal covering examples"]),
-            html.P(
-                [
-                    "Each additional example shown below covers at least one branch "
-                    "not covered by any previous, more-minimal, example."
-                ]
-            ),
-        ]
-        + [
-            html.Pre([html.Code([try_format(row[1]), row[2], "\n"])])
-            for row in last_update.get("seed_pool", [])
-        ]
-    )
-
-
-@board.callback(  # type: ignore
-    Output("live-update-graph", "figure"),
-    [Input("interval-component", "n_intervals"), Input("xaxis-state", "n_clicks")],
-)
-def update_graph_live(n: int, clicks: int) -> object:
-    fig = px.line(
-        DATA_TO_PLOT,
-        x="ninputs",
-        y="branches",
-        color="nodeid",
-        line_shape="hv",
-        hover_data=["elapsed_time"],
-        log_x=bool(clicks % 2),
-    )
-    failing = [
-        (d["ninputs"], d["branches"])
-        for d in LAST_UPDATE.values()
-        if d.get("status_counts", {}).get("INTERESTING", 0)
-    ]
-    if failing:
-        xs, ys = zip(*failing)
-        fig.add_trace(
-            go.Scatter(
-                x=xs,
-                y=ys,
-                mode="text",
-                text="💥",
-                showlegend=False,
-            )
-        )
-    fig.update_layout(
-        height=800,
-        legend_yanchor="top",
-        legend_xanchor="left",
-        legend_y=-0.08,
-        legend_x=0,
-    )
-    # Setting this to a constant prevents data updates clobbering zoom / selections
-    fig.layout.uirevision = "this key never changes"
-    return fig
-
-
-@board.callback(  # type: ignore
-    Output("summary-table-rows", "children"),
-    [Input("interval-component", "n_intervals")],
-)
-def update_table_live(n: int) -> object:
-    return [html.Tr([html.Th(h) for h in headings])] + [
-        row_for(data) for name, data in sorted(LAST_UPDATE.items()) if name
-    ]
-
-
-def estimators(data: dict) -> dict:
-    since_new_cov = data["since new cov"]
-    ninputs = data["ninputs"]
-    loaded_from_db = data["loaded_from_db"]
-    return {
-        "branch_lower": 1 / (since_new_cov + 1),
-        "branch_upper": 1 / (max(ninputs - loaded_from_db, 0) + 1),
-        "bug": 1 if data.get("failures") else 1 / max(ninputs + 1, loaded_from_db),
-    }
-
-
-@board.callback(  # type: ignore
-    Output("estimators-table-rows", "children"),
-    [Input("interval-component", "n_intervals")],
-)
-def update_estimators_table(n: int) -> object:
-    contents = [html.Col(), html.Colgroup(span=1)] + [
-        html.Colgroup(span=2) for _ in range(2)
-    ]
-    colnames = ["nodeid", "branch-lower", "branch-upper", "bug"]
-    contents = [html.Tr([html.Th(h) for h in colnames])]
-
-    for _, d in sorted(LAST_UPDATE.items()):
-        try:
-            est = estimators(d)
-        except KeyError:
-            continue
-        row = [
-            d["nodeid"],
-            int(1 / est["branch_lower"]),
-            int(1 / est["branch_upper"]),
-            int(1 / est["bug"]),
-        ]
-        contents.append(html.Tr([html.Td(x) for x in row]))
-    return contents
-
-
-@app.route("/pycrunch-recordings/<path:name>")  # type: ignore
-def download_file(name: str) -> flask.Response:
-    return flask.send_from_directory(
-        directory="pycrunch-recordings",
-        filename=name,
-        mimetype="application/octet-stream",
-    )
-
-
-def start_dashboard_process(
-    port: int, *, host: str = "localhost", debug: bool = False
-) -> None:
-    print(f"\n\tNow serving dashboard at  http://{host}:{port}/\n")  # noqa
-    app.run(host=host, port=port, debug=debug)
+"""Live web dashboard for a fuzzing run."""
+import datetime
+import os
+from typing import List, Tuple
+
+import black
+import dash
+import flask
+import plotly.express as px
+import plotly.graph_objects as go
+from dash import dcc, html
+from dash.dependencies import Input, Output
+
+DATA_TO_PLOT = [{"nodeid": "", "elapsed_time": 0, "ninputs": 0, "branches": 0}]
+LAST_UPDATE: dict = {}
+
+headings = ["nodeid", "elapsed time", "ninputs", "since new cov", "branches", "note"]
+app = flask.Flask(__name__, static_folder=os.path.abspath("pycrunch-recordings"))
+
+try:
+    import flask_cors
+    from pycrunch_trace.oop.safe_filename import SafeFilename
+except ImportError:
+    SafeFilename = None
+else:
+    flask_cors.CORS(app)
+
+
+@app.route("/", methods=["POST"])  # type: ignore
+def recv_data() -> Tuple[str, int]:
+    data = flask.request.json
+    if not isinstance(data, list):
+        data = [data]
+    for d in data:
+        add_data(d)
+    return "", 200
+
+
+def add_data(d: dict) -> None:
+    if not LAST_UPDATE:
+        del DATA_TO_PLOT[0]
+    DATA_TO_PLOT.append(
+        {k: d[k] for k in ["nodeid", "elapsed_time", "ninputs", "branches"]}
+    )
+    LAST_UPDATE[d["nodeid"]] = d
+
+
+external_stylesheets = ["https://codepen.io/chriddyp/pen/bWLwgP.css"]
+board = dash.Dash(__name__, server=app, external_stylesheets=external_stylesheets)
+board.layout = html.Div(
+    children=[
+        # represents the URL bar, doesn't render anything
+        dcc.Location(id="url", refresh=False),
+        html.H1(
+            children=[
+                html.A("HypoFuzz", href="https://hypofuzz.com"),
+                " Live Dashboard",
+            ]
+        ),
+        html.Div(id="page-content"),
+        dcc.Interval(id="interval-component", interval=5000),  # time in millis
+    ]
+)
+
+
+def row_for(data: dict, include_link: bool = True, *extra: object) -> html.Tr:
+    parts = []
+    if include_link:
+        parts.append(
+            dcc.Link(data["nodeid"], href="/" + data["nodeid"].replace("/", "_"))
+        )
+    if "elapsed_time" in data:
+        parts.append(str(datetime.timedelta(seconds=int(data["elapsed_time"]))))
+    else:
+        parts.append("")
+    for key in headings[2:]:
+        parts.append(data.get(key, ""))
+    return html.Tr([html.Td(p) for p in parts + [str(e) for e in extra]])
+
+
+def try_format(code: str) -> str:
+    try:
+        return black.format_str(code, mode=black.FileMode())
+    except Exception:
+        return code
+
+
+@board.callback(  # type: ignore
+    Output("page-content", "children"),
+    [Input("url", "pathname")],
+)
+def display_page(pathname: str) -> html.Div:
+    # Main page
+    if pathname == "/" or pathname is None:
+        return html.Div(
+            children=[
+                html.Div("Total branch coverage for each test."),
+                dcc.Graph(id="live-update-graph"),
+                html.Button("Toggle log-xaxis", id="xaxis-state", n_clicks=0),
+                html.Div(html.Table(id="summary-table-rows")),
+                html.Div("Estimated number of inputs to discover new coverage or bugs"),
+                html.Div(html.Table(id="estimators-table-rows")),
+            ]
+        )
+
+    # Target-specific subpages
+    nodeid = pathname[1:]
+    trace = [
+        d
+        for d in DATA_TO_PLOT
+        if d["nodeid"].replace("/", "_") == nodeid  # type: ignore
+    ]
+    fig1 = px.line(
+        trace, x="ninputs", y="branches", line_shape="hv", hover_data=["elapsed_time"]
+    )
+    fig2 = px.line(
+        trace, x="elapsed_time", y="branches", line_shape="hv", hover_data=["ninputs"]
+    )
+    last_update = LAST_UPDATE[trace[-1]["nodeid"]]
+    add: List[str] = []
+    if "failures" in last_update:
+        for failures in last_update["failures"]:
+            failures[0] = try_format(failures[0])
+            add.extend(html.Pre(children=[html.Code(children=[x])]) for x in failures)
+        if SafeFilename:
+            url = f"http://{flask.request.host}/pycrunch-recordings/{SafeFilename(nodeid)}/session.chunked"
+            link = dcc.Link(
+                "Debug failing example online with pytrace",
+                href=f"https://app.pytrace.com/?open={url}",
+            )
+            add.append(html.Pre(children=[link]))
+    return html.Div(
+        children=[
+            dcc.Link("Back to main dashboard", href="/"),
+            html.P(
+                children=[
+                    "Example count by status: ",
+                    str(last_update.get("status_counts", "???")),
+                ]
+            ),
+            html.Table(
+                children=[
+                    html.Tr(
+                        [html.Th(h) for h in headings[1:]] + [html.Th(["seed count"])]
+                    ),
+                    row_for(last_update, False, len(last_update.get("seed_pool", []))),
+                ]
+            ),
+            *add,
+            dcc.Graph(id=f"graph-of-{pathname}-1", figure=fig1),
+            dcc.Graph(id=f"graph-of-{pathname}-2", figure=fig2),
+            html.H3(["Minimal covering examples"]),
+            html.P(
+                [
+                    "Each additional example shown below covers at least one branch "
+                    "not covered by any previous, more-minimal, example."
+                ]
+            ),
+        ]
+        + [
+            html.Pre([html.Code([try_format(row[1]), row[2], "\n"])])
+            for row in last_update.get("seed_pool", [])
+        ]
+    )
+
+
+FIRST_FAILED_AT = {}
+
+
+@board.callback(  # type: ignore
+    Output("live-update-graph", "figure"),
+    [Input("interval-component", "n_intervals"), Input("xaxis-state", "n_clicks")],
+)
+def update_graph_live(n: int, clicks: int) -> object:
+    fig = px.line(
+        DATA_TO_PLOT,
+        x="ninputs",
+        y="branches",
+        color="nodeid",
+        line_shape="hv",
+        hover_data=["elapsed_time"],
+        log_x=bool(clicks % 2),
+    )
+    failing = {
+        d["nodeid"]: (d["ninputs"], d["branches"])
+        for d in LAST_UPDATE.values()
+        if d.get("status_counts", {}).get("INTERESTING", 0)
+    }
+    for k, v in failing.items():
+        if k not in FIRST_FAILED_AT:
+            FIRST_FAILED_AT[k] = v
+    for series, symbol in [(failing, "🔍"), (FIRST_FAILED_AT, "💥")]:
+        if series:
+            xs, ys = zip(*series.values())
+            fig.add_trace(
+                go.Scatter(
+                    x=xs,
+                    y=ys,
+                    mode="text",
+                    text=symbol,
+                    showlegend=False,
+                )
+            )
+    fig.update_layout(
+        height=800,
+        legend_yanchor="top",
+        legend_xanchor="left",
+        legend_y=-0.08,
+        legend_x=0,
+    )
+    # Setting this to a constant prevents data updates clobbering zoom / selections
+    fig.layout.uirevision = "this key never changes"
+    return fig
+
+
+@board.callback(  # type: ignore
+    Output("summary-table-rows", "children"),
+    [Input("interval-component", "n_intervals")],
+)
+def update_table_live(n: int) -> object:
+    return [html.Tr([html.Th(h) for h in headings])] + [
+        row_for(data) for name, data in sorted(LAST_UPDATE.items()) if name
+    ]
+
+
+def estimators(data: dict) -> dict:
+    since_new_cov = data["since new cov"]
+    ninputs = data["ninputs"]
+    loaded_from_db = data["loaded_from_db"]
+    return {
+        "branch_lower": 1 / (since_new_cov + 1),
+        "branch_upper": 1 / (max(ninputs - loaded_from_db, 0) + 1),
+        "bug": 1 if data.get("failures") else 1 / max(ninputs + 1, loaded_from_db),
+    }
+
+
+@board.callback(  # type: ignore
+    Output("estimators-table-rows", "children"),
+    [Input("interval-component", "n_intervals")],
+)
+def update_estimators_table(n: int) -> object:
+    contents = [html.Col(), html.Colgroup(span=1)] + [
+        html.Colgroup(span=2) for _ in range(2)
+    ]
+    colnames = ["nodeid", "branch-lower", "branch-upper", "bug"]
+    contents = [html.Tr([html.Th(h) for h in colnames])]
+
+    for _, d in sorted(LAST_UPDATE.items()):
+        try:
+            est = estimators(d)
+        except KeyError:
+            continue
+        row = [
+            d["nodeid"],
+            int(1 / est["branch_lower"]),
+            int(1 / est["branch_upper"]),
+            int(1 / est["bug"]),
+        ]
+        contents.append(html.Tr([html.Td(x) for x in row]))
+    return contents
+
+
+@app.route("/pycrunch-recordings/<path:name>")  # type: ignore
+def download_file(name: str) -> flask.Response:
+    return flask.send_from_directory(
+        directory="pycrunch-recordings",
+        filename=name,
+        mimetype="application/octet-stream",
+    )
+
+
+def start_dashboard_process(
+    port: int, *, host: str = "localhost", debug: bool = False
+) -> None:
+    print(f"\n\tNow serving dashboard at  http://{host}:{port}/\n")  # noqa
+    app.run(host=host, port=port, debug=debug)
```

### Comparing `hypofuzz-22.7.1/src/hypofuzz/debugger.py` & `hypofuzz-23.4.1/src/hypofuzz/debugger.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-"""Adaptive fuzzing for property-based tests using Hypothesis."""
-
-import sys
-from contextlib import contextmanager
-from functools import lru_cache
-from typing import Callable, Iterator
-
-import _pytest
-import pytest
-from hypothesis.internal.escalation import belongs_to, is_hypothesis_file
-from pycrunch_trace.client.api import Trace
-from pycrunch_trace.filters import CustomFileFilter
-from pycrunch_trace.oop.safe_filename import SafeFilename
-
-is_pytest_file = belongs_to(pytest)
-is__pytest_file = belongs_to(_pytest)
-is_pycrunch_file = belongs_to(sys.modules["pycrunch_trace"])
-
-
-@lru_cache()
-def is_hypofuzz_file() -> Callable:
-    # Layer of indirection to avoid import cycles
-    import hypofuzz
-
-    return belongs_to(hypofuzz)  # type: ignore
-
-
-class HypofuzzFileFilter(CustomFileFilter):
-    def should_trace(self, filename: str) -> bool:
-        return (
-            super().should_trace(filename)
-            and not filename.endswith(("contextlib.py", "reprlib.py"))
-            and not is_hypothesis_file(filename)
-            and not is_pytest_file(filename)
-            and not is__pytest_file(filename)
-            and not is_pycrunch_file(filename)
-            and not is_hypofuzz_file()(filename)
-        )
-
-
-# This is kinda evil monkeypatching, but on the other hand it saves the user
-# a lot of trouble writing config files for pytrace... so it's fine.
-sys.modules[Trace.__module__].CustomFileFilter = HypofuzzFileFilter  # type: ignore
-
-
-@contextmanager
-def record_pytrace(nodeid: str) -> Iterator:
-    rr = Trace()
-    try:
-        rr.start(session_name=str(SafeFilename(nodeid)))
-        yield
-    finally:
-        rr.stop()
+"""Adaptive fuzzing for property-based tests using Hypothesis."""
+
+import sys
+from contextlib import contextmanager
+from functools import lru_cache
+from typing import Callable, Iterator
+
+import _pytest
+import pytest
+from hypothesis.internal.escalation import belongs_to, is_hypothesis_file
+from pycrunch_trace.client.api import Trace
+from pycrunch_trace.filters import CustomFileFilter
+from pycrunch_trace.oop.safe_filename import SafeFilename
+
+is_pytest_file = belongs_to(pytest)
+is__pytest_file = belongs_to(_pytest)
+is_pycrunch_file = belongs_to(sys.modules["pycrunch_trace"])
+
+
+@lru_cache()
+def is_hypofuzz_file() -> Callable:
+    # Layer of indirection to avoid import cycles
+    import hypofuzz
+
+    return belongs_to(hypofuzz)  # type: ignore
+
+
+class HypofuzzFileFilter(CustomFileFilter):
+    def should_trace(self, filename: str) -> bool:
+        return (
+            super().should_trace(filename)
+            and not filename.endswith(("contextlib.py", "reprlib.py"))
+            and not is_hypothesis_file(filename)
+            and not is_pytest_file(filename)
+            and not is__pytest_file(filename)
+            and not is_pycrunch_file(filename)
+            and not is_hypofuzz_file()(filename)
+        )
+
+
+# This is kinda evil monkeypatching, but on the other hand it saves the user
+# a lot of trouble writing config files for pytrace... so it's fine.
+sys.modules[Trace.__module__].CustomFileFilter = HypofuzzFileFilter  # type: ignore
+
+
+@contextmanager
+def record_pytrace(nodeid: str) -> Iterator:
+    rr = Trace()
+    try:
+        rr.start(session_name=str(SafeFilename(nodeid)))
+        yield
+    finally:
+        rr.stop()
```

### Comparing `hypofuzz-22.7.1/src/hypofuzz/entrypoint.py` & `hypofuzz-23.4.1/src/hypofuzz/entrypoint.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,93 +1,99 @@
-"""CLI and Python API for the fuzzer."""
-
-from multiprocessing import Process
-from typing import NoReturn, Tuple
-
-import click
-import hypothesis.extra.cli
-import psutil
-
-
-@hypothesis.extra.cli.main.command()  # type: ignore
-@click.option(
-    "-n",
-    "--numprocesses",
-    type=click.IntRange(1, None),
-    metavar="NUM",
-    # we match the -n auto behaviour of pytest-xdist by default
-    default=psutil.cpu_count(logical=False) or psutil.cpu_count() or 1,
-    help="default: all available cores",
-)
-@click.option(
-    "--dashboard/--no-dashboard",
-    default=True,
-    help="serve / don't serve a live dashboard page",
-)
-@click.option(
-    "--port",
-    type=click.IntRange(1, 65535),
-    default=9999,
-    metavar="PORT",
-    help="Optional port for the dashboard (if any)",
-)
-@click.option(
-    "--unsafe",
-    is_flag=True,
-    help="Allow concurrent execution of each test (dashboard may report wrong results)",
-)
-@click.argument(
-    "pytest_args",
-    nargs=-1,
-    metavar="[-- PYTEST_ARGS]",
-)
-def fuzz(
-    numprocesses: int,
-    dashboard: bool,
-    port: int,
-    unsafe: bool,
-    pytest_args: Tuple[str, ...],
-) -> NoReturn:
-    """[hypofuzz] runs tests with an adaptive coverage-guided fuzzer.
-
-    Unrecognised arguments are passed through to `pytest` to select the tests
-    to run, with the additional constraint that only tests using Hypothesis
-    but not any pytest fixtures can be fuzzed.
-
-    This process will run forever unless stopped with e.g. ctrl-C.
-    """
-    # Before doing anything with our arguments, we'll check that none
-    # of HypoFuzz's arguments will be passed on to pytest instead.
-    misplaced: set = set(pytest_args) & set().union(*(p.opts for p in fuzz.params))
-    if misplaced:
-        plural = "s" * (len(misplaced) > 1)
-        names = ", ".join(map(repr, misplaced))
-        raise click.UsageError(
-            f"fuzzer option{plural} {names} would be passed to pytest instead"
-        )
-
-    from .interface import _fuzz_several, _get_hypothesis_tests_with_pytest
-
-    # With our arguments validated, it's time to actually do the work.
-    tests = _get_hypothesis_tests_with_pytest(pytest_args)
-    if not tests:
-        raise click.UsageError("No property-based tests were collected")
-    if numprocesses > len(tests) and not unsafe:
-        numprocesses = len(tests)
-
-    testnames = "\n    ".join(t.nodeid for t in tests)
-    print(f"using up to {numprocesses} processes to fuzz:\n    {testnames}\n")  # noqa
-
-    if dashboard:
-        from .dashboard import start_dashboard_process
-
-        Process(target=start_dashboard_process, kwargs={"port": port}).start()
-
-    for i in range(numprocesses):
-        nodes = {t.nodeid for t in (tests if unsafe else tests[i::numprocesses])}
-        p = Process(
-            target=_fuzz_several,
-            kwargs={"pytest_args": pytest_args, "nodeids": nodes, "port": port},
-        )
-        p.start()
-    p.join()
-    raise NotImplementedError("unreachable")
+"""CLI and Python API for the fuzzer."""
+
+import sys
+from multiprocessing import Process
+from typing import NoReturn, Tuple
+
+import click
+import hypothesis.extra.cli
+import psutil
+
+
+@hypothesis.extra.cli.main.command()  # type: ignore
+@click.option(
+    "-n",
+    "--numprocesses",
+    type=click.IntRange(1, None),
+    metavar="NUM",
+    # we match the -n auto behaviour of pytest-xdist by default
+    default=psutil.cpu_count(logical=False) or psutil.cpu_count() or 1,
+    help="default: all available cores",
+)
+@click.option(
+    "--dashboard/--no-dashboard",
+    default=True,
+    help="serve / don't serve a live dashboard page",
+)
+@click.option(
+    "--port",
+    type=click.IntRange(1, 65535),
+    default=9999,
+    metavar="PORT",
+    help="Optional port for the dashboard (if any)",
+)
+@click.option(
+    "--unsafe",
+    is_flag=True,
+    help="Allow concurrent execution of each test (dashboard may report wrong results)",
+)
+@click.argument(
+    "pytest_args",
+    nargs=-1,
+    metavar="[-- PYTEST_ARGS]",
+)
+def fuzz(
+    numprocesses: int,
+    dashboard: bool,
+    port: int,
+    unsafe: bool,
+    pytest_args: Tuple[str, ...],
+) -> NoReturn:
+    """[hypofuzz] runs tests with an adaptive coverage-guided fuzzer.
+
+    Unrecognised arguments are passed through to `pytest` to select the tests
+    to run, with the additional constraint that only tests using Hypothesis
+    but not any pytest fixtures can be fuzzed.
+
+    This process will run forever unless stopped with e.g. ctrl-C.
+    """
+    # Before doing anything with our arguments, we'll check that none
+    # of HypoFuzz's arguments will be passed on to pytest instead.
+    misplaced: set = set(pytest_args) & set().union(*(p.opts for p in fuzz.params))
+    if misplaced:
+        plural = "s" * (len(misplaced) > 1)
+        names = ", ".join(map(repr, misplaced))
+        raise click.UsageError(
+            f"fuzzer option{plural} {names} would be passed to pytest instead"
+        )
+
+    from .interface import _fuzz_several, _get_hypothesis_tests_with_pytest
+
+    # With our arguments validated, it's time to actually do the work.
+    tests = _get_hypothesis_tests_with_pytest(pytest_args)
+    if not tests:
+        raise click.UsageError("No property-based tests were collected")
+    if numprocesses > len(tests) and not unsafe:
+        numprocesses = len(tests)
+
+    testnames = "\n    ".join(t.nodeid for t in tests)
+    print(f"using up to {numprocesses} processes to fuzz:\n    {testnames}\n")  # noqa
+
+    if dashboard:
+        from .dashboard import start_dashboard_process
+
+        Process(target=start_dashboard_process, kwargs={"port": port}).start()
+
+    processes = []
+    for i in range(numprocesses):
+        nodes = {t.nodeid for t in (tests if unsafe else tests[i::numprocesses])}
+        p = Process(
+            target=_fuzz_several,
+            kwargs={"pytest_args": pytest_args, "nodeids": nodes, "port": port},
+        )
+        p.start()
+        processes.append(p)
+    for p in processes:
+        p.join()
+    print("Found a failing input for every test!", file=sys.stderr)  # noqa: T201
+    sys.exit(1)
+    raise NotImplementedError("unreachable")
```

### Comparing `hypofuzz-22.7.1/src/hypofuzz/hy.py` & `hypofuzz-23.4.1/src/hypofuzz/hy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,374 +1,390 @@
-"""Adaptive fuzzing for property-based tests using Hypothesis."""
-
-import contextlib
-import itertools
-import sys
-import time
-import traceback
-from random import Random
-from typing import Any, Callable, Dict, Generator, List, NoReturn, Union
-
-from hypothesis import settings, strategies as st
-from hypothesis.core import (
-    BuildContext,
-    deterministic_PRNG,
-    failure_exceptions_to_catch,
-    get_trimmed_traceback,
-    process_arguments_to_given,
-)
-from hypothesis.database import ExampleDatabase
-from hypothesis.errors import StopTest, UnsatisfiedAssumption
-from hypothesis.internal.conjecture.data import ConjectureData, Status
-from hypothesis.internal.conjecture.engine import BUFFER_SIZE
-from hypothesis.internal.conjecture.junkdrawer import stack_depth_of_caller
-from hypothesis.internal.conjecture.shrinker import Shrinker
-from hypothesis.internal.reflection import function_digest, get_signature
-from hypothesis.reporting import with_reporter
-from sortedcontainers import SortedKeyList
-
-from .corpus import BlackBoxMutator, CrossOverMutator, EngineStub, HowGenerated, Pool
-from .cov import CustomCollectionContext
-
-try:
-    from .debugger import record_pytrace
-except ImportError:
-    record_pytrace = None  # type: ignore
-
-Report = Dict[str, Union[int, float, str, list, Dict[str, int]]]
-
-UNDELIVERED_REPORTS: List[Report] = []
-
-
-@contextlib.contextmanager
-def constant_stack_depth() -> Generator[None, None, None]:
-    # TODO: consider extracting this upstream so we can just import it.
-    recursion_limit = sys.getrecursionlimit()
-    depth = stack_depth_of_caller()
-    # Because we add to the recursion limit, to be good citizens we also add
-    # a check for unbounded recursion.  The default limit is 1000, so this can
-    # only ever trigger if something really strange is happening and it's hard
-    # to imagine an intentionally-deeply-recursive use of this code.
-    assert depth <= 1000, (
-        f"Hypothesis would usually add {recursion_limit} to the stack depth of "
-        "{depth} here, but we are already much deeper than expected.  Aborting "
-        "now, to avoid extending the stack limit in an infinite loop..."
-    )
-    try:
-        sys.setrecursionlimit(depth + recursion_limit)
-        yield
-    finally:
-        sys.setrecursionlimit(recursion_limit)
-
-
-class FuzzProcess:
-    """Maintain all the state associated with fuzzing a single target.
-
-    This includes:
-
-        - the coverage map and associated inputs
-        - references to Hypothesis' database for this test (for failure replay)
-        - a "run one" method, and an estimate of the value of running one input
-        - checkpointing tools so we can crash and restart without losing progess
-
-    etc.  The fuzz controller will then operate on a collection of these objects.
-    """
-
-    @classmethod
-    def from_hypothesis_test(
-        cls,
-        wrapped_test: Any,
-        *,
-        nodeid: str = None,
-        extra_kw: Dict[str, object] = None,
-    ) -> "FuzzProcess":
-        """Return a FuzzProcess for an @given-decorated test function."""
-        _, _, _, search_strategy = process_arguments_to_given(
-            wrapped_test,
-            arguments=(),
-            kwargs=extra_kw or {},
-            given_kwargs=wrapped_test.hypothesis._given_kwargs,
-            params=get_signature(wrapped_test).parameters,
-        )
-        return cls(
-            test_fn=wrapped_test.hypothesis.inner_test,
-            strategy=search_strategy,
-            nodeid=nodeid,
-            database_key=function_digest(wrapped_test),
-            hypothesis_database=wrapped_test._hypothesis_internal_use_settings.database
-            or settings.default.database,
-        )
-
-    def __init__(
-        self,
-        test_fn: Callable,
-        strategy: st.SearchStrategy,
-        *,
-        random_seed: int = 0,
-        nodeid: str = None,
-        database_key: bytes,
-        hypothesis_database: ExampleDatabase,
-    ) -> None:
-        """Construct a FuzzProcess from specific arguments."""
-        # The actual fuzzer implementation
-        self.random = Random(random_seed)
-        self.__test_fn = test_fn
-        self.__strategy = strategy
-        self.nodeid = nodeid or test_fn.__qualname__
-
-        # The seed pool is responsible for managing all seed state, including saving
-        # novel seeds to the database.  This includes tracking how often each branch
-        # has been hit, minimal covering examples, and so on.
-        self.pool = Pool(hypothesis_database, database_key)
-        self._mutator_blackbox = BlackBoxMutator(self.pool, self.random)
-        self._mutator_crossover = CrossOverMutator(self.pool, self.random)
-
-        # Set up the basic data that we'll track while fuzzing
-        self.ninputs = 0
-        self.elapsed_time = 0.0
-        self.since_new_cov = 0
-        self.status_counts = {s.name: 0 for s in Status}
-        self.shrinking = False
-        # Any new examples from the database will be added to this replay buffer
-        self._replay_buffer: List[bytes] = []
-        # After replay, we stay in blackbox mode for a while, until we've generated
-        # 1000 consecutive examples without new coverage, and then switch to mutation.
-        self._early_blackbox_mode = True
-
-        # We batch updates, since frequent HTTP posts are slow
-        self._last_post_time = self.elapsed_time
-
-    def startup(self) -> None:
-        """Set up initial state and prepare to replay the saved behaviour."""
-        assert self.ninputs == 0, "already started this FuzzProcess"
-        # Report that we've started this fuzz target, and run zero examples so far
-        self._report_change(self._json_description)
-        # Next, restore progress made in previous runs by loading our saved examples.
-        # This is meant to be the minimal set of inputs that exhibits all distinct
-        # behaviours we've observed to date.  Replaying takes longer than restoring
-        # our data structures directly, but copes much better with changed behaviour.
-        self._replay_buffer.extend(self.pool.fetch())
-        self._replay_buffer.append(b"\x00" * BUFFER_SIZE)
-
-    def generate_prefix(self) -> bytes:
-        """Generate a test prefix by mutating previous examples.
-
-        This is going to be the method to override when experimenting with
-        alternative fuzzing techniques.
-
-            - for unguided fuzzing, return an empty b'' and the random postfix
-              generation in ConjectureData will do the rest.
-            - for coverage-guided fuzzing, mutate or splice together known inputs.
-
-        This version is terrible, but any coverage guidance at all is enough to help...
-        """
-        # Start by replaying any previous failures which we've retrieved from the
-        # database.  This is useful to recover state at startup, or to share
-        # progress made in other processes.
-        if self._replay_buffer:
-            return self._replay_buffer.pop()
-
-        # TODO: currently hard-coding a particular mutator; we want to do MOpt-style
-        # adaptive weighting of all the different mutators we could use.
-        # For now though, we'll just use a hardcoded swapover point
-        if self._early_blackbox_mode or self.random.random() < 0.05:
-            return self._mutator_blackbox.generate_buffer()
-        return self._mutator_crossover.generate_buffer()
-
-    def run_one(self) -> None:
-        """Run a single input through the fuzz target, or maybe more.
-
-        The "more" part is in cases where we discover new coverage, and shrink
-        to the minimal covering example.
-        """
-        # If we've been stable for a little while, try loading new examples from the
-        # database.  We do this unconditionally because even if this fuzzer doesn't
-        # know of other concurrent runs, there may be e.g. a test process sharing the
-        # database.  We do make it infrequent to manage the overhead though.
-        if self.ninputs % 1000 == 0 and self.since_new_cov > 1000:
-            self._replay_buffer.extend(self.pool.fetch())
-
-        # seen_count = len(self.pool.arc_counts)
-
-        # Run the input
-        result = self._run_test_on(self.generate_prefix())
-
-        if result.status is Status.INTERESTING:
-            # Shrink to our minimal failing example, since we'll stop after this.
-            self.shrinking = True
-            shrinker = Shrinker(
-                EngineStub(self._run_test_on, self.random),
-                result,
-                predicate=lambda d: d.status is Status.INTERESTING,
-                allow_transition=None,
-            )
-            shrinker.shrink()
-            self.shrinking = False
-            if record_pytrace:
-                # Replay minimal example under our time-travelling debug tracer
-                self._run_test_on(
-                    shrinker.shrink_target.buffer,
-                    collector=record_pytrace(self.nodeid),
-                )
-            UNDELIVERED_REPORTS.append(self._json_description)
-            self._report_change(UNDELIVERED_REPORTS)
-            del UNDELIVERED_REPORTS[:]
-
-        # Consider switching out of blackbox mode.
-        if self.since_new_cov >= 1000 and not self._replay_buffer:
-            self._early_blackbox_mode = False
-
-        # NOTE: this distillation logic works fine, it's just discovering new coverage
-        # much more slowly than jumping directly to mutational mode.
-        # if len(self.pool.arc_counts) > seen_count and not self._early_blackbox_mode:
-        #     self.pool.distill(self._run_test_on, self.random)
-
-    def _run_test_on(
-        self,
-        buffer: bytes,
-        *,
-        source: HowGenerated = HowGenerated.shrinking,
-        collector: contextlib.AbstractContextManager = None,
-    ) -> ConjectureData:
-        """Run the test_fn on a given buffer of bytes, in a way a Shrinker can handle.
-
-        In normal operation, it's called via run_one (above), but we might also
-        delegate to the shrinker to find minimal covering examples.
-        """
-        start = time.perf_counter()
-        self.ninputs += 1
-        collector = collector or CustomCollectionContext()  # type: ignore
-        assert collector is not None
-        reports: List[str] = []
-        argstrings: List[str] = []
-        data = ConjectureData(max_length=BUFFER_SIZE, prefix=buffer, random=self.random)
-        try:
-            with deterministic_PRNG(), BuildContext(
-                data, is_final=True
-            ), constant_stack_depth(), with_reporter(reports.append):
-                # Note that the data generation and test execution happen in the same
-                # coverage context.  We may later split this, or tag each separately.
-                with collector:
-                    args, kwargs = data.draw(self.__strategy)
-
-                    # Save the repr of our arguments so they can be reported later
-                    argstrings.extend(map(repr, args))
-                    argstrings.extend(f"{k}={v!r}" for k, v in kwargs.items())
-
-                    self.__test_fn(*args, **kwargs)
-        except StopTest:
-            data.status = Status.OVERRUN
-        except UnsatisfiedAssumption:
-            data.status = Status.INVALID
-        except failure_exceptions_to_catch() as e:
-            data.status = Status.INTERESTING
-            tb = get_trimmed_traceback()
-            filename, lineno, *_ = traceback.extract_tb(tb)[-1]
-            data.interesting_origin = (type(e), filename, lineno)
-            data.extra_information.traceback = "".join(
-                traceback.format_exception(etype=type(e), value=e, tb=tb)
-            )
-        finally:
-            data.extra_information.call_repr = (
-                self.__test_fn.__name__ + "(" + ", ".join(argstrings) + ")"
-            )
-            data.extra_information.reports = "\n".join(map(str, reports))
-
-        # In addition to coverage branches, use psudeo-coverage information provided via
-        # the `hypothesis.event()` function - exploiting user-defined partitions
-        # designed for diagnostic output to guide generation.  See
-        # https://hypothesis.readthedocs.io/en/latest/details.html#hypothesis.event
-        data.extra_information.branches = frozenset(
-            getattr(collector, "branches", ())  # might be a debug tracer instead
-        ).union(
-            event_str
-            for event_str in map(str, data.events)
-            if not event_str.startswith("Retried draw from ")
-            or event_str.startswith("Aborted test because unable to satisfy ")
-        )
-
-        data.freeze()
-        # Update the pool and report any changes immediately for new coverage.  If no
-        # new coverage, occasionally send an update anyway so we don't look stalled.
-        self.status_counts[data.status.name] += 1
-        if self.pool.add(data.as_result(), source):
-            self.since_new_cov = 0
-        else:
-            self.since_new_cov += 1
-        if 0 in (self.since_new_cov, self.ninputs % 100):
-            UNDELIVERED_REPORTS.append(self._json_description)
-
-        self.elapsed_time += time.perf_counter() - start
-        if UNDELIVERED_REPORTS and (self._last_post_time + 10 < self.elapsed_time):
-            self._report_change(UNDELIVERED_REPORTS)
-            del UNDELIVERED_REPORTS[:]
-
-        # The shrinker relies on returning the data object to be inspected.
-        return data.as_result()
-
-    def _report_change(self, data: Union[Report, List[Report]]) -> None:
-        """Replace this method to send JSON data to the dashboard."""
-
-    @property
-    def _json_description(self) -> Report:
-        """Summarise current state to send to dashboard."""
-        if self.ninputs == 0:
-            return {"nodeid": self.nodeid, "note": "starting up..."}
-        report: Report = {
-            "nodeid": self.nodeid,
-            "elapsed_time": self.elapsed_time,
-            "timestamp": time.time(),
-            "ninputs": self.ninputs,
-            "branches": len(self.pool.arc_counts),
-            "since new cov": self.since_new_cov,
-            "loaded_from_db": len(self.pool._loaded_from_database),
-            "status_counts": self.status_counts,
-            "seed_pool": self.pool.json_report,
-            "note": "replaying saved examples"
-            if self._replay_buffer
-            else ("shrinking known examples" if self.pool._in_distill_phase else ""),
-        }
-        if self.pool.interesting_examples:
-            report["note"] = (
-                f"raised {list(self.pool.interesting_examples)[0][0].__name__} "
-                f"({'shrinking...' if self.shrinking else 'finished'})"
-            )
-            report["failures"] = [
-                ls for _, ls in self.pool.interesting_examples.values()
-            ]
-            del report["since new cov"]
-        return report
-
-    @property
-    def has_found_failure(self) -> bool:
-        """If we've already found a failing example we might reprioritize."""
-        return bool(self.pool.interesting_examples)
-
-
-def fuzz_several(*targets_: FuzzProcess, random_seed: int = None) -> NoReturn:
-    """Take N fuzz targets and run them all."""
-    # TODO: this isn't actually multi-process yet, and that's bad.
-    rand = Random(random_seed)
-    targets = SortedKeyList(targets_, lambda t: t.since_new_cov)
-
-    # Loop forever: at each timestep, we choose a target using an epsilon-greedy
-    # strategy for simplicity (TODO: improve this later) and run it once.
-    # TODO: make this aware of test runtime, so it adapts for branches-per-second
-    #       rather than branches-per-input.
-    for t in targets:
-        t.startup()
-    for i in itertools.count():
-        if i % 20 == 0:
-            t = targets.pop(rand.randrange(len(targets)))
-            t.run_one()
-            targets.add(t)
-        else:
-            targets[0].run_one()
-            if len(targets) > 1 and targets.key(targets[0]) > targets.key(targets[1]):
-                # pay our log-n cost to keep the list sorted
-                targets.add(targets.pop(0))
-            elif targets[0].has_found_failure:
-                print(f"found failing example for {targets[0].nodeid}")  # noqa
-                targets.pop(0)
-            if not targets:
-                raise Exception("Found failures for all tests!")
-    raise NotImplementedError("unreachable")
+"""Adaptive fuzzing for property-based tests using Hypothesis."""
+
+import contextlib
+import itertools
+import sys
+import time
+import traceback
+from random import Random
+from typing import Any, Callable, Dict, Generator, List, NoReturn, Optional, Union
+
+from hypothesis import settings, strategies as st
+from hypothesis.core import (
+    BuildContext,
+    deterministic_PRNG,
+    failure_exceptions_to_catch,
+    get_trimmed_traceback,
+    process_arguments_to_given,
+)
+from hypothesis.database import ExampleDatabase
+from hypothesis.errors import StopTest, UnsatisfiedAssumption
+from hypothesis.internal.conjecture.data import ConjectureData, Status
+from hypothesis.internal.conjecture.engine import BUFFER_SIZE
+from hypothesis.internal.conjecture.junkdrawer import stack_depth_of_caller
+from hypothesis.internal.conjecture.shrinker import Shrinker
+from hypothesis.internal.reflection import function_digest, get_signature
+from hypothesis.reporting import with_reporter
+from sortedcontainers import SortedKeyList
+
+from .corpus import BlackBoxMutator, CrossOverMutator, EngineStub, HowGenerated, Pool
+from .cov import CustomCollectionContext
+
+try:
+    from .debugger import record_pytrace
+except ImportError:
+    record_pytrace = None  # type: ignore
+
+Report = Dict[str, Union[int, float, str, list, Dict[str, int]]]
+
+UNDELIVERED_REPORTS: List[Report] = []
+
+
+@contextlib.contextmanager
+def constant_stack_depth() -> Generator[None, None, None]:
+    # TODO: consider extracting this upstream so we can just import it.
+    recursion_limit = sys.getrecursionlimit()
+    depth = stack_depth_of_caller()
+    # Because we add to the recursion limit, to be good citizens we also add
+    # a check for unbounded recursion.  The default limit is 1000, so this can
+    # only ever trigger if something really strange is happening and it's hard
+    # to imagine an intentionally-deeply-recursive use of this code.
+    assert depth <= 1000, (
+        f"Hypothesis would usually add {recursion_limit} to the stack depth of "
+        "{depth} here, but we are already much deeper than expected.  Aborting "
+        "now, to avoid extending the stack limit in an infinite loop..."
+    )
+    try:
+        sys.setrecursionlimit(depth + recursion_limit)
+        yield
+    finally:
+        sys.setrecursionlimit(recursion_limit)
+
+
+class HitShrinkTimeoutError(Exception):
+    pass
+
+
+class FuzzProcess:
+    """Maintain all the state associated with fuzzing a single target.
+
+    This includes:
+
+        - the coverage map and associated inputs
+        - references to Hypothesis' database for this test (for failure replay)
+        - a "run one" method, and an estimate of the value of running one input
+        - checkpointing tools so we can crash and restart without losing progess
+
+    etc.  The fuzz controller will then operate on a collection of these objects.
+    """
+
+    @classmethod
+    def from_hypothesis_test(
+        cls,
+        wrapped_test: Any,
+        *,
+        nodeid: str = None,
+        extra_kw: Optional[Dict[str, object]] = None,
+    ) -> "FuzzProcess":
+        """Return a FuzzProcess for an @given-decorated test function."""
+        _, _, _, search_strategy = process_arguments_to_given(
+            wrapped_test,
+            arguments=(),
+            kwargs=extra_kw or {},
+            given_kwargs=wrapped_test.hypothesis._given_kwargs,
+            params=get_signature(wrapped_test).parameters,
+        )
+        return cls(
+            test_fn=wrapped_test.hypothesis.inner_test,
+            strategy=search_strategy,
+            nodeid=nodeid,
+            database_key=function_digest(wrapped_test.hypothesis.inner_test),
+            hypothesis_database=wrapped_test._hypothesis_internal_use_settings.database
+            or settings.default.database,
+        )
+
+    def __init__(
+        self,
+        test_fn: Callable,
+        strategy: st.SearchStrategy,
+        *,
+        random_seed: int = 0,
+        nodeid: str = None,
+        database_key: bytes,
+        hypothesis_database: ExampleDatabase,
+    ) -> None:
+        """Construct a FuzzProcess from specific arguments."""
+        # The actual fuzzer implementation
+        self.random = Random(random_seed)
+        self.__test_fn = test_fn
+        self.__strategy = strategy
+        self.nodeid = nodeid or test_fn.__qualname__
+
+        # The seed pool is responsible for managing all seed state, including saving
+        # novel seeds to the database.  This includes tracking how often each branch
+        # has been hit, minimal covering examples, and so on.
+        self.pool = Pool(hypothesis_database, database_key)
+        self._mutator_blackbox = BlackBoxMutator(self.pool, self.random)
+        self._mutator_crossover = CrossOverMutator(self.pool, self.random)
+
+        # Set up the basic data that we'll track while fuzzing
+        self.ninputs = 0
+        self.elapsed_time = 0.0
+        self.stop_shrinking_at = float("inf")
+        self.since_new_cov = 0
+        self.status_counts = {s.name: 0 for s in Status}
+        self.shrinking = False
+        # Any new examples from the database will be added to this replay buffer
+        self._replay_buffer: List[bytes] = []
+        # After replay, we stay in blackbox mode for a while, until we've generated
+        # 1000 consecutive examples without new coverage, and then switch to mutation.
+        self._early_blackbox_mode = True
+
+        # We batch updates, since frequent HTTP posts are slow
+        self._last_post_time = self.elapsed_time
+
+    def startup(self) -> None:
+        """Set up initial state and prepare to replay the saved behaviour."""
+        assert self.ninputs == 0, "already started this FuzzProcess"
+        # Report that we've started this fuzz target, and run zero examples so far
+        self._report_change(self._json_description)
+        # Next, restore progress made in previous runs by loading our saved examples.
+        # This is meant to be the minimal set of inputs that exhibits all distinct
+        # behaviours we've observed to date.  Replaying takes longer than restoring
+        # our data structures directly, but copes much better with changed behaviour.
+        self._replay_buffer.extend(self.pool.fetch())
+        self._replay_buffer.append(b"\x00" * BUFFER_SIZE)
+
+    def generate_prefix(self) -> bytes:
+        """Generate a test prefix by mutating previous examples.
+
+        This is going to be the method to override when experimenting with
+        alternative fuzzing techniques.
+
+            - for unguided fuzzing, return an empty b'' and the random postfix
+              generation in ConjectureData will do the rest.
+            - for coverage-guided fuzzing, mutate or splice together known inputs.
+
+        This version is terrible, but any coverage guidance at all is enough to help...
+        """
+        # Start by replaying any previous failures which we've retrieved from the
+        # database.  This is useful to recover state at startup, or to share
+        # progress made in other processes.
+        if self._replay_buffer:
+            return self._replay_buffer.pop()
+
+        # TODO: currently hard-coding a particular mutator; we want to do MOpt-style
+        # adaptive weighting of all the different mutators we could use.
+        # For now though, we'll just use a hardcoded swapover point
+        if self._early_blackbox_mode or self.random.random() < 0.05:
+            return self._mutator_blackbox.generate_buffer()
+        return self._mutator_crossover.generate_buffer()
+
+    def run_one(self) -> None:
+        """Run a single input through the fuzz target, or maybe more.
+
+        The "more" part is in cases where we discover new coverage, and shrink
+        to the minimal covering example.
+        """
+        # If we've been stable for a little while, try loading new examples from the
+        # database.  We do this unconditionally because even if this fuzzer doesn't
+        # know of other concurrent runs, there may be e.g. a test process sharing the
+        # database.  We do make it infrequent to manage the overhead though.
+        if self.ninputs % 1000 == 0 and self.since_new_cov > 1000:
+            self._replay_buffer.extend(self.pool.fetch())
+
+        # seen_count = len(self.pool.arc_counts)
+
+        # Run the input
+        result = self._run_test_on(self.generate_prefix())
+
+        if result.status is Status.INTERESTING:
+            # Shrink to our minimal failing example, since we'll stop after this.
+            self.shrinking = True
+            shrinker = Shrinker(
+                EngineStub(self._run_test_on, self.random),
+                result,
+                predicate=lambda d: d.status is Status.INTERESTING,
+                allow_transition=None,
+            )
+            self.stop_shrinking_at = self.elapsed_time + 300
+            with contextlib.suppress(HitShrinkTimeoutError):
+                shrinker.shrink()
+            self.shrinking = False
+            if record_pytrace:
+                # Replay minimal example under our time-travelling debug tracer
+                self._run_test_on(
+                    shrinker.shrink_target.buffer,
+                    collector=record_pytrace(self.nodeid),
+                )
+            UNDELIVERED_REPORTS.append(self._json_description)
+            self._report_change(UNDELIVERED_REPORTS)
+            del UNDELIVERED_REPORTS[:]
+
+        # Consider switching out of blackbox mode.
+        if self.since_new_cov >= 1000 and not self._replay_buffer:
+            self._early_blackbox_mode = False
+
+        # NOTE: this distillation logic works fine, it's just discovering new coverage
+        # much more slowly than jumping directly to mutational mode.
+        # if len(self.pool.arc_counts) > seen_count and not self._early_blackbox_mode:
+        #     self.pool.distill(self._run_test_on, self.random)
+
+    def _run_test_on(
+        self,
+        buffer: bytes,
+        *,
+        source: HowGenerated = HowGenerated.shrinking,
+        collector: contextlib.AbstractContextManager = None,
+    ) -> ConjectureData:
+        """Run the test_fn on a given buffer of bytes, in a way a Shrinker can handle.
+
+        In normal operation, it's called via run_one (above), but we might also
+        delegate to the shrinker to find minimal covering examples.
+        """
+        start = time.perf_counter()
+        self.ninputs += 1
+        collector = collector or CustomCollectionContext()  # type: ignore
+        assert collector is not None
+        reports: List[str] = []
+        argstrings: List[str] = []
+        data = ConjectureData(max_length=BUFFER_SIZE, prefix=buffer, random=self.random)
+        try:
+            with deterministic_PRNG(), BuildContext(
+                data, is_final=True
+            ), constant_stack_depth(), with_reporter(reports.append):
+                # Note that the data generation and test execution happen in the same
+                # coverage context.  We may later split this, or tag each separately.
+                with collector:
+                    args, kwargs = data.draw(self.__strategy)
+
+                    # Save the repr of our arguments so they can be reported later
+                    argstrings.extend(map(repr, args))
+                    argstrings.extend(f"{k}={v!r}" for k, v in kwargs.items())
+
+                    self.__test_fn(*args, **kwargs)
+        except StopTest:
+            data.status = Status.OVERRUN
+        except UnsatisfiedAssumption:
+            data.status = Status.INVALID
+        except failure_exceptions_to_catch() as e:
+            data.status = Status.INTERESTING
+            tb = get_trimmed_traceback()
+            filename, lineno, *_ = traceback.extract_tb(tb)[-1]
+            data.interesting_origin = (type(e), filename, lineno)
+            data.extra_information.traceback = "".join(
+                traceback.format_exception(type(e), value=e, tb=tb)
+            )
+        finally:
+            data.extra_information.call_repr = (
+                self.__test_fn.__name__ + "(" + ", ".join(argstrings) + ")"
+            )
+            data.extra_information.reports = "\n".join(map(str, reports))
+
+        # In addition to coverage branches, use psudeo-coverage information provided via
+        # the `hypothesis.event()` function - exploiting user-defined partitions
+        # designed for diagnostic output to guide generation.  See
+        # https://hypothesis.readthedocs.io/en/latest/details.html#hypothesis.event
+        data.extra_information.branches = frozenset(
+            getattr(collector, "branches", ())  # might be a debug tracer instead
+        ).union(
+            event_str
+            for event_str in map(str, data.events)
+            if not event_str.startswith("Retried draw from ")
+            or event_str.startswith("Aborted test because unable to satisfy ")
+        )
+
+        data.freeze()
+        # Update the pool and report any changes immediately for new coverage.  If no
+        # new coverage, occasionally send an update anyway so we don't look stalled.
+        self.status_counts[data.status.name] += 1
+        if self.pool.add(data.as_result(), source):
+            self.since_new_cov = 0
+        else:
+            self.since_new_cov += 1
+        if 0 in (self.since_new_cov, self.ninputs % 100):
+            UNDELIVERED_REPORTS.append(self._json_description)
+
+        self.elapsed_time += time.perf_counter() - start
+        if UNDELIVERED_REPORTS and (self._last_post_time + 10 < self.elapsed_time):
+            self._report_change(UNDELIVERED_REPORTS)
+            del UNDELIVERED_REPORTS[:]
+
+        if self.elapsed_time > self.stop_shrinking_at:
+            raise HitShrinkTimeoutError
+
+        # The shrinker relies on returning the data object to be inspected.
+        return data.as_result()
+
+    def _report_change(self, data: Union[Report, List[Report]]) -> None:
+        """Replace this method to send JSON data to the dashboard."""
+
+    @property
+    def _json_description(self) -> Report:
+        """Summarise current state to send to dashboard."""
+        if self.ninputs == 0:
+            return {
+                "nodeid": self.nodeid,
+                "note": "starting up...",
+                "ninputs": 0,
+                "branches": 0,
+                "elapsed_time": 0,
+            }
+        report: Report = {
+            "nodeid": self.nodeid,
+            "elapsed_time": self.elapsed_time,
+            "timestamp": time.time(),
+            "ninputs": self.ninputs,
+            "branches": len(self.pool.arc_counts),
+            "since new cov": self.since_new_cov,
+            "loaded_from_db": len(self.pool._loaded_from_database),
+            "status_counts": self.status_counts,
+            "seed_pool": self.pool.json_report,
+            "note": "replaying saved examples"
+            if self._replay_buffer
+            else ("shrinking known examples" if self.pool._in_distill_phase else ""),
+        }
+        if self.pool.interesting_examples:
+            report["note"] = (
+                f"raised {list(self.pool.interesting_examples)[0][0].__name__} "
+                f"({'shrinking...' if self.shrinking else 'finished'})"
+            )
+            report["failures"] = [
+                ls for _, ls in self.pool.interesting_examples.values()
+            ]
+            del report["since new cov"]
+        return report
+
+    @property
+    def has_found_failure(self) -> bool:
+        """If we've already found a failing example we might reprioritize."""
+        return bool(self.pool.interesting_examples)
+
+
+def fuzz_several(*targets_: FuzzProcess, random_seed: int = None) -> NoReturn:
+    """Take N fuzz targets and run them all."""
+    # TODO: this isn't actually multi-process yet, and that's bad.
+    rand = Random(random_seed)
+    targets = SortedKeyList(targets_, lambda t: t.since_new_cov)
+
+    # Loop forever: at each timestep, we choose a target using an epsilon-greedy
+    # strategy for simplicity (TODO: improve this later) and run it once.
+    # TODO: make this aware of test runtime, so it adapts for branches-per-second
+    #       rather than branches-per-input.
+    for t in targets:
+        t.startup()
+    for i in itertools.count():
+        if i % 20 == 0:
+            t = targets.pop(rand.randrange(len(targets)))
+            t.run_one()
+            targets.add(t)
+        else:
+            targets[0].run_one()
+            if len(targets) > 1 and targets.key(targets[0]) > targets.key(targets[1]):
+                # pay our log-n cost to keep the list sorted
+                targets.add(targets.pop(0))
+            elif targets[0].has_found_failure:
+                print(f"found failing example for {targets[0].nodeid}")  # noqa
+                targets.pop(0)
+            if not targets:
+                raise Exception("Found failures for all tests!")
+    raise NotImplementedError("unreachable")
```

### Comparing `hypofuzz-22.7.1/src/hypofuzz/interface.py` & `hypofuzz-23.4.1/src/hypofuzz/interface.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-"""CLI and Python API for the fuzzer."""
-import io
-import sys
-from contextlib import redirect_stdout, suppress
-from functools import partial
-from typing import TYPE_CHECKING, Iterable, List, NoReturn, Tuple
-
-import pytest
-import requests
-
-if TYPE_CHECKING:
-    # We have to defer imports to within functions here, because this module
-    # is a Hypothesis entry point and is thus imported earlier than the others.
-    from .hy import FuzzProcess
-
-
-class _ItemsCollector:
-    """A pytest plugin which grabs all the fuzzable tests at the end of collection."""
-
-    def __init__(self) -> None:
-        self.fuzz_targets: List["FuzzProcess"] = []
-
-    def pytest_collection_finish(self, session: pytest.Session) -> None:
-        from .hy import FuzzProcess
-
-        for item in session.items:
-            # If the test takes a fixture, we skip it - the fuzzer doesn't have
-            # pytest scopes, so we just can't support them.  TODO: note skips.
-            if item._request._fixturemanager.getfixtureinfo(
-                node=item, func=item.function, cls=None
-            ).name2fixturedefs:
-                continue
-            # For parametrized tests, we have to pass the parametrized args into
-            # wrapped_test.hypothesis.get_strategy() to avoid trivial TypeErrors
-            # from missing required arguments.
-            extra_kw = item.callspec.params if hasattr(item, "callspec") else {}
-            # Wrap it up in a FuzzTarget and we're done!
-            fuzz = FuzzProcess.from_hypothesis_test(
-                item.obj, nodeid=item.nodeid, extra_kw=extra_kw
-            )
-            self.fuzz_targets.append(fuzz)
-
-
-def _get_hypothesis_tests_with_pytest(args: Iterable[str]) -> List["FuzzProcess"]:
-    """Find the hypothesis-only test functions run by pytest.
-
-    This basically uses `pytest --collect-only -m hypothesis $args`.
-    """
-    collector = _ItemsCollector()
-    out = io.StringIO()
-    with redirect_stdout(out):
-        ret = pytest.main(
-            args=[
-                "--collect-only",
-                "-m=hypothesis",
-                "--pythonwarnings=ignore::pytest.PytestAssertRewriteWarning",
-                *args,
-            ],
-            plugins=[collector],
-        )
-    if ret:
-        print(out.getvalue())  # noqa
-        print(f"Exiting because pytest returned exit code {ret}")  # noqa
-        sys.exit(ret)
-    return collector.fuzz_targets
-
-
-def _post(port: int, data: dict) -> None:
-    with suppress(Exception):
-        requests.post(f"http://localhost:{port}/", json=data)
-
-
-def _fuzz_several(
-    pytest_args: Tuple[str, ...], nodeids: List[str], port: int = None
-) -> NoReturn:
-    """Collect and fuzz tests.
-
-    Designed to be used inside a multiprocessing.Process started with the spawn()
-    method - requires picklable arguments but works on Windows too.
-    """
-    # Import within the function to break an import cycle when used as an entry point.
-    from .hy import fuzz_several
-
-    tests = [
-        t for t in _get_hypothesis_tests_with_pytest(pytest_args) if t.nodeid in nodeids
-    ]
-    if port is not None:
-        for t in tests:
-            t._report_change = partial(_post, port)  # type: ignore
-
-    fuzz_several(*tests)
-    raise NotImplementedError("unreachable")
+"""CLI and Python API for the fuzzer."""
+import io
+import sys
+from contextlib import redirect_stdout, suppress
+from functools import partial
+from typing import TYPE_CHECKING, Iterable, List, NoReturn, Tuple
+
+import pytest
+import requests
+
+if TYPE_CHECKING:
+    # We have to defer imports to within functions here, because this module
+    # is a Hypothesis entry point and is thus imported earlier than the others.
+    from .hy import FuzzProcess
+
+
+class _ItemsCollector:
+    """A pytest plugin which grabs all the fuzzable tests at the end of collection."""
+
+    def __init__(self) -> None:
+        self.fuzz_targets: List["FuzzProcess"] = []
+
+    def pytest_collection_finish(self, session: pytest.Session) -> None:
+        from .hy import FuzzProcess
+
+        for item in session.items:
+            # If the test takes a fixture, we skip it - the fuzzer doesn't have
+            # pytest scopes, so we just can't support them.  TODO: note skips.
+            if item._request._fixturemanager.getfixtureinfo(
+                node=item, func=item.function, cls=None
+            ).name2fixturedefs:
+                continue
+            # For parametrized tests, we have to pass the parametrized args into
+            # wrapped_test.hypothesis.get_strategy() to avoid trivial TypeErrors
+            # from missing required arguments.
+            extra_kw = item.callspec.params if hasattr(item, "callspec") else {}
+            # Wrap it up in a FuzzTarget and we're done!
+            fuzz = FuzzProcess.from_hypothesis_test(
+                item.obj, nodeid=item.nodeid, extra_kw=extra_kw
+            )
+            self.fuzz_targets.append(fuzz)
+
+
+def _get_hypothesis_tests_with_pytest(args: Iterable[str]) -> List["FuzzProcess"]:
+    """Find the hypothesis-only test functions run by pytest.
+
+    This basically uses `pytest --collect-only -m hypothesis $args`.
+    """
+    collector = _ItemsCollector()
+    out = io.StringIO()
+    with redirect_stdout(out):
+        ret = pytest.main(
+            args=[
+                "--collect-only",
+                "-m=hypothesis",
+                "--pythonwarnings=ignore::pytest.PytestAssertRewriteWarning",
+                *args,
+            ],
+            plugins=[collector],
+        )
+    if ret:
+        print(out.getvalue())  # noqa
+        print(f"Exiting because pytest returned exit code {ret}")  # noqa
+        sys.exit(ret)
+    return collector.fuzz_targets
+
+
+def _post(port: int, data: dict) -> None:
+    with suppress(Exception):
+        requests.post(f"http://localhost:{port}/", json=data)
+
+
+def _fuzz_several(
+    pytest_args: Tuple[str, ...], nodeids: List[str], port: int = None
+) -> NoReturn:
+    """Collect and fuzz tests.
+
+    Designed to be used inside a multiprocessing.Process started with the spawn()
+    method - requires picklable arguments but works on Windows too.
+    """
+    # Import within the function to break an import cycle when used as an entry point.
+    from .hy import fuzz_several
+
+    tests = [
+        t for t in _get_hypothesis_tests_with_pytest(pytest_args) if t.nodeid in nodeids
+    ]
+    if port is not None:
+        for t in tests:
+            t._report_change = partial(_post, port)  # type: ignore
+
+    fuzz_several(*tests)
+    raise NotImplementedError("unreachable")
```

### Comparing `hypofuzz-22.7.1/src/hypofuzz.egg-info/PKG-INFO` & `hypofuzz-23.4.1/src/hypofuzz.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,63 @@
 Metadata-Version: 2.1
 Name: hypofuzz
-Version: 22.7.1
+Version: 23.4.1
 Summary: Adaptive fuzzing for property-based tests
 Home-page: https://hypofuzz.com/
 Author: Zac Hatfield-Dodds
 Author-email: zac@hypofuzz.com
-License: Proprietary License
-Project-URL: Funding, https://hypofuzz.com/pricing/
+License: AGPL-3.0
 Project-URL: Documentation, https://hypofuzz.com/docs/
 Project-URL: Changelog, https://hypofuzz.com/docs/changelog.html
 Keywords: python testing fuzzing property-based-testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Hypothesis
 Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Testing
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pytrace
+License-File: LICENSE
 
 # [HypoFuzz](https://hypofuzz.com/)
 
 *Adaptive fuzzing of [Hypothesis](https://hypothesis.readthedocs.io) tests.*
 
 
 Property-based approaches help you to write better tests which find more bugs,
 but don't have great ways to exchange much more CPU time for more bugs.
 The goal of this project is to bring togther the best parts of fuzzing and PBT.
 
 
 ## Motivation
 
 You can [run a traditional fuzzer](https://hypothesis.readthedocs.io/en/latest/details.html#use-with-external-fuzzers)
-like AFL on Hypothesis tests to get basic coverage guidance.
-
-- This does actually work, which is pretty cool
-- It's very slow though, and often fails to parse the bytes into an example
-- Installing, configuring, and connecting all the parts is a pain
-- Also assumes one fuzz target per core, which doesn't scale very far
+like AFL on Hypothesis tests to get basic coverage guidance.  This works OK, but there's
+a lot of performance overhead.  Installing, configuring, and connecting all the parts is
+a pain, and because it assumes one fuzz target per core you probably can't scale up far
+enough to fuzz your whole test suite.
 
 Alternatively, you can just run Hypothesis with a large `max_examples` setting.
-This also works pretty well, but doesn't get the benefits of coverage guidance
-(i.e. avoiding the exponential scaling cliff by learning from feedback) and
-also occupies one fuzz target per core.
-
-(turns out that you can [emulate coverage guidance](https://engineering.backtrace.io/posts/2020-03-11-how-hard-is-it-to-guide-test-case-generators-with-branch-coverage-feedback/)
-with `hypothesis.target()`, which appears to work well enough as a starting point)
-
-(also Hypothesis used to have coverage guidance built in, but we took it back out
-because of performance and ecosystem integration problems - as a rule of thumb it's
-just not worth the trouble for less than a thousand inputs.
-[see here](https://github.com/HypothesisWorks/hypothesis/pulls?q=is%3Amerged+use_coverage).)
+This also works pretty well, but doesn't get the benefits of coverage guidance and
+you have to guess how long it'll take to run the tests - each gets the same budget.
+
+HypoFuzz solves all of these problems, and more!
 
 
 ## Features
 
 - Interleave execution of many test functions
 - Prioritise functions where we expect to make progress
 - Coverage-guided exploration of your system-under-test
-- Seamless python-native and CLI integrations
+- Seamless python-native and CLI integrations (replaces the `pytest` command)
 - Web-based time-travel debugging with [PyTrace](https://pytrace.com/)
   (automatic if you `pip install hypofuzz[pytrace]`)
 
-
-## Changelog
-
-Patch notes [can be found in `CHANGELOG.md`](https://github.com/Zac-HD/hypofuzz/blob/master/CHANGELOG.md).
-
-
-## License
-
-This is an active research project as part of my (Zac Hatfield-Dodds) PhD.
-
-Unlike Hypothesis, it is *not* open source and I am not seeking external contributions.
-
-As a complement to users of free, world-class PBT tools, I'm planning to sell
-licenses in order to fund ongoing work on both this project and Hypothesis itself.
-Please [contact me](mailto:sales@hypofuzz.com) if you are interested.
+Read more about HypoFuzz at https://hypofuzz.com/docs/, including
+[the changelog](https://hypofuzz.com/docs/changelog.html).
```

