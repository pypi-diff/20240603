# Comparing `tmp/gamdl-2.2.4.tar.gz` & `tmp/gamdl-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-2.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamdl-2.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-2.2.4.tar` & `gamdl-2.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       17 2024-05-20 18:54:11.800668 gamdl-2.2.4/.github/FUNDING.yml
--rw-r--r--   0        0        0     1137 2024-05-20 18:54:11.800668 gamdl-2.2.4/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2024-05-20 18:54:11.800668 gamdl-2.2.4/.gitignore
--rw-r--r--   0        0        0    12354 2024-05-20 18:54:11.800668 gamdl-2.2.4/README.md
--rw-r--r--   0        0        0       22 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/__init__.py
--rw-r--r--   0        0        0       30 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/__main__.py
--rw-r--r--   0        0        0     8791 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/apple_music_api.py
--rw-r--r--   0        0        0    27001 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/cli.py
--rw-r--r--   0        0        0     5570 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/constants.py
--rw-r--r--   0        0        0    16263 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/downloader.py
--rw-r--r--   0        0        0    10340 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/downloader_music_video.py
--rw-r--r--   0        0        0     2294 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/downloader_post.py
--rw-r--r--   0        0        0    14146 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/downloader_song.py
--rw-r--r--   0        0        0     4016 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/downloader_song_legacy.py
--rw-r--r--   0        0        0      797 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/enums.py
--rw-r--r--   0        0        0     4015 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/hardcoded_wvd.py
--rw-r--r--   0        0        0     2418 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/itunes_api.py
--rw-r--r--   0        0        0      369 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/models.py
--rw-r--r--   0        0        0      576 2024-05-20 18:54:11.804668 gamdl-2.2.4/pyproject.toml
--rw-r--r--   0        0        0       56 2024-05-20 18:54:11.804668 gamdl-2.2.4/requirements.txt
--rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 gamdl-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-06-03 00:26:25.934586 gamdl-2.2.5/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1137 2024-06-03 00:26:25.934586 gamdl-2.2.5/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2024-06-03 00:26:25.934586 gamdl-2.2.5/.gitignore
+-rw-r--r--   0        0        0    11856 2024-06-03 00:26:25.934586 gamdl-2.2.5/README.md
+-rw-r--r--   0        0        0       22 2024-06-03 00:26:25.934586 gamdl-2.2.5/gamdl/__init__.py
+-rw-r--r--   0        0        0       30 2024-06-03 00:26:25.934586 gamdl-2.2.5/gamdl/__main__.py
+-rw-r--r--   0        0        0     8791 2024-06-03 00:26:25.934586 gamdl-2.2.5/gamdl/apple_music_api.py
+-rw-r--r--   0        0        0    27001 2024-06-03 00:26:25.934586 gamdl-2.2.5/gamdl/cli.py
+-rw-r--r--   0        0        0     5570 2024-06-03 00:26:25.934586 gamdl-2.2.5/gamdl/constants.py
+-rw-r--r--   0        0        0    16869 2024-06-03 00:26:25.934586 gamdl-2.2.5/gamdl/downloader.py
+-rw-r--r--   0        0        0    10340 2024-06-03 00:26:25.934586 gamdl-2.2.5/gamdl/downloader_music_video.py
+-rw-r--r--   0        0        0     2294 2024-06-03 00:26:25.934586 gamdl-2.2.5/gamdl/downloader_post.py
+-rw-r--r--   0        0        0    14146 2024-06-03 00:26:25.934586 gamdl-2.2.5/gamdl/downloader_song.py
+-rw-r--r--   0        0        0     4016 2024-06-03 00:26:25.934586 gamdl-2.2.5/gamdl/downloader_song_legacy.py
+-rw-r--r--   0        0        0      813 2024-06-03 00:26:25.934586 gamdl-2.2.5/gamdl/enums.py
+-rw-r--r--   0        0        0     4015 2024-06-03 00:26:25.934586 gamdl-2.2.5/gamdl/hardcoded_wvd.py
+-rw-r--r--   0        0        0     2418 2024-06-03 00:26:25.934586 gamdl-2.2.5/gamdl/itunes_api.py
+-rw-r--r--   0        0        0      369 2024-06-03 00:26:25.934586 gamdl-2.2.5/gamdl/models.py
+-rw-r--r--   0        0        0      576 2024-06-03 00:26:25.934586 gamdl-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-06-03 00:26:25.934586 gamdl-2.2.5/requirements.txt
+-rw-r--r--   0        0        0    12347 1970-01-01 00:00:00.000000 gamdl-2.2.5/PKG-INFO
```

### Comparing `gamdl-2.2.4/.github/workflows/main.yml` & `gamdl-2.2.5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.4/README.md` & `gamdl-2.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Glomatico's Apple Music Downloader
 A Python CLI app for downloading Apple Music songs/music videos/posts.
 
 **Discord Server:** https://discord.gg/aBjMEZ9tnq
 
 ## Features
