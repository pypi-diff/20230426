# Comparing `tmp/img2texture-1.0.6.tar.gz` & `tmp/img2texture-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "img2texture-1.0.6.tar", last modified: Sun Oct 16 14:08:57 2022, max compression
+gzip compressed data, was "img2texture-1.1.0.tar", last modified: Wed Apr 26 00:00:49 2023, max compression
```

## Comparing `img2texture-1.0.6.tar` & `img2texture-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 14:08:57.006425 img2texture-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-10-16 14:08:46.000000 img2texture-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3818 2022-10-16 14:08:57.006425 img2texture-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-10-16 14:08:46.000000 img2texture-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 14:08:57.006425 img2texture-1.0.6/img2texture/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-16 14:08:46.000000 img2texture-1.0.6/img2texture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-16 14:08:46.000000 img2texture-1.0.6/img2texture/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4374 2022-10-16 14:08:46.000000 img2texture-1.0.6/img2texture/_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-10-16 14:08:46.000000 img2texture-1.0.6/img2texture/_common.py
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-10-16 14:08:46.000000 img2texture-1.0.6/img2texture/_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4469 2022-10-16 14:08:46.000000 img2texture-1.0.6/img2texture/_texturizing.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-10-16 14:08:46.000000 img2texture-1.0.6/img2texture/_tiling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 14:08:57.006425 img2texture-1.0.6/img2texture.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3818 2022-10-16 14:08:56.000000 img2texture-1.0.6/img2texture.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-10-16 14:08:56.000000 img2texture-1.0.6/img2texture.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-16 14:08:56.000000 img2texture-1.0.6/img2texture.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-16 14:08:56.000000 img2texture-1.0.6/img2texture.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-16 14:08:56.000000 img2texture-1.0.6/img2texture.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-16 14:08:56.000000 img2texture-1.0.6/img2texture.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-16 14:08:57.006425 img2texture-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-10-16 14:08:46.000000 img2texture-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:00:49.313824 img2texture-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-26 00:00:31.000000 img2texture-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-26 00:00:49.313824 img2texture-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-26 00:00:31.000000 img2texture-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:00:49.313824 img2texture-1.1.0/img2texture/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 00:00:31.000000 img2texture-1.1.0/img2texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 00:00:31.000000 img2texture-1.1.0/img2texture/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-26 00:00:31.000000 img2texture-1.1.0/img2texture/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 00:00:31.000000 img2texture-1.1.0/img2texture/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-26 00:00:31.000000 img2texture-1.1.0/img2texture/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-04-26 00:00:31.000000 img2texture-1.1.0/img2texture/_texturizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-26 00:00:31.000000 img2texture-1.1.0/img2texture/_tiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 00:00:31.000000 img2texture-1.1.0/img2texture/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:00:49.313824 img2texture-1.1.0/img2texture.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-26 00:00:49.000000 img2texture-1.1.0/img2texture.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-26 00:00:49.000000 img2texture-1.1.0/img2texture.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:00:49.000000 img2texture-1.1.0/img2texture.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-26 00:00:49.000000 img2texture-1.1.0/img2texture.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 00:00:49.000000 img2texture-1.1.0/img2texture.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 00:00:49.000000 img2texture-1.1.0/img2texture.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 00:00:49.313824 img2texture-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-26 00:00:31.000000 img2texture-1.1.0/setup.py
```

### Comparing `img2texture-1.0.6/LICENSE` & `img2texture-1.1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Artsiom iG <github.com/rtmigo>
+Copyright (c) 2021 Artёm iG <github.com/rtmigo>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `img2texture-1.0.6/PKG-INFO` & `img2texture-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: img2texture
-Version: 1.0.6
+Version: 1.1.0
 Summary: Command line utility for converting images to seamless tiles.
 Home-page: https://github.com/rtmigo/img2texture#readme
-Author: Artsiom iG
+Author: Artёm iG
 Author-email: ortemeo@gmail.com
 License: MIT
 Keywords: photo,image,texture,tile,seamless
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -121,11 +121,31 @@
 
 ```bash
 img2texture source.jpg seamless.jpg --tile 
 ```
 
 All the samples on this page were created with `--tile`.
 
+# Use programmatically
+
+If you don't need CLI but need to create seamless image in your own program:
+
+```python3
+from PIL import Image
+from img2texture import image_to_seamless
+
+# load PIL image
+src_image = Image.open("/path/to/source.png")
+
+# convert to seamless PIL image
+result_image = image_to_seamless(src_image, overlap=0.1)
+
+# save
+result_image.save("/path/to/result.png")
+```
+
+`overlap=0.1` means 10%, and `overlap=(0.1, 0.2)` means 10% horizontal, 20% vertical. 
+
 # License
 
-Copyright © 2021 [Artsiom iG](https://github.com/rtmigo).
+Copyright © 2021 [Artёm iG](https://github.com/rtmigo).
 Released under the [MIT License](LICENSE).
```

