# Comparing `tmp/music_kraken-2.0.1.dev18.tar.gz` & `tmp/music_kraken-2.0.1.dev3.tar.gz`

## Comparing `music_kraken-2.0.1.dev18.tar` & `music_kraken-2.0.1.dev3.tar`

### file list

```diff
@@ -1,83 +1,82 @@
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/__init__.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/__main__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/_version.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/audio/__init__.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/audio/codec.py
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/audio/metadata.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/cli/__init__.py
--rw-r--r--   0        0        0    14401 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/cli/main_downloader.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/cli/utils.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/cli/informations/__init__.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/cli/informations/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/cli/options/__init__.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/cli/options/cache.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/cli/options/first_config.py
--rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/cli/options/frontend.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/cli/options/settings.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/connection/__init__.py
--rw-r--r--   0        0        0     6833 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/connection/cache.py
--rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/connection/connection.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/connection/rotating.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/download/__init__.py
--rw-r--r--   0        0        0    12524 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/download/page_attributes.py
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/download/results.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/objects/__init__.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/objects/artwork.py
--rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/objects/collection.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/objects/contact.py
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/objects/country.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/objects/formatted_text.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/objects/lint_default_factories.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/objects/lyrics.py
--rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/objects/metadata.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/objects/option.py
--rw-r--r--   0        0        0    11281 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/objects/parents.py
--rw-r--r--   0        0        0    23480 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/objects/song.py
--rw-r--r--   0        0        0     7832 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/objects/source.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/objects/target.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/pages/__init__.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/pages/abstract.py
--rw-r--r--   0        0        0    14081 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/pages/bandcamp.py
--rw-r--r--   0        0        0    30308 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/pages/encyclopaedia_metallum.py
--rw-r--r--   0        0        0    10799 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/pages/genius.py
--rw-r--r--   0        0        0    44109 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/pages/musify.py
--rw-r--r--   0        0        0    13074 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/pages/youtube.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/pages/youtube_music/__init__.py
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/pages/youtube_music/_list_render.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/pages/youtube_music/_music_object_render.py
--rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/pages/youtube_music/super_youtube.py
--rw-r--r--   0        0        0    27173 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/pages/youtube_music/youtube_music.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/__init__.py
--rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/hacking.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/shared.py
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/string_processing.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/config/__init__.py
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/config/config.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/config/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/config/attributes/__init__.py
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/config/attributes/attribute.py
--rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/config/attributes/special_attributes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/config/config_files/__init__.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/config/config_files/logging_config.py
--rw-r--r--   0        0        0     7956 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/config/config_files/main_config.py
--rw-r--r--   0        0        0     6296 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/config/config_files/youtube_config.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/enums/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/enums/album.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/enums/colors.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/enums/contact.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/exception/__init__.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/exception/config.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/exception/download.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/exception/objects.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/path_manager/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/path_manager/config_directory.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/path_manager/locations.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/path_manager/music_directory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/support_classes/__init__.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/support_classes/download_result.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/music_kraken/utils/support_classes/query.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/LICENSE
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/README.md
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/pyproject.toml
--rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev18/PKG-INFO
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/__init__.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/__main__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/_version.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/audio/__init__.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/audio/codec.py
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/audio/metadata.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/__init__.py
+-rw-r--r--   0        0        0    14401 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/main_downloader.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/utils.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/informations/__init__.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/informations/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/options/__init__.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/options/cache.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/options/first_config.py
+-rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/options/frontend.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/cli/options/settings.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/connection/__init__.py
+-rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/connection/cache.py
+-rw-r--r--   0        0        0    13408 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/connection/connection.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/connection/rotating.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/download/__init__.py
+-rw-r--r--   0        0        0    12504 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/download/page_attributes.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/download/results.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/__init__.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/artwork.py
+-rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/collection.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/contact.py
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/country.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/formatted_text.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/lint_default_factories.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/lyrics.py
+-rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/metadata.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/option.py
+-rw-r--r--   0        0        0    11281 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/parents.py
+-rw-r--r--   0        0        0    23480 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/song.py
+-rw-r--r--   0        0        0     7832 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/source.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/objects/target.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/__init__.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/abstract.py
+-rw-r--r--   0        0        0    14081 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/bandcamp.py
+-rw-r--r--   0        0        0    30308 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/encyclopaedia_metallum.py
+-rw-r--r--   0        0        0    44109 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/musify.py
+-rw-r--r--   0        0        0    13074 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/youtube.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/__init__.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/_list_render.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/_music_object_render.py
+-rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/super_youtube.py
+-rw-r--r--   0        0        0    27173 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/youtube_music.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/__init__.py
+-rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/hacking.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/shared.py
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/string_processing.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/__init__.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/config.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/attributes/__init__.py
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/attributes/attribute.py
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/attributes/special_attributes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/config_files/__init__.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/config_files/logging_config.py
+-rw-r--r--   0        0        0     7956 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/config_files/main_config.py
+-rw-r--r--   0        0        0     6296 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/config/config_files/youtube_config.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/enums/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/enums/album.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/enums/colors.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/enums/contact.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/exception/__init__.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/exception/config.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/exception/download.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/exception/objects.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/path_manager/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/path_manager/config_directory.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/path_manager/locations.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/path_manager/music_directory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/support_classes/__init__.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/support_classes/download_result.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/music_kraken/utils/support_classes/query.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/LICENSE
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/README.md
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/pyproject.toml
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 music_kraken-2.0.1.dev3/PKG-INFO
```