-* Download songs in AAC/Spatial AAC/Dolby Atmos/ALAC*
+* Download songs in AAC 256kbps and other codecs
 * Download music videos up to 4K
 * Download synced lyrics in LRC, SRT or TTML
 * Choose between FFmpeg and MP4Box for remuxing
 * Choose between yt-dlp and N_m3u8DL-RE for downloading
 * Highly customizable
 * Use artist links to download all of their albums or music videos
 
@@ -57,52 +57,52 @@
 * Arrow keys - Move selection
 * Space - Toggle selection
 * Ctrl + A - Select all
 * Enter - Confirm selection
 
 ## Configuration
 gamdl can be configured by using the command line arguments or the config file. The config file is created automatically when you run gamdl for the first time at `~/.gamdl/config.json` on Linux and `%USERPROFILE%\.gamdl\config.json` on Windows. Config file values can be overridden using command line arguments.
-| Command line argument / Config file key                         | Description                                                                  | Default value                                |
-| --------------------------------------------------------------- | ---------------------------------------------------------------------------- | -------------------------------------------- |
-| `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.                     | `false`                                      |
-| `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                               | `false`                                      |
-| `--overwrite` / `overwrite`                                     | Overwrite existing files.                                                    | `false`                                      |
-| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs separated by newlines. | `false`                                      |
-| `--synced-lyrics-only` / `synced_lyrics_only`                   | Download only the synced lyrics.                                             | `false`                                      |
-| `--no-synced-lyrics` / `no_synced_lyrics`                       | Don't download the synced lyrics.                                            | `false`                                      |
-| `--config-path` / -                                             | Path to config file.                                                         | `<home>/.spotify-web-downloader/config.json` |
-| `--log-level` / `log_level`                                     | Log level.                                                                   | `INFO`                                       |
-| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                            | `false`                                      |
-| `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                                   | `./cookies.txt`                              |
-| `--language`, `-l` / `language`                                 | Metadata language as an ISO-2A language code (don't always work for videos). | `en-US`                                      |
-| `--output-path`, `-o` / `output_path`                           | Path to output directory.                                                    | `./Apple Music`                              |
-| `--temp-path` / `temp_path`                                     | Path to temporary directory.                                                 | `./temp`                                     |
-| `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                           | `null`                                       |
-| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                                  | `N_m3u8DL-RE`                                |
-| `--mp4decrypt-path` / `mp4decrypt_path`                         | Path to mp4decrypt binary.                                                   | `mp4decrypt`                                 |
-| `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                                       | `ffmpeg`                                     |
-| `--mp4box-path` / `mp4box_path`                                 | Path to MP4Box binary.                                                       | `MP4Box`                                     |
-| `--download-mode` / `download_mode`                             | Download mode.                                                               | `ytdlp`                                      |
-| `--remux-mode` / `remux_mode`                                   | Remux mode.                                                                  | `ffmpeg`                                     |
-| `--cover-format` / `cover_format`                               | Cover format.                                                                | `jpg`                                        |
-| `--template-folder-album` / `template_folder_album`             | Template folder for tracks that are part of an album.                        | `{album_artist}/{album}`                     |
-| `--template-folder-compilation` / `template_folder_compilation` | Template folder for tracks that are part of a compilation album.             | `Compilations/{album}`                       |
-| `--template-file-single-disc` / `template_file_single_disc`     | Template file for the tracks that are part of a single-disc album.           | `{track:02d} {title}`                        |
-| `--template-file-multi-disc` / `template_file_multi_disc`       | Template file for the tracks that are part of a multi-disc album.            | `{disc}-{track:02d} {title}`                 |
-| `--template-folder-no-album` / `template_folder_no_album`       | Template folder for the tracks that are not part of an album.                | `{artist}/Unknown Album`                     |
-| `--template-file-no-album` / `template_file_no_album`           | Template file for the tracks that are not part of an album.                  | `{title}`                                    |
-| `--template-date` / `template_date`                             | Date tag template.                                                           | `%Y-%m-%dT%H:%M:%SZ`                         |
-| `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                             | `null`                                       |
-| `--cover-size` / `cover_size`                                   | Cover size.                                                                  | `1200`                                       |
-| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                                     | `40`                                         |
-| `--codec-song` / `codec_song`                                   | Song codec.                                                                  | `aac-legacy`                                 |
-| `--synced-lyrics-format` / `synced_lyrics_format`               | Synced lyrics format.                                                        | `lrc`                                        |
-| `--codec-music-video` / `codec_music_video`                     | Music video codec.                                                           | `h264`                                       |
-| `--quality-post` / `quality_post`                               | Post video quality.                                                          | `best`                                       |
-| `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                                      |
+| Command line argument / Config file key                         | Description                                                                  | Default value                |
+| --------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------- |
+| `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.                     | `false`                      |
+| `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                               | `false`                      |
+| `--overwrite` / `overwrite`                                     | Overwrite existing files.                                                    | `false`                      |
+| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs separated by newlines. | `false`                      |
+| `--synced-lyrics-only` / `synced_lyrics_only`                   | Download only the synced lyrics.                                             | `false`                      |
+| `--no-synced-lyrics` / `no_synced_lyrics`                       | Don't download the synced lyrics.                                            | `false`                      |
+| `--config-path` / -                                             | Path to config file.                                                         | `<home>/.gamdl/config.json`  |
+| `--log-level` / `log_level`                                     | Log level.                                                                   | `INFO`                       |
+| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                            | `false`                      |
+| `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                                   | `./cookies.txt`              |
+| `--language`, `-l` / `language`                                 | Metadata language as an ISO-2A language code (don't always work for videos). | `en-US`                      |
+| `--output-path`, `-o` / `output_path`                           | Path to output directory.                                                    | `./Apple Music`              |
+| `--temp-path` / `temp_path`                                     | Path to temporary directory.                                                 | `./temp`                     |
+| `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                           | `null`                       |
+| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                                  | `N_m3u8DL-RE`                |
+| `--mp4decrypt-path` / `mp4decrypt_path`                         | Path to mp4decrypt binary.                                                   | `mp4decrypt`                 |
+| `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                                       | `ffmpeg`                     |
+| `--mp4box-path` / `mp4box_path`                                 | Path to MP4Box binary.                                                       | `MP4Box`                     |
+| `--download-mode` / `download_mode`                             | Download mode.                                                               | `ytdlp`                      |
+| `--remux-mode` / `remux_mode`                                   | Remux mode.                                                                  | `ffmpeg`                     |
+| `--cover-format` / `cover_format`                               | Cover format.                                                                | `jpg`                        |
+| `--template-folder-album` / `template_folder_album`             | Template folder for tracks that are part of an album.                        | `{album_artist}/{album}`     |
+| `--template-folder-compilation` / `template_folder_compilation` | Template folder for tracks that are part of a compilation album.             | `Compilations/{album}`       |
+| `--template-file-single-disc` / `template_file_single_disc`     | Template file for the tracks that are part of a single-disc album.           | `{track:02d} {title}`        |
+| `--template-file-multi-disc` / `template_file_multi_disc`       | Template file for the tracks that are part of a multi-disc album.            | `{disc}-{track:02d} {title}` |
+| `--template-folder-no-album` / `template_folder_no_album`       | Template folder for the tracks that are not part of an album.                | `{artist}/Unknown Album`     |
+| `--template-file-no-album` / `template_file_no_album`           | Template file for the tracks that are not part of an album.                  | `{title}`                    |
+| `--template-date` / `template_date`                             | Date tag template.                                                           | `%Y-%m-%dT%H:%M:%SZ`         |
+| `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                             | `null`                       |
+| `--cover-size` / `cover_size`                                   | Cover size.                                                                  | `1200`                       |
+| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                                     | `40`                         |
+| `--codec-song` / `codec_song`                                   | Song codec.                                                                  | `aac-legacy`                 |
+| `--synced-lyrics-format` / `synced_lyrics_format`               | Synced lyrics format.                                                        | `lrc`                        |
+| `--codec-music-video` / `codec_music_video`                     | Music video codec.                                                           | `h264`                       |
+| `--quality-post` / `quality_post`                               | Post video quality.                                                          | `best`                       |
+| `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                      |
 
 
 ### Tags variables
 The following variables can be used in the template folders/files and/or in the `exclude_tags` list:
 * `album`
 * `album_artist`
 * `album_id`
@@ -152,27 +152,27 @@
     * Can be obtained from here: https://github.com/nilaoda/N_m3u8DL-RE/releases
 
 
 ### Song codecs
 The following codecs are available:
 * `aac-legacy`
 * `aac-he-legacy`
+
+The following codecs are also available, **but are not guaranteed to work**, as currently most (or all) of the songs fails to be downloaded when using them:
 * `aac`
 * `aac-he`
 * `aac-binaural`
 * `aac-downmix`
 * `aac-he-binaural`
 * `aac-he-downmix`
 * `atmos`
 * `ac3`
 * `alac`
 * `ask`
-    * When using this option, gamdl will ask you which **non-legacy** codec to use that is available for the song.
-
-**Support for non-legacy codecs are not guaranteed, as most of the songs cannot be downloaded when using non-legacy codecs.**
+    * When using this option, gamdl will ask you which codec from this list to use that is available for the song.
 
 ### Music videos codecs
 The following codecs are available:
 * `h264` (up to 1080p, with AAC 256kbps)
 * `h265` (up to 2160p, with AAC 256kpbs)
 * `ask`
     * When using this option, gamdl will ask you which audio and video codec to use that is available for the music video.
@@ -193,7 +193,9 @@
     * Native format for Apple Music synced lyrics.
     * Highly unsupported by most media players.
   
 ### Cover formats
 The following cover formats are available:
 * `jpg`
 * `png`
+* `raw`
+    * This format gets the raw cover without any processing in JPEG format.
```

### Comparing `gamdl-2.2.4/gamdl/apple_music_api.py` & `gamdl-2.2.5/gamdl/apple_music_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.4/gamdl/cli.py` & `gamdl-2.2.5/gamdl/cli.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.4/gamdl/constants.py` & `gamdl-2.2.5/gamdl/constants.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.4/gamdl/downloader.py` & `gamdl-2.2.5/gamdl/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,27 +349,46 @@
         ] + [
             self.get_sanitized_string(final_path_file[-1].format(**tags), False)
             + file_extension
         ]
         return self.output_path.joinpath(*final_path_folder).joinpath(*final_path_file)
 
     def get_cover_url(self, metadata: dict) -> str:
