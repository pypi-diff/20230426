# Comparing `tmp/mediaify-3.0.0.tar.gz` & `tmp/mediaify-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediaify-3.0.0.tar", last modified: Tue Apr 25 23:09:00 2023, max compression
+gzip compressed data, was "mediaify-3.0.1.tar", last modified: Wed Apr 26 00:08:51 2023, max compression
```

## Comparing `mediaify-3.0.0.tar` & `mediaify-3.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1147 2023-04-25 23:08:50.669186 mediaify-3.0.0/LICENSE
--rw-r--r--   0        0        0     4126 2023-04-25 23:08:50.669186 mediaify-3.0.0/README.md
--rw-r--r--   0        0        0     1770 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/__init__.py
--rw-r--r--   0        0        0      198 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/animation/__init__.py
--rw-r--r--   0        0        0     2397 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/animation/encode.py
--rw-r--r--   0        0        0     1272 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/animation/exports.py
--rw-r--r--   0        0        0     2559 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/animation/formats.py
--rw-r--r--   0        0        0     1280 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/animation/utils.py
--rw-r--r--   0        0        0      143 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/audio/__init__.py
--rw-r--r--   0        0        0      914 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/audio/encode.py
--rw-r--r--   0        0        0      989 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/audio/exports.py
--rw-r--r--   0        0        0     2046 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/audio/formats.py
--rw-r--r--   0        0        0     1243 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/configs/__init__.py
--rw-r--r--   0        0        0     1021 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/configs/animation.py
--rw-r--r--   0        0        0      884 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/configs/audio.py
--rw-r--r--   0        0        0      599 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/configs/base.py
--rw-r--r--   0        0        0     2121 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/configs/codecs.py
--rw-r--r--   0        0        0     1387 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/configs/image.py
--rw-r--r--   0        0        0      770 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/configs/resize.py
--rw-r--r--   0        0        0      486 2023-04-25 23:08:50.765186 mediaify-3.0.0/mediaify/configs/shared.py
--rw-r--r--   0        0        0     2418 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/configs/video.py
--rw-r--r--   0        0        0     3672 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/files.py
--rw-r--r--   0        0        0        0 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/format.py
--rw-r--r--   0        0        0      162 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/image/__init__.py
--rw-r--r--   0        0        0     1948 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/image/encode.py
--rw-r--r--   0        0        0     1149 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/image/exports.py
--rw-r--r--   0        0        0     2078 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/image/formats.py
--rw-r--r--   0        0        0      977 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/resize.py
--rw-r--r--   0        0        0      995 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/utils.py
--rw-r--r--   0        0        0      175 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/video/__init__.py
--rw-r--r--   0        0        0     2330 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/video/codecs.py
--rw-r--r--   0        0        0     1212 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/video/encode.py
--rw-r--r--   0        0        0     1424 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/video/exports.py
--rw-r--r--   0        0        0     2752 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/video/formats.py
--rw-r--r--   0        0        0     1303 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/video/info.py
--rw-r--r--   0        0        0     2816 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/video/process.py
--rw-r--r--   0        0        0     1451 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/video/summary.py
--rw-r--r--   0        0        0     1057 2023-04-25 23:08:50.769186 mediaify-3.0.0/mediaify/video/thumbnail.py
--rw-r--r--   0        0        0     1723 2023-04-25 23:08:50.769186 mediaify-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     5586 1970-01-01 00:00:00.000000 mediaify-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1147 2023-04-26 00:08:32.929485 mediaify-3.0.1/LICENSE
+-rw-r--r--   0        0        0     3830 2023-04-26 00:08:32.929485 mediaify-3.0.1/README.md
+-rw-r--r--   0        0        0     1770 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/animation/__init__.py
+-rw-r--r--   0        0        0     2397 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/animation/encode.py
+-rw-r--r--   0        0        0     1272 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/animation/exports.py
+-rw-r--r--   0        0        0     2559 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/animation/formats.py
+-rw-r--r--   0        0        0     1280 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/animation/utils.py
+-rw-r--r--   0        0        0      143 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/audio/__init__.py
+-rw-r--r--   0        0        0      914 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/audio/encode.py
+-rw-r--r--   0        0        0      989 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/audio/exports.py
+-rw-r--r--   0        0        0     2046 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/audio/formats.py
+-rw-r--r--   0        0        0     1243 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/__init__.py
+-rw-r--r--   0        0        0     1021 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/animation.py
+-rw-r--r--   0        0        0      884 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/audio.py
+-rw-r--r--   0        0        0      599 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/base.py
+-rw-r--r--   0        0        0     2119 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/codecs.py
+-rw-r--r--   0        0        0     1387 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/image.py
+-rw-r--r--   0        0        0      770 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/resize.py
+-rw-r--r--   0        0        0      486 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/shared.py
+-rw-r--r--   0        0        0     2418 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/video.py
+-rw-r--r--   0        0        0     3672 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/files.py
+-rw-r--r--   0        0        0        0 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/format.py
+-rw-r--r--   0        0        0      162 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/image/__init__.py
+-rw-r--r--   0        0        0     1948 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/image/encode.py
+-rw-r--r--   0        0        0     1149 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/image/exports.py
+-rw-r--r--   0        0        0     2078 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/image/formats.py
+-rw-r--r--   0        0        0      977 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/resize.py
+-rw-r--r--   0        0        0      995 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/utils.py
+-rw-r--r--   0        0        0      175 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/__init__.py
+-rw-r--r--   0        0        0     2330 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/codecs.py
+-rw-r--r--   0        0        0     1212 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/encode.py
+-rw-r--r--   0        0        0     1424 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/exports.py
+-rw-r--r--   0        0        0     2752 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/formats.py
+-rw-r--r--   0        0        0     1303 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/info.py
+-rw-r--r--   0        0        0     2822 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/process.py
+-rw-r--r--   0        0        0     1451 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/summary.py
+-rw-r--r--   0        0        0     1057 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/thumbnail.py
+-rw-r--r--   0        0        0     1743 2023-04-26 00:08:33.045485 mediaify-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5318 1970-01-01 00:00:00.000000 mediaify-3.0.1/PKG-INFO
```

### Comparing `mediaify-3.0.0/LICENSE` & `mediaify-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/README.md` & `mediaify-3.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,112 +5,114 @@
 
 Encode media without the hassle of wrangling ffmpeg and pillow, instead declare your output declaratively!
 
 [Documentation](https://mediaify.readthedocs.io/)
 
 [![Documentation Status](https://readthedocs.org/projects/mediaify/badge/?version=latest)](https://mediaify.readthedocs.io/en/latest/?badge=latest)
 
-## Simple
-
 ```python
 import mediaify
 
 with open('./image.png', 'rb') as f:
     data = f.read()
 
-mediaify.encode_image(data, mediaify.WEBPImageFormat(quality=90))
->>> ImageFile(1200x1600, image/webp, 162.6KB)
+image = mediaify.encode_image(data, mediaify.WEBPImageFormat(quality=90))
+image.save("./image.webp")
+```
+
+## Multimedia Support
+
+Supports transcoding of several different media types.
+
+- Audio
+- Image
+- Animation
+- Video
+
+```python
+with open("./audio.mp4", "rb") as f:
+    data = f.read()
+
+mediaify.encode_audio(data)
+>>> AudioFile(audio/mpeg, 2.5MB)
+
+with open("./image.png", "rb") as f:
+    data = f.read()
+
+mediaify.encode_image(data)
+>>> ImageFile(1200x1600, image/png, 35.4KB)
+
+
+with open("./animation.gif", "rb") as f:
+    data = f.read()
+
+mediaify.encode_animation(data)
+>>> AnimationFile(1280x800, 1.1s 11 frames, 10.0fps, image/gif, 132.8KB)
+
+
+with open("./examples/input/video.mp4", "rb") as f:
+    data = f.read()
+
+mediaify.encode_video(data)
+>>> VideoFile(1280x720, 60.458s, 24.0fps, audio, video/mp4, 8.5MB)
 ```
 
 ## Customisable
 
 Encode videos with multiple resolutions, formats, codecs as well as thumbnails and previews easily.
 
 ```python
 import mediaify
 
 thumbnail = mediaify.ThumbnailEncoding(
     encoding=mediaify.WEBPImageFormat(
-        resize=mediaify.TargetResolutionResize(width=192, height=108),
+        resize=mediaify.TargetResolutionResize(width=640, height=360),
         quality=80,
     ),
 )
 preview = mediaify.VideoPreviewAnimationEncoding(
     encoding=mediaify.WEBPAnimationFormat(
+        quality=50,
+        lossless=False,
         resize=mediaify.TargetResolutionResize(width=640, height=360)
-    )
-)
-fallback = mediaify.MP4Format(
-    video_codec=mediaify.H264Codec(crf=21, preset="medium"),
-    audio_codec=mediaify.OpusCodec(bitrate=128_000),
-    resize=mediaify.TargetResolutionResize(width=1280, height=720),
+    ),
+    framerate=5,
+    frames=60,
 )
-video_144p = mediaify.WEBMFormat(
-    video_codec=mediaify.AV1Codec(crf=55, preset=8),
+video_360p = mediaify.WEBMFormat(
+    video_codec=mediaify.AV1Codec(crf=50, preset=7),
     audio_codec=mediaify.OpusCodec(bitrate=128_000),
-    resize=mediaify.TargetResolutionResize(width=256, height=144),
+    resize=mediaify.TargetResolutionResize(width=640, height=360),
 )
 video_720p = mediaify.WEBMFormat(
     video_codec=mediaify.AV1Codec(crf=45, preset=6),
     audio_codec=mediaify.OpusCodec(bitrate=128_000),
     resize=mediaify.TargetResolutionResize(width=1280, height=720),
 )
+fallback = mediaify.MP4Format(
+    video_codec=mediaify.H264Codec(crf=21, preset="medium"),
+    audio_codec=mediaify.OpusCodec(bitrate=128_000),
+    resize=mediaify.TargetResolutionResize(width=1280, height=720),
+)
 
-configs = [thumbnail, preview, fallback, video_144p, video_720p]
+
+configs = [thumbnail, preview, video_360p, video_720p, fallback]
 with open('./examples/input/video.mp4', 'rb') as f:
     data = f.read()
 
 mediaify.batch_encode_video(data, configs)
 >>> [
-    ImageFile(192x108, image/webp, 2.2KB),
-    AnimationFile(1280x720, 2.99s 45 frames, 15.05fps, image/webp, 4.5MB),
-    VideoFile(1280x720, 60.458s, 24.0fps, audio, video/mp4, 14.7MB),
-    VideoFile(256x144, 34824.0s, 24.0fps, audio, video/webm, 1.3MB),
-    VideoFile(1280x720, 34824.0s, 24.0fps, audio, video/webm, 4.1MB),
+    ImageFile(640x360, image/webp, 10.1KB),
+    AnimationFile(640x360, 12.0s 60 frames, 5.0fps, image/webp, 1.8MB),
+    VideoFile(640x360, 60.45s, 24.0fps, audio, video/webm, 2.2MB),
+    VideoFile(1280x720, 60.45s, 24.0fps, audio, video/webm, 4.2MB),
+    VideoFile(1280x720, 60.45s, 24.0fps, audio, video/mp4, 14.2MB),
 ]
 ```
 
-| Thumbnail | Summary | Fallback | 144p | 720 |
-| - | - | - | - | - |
-| ![](./examples/output/video_encoding-thumbnail.webp) | ![](./examples/output/video_encoding-preview.webp) | ![](./examples/output/video_encoding-fallback.mp4) | ![](./examples/output/video_encoding-144p.webm) | ![](./examples/output/video_encoding-720p.webm) |
-
-
-## Multimedia Support
-
-Supports transcoding of several different media types.
-
-- Audio
-- Image
-- Animation
-- Video
-
-```python
-with open("./image.png", "rb") as f:
-    data = f.read()
-    print(mediaify.encode_audio(data))
-
-with open("./image.png", "rb") as f:
-    data = f.read()
-    print(mediaify.encode_image(data))
-
-
-with open("./animation.gif", "rb") as f:
-    data = f.read()
-    print(mediaify.encode_animation(data))
-
-
-with open("./examples/input/video.mp4", "rb") as f:
-    data = f.read()
-    print(mediaify.encode_video(data))
-
->>> ImageFile(1200x1600, image/png, 35.4KB)
->>> AnimationFile(1280x800, 1.1s 11 frames, 10.00fps, image/gif, 132.8KB)
->>> VideoFile(1242x1242, 17.800s, 25.0fps, audio, video/mp4, 4.2MB)
-```
-
 # Installation
 
 [https://pypi.org/project/mediaify/](https://pypi.org/project/mediaify/)
 
 ```bash
 python -m pip install mediaify
 ```
```

### Comparing `mediaify-3.0.0/mediaify/__init__.py` & `mediaify-3.0.1/mediaify/__init__.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/animation/encode.py` & `mediaify-3.0.1/mediaify/animation/encode.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/animation/exports.py` & `mediaify-3.0.1/mediaify/animation/exports.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/animation/formats.py` & `mediaify-3.0.1/mediaify/animation/formats.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/animation/utils.py` & `mediaify-3.0.1/mediaify/animation/utils.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/audio/encode.py` & `mediaify-3.0.1/mediaify/audio/encode.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/audio/exports.py` & `mediaify-3.0.1/mediaify/audio/exports.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/audio/formats.py` & `mediaify-3.0.1/mediaify/audio/formats.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/configs/__init__.py` & `mediaify-3.0.1/mediaify/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/configs/animation.py` & `mediaify-3.0.1/mediaify/configs/animation.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/configs/audio.py` & `mediaify-3.0.1/mediaify/configs/audio.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/configs/base.py` & `mediaify-3.0.1/mediaify/configs/base.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/configs/codecs.py` & `mediaify-3.0.1/mediaify/configs/codecs.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     The speed to encode the video at, slower means lower filesize at same quality.
 
     From fastest to slowest:
         `ultrafast`, `superfast`, `veryfast`, `faster`, `fast`,
         `medium`, `slow`, `slower`, `veryslow`, `placebo`
     """
     def __repr__(self) -> str:
-        return f"<H264 '{self.preset}' crf={self.crf}>"
+        return f"H264('{self.preset}' crf={self.crf})"
 
 
 
 @dataclass
 class VP9Codec:
     "The VP9 video codec"
     crf: int = 21
@@ -37,15 +37,15 @@
     The speed to encode the video at, slower means lower filesize at same quality.
     \n`realtime` is the fastest, worst quality
     \n`good` is the default, a mix of speed and file size, default
     \n`best` is the slowest, smallest file size
     """
 
     def __repr__(self) -> str:
-        return f"VP9('{self.preset}' crf={self.crf})>"
+        return f"VP9('{self.preset}' crf={self.crf})"
 
 
 @dataclass
 class AV1Codec:
     "The AV1 video codec"
     crf: int = 50
     """Constant Rate Factor. Lower is better quality, but larger file size.\n
@@ -53,15 +53,15 @@
     preset: Literal[0, 1, 2, 3, 4, 5, 6, 7, 8] = 5
     """The speed to encode the video at,
     slower means lower filesize at same quality.
     \n0 is the slowest, best quality. 8 is the fastest, worst quality.
     """
 
     def __repr__(self) -> str:
-        return f"AV1({self.preset} preset crf={self.crf})"
+        return f"AV1(preset:{self.preset} crf={self.crf})"
 
 
 @dataclass
 class OpusCodec:
     "The Opus audio codec"
     bitrate: int = 128_000
     "The bitrate to encode the audio in bits per second, defaults to 128kbps"
```

### Comparing `mediaify-3.0.0/mediaify/configs/image.py` & `mediaify-3.0.1/mediaify/configs/image.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/configs/resize.py` & `mediaify-3.0.1/mediaify/configs/resize.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/configs/video.py` & `mediaify-3.0.1/mediaify/configs/video.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/files.py` & `mediaify-3.0.1/mediaify/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     "Does this video contain audio?"
 
     def __repr__(self) -> str:
         FORMAT = "VideoFile({w}x{h}, {dur}s, {fps}fps, {audio}, {mime}, {size})"
         return FORMAT.format(
             w=self.width,
             h=self.height,
-            dur=round(self.duration, 3),
+            dur=round(self.duration, 2),
             fps=round(self.framerate, 2),
             audio="audio" if self.hasAudio else "no audio",
             mime=self.mimetype,
             size=format_bytes(len(self.data)),
         )
```

### Comparing `mediaify-3.0.0/mediaify/image/encode.py` & `mediaify-3.0.1/mediaify/image/encode.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/image/exports.py` & `mediaify-3.0.1/mediaify/image/exports.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/image/formats.py` & `mediaify-3.0.1/mediaify/image/formats.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/resize.py` & `mediaify-3.0.1/mediaify/resize.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/utils.py` & `mediaify-3.0.1/mediaify/utils.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/video/codecs.py` & `mediaify-3.0.1/mediaify/video/codecs.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/video/encode.py` & `mediaify-3.0.1/mediaify/video/encode.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/video/exports.py` & `mediaify-3.0.1/mediaify/video/exports.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/video/formats.py` & `mediaify-3.0.1/mediaify/video/formats.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/video/info.py` & `mediaify-3.0.1/mediaify/video/info.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/video/process.py` & `mediaify-3.0.1/mediaify/video/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,16 @@
     progress_bar = tqdm(
         total=frames,
         desc=encoding_name,
         unit="frame"
     )
 
     last_frame = 0
-    ffmpeg.on("progress")
+    
+    @ffmpeg.on("progress")
     def on_progress(progress: Progress) -> None:
         nonlocal last_frame
         frames_processed = progress.frame - last_frame
         progress_bar.update(frames_processed)
         last_frame = progress.frame
 
     @ffmpeg.on("completed")
```

### Comparing `mediaify-3.0.0/mediaify/video/summary.py` & `mediaify-3.0.1/mediaify/video/summary.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/mediaify/video/thumbnail.py` & `mediaify-3.0.1/mediaify/video/thumbnail.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.0/pyproject.toml` & `mediaify-3.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.8.0,<4"]
 
 [project]
 name = "mediaify"
-version = "3.0.0"
+version = "3.0.1"
 description = "Media encoding made simple"
 license = {file = "LICENSE"}
 readme = "README.md"
 authors = [
     {name = "Ben Brady", email = "benbradybusiness@gmail.com"},
 ]
 classifiers = [
@@ -26,14 +26,15 @@
     "Topic :: Multimedia :: Graphics :: Graphics Conversion",
     "Topic :: Multimedia :: Video",
     "Topic :: Multimedia :: Video :: Conversion",
     "Typing :: Typed",
 ]
 requires-python = ">=3.9"
 dependencies = [
+    "tqdm~=4.65.0",
     "python-ffmpeg~=2.0.4",
     "MediaInfo~=0.0.9",
     "pillow~=9.5.0",
     "python_magic~=0.4.27",
     "python-magic-bin; sys_platform == 'win32'",
     "numexpr",
 ]
```

### Comparing `mediaify-3.0.0/PKG-INFO` & `mediaify-3.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediaify
-Version: 3.0.0
+Version: 3.0.1
 Summary: Media encoding made simple
 Author-email: Ben Brady <benbradybusiness@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Multimedia :: Video :: Conversion
 Classifier: Typing :: Typed
+Requires-Dist: tqdm~=4.65.0
 Requires-Dist: python-ffmpeg~=2.0.4
 Requires-Dist: MediaInfo~=0.0.9
 Requires-Dist: pillow~=9.5.0
 Requires-Dist: python_magic~=0.4.27
 Requires-Dist: python-magic-bin; sys_platform == 'win32'
 Requires-Dist: numexpr
 Requires-Dist: libmagic ; extra == "docs"
@@ -42,112 +43,114 @@
 
 Encode media without the hassle of wrangling ffmpeg and pillow, instead declare your output declaratively!
 
 [Documentation](https://mediaify.readthedocs.io/)
 
 [![Documentation Status](https://readthedocs.org/projects/mediaify/badge/?version=latest)](https://mediaify.readthedocs.io/en/latest/?badge=latest)
 
-## Simple
-
 ```python
 import mediaify
 
 with open('./image.png', 'rb') as f:
     data = f.read()
 
-mediaify.encode_image(data, mediaify.WEBPImageFormat(quality=90))
->>> ImageFile(1200x1600, image/webp, 162.6KB)
+image = mediaify.encode_image(data, mediaify.WEBPImageFormat(quality=90))
+image.save("./image.webp")
+```
+
+## Multimedia Support
+
+Supports transcoding of several different media types.
+
+- Audio
+- Image
+- Animation
+- Video
+
+```python
+with open("./audio.mp4", "rb") as f:
+    data = f.read()
+
+mediaify.encode_audio(data)
+>>> AudioFile(audio/mpeg, 2.5MB)
+
+with open("./image.png", "rb") as f:
+    data = f.read()
+
+mediaify.encode_image(data)
+>>> ImageFile(1200x1600, image/png, 35.4KB)
+
+
+with open("./animation.gif", "rb") as f:
+    data = f.read()
+
+mediaify.encode_animation(data)
+>>> AnimationFile(1280x800, 1.1s 11 frames, 10.0fps, image/gif, 132.8KB)
+
+
+with open("./examples/input/video.mp4", "rb") as f:
+    data = f.read()
+
+mediaify.encode_video(data)
+>>> VideoFile(1280x720, 60.458s, 24.0fps, audio, video/mp4, 8.5MB)
 ```
 
 ## Customisable
 
 Encode videos with multiple resolutions, formats, codecs as well as thumbnails and previews easily.
 
 ```python
 import mediaify
 
 thumbnail = mediaify.ThumbnailEncoding(
     encoding=mediaify.WEBPImageFormat(
-        resize=mediaify.TargetResolutionResize(width=192, height=108),
+        resize=mediaify.TargetResolutionResize(width=640, height=360),
         quality=80,
     ),
 )
 preview = mediaify.VideoPreviewAnimationEncoding(
     encoding=mediaify.WEBPAnimationFormat(
+        quality=50,
+        lossless=False,
         resize=mediaify.TargetResolutionResize(width=640, height=360)
-    )
-)
-fallback = mediaify.MP4Format(
-    video_codec=mediaify.H264Codec(crf=21, preset="medium"),
-    audio_codec=mediaify.OpusCodec(bitrate=128_000),
-    resize=mediaify.TargetResolutionResize(width=1280, height=720),
+    ),
+    framerate=5,
+    frames=60,
 )
-video_144p = mediaify.WEBMFormat(
-    video_codec=mediaify.AV1Codec(crf=55, preset=8),
+video_360p = mediaify.WEBMFormat(
+    video_codec=mediaify.AV1Codec(crf=50, preset=7),
     audio_codec=mediaify.OpusCodec(bitrate=128_000),
-    resize=mediaify.TargetResolutionResize(width=256, height=144),
+    resize=mediaify.TargetResolutionResize(width=640, height=360),
 )
 video_720p = mediaify.WEBMFormat(
     video_codec=mediaify.AV1Codec(crf=45, preset=6),
     audio_codec=mediaify.OpusCodec(bitrate=128_000),
     resize=mediaify.TargetResolutionResize(width=1280, height=720),
 )
+fallback = mediaify.MP4Format(
+    video_codec=mediaify.H264Codec(crf=21, preset="medium"),
+    audio_codec=mediaify.OpusCodec(bitrate=128_000),
+    resize=mediaify.TargetResolutionResize(width=1280, height=720),
+)
 
-configs = [thumbnail, preview, fallback, video_144p, video_720p]
+
+configs = [thumbnail, preview, video_360p, video_720p, fallback]
 with open('./examples/input/video.mp4', 'rb') as f:
     data = f.read()
 
 mediaify.batch_encode_video(data, configs)
 >>> [
-    ImageFile(192x108, image/webp, 2.2KB),
-    AnimationFile(1280x720, 2.99s 45 frames, 15.05fps, image/webp, 4.5MB),
-    VideoFile(1280x720, 60.458s, 24.0fps, audio, video/mp4, 14.7MB),
-    VideoFile(256x144, 34824.0s, 24.0fps, audio, video/webm, 1.3MB),
-    VideoFile(1280x720, 34824.0s, 24.0fps, audio, video/webm, 4.1MB),
+    ImageFile(640x360, image/webp, 10.1KB),
+    AnimationFile(640x360, 12.0s 60 frames, 5.0fps, image/webp, 1.8MB),
+    VideoFile(640x360, 60.45s, 24.0fps, audio, video/webm, 2.2MB),
+    VideoFile(1280x720, 60.45s, 24.0fps, audio, video/webm, 4.2MB),
+    VideoFile(1280x720, 60.45s, 24.0fps, audio, video/mp4, 14.2MB),
 ]
 ```
 
-| Thumbnail | Summary | Fallback | 144p | 720 |
-| - | - | - | - | - |
-| ![](./examples/output/video_encoding-thumbnail.webp) | ![](./examples/output/video_encoding-preview.webp) | ![](./examples/output/video_encoding-fallback.mp4) | ![](./examples/output/video_encoding-144p.webm) | ![](./examples/output/video_encoding-720p.webm) |
-
-
-## Multimedia Support
-
-Supports transcoding of several different media types.
-
-- Audio
-- Image
-- Animation
-- Video
-
-```python
-with open("./image.png", "rb") as f:
-    data = f.read()
-    print(mediaify.encode_audio(data))
-
-with open("./image.png", "rb") as f:
-    data = f.read()
-    print(mediaify.encode_image(data))
-
-
-with open("./animation.gif", "rb") as f:
-    data = f.read()
-    print(mediaify.encode_animation(data))
-
-
-with open("./examples/input/video.mp4", "rb") as f:
-    data = f.read()
-    print(mediaify.encode_video(data))
-
->>> ImageFile(1200x1600, image/png, 35.4KB)
->>> AnimationFile(1280x800, 1.1s 11 frames, 10.00fps, image/gif, 132.8KB)
->>> VideoFile(1242x1242, 17.800s, 25.0fps, audio, video/mp4, 4.2MB)
-```
-
 # Installation
 
 [https://pypi.org/project/mediaify/](https://pypi.org/project/mediaify/)
 
 ```bash
 python -m pip install mediaify
 ```
```