### Comparing `music_kraken-2.0.1.dev18/music_kraken/__init__.py` & `music_kraken-2.0.1.dev3/music_kraken/__init__.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/__main__.py` & `music_kraken-2.0.1.dev3/music_kraken/__main__.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/audio/codec.py` & `music_kraken-2.0.1.dev3/music_kraken/audio/codec.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/audio/metadata.py` & `music_kraken-2.0.1.dev3/music_kraken/audio/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,18 +89,14 @@
                     img = img.crop((width // 2 - height // 2, 0, width // 2 + height // 2, height))
                 else:
                     img = img.crop((0, height // 2 - width // 2, width, height // 2 + width // 2))
 
             # resize the image to the preferred resolution
             img.thumbnail((main_settings["preferred_artwork_resolution"], main_settings["preferred_artwork_resolution"]))
 
-            # https://stackoverflow.com/a/59476938/16804841
-            if img.mode != 'RGB':
-                img = img.convert('RGB')
-
             img.save(converted_target.file_path, "JPEG")
 
         # https://stackoverflow.com/questions/70228440/mutagen-how-can-i-correctly-embed-album-art-into-mp3-file-so-that-i-can-see-t
         id3_object.frames.delall("APIC")
         id3_object.frames.add(
             APIC(
                 encoding=0,
```

### Comparing `music_kraken-2.0.1.dev18/music_kraken/cli/main_downloader.py` & `music_kraken-2.0.1.dev3/music_kraken/cli/main_downloader.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/cli/utils.py` & `music_kraken-2.0.1.dev3/music_kraken/cli/utils.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/cli/informations/paths.py` & `music_kraken-2.0.1.dev3/music_kraken/cli/informations/paths.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/cli/options/frontend.py` & `music_kraken-2.0.1.dev3/music_kraken/cli/options/frontend.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/cli/options/settings.py` & `music_kraken-2.0.1.dev3/music_kraken/cli/options/settings.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/connection/cache.py` & `music_kraken-2.0.1.dev3/music_kraken/connection/cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -133,21 +133,21 @@
             name=name,
             created=datetime.now(),
             expires=datetime.now() + timedelta(days=expires_in),
             additional_info=additional_info,
         )
         self._write_attribute(cache_attribute)
 
-        cache_path = fit_to_file_system(Path(module_path, name.replace("/", "_")), hidden_ok=True)
+        cache_path = fit_to_file_system(Path(module_path, name), hidden_ok=True)
         with cache_path.open("wb") as content_file:
             self.logger.debug(f"writing cache to {cache_path}")
             content_file.write(content)
 
     def get(self, name: str) -> Optional[CacheResult]:
-        path = fit_to_file_system(Path(self._dir, self.module, name.replace("/", "_")), hidden_ok=True)
+        path = fit_to_file_system(Path(self._dir, self.module, name), hidden_ok=True)
 
         if not path.is_file():
             return None
 
         # check if it is outdated
         if f"{self.module}_{name}" not in self._id_to_attribute:
             path.unlink()
@@ -162,15 +162,15 @@
     def clean(self):
         keep = set()
 
         for ca in self.cached_attributes.copy():
             if ca.name == "":
                 continue
 
-            file = fit_to_file_system(Path(self._dir, ca.module, ca.name.replace("/", "_")), hidden_ok=True)
+            file = fit_to_file_system(Path(self._dir, ca.module, ca.name), hidden_ok=True)
 
             if not ca.is_valid:
                 self.logger.debug(f"deleting cache {ca.id}")
                 file.unlink()
                 self.cached_attributes.remove(ca)
                 del self._id_to_attribute[ca.id]
```

### Comparing `music_kraken-2.0.1.dev18/music_kraken/connection/connection.py` & `music_kraken-2.0.1.dev3/music_kraken/connection/connection.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/connection/rotating.py` & `music_kraken-2.0.1.dev3/music_kraken/connection/rotating.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/download/__init__.py` & `music_kraken-2.0.1.dev3/music_kraken/download/__init__.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/download/page_attributes.py` & `music_kraken-2.0.1.dev3/music_kraken/download/page_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,20 +26,19 @@
 from ..utils.support_classes.download_result import DownloadResult
 from ..utils.support_classes.query import Query
 from ..utils.support_classes.download_result import DownloadResult
 from ..utils.exception import MKMissingNameException
 from ..utils.exception.download import UrlNotFoundException
 from ..utils.shared import DEBUG_PAGES
 
-from ..pages import Page, EncyclopaediaMetallum, Musify, YouTube, YoutubeMusic, Bandcamp, Genius, INDEPENDENT_DB_OBJECTS
+from ..pages import Page, EncyclopaediaMetallum, Musify, YouTube, YoutubeMusic, Bandcamp, INDEPENDENT_DB_OBJECTS
 
 
 ALL_PAGES: Set[Type[Page]] = {
     # EncyclopaediaMetallum,
-    Genius,
     Musify,
     YoutubeMusic,
     Bandcamp
 }
 
 if youtube_settings["use_youtube_alongside_youtube_music"]:
     ALL_PAGES.add(YouTube)
```

### Comparing `music_kraken-2.0.1.dev18/music_kraken/download/results.py` & `music_kraken-2.0.1.dev3/music_kraken/download/results.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/objects/artwork.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/artwork.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,10 +55,8 @@
 
     def __merge__(self, other: Artwork, **kwargs) -> None:
         for key, value in other._variant_mapping.items():
             if key not in self._variant_mapping:
                 self._variant_mapping[key] = value
 
     def __eq__(self, other: Artwork) -> bool:
-        if not isinstance(other, Artwork):
-            return False
         return any(a == b for a, b in zip(self._variant_mapping.keys(), other._variant_mapping.keys()))
```

### Comparing `music_kraken-2.0.1.dev18/music_kraken/objects/collection.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/collection.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/objects/contact.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/contact.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/objects/country.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/country.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/objects/lint_default_factories.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/lint_default_factories.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/objects/lyrics.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/lyrics.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/objects/metadata.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/metadata.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/objects/option.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/option.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/objects/parents.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/parents.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/objects/song.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/song.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/objects/source.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/source.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/objects/target.py` & `music_kraken-2.0.1.dev3/music_kraken/objects/target.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/pages/abstract.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/abstract.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/pages/bandcamp.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/bandcamp.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/pages/encyclopaedia_metallum.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/encyclopaedia_metallum.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/pages/musify.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/musify.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/pages/youtube.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/youtube.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/pages/youtube_music/_list_render.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/_list_render.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/pages/youtube_music/_music_object_render.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/_music_object_render.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/pages/youtube_music/super_youtube.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/super_youtube.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/pages/youtube_music/youtube_music.py` & `music_kraken-2.0.1.dev3/music_kraken/pages/youtube_music/youtube_music.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/__init__.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/hacking.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/hacking.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/shared.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/shared.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,19 @@
     load_dotenv(Path(__file__).parent.parent.parent / ".env.example")
 
 __stage__ = os.getenv("STAGE", "prod")
 
 DEBUG = (__stage__ == "dev") and True
 DEBUG_LOGGING = DEBUG and False
 DEBUG_TRACE = DEBUG and True
-DEBUG_OBJECT_TRACE = DEBUG and False
+DEBUG_OBJECT_TRACE = DEBUG and True
 DEBUG_OBJECT_TRACE_CALLSTACK = DEBUG_OBJECT_TRACE and False
 DEBUG_YOUTUBE_INITIALIZING = DEBUG and False
 DEBUG_PAGES = DEBUG and False
-DEBUG_DUMP = DEBUG and True
+DEBUG_DUMP = DEBUG and False
 DEBUG_PRINT_ID = DEBUG and True
 
 if DEBUG:
     print("DEBUG ACTIVE")
 
 
 def get_random_message() -> str:
```

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/string_processing.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/string_processing.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/config/__init__.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/config/__init__.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/config/config.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/config/config.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/config/attributes/attribute.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/config/attributes/attribute.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/config/attributes/special_attributes.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/config/attributes/special_attributes.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/config/config_files/logging_config.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/config/config_files/logging_config.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/config/config_files/main_config.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/config/config_files/main_config.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/config/config_files/youtube_config.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/config/config_files/youtube_config.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/enums/__init__.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/enums/album.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/enums/album.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/exception/config.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/exception/config.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/path_manager/locations.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/path_manager/locations.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/path_manager/music_directory.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/path_manager/music_directory.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/support_classes/download_result.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/support_classes/download_result.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/music_kraken/utils/support_classes/query.py` & `music_kraken-2.0.1.dev3/music_kraken/utils/support_classes/query.py`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/LICENSE` & `music_kraken-2.0.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/README.md` & `music_kraken-2.0.1.dev3/README.md`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/pyproject.toml` & `music_kraken-2.0.1.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `music_kraken-2.0.1.dev18/PKG-INFO` & `music_kraken-2.0.1.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: music-kraken
-Version: 2.0.1.dev18
+Version: 2.0.1.dev3
 Summary: An extensive music downloader crawling the internet. It gets its metadata from a couple of metadata providers, and it scrapes the audiofiles.
 Author-email: Hellow2 <hazel_is_cute@proton.me>
 License-Expression: AGPL-3.0-or-later
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

