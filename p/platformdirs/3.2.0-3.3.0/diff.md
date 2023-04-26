# Comparing `tmp/platformdirs-3.2.0.tar.gz` & `tmp/platformdirs-3.3.0.tar.gz`

## Comparing `platformdirs-3.2.0.tar` & `platformdirs-3.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    17931 2020-02-02 00:00:00.000000 platformdirs-3.2.0/src/platformdirs/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 platformdirs-3.2.0/src/platformdirs/__main__.py
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 platformdirs-3.2.0/src/platformdirs/android.py
--rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 platformdirs-3.2.0/src/platformdirs/api.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 platformdirs-3.2.0/src/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.2.0/src/platformdirs/py.typed
--rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 platformdirs-3.2.0/src/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.2.0/src/platformdirs/version.py
--rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 platformdirs-3.2.0/src/platformdirs/windows.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 platformdirs-3.2.0/tests/conftest.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 platformdirs-3.2.0/tests/test_android.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 platformdirs-3.2.0/tests/test_api.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 platformdirs-3.2.0/tests/test_comp_with_appdirs.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 platformdirs-3.2.0/tests/test_macos.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.2.0/tests/test_main.py
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 platformdirs-3.2.0/tests/test_unix.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.2.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.2.0/LICENSE
--rw-r--r--   0        0        0     7403 2020-02-02 00:00:00.000000 platformdirs-3.2.0/README.rst
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 platformdirs-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 platformdirs-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0    18268 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/__main__.py
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/android.py
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/api.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/py.typed
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/version.py
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/windows.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 platformdirs-3.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 platformdirs-3.3.0/tests/test_android.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 platformdirs-3.3.0/tests/test_api.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 platformdirs-3.3.0/tests/test_comp_with_appdirs.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 platformdirs-3.3.0/tests/test_macos.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.3.0/tests/test_main.py
+-rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 platformdirs-3.3.0/tests/test_unix.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.3.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.3.0/LICENSE
+-rw-r--r--   0        0        0     7403 2020-02-02 00:00:00.000000 platformdirs-3.3.0/README.rst
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 platformdirs-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 platformdirs-3.3.0/PKG-INFO
```

### Comparing `platformdirs-3.2.0/src/platformdirs/__init__.py` & `platformdirs-3.3.0/src/platformdirs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,14 +239,21 @@
 def user_documents_dir() -> str:
     """
     :returns: documents directory tied to the user
     """
     return PlatformDirs().user_documents_dir
 
 
+def user_pictures_dir() -> str:
+    """
+    :returns: pictures directory tied to the user
+    """
+    return PlatformDirs().user_pictures_dir
+
+
 def user_runtime_dir(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
     opinion: bool = True,
     ensure_exists: bool = False,
 ) -> str:
@@ -462,14 +469,21 @@
 def user_documents_path() -> Path:
     """
     :returns: documents path tied to the user
     """
     return PlatformDirs().user_documents_path
 
 
+def user_pictures_path() -> Path:
+    """
+    :returns: pictures path tied to the user
+    """
+    return PlatformDirs().user_pictures_path
+
+
 def user_runtime_path(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
     opinion: bool = True,
     ensure_exists: bool = False,
 ) -> Path:
@@ -498,22 +512,24 @@
     "PlatformDirsABC",
     "user_data_dir",
     "user_config_dir",
     "user_cache_dir",
     "user_state_dir",
     "user_log_dir",
     "user_documents_dir",
+    "user_pictures_dir",
     "user_runtime_dir",
     "site_data_dir",
     "site_config_dir",
     "site_cache_dir",
     "user_data_path",
     "user_config_path",
     "user_cache_path",
     "user_state_path",
     "user_log_path",
     "user_documents_path",
+    "user_pictures_path",
     "user_runtime_path",
     "site_data_path",
     "site_config_path",
     "site_cache_path",
 ]
```

### Comparing `platformdirs-3.2.0/src/platformdirs/__main__.py` & `platformdirs-3.3.0/src/platformdirs/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 PROPS = (
     "user_data_dir",
     "user_config_dir",
     "user_cache_dir",
     "user_state_dir",
     "user_log_dir",
     "user_documents_dir",
+    "user_pictures_dir",
     "user_runtime_dir",
     "site_data_dir",
     "site_config_dir",
     "site_cache_dir",
 )
