# Comparing `tmp/spotify-aac-downloader-1.1.tar.gz` & `tmp/spotify-aac-downloader-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify-aac-downloader-1.1.tar", last modified: Fri Mar 17 17:42:59 2023, max compression
+gzip compressed data, was "spotify-aac-downloader-1.2.tar", last modified: Tue Apr 25 17:49:46 2023, max compression
```

## Comparing `spotify-aac-downloader-1.1.tar` & `spotify-aac-downloader-1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1137 2023-03-17 17:42:50.883851 spotify-aac-downloader-1.1/.github/workflows/main.yml
--rw-r--r--   0        0        0       96 2023-03-17 17:42:50.887851 spotify-aac-downloader-1.1/.gitignore
--rw-r--r--   0        0        0     2694 2023-03-17 17:42:50.887851 spotify-aac-downloader-1.1/README.md
--rw-r--r--   0        0        0      536 2023-03-17 17:42:50.887851 spotify-aac-downloader-1.1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-17 17:42:50.887851 spotify-aac-downloader-1.1/requirements.txt
--rw-r--r--   0        0        0     4854 2023-03-17 17:42:50.887851 spotify-aac-downloader-1.1/spotify_aac_downloader/__init__.py
--rw-r--r--   0        0        0       58 2023-03-17 17:42:50.887851 spotify-aac-downloader-1.1/spotify_aac_downloader/__main__.py
--rw-r--r--   0        0        0    11046 2023-03-17 17:42:50.887851 spotify-aac-downloader-1.1/spotify_aac_downloader/spotify_aac_downloader.py
--rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 spotify-aac-downloader-1.1/PKG-INFO
+-rw-r--r--   0        0        0     1137 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/.github/workflows/main.yml
+-rw-r--r--   0        0        0       96 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/.gitignore
+-rw-r--r--   0        0        0     2742 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/README.md
+-rw-r--r--   0        0        0      536 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/requirements.txt
+-rw-r--r--   0        0        0     4619 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/spotify_aac_downloader/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/spotify_aac_downloader/__main__.py
+-rw-r--r--   0        0        0    10581 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/spotify_aac_downloader/spotify_aac_downloader.py
+-rw-r--r--   0        0        0     3130 1970-01-01 00:00:00.000000 spotify-aac-downloader-1.2/PKG-INFO
```

### Comparing `spotify-aac-downloader-1.1/.github/workflows/main.yml` & `spotify-aac-downloader-1.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `spotify-aac-downloader-1.1/README.md` & `spotify-aac-downloader-1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,31 @@
+Metadata-Version: 2.1
+Name: spotify-aac-downloader
+Version: 1.2
+Summary: Download songs/albums/playlists directly from Spotify in AAC
+Author: glomatico
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: pywidevine
+Requires-Dist: pyyaml
+Requires-Dist: pybase62
+Requires-Dist: yt-dlp
+Project-URL: repository, https://github.com/glomatico/spotify-aac-downloader
+
 # Spotify ✨ AAC ✨ Downloader
 A Python script to download songs/albums/playlists directly from Spotify in 256kbps/128kbps AAC.
 
 ## Setup
 1. Install Python 3.7 or newer
 2. Install spotify-aac-downloader with pip
     ```
     pip install spotify-aac-downloader
     ```
-3. Add mp4decrypt and ffmpeg to your PATH
-    * You can get them from here:
-        * mp4decrypt: https://www.bento4.com/downloads/
-        * ffmpeg: https://ffmpeg.org/download.html
+3. Add FFMPEG to your PATH. You can get it from here: https://ffmpeg.org/download.html
+    * If you are on Windows you can move the ffmpeg.exe file to the same folder that you will run the script instead of adding it to your PATH.
 4. Export your Spotify cookies as `cookies.txt` to the same folder that you will run the script
     * You can export your cookies by using this Google Chrome extension on Spotify website: https://chrome.google.com/webstore/detail/open-cookiestxt/gdocmgbfkjnnpapoeobnolbbkoibbcif. Make sure to be logged in.
 5. Put your Widevine Device file (.wvd) in the same folder that you will run the script
     * You can use Dumper to dump your phone's L3 CDM: https://github.com/Diazole/dumper. Once you have the L3 CDM, you can use pywidevine to create the .wvd file from it.
         1. Install pywidevine with pip
             ```
             pip install pywidevine pyyaml
@@ -52,7 +63,8 @@
                         Download 256kbps AAC instead of 128kbps AAC (default: False)
   -o, --overwrite       Overwrite existing files (default: False)
   -s, --skip-cleanup    Skip cleanup (default: False)
   -e, --print-exceptions
                         Print execeptions (default: False)
   -v, --version         show program's version number and exit
 ```
+
```

### Comparing `spotify-aac-downloader-1.1/pyproject.toml` & `spotify-aac-downloader-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spotify-aac-downloader-1.1/spotify_aac_downloader/__init__.py` & `spotify-aac-downloader-1.2/spotify_aac_downloader/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import shutil
 import argparse
 import traceback
 from .spotify_aac_downloader import SpotifyAacDownloader
 
