# Comparing `tmp/platformdirs-3.3.0.tar.gz` & `tmp/platformdirs-3.4.0.tar.gz`

## Comparing `platformdirs-3.3.0.tar` & `platformdirs-3.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    18268 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/__init__.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/__main__.py
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/android.py
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/api.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/py.typed
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/version.py
--rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 platformdirs-3.3.0/src/platformdirs/windows.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 platformdirs-3.3.0/tests/conftest.py
--rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 platformdirs-3.3.0/tests/test_android.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 platformdirs-3.3.0/tests/test_api.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 platformdirs-3.3.0/tests/test_comp_with_appdirs.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 platformdirs-3.3.0/tests/test_macos.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.3.0/tests/test_main.py
--rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 platformdirs-3.3.0/tests/test_unix.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.3.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.3.0/LICENSE
--rw-r--r--   0        0        0     7403 2020-02-02 00:00:00.000000 platformdirs-3.3.0/README.rst
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 platformdirs-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 platformdirs-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0    18589 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/__main__.py
+-rw-r--r--   0        0        0     5805 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/android.py
+-rw-r--r--   0        0        0     6274 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/api.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/py.typed
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/version.py
+-rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 platformdirs-3.4.0/src/platformdirs/windows.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 platformdirs-3.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 platformdirs-3.4.0/tests/test_android.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 platformdirs-3.4.0/tests/test_api.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 platformdirs-3.4.0/tests/test_comp_with_appdirs.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 platformdirs-3.4.0/tests/test_macos.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.4.0/tests/test_main.py
+-rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 platformdirs-3.4.0/tests/test_unix.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.4.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.4.0/LICENSE
+-rw-r--r--   0        0        0     7403 2020-02-02 00:00:00.000000 platformdirs-3.4.0/README.rst
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 platformdirs-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 platformdirs-3.4.0/PKG-INFO
```

### Comparing `platformdirs-3.3.0/src/platformdirs/__init__.py` & `platformdirs-3.4.0/src/platformdirs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,14 +246,21 @@
 def user_pictures_dir() -> str:
     """
     :returns: pictures directory tied to the user
     """
     return PlatformDirs().user_pictures_dir
 
 
+def user_videos_dir() -> str:
+    """
+    :returns: videos directory tied to the user
+    """
+    return PlatformDirs().user_videos_dir
+
+
 def user_runtime_dir(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
     opinion: bool = True,
     ensure_exists: bool = False,
 ) -> str:
@@ -476,14 +483,21 @@
 def user_pictures_path() -> Path:
     """
     :returns: pictures path tied to the user
     """
     return PlatformDirs().user_pictures_path
 
 
+def user_videos_path() -> Path:
+    """
+    :returns: videos path tied to the user
+    """
+    return PlatformDirs().user_videos_path
+
+
 def user_runtime_path(
     appname: str | None = None,
     appauthor: str | None | Literal[False] = None,
     version: str | None = None,
     opinion: bool = True,
     ensure_exists: bool = False,
 ) -> Path:
@@ -513,23 +527,25 @@
     "user_data_dir",
     "user_config_dir",
     "user_cache_dir",
     "user_state_dir",
     "user_log_dir",
     "user_documents_dir",
     "user_pictures_dir",
+    "user_videos_dir",
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
     "user_pictures_path",
+    "user_videos_path",
     "user_runtime_path",
     "site_data_path",
     "site_config_path",
     "site_cache_path",
 ]
```

### Comparing `platformdirs-3.3.0/src/platformdirs/__main__.py` & `platformdirs-3.4.0/src/platformdirs/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     "user_data_dir",
     "user_config_dir",
     "user_cache_dir",
     "user_state_dir",
     "user_log_dir",
     "user_documents_dir",
     "user_pictures_dir",
+    "user_videos_dir",
     "user_runtime_dir",
     "site_data_dir",
     "site_config_dir",
     "site_cache_dir",
 )
```

### Comparing `platformdirs-3.3.0/src/platformdirs/android.py` & `platformdirs-3.4.0/src/platformdirs/android.py`

 * *Files 11% similar despite different names*

```diff
@@ -76,14 +76,21 @@
     def user_pictures_dir(self) -> str:
         """
         :return: pictures directory tied to the user e.g. ``/storage/emulated/0/Pictures``
         """
         return _android_pictures_folder()
 
     @property