```

### Comparing `platformdirs-3.2.0/src/platformdirs/android.py` & `platformdirs-3.3.0/src/platformdirs/android.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,14 +69,21 @@
     def user_documents_dir(self) -> str:
         """
         :return: documents directory tied to the user e.g. ``/storage/emulated/0/Documents``
         """
         return _android_documents_folder()
 
     @property
+    def user_pictures_dir(self) -> str:
+        """
+        :return: pictures directory tied to the user e.g. ``/storage/emulated/0/Pictures``
+        """
+        return _android_pictures_folder()
+
+    @property
     def user_runtime_dir(self) -> str:
         """
         :return: runtime directory tied to the user, same as `user_cache_dir` if not opinionated else ``tmp`` in it,
           e.g. ``/data/user/<userid>/<packagename>/cache/<AppName>/tmp``
         """
         path = self.user_cache_dir
         if self.opinion:
@@ -117,10 +124,26 @@
         documents_dir: str = Context.getExternalFilesDir(Environment.DIRECTORY_DOCUMENTS).getAbsolutePath()
     except Exception:
         documents_dir = "/storage/emulated/0/Documents"
 
     return documents_dir
 
 
+@lru_cache(maxsize=1)
+def _android_pictures_folder() -> str:
+    """:return: pictures folder for the Android OS"""
+    # Get directories with pyjnius
+    try:
+        from jnius import autoclass
+
+        Context = autoclass("android.content.Context")  # noqa: N806
+        Environment = autoclass("android.os.Environment")  # noqa: N806
+        pictures_dir: str = Context.getExternalFilesDir(Environment.DIRECTORY_PICTURES).getAbsolutePath()
+    except Exception:
+        pictures_dir = "/storage/emulated/0/Pictures"
+
+    return pictures_dir
+
+
 __all__ = [
     "Android",
 ]
```

### Comparing `platformdirs-3.2.0/src/platformdirs/api.py` & `platformdirs-3.3.0/src/platformdirs/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,19 @@
     @property
     @abstractmethod
     def user_documents_dir(self) -> str:
         """:return: documents directory tied to the user"""
 
     @property
     @abstractmethod
+    def user_pictures_dir(self) -> str:
+        """:return: pictures directory tied to the user"""
+
+    @property
+    @abstractmethod
     def user_runtime_dir(self) -> str:
         """:return: runtime directory tied to the user"""
 
     @property
     def user_data_path(self) -> Path:
         """:return: data path tied to the user"""
         return Path(self.user_data_dir)
@@ -170,10 +175,15 @@
 
     @property
     def user_documents_path(self) -> Path:
         """:return: documents path tied to the user"""
         return Path(self.user_documents_dir)
 
     @property
+    def user_pictures_path(self) -> Path:
+        """:return: pictures path tied to the user"""
+        return Path(self.user_pictures_dir)
+
+    @property
     def user_runtime_path(self) -> Path:
         """:return: runtime path tied to the user"""
         return Path(self.user_runtime_dir)
```

### Comparing `platformdirs-3.2.0/src/platformdirs/macos.py` & `platformdirs-3.3.0/src/platformdirs/macos.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,19 @@
 
     @property
     def user_documents_dir(self) -> str:
         """:return: documents directory tied to the user, e.g. ``~/Documents``"""
         return os.path.expanduser("~/Documents")
 
     @property