-__version__ = '1.1'
+__version__ = '1.2'
 
 
 def main():
-    if not shutil.which('mp4decrypt'):
-        raise Exception('mp4decrypt is not on PATH')
     if not shutil.which('ffmpeg'):
         raise Exception('ffmpeg is not on PATH')
     parser = argparse.ArgumentParser(
         description = 'Download songs/albums/playlists directly from Spotify in AAC',
         formatter_class = argparse.ArgumentDefaultsHelpFormatter
     )
     parser.add_argument(
@@ -124,22 +122,20 @@
                 unsynced_lyrics, synced_lyrics = dl.get_lyrics(track_id)
                 tags = dl.get_tags(metadata, unsynced_lyrics)
                 final_location = dl.get_final_location(tags)
                 if not args.overwrite and final_location.exists():
                     continue
                 file_id = dl.get_file_id(metadata)
                 pssh = dl.get_pssh(file_id)
-                decryption_keys = dl.get_decryption_keys(pssh)
+                decryption_key = dl.get_decryption_key(pssh)
                 stream_url = dl.get_stream_url(file_id)
                 encrypted_location = dl.get_encrypted_location(track_id)
                 dl.download(encrypted_location, stream_url)
-                decrypted_location = dl.get_decrypted_location(track_id)
-                dl.decrypt(decryption_keys, encrypted_location, decrypted_location)
                 fixed_location = dl.get_fixed_location(track_id)
-                dl.fixup(decrypted_location, fixed_location)
+                dl.fixup(decryption_key, encrypted_location, fixed_location)
                 dl.make_final(fixed_location, final_location, tags)
                 dl.make_lrc(final_location, synced_lyrics)
             except KeyboardInterrupt:
                 exit(1)
             except:
                 error_count += 1
                 print(f'Failed to download "{track["name"]}" (track {j + 1}/{len(url)} from URL {i + 1}/{len(download_queue)})')
```

### Comparing `spotify-aac-downloader-1.1/spotify_aac_downloader/spotify_aac_downloader.py` & `spotify-aac-downloader-1.2/spotify_aac_downloader/spotify_aac_downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,34 +41,34 @@
             'referer': 'https://open.spotify.com/',
             'sec-ch-ua': '"Not?A_Brand";v="8", "Chromium";v="108", "Google Chrome";v="108"',
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"Windows"',
             'sec-fetch-dest': 'empty',
             'sec-fetch-mode': 'cors',
             'sec-fetch-site': 'same-site',
-            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36'
+            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36',
         })
         self.session.cookies.update(cookies)
         web_page = self.session.get('https://open.spotify.com/').text
         token = re.search(r'accessToken":"(.*?)"', web_page).group(1)
         self.session.headers.update({
             'authorization': f'Bearer {token}'
         })
     
 
     def get_download_queue(self, url):
         uri = url.split('/')[-1].split('?')[0]
         download_queue = []
-        if 'track' in url:
-            download_queue.append(self.get_track(uri))
-        elif 'album' in url:
+        if 'album' in url:
             download_queue.extend(self.get_album(uri)['tracks']['items'])
+        elif 'track' in url:
+            download_queue.append(self.get_track(uri))
         elif 'playlist' in url:
             download_queue.extend([i['track'] for i in self.get_playlist(uri)['tracks']['items']])
-        if not download_queue:
+        else:
             raise Exception('Not a valid Spotify URL')
         return download_queue
 
 
     def uri_to_gid(self, uri):
         return hex(base62.decode(uri, base62.CHARSET_INVERTED))[2:].zfill(32)
     
@@ -110,23 +110,23 @@
         return next(i["file_id"] for i in track["file"] if i["format"] == self.audio_quality)
     
 
     def get_pssh(self, file_id):
         return self.session.get(f'https://seektables.scdn.co/seektable/{file_id}.json').json()['pssh']
     
 
-    def get_decryption_keys(self, pssh):
+    def get_decryption_key(self, pssh):
         pssh = PSSH(pssh)
         challenge = self.cdm.get_license_challenge(self.cdm_session, pssh)
         license = self.session.post(
             'https://gue1-spclient.spotify.com/widevine-license/v1/audio/license', 
-            challenge
+            challenge,
         ).content
         self.cdm.parse_license(self.cdm_session, license)
-        return f'1:{next(i for i in self.cdm.get_keys(self.cdm_session) if i.type == "CONTENT").key.hex()}'
+        return next(i for i in self.cdm.get_keys(self.cdm_session) if i.type == "CONTENT").key.hex()
     
     
     def get_stream_url(self, file_id):
         return self.session.get(
             f'https://gue1-spclient.spotify.com/storage-resolve/v2/files/audio/interactive/11/{file_id}?version=10000000&product=9&platform=39&alt=json'
         ).json()['cdnurl'][0]
     
@@ -176,20 +176,15 @@
             '\xa9nam': [track['name']],
             '\xa9ART': [self.get_artist(track['artist'])],
             'aART': [self.get_artist(track['album']['artist'])],
             '\xa9alb': [track['album']['name']],
             'trkn': [(track['number'], total_tracks)],
             'disk': [(track['disc_number'], total_discs)],
             '\xa9day': [f'{release_date}T00:00:00Z'],