+    def user_videos_dir(self) -> str:
+        """
+        :return: videos directory tied to the user e.g. ``/storage/emulated/0/DCIM/Camera``
+        """
+        return _android_videos_folder()
+
+    @property
     def user_runtime_dir(self) -> str:
         """
         :return: runtime directory tied to the user, same as `user_cache_dir` if not opinionated else ``tmp`` in it,
           e.g. ``/data/user/<userid>/<packagename>/cache/<AppName>/tmp``
         """
         path = self.user_cache_dir
         if self.opinion:
@@ -140,10 +147,26 @@
         pictures_dir: str = Context.getExternalFilesDir(Environment.DIRECTORY_PICTURES).getAbsolutePath()
     except Exception:
         pictures_dir = "/storage/emulated/0/Pictures"
 
     return pictures_dir
 
 
+@lru_cache(maxsize=1)
+def _android_videos_folder() -> str:
+    """:return: videos folder for the Android OS"""
+    # Get directories with pyjnius
+    try:
+        from jnius import autoclass
+
+        Context = autoclass("android.content.Context")  # noqa: N806
+        Environment = autoclass("android.os.Environment")  # noqa: N806
+        videos_dir: str = Context.getExternalFilesDir(Environment.DIRECTORY_DCIM).getAbsolutePath()
+    except Exception:
+        videos_dir = "/storage/emulated/0/DCIM/Camera"
+
+    return videos_dir
+
+
 __all__ = [
     "Android",
 ]
```

### Comparing `platformdirs-3.3.0/src/platformdirs/api.py` & `platformdirs-3.4.0/src/platformdirs/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,14 +126,19 @@
     @property
     @abstractmethod
     def user_pictures_dir(self) -> str:
         """:return: pictures directory tied to the user"""
 
     @property
     @abstractmethod
+    def user_videos_dir(self) -> str:
+        """:return: videos directory tied to the user"""
+
+    @property
+    @abstractmethod
     def user_runtime_dir(self) -> str:
         """:return: runtime directory tied to the user"""
 
     @property
     def user_data_path(self) -> Path:
         """:return: data path tied to the user"""
         return Path(self.user_data_dir)
@@ -180,10 +185,15 @@
 
     @property
     def user_pictures_path(self) -> Path:
         """:return: pictures path tied to the user"""
         return Path(self.user_pictures_dir)
 
     @property
+    def user_videos_path(self) -> Path:
+        """:return: videos path tied to the user"""
+        return Path(self.user_videos_dir)
+
+    @property
     def user_runtime_path(self) -> Path:
         """:return: runtime path tied to the user"""
         return Path(self.user_runtime_dir)
```

### Comparing `platformdirs-3.3.0/src/platformdirs/macos.py` & `platformdirs-3.4.0/src/platformdirs/macos.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,14 +61,19 @@
 
     @property
     def user_pictures_dir(self) -> str:
         """:return: pictures directory tied to the user, e.g. ``~/Pictures``"""
         return os.path.expanduser("~/Pictures")
 
     @property