+        if self.cover_format == CoverFormat.RAW:
+            return self._get_raw_cover_url(metadata["attributes"]["artwork"]["url"])
         return self._get_cover_url(metadata["attributes"]["artwork"]["url"])
 
+    def _get_raw_cover_url(self, cover_url_template: str) -> str:
+        return re.sub(
+            r"image/thumb/",
+            "",
+            re.sub(
+                r"is1-ssl",
+                "a1",
+                re.sub(
+                    r"/\{w\}x\{h\}([a-z]{2})\.jpg",
+                    "",
+                    cover_url_template,
+                ),
+            ),
+        )
+
     def _get_cover_url(self, cover_url_template: str) -> str:
         return re.sub(
             r"\{w\}x\{h\}([a-z]{2})\.jpg",
             f"{self.cover_size}x{self.cover_size}bb.{self.cover_format.value}",
             cover_url_template,
         )
 
     @staticmethod
     @functools.lru_cache()
     def get_url_response_bytes(url: str) -> bytes:
-        return requests.get(url).content
+        response = requests.get(url)
+        response.raise_for_status()
+        return response.content
 
     def apply_tags(
         self,
         path: Path,
         tags: dict,
         cover_url: str,
     ):
@@ -405,15 +424,15 @@
                 mp4_tags[MP4_TAGS_MAP[tag_name]] = [tags[tag_name]]
         if "cover" not in self.exclude_tags_list:
             mp4_tags["covr"] = [
                 MP4Cover(
                     self.get_url_response_bytes(cover_url),
                     imageformat=(
                         MP4Cover.FORMAT_JPEG
-                        if self.cover_format == CoverFormat.JPG
+                        if self.cover_format in (CoverFormat.JPG, CoverFormat.RAW)
                         else MP4Cover.FORMAT_PNG
                     ),
                 )
             ]
         mp4 = MP4(path)
         mp4.clear()
         mp4.update(mp4_tags)