+    def user_pictures_dir(self) -> str:
+        """:return: pictures directory tied to the user, e.g. ``~/Pictures``"""
+        return os.path.expanduser("~/Pictures")
+
+    @property
     def user_runtime_dir(self) -> str:
         """:return: runtime directory tied to the user, e.g. ``~/Library/Caches/TemporaryItems/$appname/$version``"""
         return self._append_app_name_and_version(os.path.expanduser("~/Library/Caches/TemporaryItems"))
 
 
 __all__ = [
     "MacOS",
```

### Comparing `platformdirs-3.2.0/src/platformdirs/unix.py` & `platformdirs-3.3.0/src/platformdirs/unix.py`

 * *Files 7% similar despite different names*

```diff
@@ -123,21 +123,22 @@
         return path
 
     @property
     def user_documents_dir(self) -> str:
         """
         :return: documents directory tied to the user, e.g. ``~/Documents``
         """
-        documents_dir = _get_user_dirs_folder("XDG_DOCUMENTS_DIR")
-        if documents_dir is None:
-            documents_dir = os.environ.get("XDG_DOCUMENTS_DIR", "").strip()
-            if not documents_dir:
-                documents_dir = os.path.expanduser("~/Documents")
+        return _get_user_media_dir("XDG_DOCUMENTS_DIR", "~/Documents")
 
-        return documents_dir
+    @property
+    def user_pictures_dir(self) -> str:
+        """
+        :return: pictures directory tied to the user, e.g. ``~/Pictures``
+        """
+        return _get_user_media_dir("XDG_PICTURES_DIR", "~/Pictures")
 
     @property
     def user_runtime_dir(self) -> str:
         """
         :return: runtime directory tied to the user, e.g. ``/run/user/$(id -u)/$appname/$version`` or
          ``$XDG_RUNTIME_DIR/$appname/$version``
         """
@@ -164,14 +165,24 @@
     def _first_item_as_path_if_multipath(self, directory: str) -> Path:
         if self.multipath:
             # If multipath is True, the first path is returned.
             directory = directory.split(os.pathsep)[0]
         return Path(directory)
 
 
+def _get_user_media_dir(env_var: str, fallback_tilde_path: str) -> str:
+    media_dir = _get_user_dirs_folder(env_var)
+    if media_dir is None:
+        media_dir = os.environ.get(env_var, "").strip()
+        if not media_dir:
+            media_dir = os.path.expanduser(fallback_tilde_path)
+
+    return media_dir
+
+
 def _get_user_dirs_folder(key: str) -> str | None:
     """Return directory from user-dirs.dirs config file. See https://freedesktop.org/wiki/Software/xdg-user-dirs/"""
     user_dirs_config_path = os.path.join(Unix().user_config_dir, "user-dirs.dirs")
     if os.path.exists(user_dirs_config_path):
         parser = ConfigParser()
 
         with open(user_dirs_config_path) as stream:
```

### Comparing `platformdirs-3.2.0/src/platformdirs/windows.py` & `platformdirs-3.3.0/src/platformdirs/windows.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,28 +98,38 @@
     def user_documents_dir(self) -> str:
         """
         :return: documents directory tied to the user e.g. ``%USERPROFILE%\\Documents``
         """
         return os.path.normpath(get_win_folder("CSIDL_PERSONAL"))
 
     @property
+    def user_pictures_dir(self) -> str:
+        """
+        :return: pictures directory tied to the user e.g. ``%USERPROFILE%\\Pictures``
+        """
+        return os.path.normpath(get_win_folder("CSIDL_MYPICTURES"))
+
+    @property
     def user_runtime_dir(self) -> str:
         """
         :return: runtime directory tied to the user, e.g.
          ``%USERPROFILE%\\AppData\\Local\\Temp\\$appauthor\\$appname``
         """
         path = os.path.normpath(os.path.join(get_win_folder("CSIDL_LOCAL_APPDATA"), "Temp"))
         return self._append_parts(path)
 
 
 def get_win_folder_from_env_vars(csidl_name: str) -> str:
     """Get folder from environment variables."""
     if csidl_name == "CSIDL_PERSONAL":  # does not have an environment name
         return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Documents")
 
+    if csidl_name == "CSIDL_MYPICTURES":  # does not have an environment name
+        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Pictures")
+
     env_var_name = {
         "CSIDL_APPDATA": "APPDATA",
         "CSIDL_COMMON_APPDATA": "ALLUSERSPROFILE",
         "CSIDL_LOCAL_APPDATA": "LOCALAPPDATA",
     }.get(csidl_name)
     if env_var_name is None:
         raise ValueError(f"Unknown CSIDL name: {csidl_name}")
@@ -137,14 +147,15 @@
     names.
     """
     shell_folder_name = {
         "CSIDL_APPDATA": "AppData",
         "CSIDL_COMMON_APPDATA": "Common AppData",
         "CSIDL_LOCAL_APPDATA": "Local AppData",
         "CSIDL_PERSONAL": "Personal",
+        "CSIDL_MYPICTURES": "My Pictures",
     }.get(csidl_name)
     if shell_folder_name is None:
         raise ValueError(f"Unknown CSIDL name: {csidl_name}")
     if sys.platform != "win32":  # only needed for mypy type checker to know that this code runs only on Windows
         raise NotImplementedError
     import winreg
 
@@ -156,14 +167,15 @@
 def get_win_folder_via_ctypes(csidl_name: str) -> str:
     """Get folder with ctypes."""
     csidl_const = {
         "CSIDL_APPDATA": 26,
         "CSIDL_COMMON_APPDATA": 35,
         "CSIDL_LOCAL_APPDATA": 28,
         "CSIDL_PERSONAL": 5,
+        "CSIDL_MYPICTURES": 39,
     }.get(csidl_name)
     if csidl_const is None:
         raise ValueError(f"Unknown CSIDL name: {csidl_name}")
 
     buf = ctypes.create_unicode_buffer(1024)
     windll = getattr(ctypes, "windll")  # noqa: B009 # using getattr to avoid false positive with mypy type checker
     windll.shell32.SHGetFolderPathW(None, csidl_const, None, 0, buf)
```

### Comparing `platformdirs-3.2.0/tests/conftest.py` & `platformdirs-3.3.0/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 PROPS = (
     "user_data_dir",
     "user_config_dir",
     "user_cache_dir",
     "user_state_dir",
     "user_log_dir",
     "user_documents_dir",
+    "user_pictures_dir",
     "user_runtime_dir",
     "site_data_dir",
     "site_config_dir",
     "site_cache_dir",
 )
```

### Comparing `platformdirs-3.2.0/tests/test_android.py` & `platformdirs-3.3.0/tests/test_android.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         "user_config_dir": f"/data/data/com.example/shared_prefs{suffix}",
         "site_config_dir": f"/data/data/com.example/shared_prefs{suffix}",
         "user_cache_dir": f"/data/data/com.example/cache{suffix}",
         "site_cache_dir": f"/data/data/com.example/cache{suffix}",
         "user_state_dir": f"/data/data/com.example/files{suffix}",
         "user_log_dir": f"/data/data/com.example/cache{suffix}{'' if params.get('opinion', True) is False else '/log'}",
         "user_documents_dir": "/storage/emulated/0/Documents",
+        "user_pictures_dir": "/storage/emulated/0/Pictures",
         "user_runtime_dir": f"/data/data/com.example/cache{suffix}{'' if not params.get('opinion', True) else '/tmp'}",
     }
     expected = expected_map[func]
 
     assert result == expected
```

### Comparing `platformdirs-3.2.0/tests/test_api.py` & `platformdirs-3.3.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.2.0/tests/test_comp_with_appdirs.py` & `platformdirs-3.3.0/tests/test_comp_with_appdirs.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.2.0/tests/test_macos.py` & `platformdirs-3.3.0/tests/test_macos.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,12 +29,13 @@
         "user_config_dir": f"{home}/Library/Application Support{suffix}",
         "site_config_dir": f"/Library/Application Support{suffix}",
         "user_cache_dir": f"{home}/Library/Caches{suffix}",
         "site_cache_dir": f"/Library/Caches{suffix}",
         "user_state_dir": f"{home}/Library/Application Support{suffix}",
         "user_log_dir": f"{home}/Library/Logs{suffix}",
         "user_documents_dir": f"{home}/Documents",
+        "user_pictures_dir": f"{home}/Pictures",
         "user_runtime_dir": f"{home}/Library/Caches/TemporaryItems{suffix}",
     }
     expected = expected_map[func]
 
     assert result == expected
```

### Comparing `platformdirs-3.2.0/tests/test_unix.py` & `platformdirs-3.3.0/tests/test_unix.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,14 +43,48 @@
     mocker.patch.dict(os.environ, {"HOME": "/home/example"})
     # Mock home directory for running the test on Windows
     mocker.patch.dict(os.environ, {"USERPROFILE": "/home/example"})
 
     assert Unix().user_documents_dir == "/home/example/Documents"
 
 
+def test_user_pictures_dir(mocker: MockerFixture) -> None:
+    example_path = "/home/example/ExamplePicturesFolder"
+    mock = mocker.patch("platformdirs.unix._get_user_dirs_folder")
+    mock.return_value = example_path
+    assert Unix().user_pictures_dir == example_path
+
+
+def test_user_pictures_dir_env_var(mocker: MockerFixture) -> None:
+    # Mock pictures dir not being in user-dirs.dirs file
+    mock = mocker.patch("platformdirs.unix._get_user_dirs_folder")
+    mock.return_value = None
+
+    example_path = "/home/example/ExamplePicturesFolder"
+    mocker.patch.dict(os.environ, {"XDG_PICTURES_DIR": example_path})
+
+    assert Unix().user_pictures_dir == example_path
+
+
+def test_user_pictures_dir_default(mocker: MockerFixture) -> None:
+    # Mock pictures dir not being in user-dirs.dirs file
+    mock = mocker.patch("platformdirs.unix._get_user_dirs_folder")
+    mock.return_value = None
+
+    # Mock no XDG_PICTURES_DIR env variable being set
+    mocker.patch.dict(os.environ, {"XDG_PICTURES_DIR": ""})
+
+    # Mock home directory
+    mocker.patch.dict(os.environ, {"HOME": "/home/example"})
+    # Mock home directory for running the test on Windows
+    mocker.patch.dict(os.environ, {"USERPROFILE": "/home/example"})
+
+    assert Unix().user_pictures_dir == "/home/example/Pictures"
+
+
 class XDGVariable(typing.NamedTuple):
     name: str
     default_value: str
 
 
 def _func_to_path(func: str) -> XDGVariable | None:
     mapping = {
```

### Comparing `platformdirs-3.2.0/LICENSE` & `platformdirs-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `platformdirs-3.2.0/README.rst` & `platformdirs-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `platformdirs-3.2.0/pyproject.toml` & `platformdirs-3.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = [
   "hatch-vcs>=0.3",
-  "hatchling>=1.13",
+  "hatchling>=1.14",
 ]
 
 [project]
 name = "platformdirs"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 readme = "README.rst"
 keywords = [
@@ -45,23 +45,23 @@
 dynamic = [
   "version",
 ]
 dependencies = [
   'typing-extensions>=4.5; python_version < "3.8"',
 ]
 optional-dependencies.docs = [
-  "furo>=2022.12.7",
+  "furo>=2023.3.27",
   "proselint>=0.13",
   "sphinx>=6.1.3",
-  "sphinx-autodoc-typehints!=1.23.4,>=1.22",
+  "sphinx-autodoc-typehints!=1.23.4,>=1.23",
 ]
 optional-dependencies.test = [
   "appdirs==1.4.4",
   "covdefaults>=2.3",
-  "pytest>=7.2.2",
+  "pytest>=7.3.1",
   "pytest-cov>=4",
   "pytest-mock>=3.10",
 ]
 urls.Documentation = "https://platformdirs.readthedocs.io"
 urls.Homepage = "https://github.com/platformdirs/platformdirs"
 urls.Source = "https://github.com/platformdirs/platformdirs"
 urls.Tracker = "https://github.com/platformdirs/platformdirs/issues"
```

### Comparing `platformdirs-3.2.0/PKG-INFO` & `platformdirs-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platformdirs
-Version: 3.2.0
+Version: 3.3.0
 Summary: A small Python package for determining appropriate platform-specific dirs, e.g. a "user data dir".
 Project-URL: Documentation, https://platformdirs.readthedocs.io
 Project-URL: Homepage, https://github.com/platformdirs/platformdirs
 Project-URL: Source, https://github.com/platformdirs/platformdirs
 Project-URL: Tracker, https://github.com/platformdirs/platformdirs/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Julian Berman <Julian@GrayVines.com>, Ofek Lev <oss@ofek.dev>, Ronny Pfannschmidt <opensource@ronnypfannschmidt.de>
 License-Expression: MIT
@@ -24,24 +24,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: typing-extensions>=4.5; python_version < '3.8'
 Provides-Extra: docs
-Requires-Dist: furo>=2022.12.7; extra == 'docs'
+Requires-Dist: furo>=2023.3.27; extra == 'docs'
 Requires-Dist: proselint>=0.13; extra == 'docs'
-Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.22; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.23; extra == 'docs'
 Requires-Dist: sphinx>=6.1.3; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: appdirs==1.4.4; extra == 'test'
 Requires-Dist: covdefaults>=2.3; extra == 'test'
 Requires-Dist: pytest-cov>=4; extra == 'test'
 Requires-Dist: pytest-mock>=3.10; extra == 'test'
-Requires-Dist: pytest>=7.2.2; extra == 'test'
+Requires-Dist: pytest>=7.3.1; extra == 'test'
 Description-Content-Type: text/x-rst
 
 The problem
 ===========
 
 .. image:: https://github.com/platformdirs/platformdirs/workflows/Test/badge.svg
    :target: https://github.com/platformdirs/platformdirs/actions?query=workflow%3ATest
```