+    def user_videos_dir(self) -> str:
+        """:return: videos directory tied to the user, e.g. ``~/Movies``"""
+        return os.path.expanduser("~/Movies")
+
+    @property
     def user_runtime_dir(self) -> str:
         """:return: runtime directory tied to the user, e.g. ``~/Library/Caches/TemporaryItems/$appname/$version``"""
         return self._append_app_name_and_version(os.path.expanduser("~/Library/Caches/TemporaryItems"))
 
 
 __all__ = [
     "MacOS",
```

### Comparing `platformdirs-3.3.0/src/platformdirs/unix.py` & `platformdirs-3.4.0/src/platformdirs/unix.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,21 @@
     def user_pictures_dir(self) -> str:
         """
         :return: pictures directory tied to the user, e.g. ``~/Pictures``
         """
         return _get_user_media_dir("XDG_PICTURES_DIR", "~/Pictures")
 
     @property
+    def user_videos_dir(self) -> str:
+        """
+        :return: videos directory tied to the user, e.g. ``~/Videos``
+        """
+        return _get_user_media_dir("XDG_VIDEOS_DIR", "~/Videos")
+
+    @property
     def user_runtime_dir(self) -> str:
         """
         :return: runtime directory tied to the user, e.g. ``/run/user/$(id -u)/$appname/$version`` or
          ``$XDG_RUNTIME_DIR/$appname/$version``
         """
         path = os.environ.get("XDG_RUNTIME_DIR", "")
         if not path.strip():
```

### Comparing `platformdirs-3.3.0/src/platformdirs/windows.py` & `platformdirs-3.4.0/src/platformdirs/windows.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,14 +105,21 @@
     def user_pictures_dir(self) -> str:
         """
         :return: pictures directory tied to the user e.g. ``%USERPROFILE%\\Pictures``
         """
         return os.path.normpath(get_win_folder("CSIDL_MYPICTURES"))
 
     @property
+    def user_videos_dir(self) -> str:
+        """
+        :return: videos directory tied to the user e.g. ``%USERPROFILE%\\Videos``
+        """
+        return os.path.normpath(get_win_folder("CSIDL_MYVIDEO"))
+
+    @property
     def user_runtime_dir(self) -> str:
         """
         :return: runtime directory tied to the user, e.g.
          ``%USERPROFILE%\\AppData\\Local\\Temp\\$appauthor\\$appname``
         """
         path = os.path.normpath(os.path.join(get_win_folder("CSIDL_LOCAL_APPDATA"), "Temp"))
         return self._append_parts(path)
@@ -122,14 +129,17 @@
     """Get folder from environment variables."""
     if csidl_name == "CSIDL_PERSONAL":  # does not have an environment name
         return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Documents")
 
     if csidl_name == "CSIDL_MYPICTURES":  # does not have an environment name
         return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Pictures")
 
+    if csidl_name == "CSIDL_MYVIDEO":  # does not have an environment name
+        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Videos")
+
     env_var_name = {
         "CSIDL_APPDATA": "APPDATA",
         "CSIDL_COMMON_APPDATA": "ALLUSERSPROFILE",
         "CSIDL_LOCAL_APPDATA": "LOCALAPPDATA",
     }.get(csidl_name)
     if env_var_name is None:
         raise ValueError(f"Unknown CSIDL name: {csidl_name}")
@@ -148,14 +158,15 @@
     """
     shell_folder_name = {
         "CSIDL_APPDATA": "AppData",
         "CSIDL_COMMON_APPDATA": "Common AppData",
         "CSIDL_LOCAL_APPDATA": "Local AppData",
         "CSIDL_PERSONAL": "Personal",
         "CSIDL_MYPICTURES": "My Pictures",
+        "CSIDL_MYVIDEO": "My Video",
     }.get(csidl_name)
     if shell_folder_name is None:
         raise ValueError(f"Unknown CSIDL name: {csidl_name}")
     if sys.platform != "win32":  # only needed for mypy type checker to know that this code runs only on Windows
         raise NotImplementedError
     import winreg
 
@@ -168,14 +179,15 @@
     """Get folder with ctypes."""
     csidl_const = {
         "CSIDL_APPDATA": 26,
         "CSIDL_COMMON_APPDATA": 35,
         "CSIDL_LOCAL_APPDATA": 28,
         "CSIDL_PERSONAL": 5,
         "CSIDL_MYPICTURES": 39,
+        "CSIDL_MYVIDEO": 14,
     }.get(csidl_name)
     if csidl_const is None:
         raise ValueError(f"Unknown CSIDL name: {csidl_name}")
 
     buf = ctypes.create_unicode_buffer(1024)
     windll = getattr(ctypes, "windll")  # noqa: B009 # using getattr to avoid false positive with mypy type checker
     windll.shell32.SHGetFolderPathW(None, csidl_const, None, 0, buf)
```

### Comparing `platformdirs-3.3.0/tests/conftest.py` & `platformdirs-3.4.0/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     "user_data_dir",
     "user_config_dir",
     "user_cache_dir",
     "user_state_dir",
     "user_log_dir",
     "user_documents_dir",
     "user_pictures_dir",
+    "user_videos_dir",
     "user_runtime_dir",
     "site_data_dir",
     "site_config_dir",
     "site_cache_dir",
 )
```

### Comparing `platformdirs-3.3.0/tests/test_android.py` & `platformdirs-3.4.0/tests/test_android.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         "site_config_dir": f"/data/data/com.example/shared_prefs{suffix}",
         "user_cache_dir": f"/data/data/com.example/cache{suffix}",
         "site_cache_dir": f"/data/data/com.example/cache{suffix}",
         "user_state_dir": f"/data/data/com.example/files{suffix}",
         "user_log_dir": f"/data/data/com.example/cache{suffix}{'' if params.get('opinion', True) is False else '/log'}",
         "user_documents_dir": "/storage/emulated/0/Documents",
         "user_pictures_dir": "/storage/emulated/0/Pictures",
+        "user_videos_dir": "/storage/emulated/0/DCIM/Camera",
         "user_runtime_dir": f"/data/data/com.example/cache{suffix}{'' if not params.get('opinion', True) else '/tmp'}",
     }
     expected = expected_map[func]
 
     assert result == expected
```

### Comparing `platformdirs-3.3.0/tests/test_api.py` & `platformdirs-3.4.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.3.0/tests/test_comp_with_appdirs.py` & `platformdirs-3.4.0/tests/test_comp_with_appdirs.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.3.0/tests/test_macos.py` & `platformdirs-3.4.0/tests/test_macos.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,12 +30,13 @@
         "site_config_dir": f"/Library/Application Support{suffix}",
         "user_cache_dir": f"{home}/Library/Caches{suffix}",
         "site_cache_dir": f"/Library/Caches{suffix}",
         "user_state_dir": f"{home}/Library/Application Support{suffix}",
         "user_log_dir": f"{home}/Library/Logs{suffix}",
         "user_documents_dir": f"{home}/Documents",
         "user_pictures_dir": f"{home}/Pictures",
+        "user_videos_dir": f"{home}/Movies",
         "user_runtime_dir": f"{home}/Library/Caches/TemporaryItems{suffix}",
     }
     expected = expected_map[func]
 
     assert result == expected
```

### Comparing `platformdirs-3.3.0/tests/test_unix.py` & `platformdirs-3.4.0/tests/test_unix.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,80 +9,63 @@
 import pytest
 from _pytest.monkeypatch import MonkeyPatch
 from pytest_mock import MockerFixture
 
 from platformdirs.unix import Unix
 
 
-def test_user_documents_dir(mocker: MockerFixture) -> None:
-    example_path = "/home/example/ExampleDocumentsFolder"
+@pytest.mark.parametrize("prop", ["user_documents_dir", "user_pictures_dir", "user_videos_dir"])
+def test_user_media_dir(mocker: MockerFixture, prop: str) -> None:
+    example_path = "/home/example/ExampleMediaFolder"
     mock = mocker.patch("platformdirs.unix._get_user_dirs_folder")
     mock.return_value = example_path
-    assert Unix().user_documents_dir == example_path
+    assert getattr(Unix(), prop) == example_path
 
 
-def test_user_documents_dir_env_var(mocker: MockerFixture) -> None:
-    # Mock documents dir not being in user-dirs.dirs file
+@pytest.mark.parametrize(
+    ("env_var", "prop"),
+    [
+        pytest.param("XDG_DOCUMENTS_DIR", "user_documents_dir", id="user_documents_dir"),
+        pytest.param("XDG_PICTURES_DIR", "user_pictures_dir", id="user_pictures_dir"),
+        pytest.param("XDG_VIDEOS_DIR", "user_videos_dir", id="user_videos_dir"),
+    ],
+)
+def test_user_media_dir_env_var(mocker: MockerFixture, env_var: str, prop: str) -> None:
+    # Mock media dir not being in user-dirs.dirs file
     mock = mocker.patch("platformdirs.unix._get_user_dirs_folder")
     mock.return_value = None
 
-    example_path = "/home/example/ExampleDocumentsFolder"
-    mocker.patch.dict(os.environ, {"XDG_DOCUMENTS_DIR": example_path})
+    example_path = "/home/example/ExampleMediaFolder"
+    mocker.patch.dict(os.environ, {env_var: example_path})
 
-    assert Unix().user_documents_dir == example_path
+    assert getattr(Unix(), prop) == example_path
 
 
-def test_user_documents_dir_default(mocker: MockerFixture) -> None:
-    # Mock documents dir not being in user-dirs.dirs file
+@pytest.mark.parametrize(
+    ("env_var", "prop", "default_abs_path"),
+    [
+        pytest.param("XDG_DOCUMENTS_DIR", "user_documents_dir", "/home/example/Documents", id="user_documents_dir"),
+        pytest.param("XDG_PICTURES_DIR", "user_pictures_dir", "/home/example/Pictures", id="user_pictures_dir"),
+        pytest.param("XDG_VIDEOS_DIR", "user_videos_dir", "/home/example/Videos", id="user_videos_dir"),
+    ],
+)
+def test_user_media_dir_default(mocker: MockerFixture, env_var: str, prop: str, default_abs_path: str) -> None:
+    # Mock media dir not being in user-dirs.dirs file
     mock = mocker.patch("platformdirs.unix._get_user_dirs_folder")
     mock.return_value = None
 
-    # Mock no XDG_DOCUMENTS_DIR env variable being set
-    mocker.patch.dict(os.environ, {"XDG_DOCUMENTS_DIR": ""})
+    # Mock no XDG env variable being set
+    mocker.patch.dict(os.environ, {env_var: ""})
 
     # Mock home directory
     mocker.patch.dict(os.environ, {"HOME": "/home/example"})
     # Mock home directory for running the test on Windows
     mocker.patch.dict(os.environ, {"USERPROFILE": "/home/example"})
 
-    assert Unix().user_documents_dir == "/home/example/Documents"
-
-
-def test_user_pictures_dir(mocker: MockerFixture) -> None:
-    example_path = "/home/example/ExamplePicturesFolder"
-    mock = mocker.patch("platformdirs.unix._get_user_dirs_folder")
-    mock.return_value = example_path
-    assert Unix().user_pictures_dir == example_path
-
-
-def test_user_pictures_dir_env_var(mocker: MockerFixture) -> None:
-    # Mock pictures dir not being in user-dirs.dirs file
-    mock = mocker.patch("platformdirs.unix._get_user_dirs_folder")
-    mock.return_value = None
-
-    example_path = "/home/example/ExamplePicturesFolder"
-    mocker.patch.dict(os.environ, {"XDG_PICTURES_DIR": example_path})
-
-    assert Unix().user_pictures_dir == example_path
-
-
-def test_user_pictures_dir_default(mocker: MockerFixture) -> None:
-    # Mock pictures dir not being in user-dirs.dirs file
-    mock = mocker.patch("platformdirs.unix._get_user_dirs_folder")
-    mock.return_value = None
-
-    # Mock no XDG_PICTURES_DIR env variable being set
-    mocker.patch.dict(os.environ, {"XDG_PICTURES_DIR": ""})
-
-    # Mock home directory
-    mocker.patch.dict(os.environ, {"HOME": "/home/example"})
-    # Mock home directory for running the test on Windows
-    mocker.patch.dict(os.environ, {"USERPROFILE": "/home/example"})
-
-    assert Unix().user_pictures_dir == "/home/example/Pictures"
+    assert getattr(Unix(), prop) == default_abs_path
 
 
 class XDGVariable(typing.NamedTuple):
     name: str
     default_value: str
```

### Comparing `platformdirs-3.3.0/LICENSE` & `platformdirs-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `platformdirs-3.3.0/README.rst` & `platformdirs-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `platformdirs-3.3.0/pyproject.toml` & `platformdirs-3.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `platformdirs-3.3.0/PKG-INFO` & `platformdirs-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platformdirs
-Version: 3.3.0
+Version: 3.4.0
 Summary: A small Python package for determining appropriate platform-specific dirs, e.g. a "user data dir".
 Project-URL: Documentation, https://platformdirs.readthedocs.io
 Project-URL: Homepage, https://github.com/platformdirs/platformdirs
 Project-URL: Source, https://github.com/platformdirs/platformdirs
 Project-URL: Tracker, https://github.com/platformdirs/platformdirs/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Julian Berman <Julian@GrayVines.com>, Ofek Lev <oss@ofek.dev>, Ronny Pfannschmidt <opensource@ronnypfannschmidt.de>
 License-Expression: MIT
```