### Comparing `img2texture-1.0.6/README.md` & `img2texture-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -100,11 +100,31 @@
 
 ```bash
 img2texture source.jpg seamless.jpg --tile 
 ```
 
 All the samples on this page were created with `--tile`.
 
+# Use programmatically
+
+If you don't need CLI but need to create seamless image in your own program:
+
+```python3
+from PIL import Image
+from img2texture import image_to_seamless
+
+# load PIL image
+src_image = Image.open("/path/to/source.png")
+
+# convert to seamless PIL image
+result_image = image_to_seamless(src_image, overlap=0.1)
+
+# save
+result_image.save("/path/to/result.png")
+```
+
+`overlap=0.1` means 10%, and `overlap=(0.1, 0.2)` means 10% horizontal, 20% vertical. 
+
 # License
 
-Copyright © 2021 [Artsiom iG](https://github.com/rtmigo).
+Copyright © 2021 [Artёm iG](https://github.com/rtmigo).
 Released under the [MIT License](LICENSE).
```

### Comparing `img2texture-1.0.6/img2texture/_cli.py` & `img2texture-1.1.0/img2texture/_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import argparse
 import os
 import sys
 import traceback
 from enum import Enum
 from pathlib import Path
 
+from PIL import Image
+
 import img2texture._constants as constants
-from img2texture import img2tex
+from img2texture import img2tex, file_to_seamless
 from ._tiling import tile
 
 
 def in_pyinstaller() -> bool:
     return getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS')
 
 
@@ -112,21 +114,27 @@
     basename += "_2x2.jpg"
     return texture.parent / basename
 
 
 def cli():
     args = ParsedArgs()
 
+    # preventing exception "Image.DecompressionBombError: Image size (324000000
+    # pixels) exceeds limit of 178956970 pixels, could be decompression bomb DOS
+    # attack". In case of CLI we are not expecting attacks. Just processing
+    # large files
+    Image.MAX_IMAGE_PIXELS = None
+
     try:
         if args.target.exists():
             if not confirm(f"File '{args.target.name}' exists. Overwrite?"):
                 sys.exit(3)
             os.remove(args.target)
 
-        img2tex(args.source, args.target, pct=args.overlap_pct)
+        file_to_seamless(args.source, args.target, overlap=args.overlap_pct)
 
         if args.tile:
             tile_src = args.target if args.mode != Mode.none else args.source
             tile_fn = tile_filename(tile_src)
             if tile_fn.exists() and not confirm(
                     f"File '{tile_fn}' exists. Overwrite?"):
                 sys.exit(3)
```

### Comparing `img2texture-1.0.6/img2texture/_texturizing.py` & `img2texture-1.1.0/img2texture/_texturizing.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# SPDX-FileCopyrightText: (c) 2021 Artsiom iG <github.com/rtmigo>
+# SPDX-FileCopyrightText: (c) 2021 Artёm iG <github.com/rtmigo>
 # SPDX-License-Identifier: MIT
+import warnings
 from math import floor
 from pathlib import Path
-from typing import Tuple
+from typing import Tuple, Union
 
 from ._common import Image  # importing with tweaked options
 
 
 # todo Find a way to add dithering noise to 8-bit grading
 #
 # It looks like in 2021 Pillow cannot alpha-blend 16-bit or 32-bit images.
@@ -74,22 +75,22 @@
         return stripe_size(self.src_height, self.pct)
 
     def _left_stripe_image(self):
         return self.source.crop(
             (0, 0, self.horizontal_stripe_width, self.src_height))
 
     def _right_stripe_image(self):
-        return self.source.crop(
-            (self.src_width - self.horizontal_stripe_width, 0,
-             self.src_width, self.src_height))
+        return self.source.crop((
+            self.src_width - self.horizontal_stripe_width, 0, self.src_width,
+            self.src_height))
 
     def _bottom_stripe_image(self):
-        return self.source.crop(
-            (0, self.src_height - self.vertical_stripe_height,
-             self.src_width, self.src_height))
+        return self.source.crop((
+            0, self.src_height - self.vertical_stripe_height, self.src_width,
+            self.src_height))
 
     def _to_rgba(self, image: Image) -> Image:
         if image.mode != 'RGBA':
             converted = image.convert('RGBA')
             assert converted is not None
             return converted
         return image
@@ -98,43 +99,67 @@
         stripe = self._to_rgba(self._right_stripe_image())
         stripe.putalpha(
             horizontal_gradient_256_scaled(stripe.size, reverse=False))
 
         overlay = Image.new('RGBA', size=self.source.size, color=0x00)
         overlay.paste(stripe, box=(0, 0))
 
-        comp = Image.alpha_composite(self._to_rgba(self.source),
-                                     overlay)
+        comp = Image.alpha_composite(self._to_rgba(self.source), overlay)
 
-        comp = comp.crop((0,
-                          0,
-                          comp.size[0] - self.horizontal_stripe_width,
-                          comp.size[1]))
+        comp = comp.crop(
+            (0, 0, comp.size[0] - self.horizontal_stripe_width, comp.size[1]))
         return comp
 
     def make_seamless_v(self) -> Image:
         stripe = self._to_rgba(self._bottom_stripe_image())
         stripe.putalpha(
             vertical_gradient_256_scaled(stripe.size, reverse=False))
 
         overlay = Image.new('RGBA', size=self.source.size, color=0x00)
         overlay.paste(stripe, box=(0, 0))
 
-        comp = Image.alpha_composite(self._to_rgba(self.source),
-                                     overlay)
+        comp = Image.alpha_composite(self._to_rgba(self.source), overlay)
 
-        comp = comp.crop((0,
-                          0,
-                          comp.size[0],
-                          comp.size[1] - self.vertical_stripe_height))
+        comp = comp.crop(
+            (0, 0, comp.size[0], comp.size[1] - self.vertical_stripe_height))
         return comp
 
 
 def img2tex(src: Path, dst: Path, pct=0.25):
-    mixer1 = Mixer(Image.open(src), pct=pct)
+    warnings.warn("Replaced by `file_to_seamless`", DeprecationWarning,
+                  stacklevel=2)
+    file_to_seamless(src, dst, overlap=pct)
+
+Overlap = Union[float, Tuple[float, float]]
+
+def file_to_seamless(src: Path, dst: Path, overlap: Overlap = 0.25) -> None:
+    """Reads image from `src` file, converts it to seamless tile and saves
+    to `dst` file."""
+    image_to_seamless(Image.open(src), overlap=overlap).save(dst)
+
+
+def image_to_seamless(src: Image, overlap: Overlap = 0.25) -> Image:
+    """Converts `PIL.Image` to seamless `PIL.Image`."""
+    mixer1 = Mixer(src, pct=_horizontal_overlap(overlap))
     result = mixer1.make_seamless_h()
 
-    mixer2 = Mixer(result, pct=pct)
+    mixer2 = Mixer(result, pct=_vertical_overlap(overlap))
     result = mixer2.make_seamless_v()
     if result.mode != "RGB":
         result = result.convert("RGB")
-    result.save(dst)
+    return result
+
+
+def _float_or_index(dynamic: Overlap,
+                    idx: int) -> float:
+    if isinstance(dynamic, float):
+        return dynamic
+    else:
+        return dynamic[idx]
+
+
+def _horizontal_overlap(overlaps: Overlap) -> float:
+    return _float_or_index(overlaps, 0)
+
+
+def _vertical_overlap(overlaps: Overlap) -> float:
+    return _float_or_index(overlaps, 1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `img2texture-1.0.6/img2texture/_tiling.py` & `img2texture-1.1.0/img2texture/_tiling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: (c) 2021 Artsiom iG <github.com/rtmigo>
+# SPDX-FileCopyrightText: (c) 2021 Artёm iG <github.com/rtmigo>
 # SPDX-License-Identifier: MIT
 
 from pathlib import Path
 
 from ._common import Image  # importing with tweaked options
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `img2texture-1.0.6/img2texture.egg-info/PKG-INFO` & `img2texture-1.1.0/img2texture.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: img2texture
-Version: 1.0.6
+Version: 1.1.0
 Summary: Command line utility for converting images to seamless tiles.
 Home-page: https://github.com/rtmigo/img2texture#readme
-Author: Artsiom iG
+Author: Artёm iG
 Author-email: ortemeo@gmail.com
 License: MIT
 Keywords: photo,image,texture,tile,seamless
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -121,11 +121,31 @@
 
 ```bash
 img2texture source.jpg seamless.jpg --tile 
 ```
 
 All the samples on this page were created with `--tile`.
 
+# Use programmatically
+
+If you don't need CLI but need to create seamless image in your own program:
+
+```python3
+from PIL import Image
+from img2texture import image_to_seamless
+
+# load PIL image
+src_image = Image.open("/path/to/source.png")
+
+# convert to seamless PIL image
+result_image = image_to_seamless(src_image, overlap=0.1)
+
+# save
+result_image.save("/path/to/result.png")
+```
+
+`overlap=0.1` means 10%, and `overlap=(0.1, 0.2)` means 10% horizontal, 20% vertical. 
+
 # License
 
-Copyright © 2021 [Artsiom iG](https://github.com/rtmigo).
+Copyright © 2021 [Artёm iG](https://github.com/rtmigo).
 Released under the [MIT License](LICENSE).
```

### Comparing `img2texture-1.0.6/setup.py` & `img2texture-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 readme = (Path(__file__).parent / 'README.md').read_text(encoding="utf-8")
 readme = "#"+readme.partition('\n#')[-1]
 
 setup(
     name=name,
     version=constants['__version__'],
 
-    author="Artsiom iG",
+    author="Artёm iG",
     author_email="ortemeo@gmail.com",
     url='https://github.com/rtmigo/img2texture#readme',
 
     packages=find_packages(include=[name, f'{name}.*']),
+    package_data={name: ["py.typed"]},
 
     python_requires='>=3.7, <4',
     install_requires=["pillow>=9.2, <10"],
 
     description="Command line utility for converting images to seamless tiles.",
     long_description=readme,
     long_description_content_type='text/markdown',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