```

### Comparing `gamdl-2.2.4/gamdl/downloader_music_video.py` & `gamdl-2.2.5/gamdl/downloader_music_video.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.4/gamdl/downloader_post.py` & `gamdl-2.2.5/gamdl/downloader_post.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.4/gamdl/downloader_song.py` & `gamdl-2.2.5/gamdl/downloader_song.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.4/gamdl/downloader_song_legacy.py` & `gamdl-2.2.5/gamdl/downloader_song_legacy.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.4/gamdl/enums.py` & `gamdl-2.2.5/gamdl/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,7 +42,8 @@
     BEST = "best"
     ASK = "ask"
 
 
 class CoverFormat(Enum):
     JPG = "jpg"
     PNG = "png"
+    RAW = "raw"
```

### Comparing `gamdl-2.2.4/gamdl/hardcoded_wvd.py` & `gamdl-2.2.5/gamdl/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.4/gamdl/itunes_api.py` & `gamdl-2.2.5/gamdl/itunes_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.4/pyproject.toml` & `gamdl-2.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.4/PKG-INFO` & `gamdl-2.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 2.2.4
+Version: 2.2.5
 Summary: A Python CLI app for downloading Apple Music songs/music videos/posts.
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ciso8601
 Requires-Dist: click
 Requires-Dist: inquirerpy