-            'covr': [
-                MP4Cover(
-                    self.get_cover('https://i.scdn.co/image/' + next(i['file_id'] for i in track['album']['cover_group']['image'] if i['size'] == 'LARGE')),
-                    imageformat = MP4Cover.FORMAT_JPEG
-                )
-            ],
+            'covr': [MP4Cover(self.get_cover('https://i.scdn.co/image/' + next(i['file_id'] for i in track['album']['cover_group']['image'] if i['size'] == 'LARGE')), MP4Cover.FORMAT_JPEG)],
             '\xa9cmt': [f'https://open.spotify.com/track/{track["canonical_uri"].split(":")[-1]}'],
             'cprt': [copyright],
             'rtng': [1] if 'explicit' in track else [0],
         }
         if unsynced_lyrics is not None:
             tags['\xa9lyr'] = [unsynced_lyrics]
         return tags
@@ -205,18 +200,14 @@
         else:
             dirty_string = dirty_string[:36]
         return dirty_string.strip()
     
 
     def get_encrypted_location(self, track_id):
         return self.temp_path / f'{track_id}_encrypted.mp4'
-
-    
-    def get_decrypted_location(self, track_id):
-        return self.temp_path / f'{track_id}_decrypted.mp4'
     
 
     def get_fixed_location(self, track_id):
         return self.temp_path / f'{track_id}_fixed.m4a'
     
 
     def get_final_location(self, tags):
@@ -230,44 +221,33 @@
     def download(self, encrypted_location, stream_url):
         with YoutubeDL({
             'quiet': True,
             'no_warnings': True,
             'outtmpl': str(encrypted_location),
             'allow_unplayable_formats': True,
             'fixup': 'never',
-            'overwrites': self.overwrite
+            'overwrites': self.overwrite,
         }) as ydl:
             ydl.download(stream_url)
     
 
-    def decrypt(self, keys, encrypted_location, decrypted_location):
-        subprocess.run(
-            [
-                'mp4decrypt',
-                encrypted_location,
-                '--key',
-                keys,
-                decrypted_location
-            ],
-            check = True
-        )
-    
-
-    def fixup(self, decrypted_location, fixed_location):
+    def fixup(self, decryption_key, encrypted_location, fixed_location):
         subprocess.run(
             [
                 'ffmpeg',
                 '-loglevel',
                 'error',
                 '-y',
+                '-decryption_key',
+                decryption_key,
                 '-i',
-                decrypted_location,
+                encrypted_location,
                 '-c',
                 'copy',
-                fixed_location
+                fixed_location,
             ],
             check = True
         )
     
 
     def make_final(self, fixed_location, final_location, tags):
         final_location.parent.mkdir(parents = True, exist_ok = True)
```

### Comparing `spotify-aac-downloader-1.1/PKG-INFO` & `spotify-aac-downloader-1.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,18 @@
-Metadata-Version: 2.1
-Name: spotify-aac-downloader
-Version: 1.1
-Summary: Download songs/albums/playlists directly from Spotify in AAC
-Author: glomatico
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: pywidevine
-Requires-Dist: pyyaml
-Requires-Dist: pybase62
-Requires-Dist: yt-dlp
-Project-URL: repository, https://github.com/glomatico/spotify-aac-downloader
-
 # Spotify ✨ AAC ✨ Downloader
 A Python script to download songs/albums/playlists directly from Spotify in 256kbps/128kbps AAC.
 
 ## Setup
 1. Install Python 3.7 or newer
 2. Install spotify-aac-downloader with pip
     ```
     pip install spotify-aac-downloader
     ```
-3. Add mp4decrypt and ffmpeg to your PATH
-    * You can get them from here:
-        * mp4decrypt: https://www.bento4.com/downloads/
-        * ffmpeg: https://ffmpeg.org/download.html
+3. Add FFMPEG to your PATH. You can get it from here: https://ffmpeg.org/download.html
+    * If you are on Windows you can move the ffmpeg.exe file to the same folder that you will run the script instead of adding it to your PATH.
 4. Export your Spotify cookies as `cookies.txt` to the same folder that you will run the script
     * You can export your cookies by using this Google Chrome extension on Spotify website: https://chrome.google.com/webstore/detail/open-cookiestxt/gdocmgbfkjnnpapoeobnolbbkoibbcif. Make sure to be logged in.
 5. Put your Widevine Device file (.wvd) in the same folder that you will run the script
     * You can use Dumper to dump your phone's L3 CDM: https://github.com/Diazole/dumper. Once you have the L3 CDM, you can use pywidevine to create the .wvd file from it.
         1. Install pywidevine with pip
             ```
             pip install pywidevine pyyaml
@@ -65,8 +50,7 @@
                         Download 256kbps AAC instead of 128kbps AAC (default: False)
   -o, --overwrite       Overwrite existing files (default: False)
   -s, --skip-cleanup    Skip cleanup (default: False)
   -e, --print-exceptions
                         Print execeptions (default: False)
   -v, --version         show program's version number and exit
 ```
-
```