@@ -17,15 +17,15 @@
 
 # Glomatico's Apple Music Downloader
 A Python CLI app for downloading Apple Music songs/music videos/posts.
 
 **Discord Server:** https://discord.gg/aBjMEZ9tnq
 
 ## Features
-* Download songs in AAC/Spatial AAC/Dolby Atmos/ALAC*
+* Download songs in AAC 256kbps and other codecs
 * Download music videos up to 4K
 * Download synced lyrics in LRC, SRT or TTML
 * Choose between FFmpeg and MP4Box for remuxing
 * Choose between yt-dlp and N_m3u8DL-RE for downloading
 * Highly customizable
 * Use artist links to download all of their albums or music videos
 
@@ -74,52 +74,52 @@
 * Arrow keys - Move selection
 * Space - Toggle selection
 * Ctrl + A - Select all
 * Enter - Confirm selection
 
 ## Configuration
 gamdl can be configured by using the command line arguments or the config file. The config file is created automatically when you run gamdl for the first time at `~/.gamdl/config.json` on Linux and `%USERPROFILE%\.gamdl\config.json` on Windows. Config file values can be overridden using command line arguments.
-| Command line argument / Config file key                         | Description                                                                  | Default value                                |
-| --------------------------------------------------------------- | ---------------------------------------------------------------------------- | -------------------------------------------- |
-| `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.                     | `false`                                      |
-| `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                               | `false`                                      |
-| `--overwrite` / `overwrite`                                     | Overwrite existing files.                                                    | `false`                                      |
-| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs separated by newlines. | `false`                                      |
-| `--synced-lyrics-only` / `synced_lyrics_only`                   | Download only the synced lyrics.                                             | `false`                                      |
-| `--no-synced-lyrics` / `no_synced_lyrics`                       | Don't download the synced lyrics.                                            | `false`                                      |
-| `--config-path` / -                                             | Path to config file.                                                         | `<home>/.spotify-web-downloader/config.json` |
-| `--log-level` / `log_level`                                     | Log level.                                                                   | `INFO`                                       |
-| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                            | `false`                                      |
-| `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                                   | `./cookies.txt`                              |
-| `--language`, `-l` / `language`                                 | Metadata language as an ISO-2A language code (don't always work for videos). | `en-US`                                      |
-| `--output-path`, `-o` / `output_path`                           | Path to output directory.                                                    | `./Apple Music`                              |
-| `--temp-path` / `temp_path`                                     | Path to temporary directory.                                                 | `./temp`                                     |
-| `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                           | `null`                                       |
-| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                                  | `N_m3u8DL-RE`                                |
-| `--mp4decrypt-path` / `mp4decrypt_path`                         | Path to mp4decrypt binary.                                                   | `mp4decrypt`                                 |
-| `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                                       | `ffmpeg`                                     |
-| `--mp4box-path` / `mp4box_path`                                 | Path to MP4Box binary.                                                       | `MP4Box`                                     |
-| `--download-mode` / `download_mode`                             | Download mode.                                                               | `ytdlp`                                      |
-| `--remux-mode` / `remux_mode`                                   | Remux mode.                                                                  | `ffmpeg`                                     |
-| `--cover-format` / `cover_format`                               | Cover format.                                                                | `jpg`                                        |
-| `--template-folder-album` / `template_folder_album`             | Template folder for tracks that are part of an album.                        | `{album_artist}/{album}`                     |
-| `--template-folder-compilation` / `template_folder_compilation` | Template folder for tracks that are part of a compilation album.             | `Compilations/{album}`                       |
-| `--template-file-single-disc` / `template_file_single_disc`     | Template file for the tracks that are part of a single-disc album.           | `{track:02d} {title}`                        |
-| `--template-file-multi-disc` / `template_file_multi_disc`       | Template file for the tracks that are part of a multi-disc album.            | `{disc}-{track:02d} {title}`                 |
-| `--template-folder-no-album` / `template_folder_no_album`       | Template folder for the tracks that are not part of an album.                | `{artist}/Unknown Album`                     |
-| `--template-file-no-album` / `template_file_no_album`           | Template file for the tracks that are not part of an album.                  | `{title}`                                    |
-| `--template-date` / `template_date`                             | Date tag template.                                                           | `%Y-%m-%dT%H:%M:%SZ`                         |
-| `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                             | `null`                                       |
-| `--cover-size` / `cover_size`                                   | Cover size.                                                                  | `1200`                                       |
-| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                                     | `40`                                         |
-| `--codec-song` / `codec_song`                                   | Song codec.                                                                  | `aac-legacy`                                 |
-| `--synced-lyrics-format` / `synced_lyrics_format`               | Synced lyrics format.                                                        | `lrc`                                        |
-| `--codec-music-video` / `codec_music_video`                     | Music video codec.                                                           | `h264`                                       |
-| `--quality-post` / `quality_post`                               | Post video quality.                                                          | `best`                                       |
-| `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                                      |
+| Command line argument / Config file key                         | Description                                                                  | Default value                |
+| --------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------- |
+| `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.                     | `false`                      |
+| `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                               | `false`                      |
+| `--overwrite` / `overwrite`                                     | Overwrite existing files.                                                    | `false`                      |
+| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs separated by newlines. | `false`                      |
+| `--synced-lyrics-only` / `synced_lyrics_only`                   | Download only the synced lyrics.                                             | `false`                      |
+| `--no-synced-lyrics` / `no_synced_lyrics`                       | Don't download the synced lyrics.                                            | `false`                      |
+| `--config-path` / -                                             | Path to config file.                                                         | `<home>/.gamdl/config.json`  |
+| `--log-level` / `log_level`                                     | Log level.                                                                   | `INFO`                       |
+| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                            | `false`                      |
+| `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                                   | `./cookies.txt`              |
+| `--language`, `-l` / `language`                                 | Metadata language as an ISO-2A language code (don't always work for videos). | `en-US`                      |
+| `--output-path`, `-o` / `output_path`                           | Path to output directory.                                                    | `./Apple Music`              |
+| `--temp-path` / `temp_path`                                     | Path to temporary directory.                                                 | `./temp`                     |
+| `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                           | `null`                       |
+| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                                  | `N_m3u8DL-RE`                |
+| `--mp4decrypt-path` / `mp4decrypt_path`                         | Path to mp4decrypt binary.                                                   | `mp4decrypt`                 |
+| `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                                       | `ffmpeg`                     |
+| `--mp4box-path` / `mp4box_path`                                 | Path to MP4Box binary.                                                       | `MP4Box`                     |
+| `--download-mode` / `download_mode`                             | Download mode.                                                               | `ytdlp`                      |
+| `--remux-mode` / `remux_mode`                                   | Remux mode.                                                                  | `ffmpeg`                     |
+| `--cover-format` / `cover_format`                               | Cover format.                                                                | `jpg`                        |
+| `--template-folder-album` / `template_folder_album`             | Template folder for tracks that are part of an album.                        | `{album_artist}/{album}`     |
+| `--template-folder-compilation` / `template_folder_compilation` | Template folder for tracks that are part of a compilation album.             | `Compilations/{album}`       |
+| `--template-file-single-disc` / `template_file_single_disc`     | Template file for the tracks that are part of a single-disc album.           | `{track:02d} {title}`        |
+| `--template-file-multi-disc` / `template_file_multi_disc`       | Template file for the tracks that are part of a multi-disc album.            | `{disc}-{track:02d} {title}` |
+| `--template-folder-no-album` / `template_folder_no_album`       | Template folder for the tracks that are not part of an album.                | `{artist}/Unknown Album`     |
+| `--template-file-no-album` / `template_file_no_album`           | Template file for the tracks that are not part of an album.                  | `{title}`                    |
+| `--template-date` / `template_date`                             | Date tag template.                                                           | `%Y-%m-%dT%H:%M:%SZ`         |
+| `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                             | `null`                       |
+| `--cover-size` / `cover_size`                                   | Cover size.                                                                  | `1200`                       |
+| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                                     | `40`                         |
+| `--codec-song` / `codec_song`                                   | Song codec.                                                                  | `aac-legacy`                 |
+| `--synced-lyrics-format` / `synced_lyrics_format`               | Synced lyrics format.                                                        | `lrc`                        |
+| `--codec-music-video` / `codec_music_video`                     | Music video codec.                                                           | `h264`                       |
+| `--quality-post` / `quality_post`                               | Post video quality.                                                          | `best`                       |
+| `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                      |
 
 
 ### Tags variables
 The following variables can be used in the template folders/files and/or in the `exclude_tags` list:
 * `album`
 * `album_artist`
 * `album_id`
@@ -169,27 +169,27 @@
     * Can be obtained from here: https://github.com/nilaoda/N_m3u8DL-RE/releases
 
 
 ### Song codecs
 The following codecs are available:
 * `aac-legacy`
 * `aac-he-legacy`
+
+The following codecs are also available, **but are not guaranteed to work**, as currently most (or all) of the songs fails to be downloaded when using them:
 * `aac`
 * `aac-he`
 * `aac-binaural`
 * `aac-downmix`
 * `aac-he-binaural`
 * `aac-he-downmix`
 * `atmos`
 * `ac3`
 * `alac`
 * `ask`
-    * When using this option, gamdl will ask you which **non-legacy** codec to use that is available for the song.
-
-**Support for non-legacy codecs are not guaranteed, as most of the songs cannot be downloaded when using non-legacy codecs.**
+    * When using this option, gamdl will ask you which codec from this list to use that is available for the song.
 
 ### Music videos codecs
 The following codecs are available:
 * `h264` (up to 1080p, with AAC 256kbps)
 * `h265` (up to 2160p, with AAC 256kpbs)
 * `ask`
     * When using this option, gamdl will ask you which audio and video codec to use that is available for the music video.
@@ -210,8 +210,10 @@
     * Native format for Apple Music synced lyrics.
     * Highly unsupported by most media players.
   
 ### Cover formats
 The following cover formats are available:
 * `jpg`
 * `png`
+* `raw`
+    * This format gets the raw cover without any processing in JPEG format.
```

