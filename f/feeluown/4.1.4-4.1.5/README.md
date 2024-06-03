# Comparing `tmp/feeluown-4.1.4.tar.gz` & `tmp/feeluown-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feeluown-4.1.4.tar", last modified: Tue May 21 15:53:38 2024, max compression
+gzip compressed data, was "feeluown-4.1.5.tar", last modified: Mon Jun  3 14:56:39 2024, max compression
```

## Comparing `feeluown-4.1.4.tar` & `feeluown-4.1.5.tar`

### file list

```diff
@@ -1,287 +1,287 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.112632 feeluown-4.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-21 15:53:36.000000 feeluown-4.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-21 15:53:38.112632 feeluown-4.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-21 15:53:36.000000 feeluown-4.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.076632 feeluown-4.1.4/feeluown/
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      158 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.080632 feeluown-4.1.4/feeluown/app/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/gui_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/mixed_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/once_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/app/server_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.080632 feeluown-4.1.4/feeluown/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/cli/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4208 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.080632 feeluown-4.1.4/feeluown/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/entry_points/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/entry_points/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/entry_points/run_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/entry_points/run_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/excs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.080632 feeluown-4.1.4/feeluown/fuoexec/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/fuoexec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/fuoexec/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/fuoexec/fuoexec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/fuoexec/signal_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.084632 feeluown-4.1.4/feeluown/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.072632 feeluown-4.1.4/feeluown/gui/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.084632 feeluown-4.1.4/feeluown/gui/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/already_download.png
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/already_downloaded_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/cur_playlist.png
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/cur_playlist_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/download.png
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/download_dark.png
--rwxr-xr-x   0 runner    (1001) docker     (127)   303153 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/feeluown.icns
--rw-r--r--   0 runner    (1001) docker     (127)   112526 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/feeluown.ico
--rw-r--r--   0 runner    (1001) docker     (127)    35773 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/feeluown.png
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/like.png
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/like_checked.png
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/like_checked_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/like_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/tray-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/icons/tray-light.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.084632 feeluown-4.1.4/feeluown/gui/assets/themes/
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/themes/common.qss
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/themes/dark.qss
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/themes/light.qss
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/assets/themes/macos_dark.colors
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/base_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.088632 feeluown-4.1.4/feeluown/gui/components/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/avatar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/btns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/line_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/nowplaying.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/player_playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/player_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/playlist_btn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/song_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/components/volume_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/drawers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20611 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/hotkey.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/mimedata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.088632 feeluown-4.1.4/feeluown/gui/page_containers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/page_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/page_containers/scroll_area.py
--rw-r--r--   0 runner    (1001) docker     (127)    20407 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/page_containers/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.088632 feeluown-4.1.4/feeluown/gui/pages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/coll_mixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/homepage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/my_fav.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/provider_home.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/recently_played.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/recommendation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/recommendation_daily_songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/song_explore.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/pages/toplist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/provider_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/tips.py
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/tray.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.092632 feeluown-4.1.4/feeluown/gui/uimain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/floating_box.py
--rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/lyric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/nowplaying_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/page_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/player_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/playlist_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    13716 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/sidebar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimain/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.092632 feeluown-4.1.4/feeluown/gui/uimodels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimodels/my_music.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimodels/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/uimodels/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.096632 feeluown-4.1.4/feeluown/gui/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/accordion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/comment_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/cover_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/frameless.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/header.py
--rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/img_card_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/lyric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/magicbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/messageline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/mpv_.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/my_music.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/playlist_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/progress_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/selfpaint_btn.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/separator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/size_grip.py
--rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/song_minicard_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    27444 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/statusline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.096632 feeluown-4.1.4/feeluown/gui/widgets/statusline_items/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/statusline_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/statusline_items/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/statusline_items/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/tabbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/table_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/textbtn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/textlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/volume_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/gui/widgets/weblogin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.100632 feeluown-4.1.4/feeluown/library/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/excs.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/model_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/model_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/provider_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/library/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.100632 feeluown-4.1.4/feeluown/local/
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/local/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/local/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/local/provider_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/local/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/local/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    79978 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/mpv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.100632 feeluown-4.1.4/feeluown/nowplaying/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/nowplaying/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.100632 feeluown-4.1.4/feeluown/nowplaying/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/nowplaying/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/nowplaying/linux/introspect.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/nowplaying/linux/mpris2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/nowplaying/macos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/nowplaying/nowplaying.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.104632 feeluown-4.1.4/feeluown/player/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/base_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/fm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/lyric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/mpvplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    25849 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/player/recently_played.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.104632 feeluown-4.1.4/feeluown/pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/pyinstaller/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/pyinstaller/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.104632 feeluown-4.1.4/feeluown/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/_plain_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/json_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/model_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/objs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/plain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/serializers/typename.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.104632 feeluown-4.1.4/feeluown/server/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/data_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.104632 feeluown-4.1.4/feeluown/server/dslv1/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/dslv1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/dslv1/codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/dslv1/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/dslv1/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/dslv2.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/excs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.108632 feeluown-4.1.4/feeluown/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/excs.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/exec_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/handle.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/set_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/show.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/handlers/sub.py
--rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.108632 feeluown-4.1.4/feeluown/server/pubsub/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/pubsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/pubsub/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/pubsub/publishers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.108632 feeluown-4.1.4/feeluown/server/rpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/server/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.108632 feeluown-4.1.4/feeluown/uimodels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/uimodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/uimodels/my_music.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/uimodels/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/uimodels/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.112632 feeluown-4.1.4/feeluown/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/aio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/lang.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12691 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    13634 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/typing_.py
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    54535 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/utils/yt_dlp_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.112632 feeluown-4.1.4/feeluown/webserver/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/webserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/webserver/jsonrpc_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-21 15:53:36.000000 feeluown-4.1.4/feeluown/webserver/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:53:38.076632 feeluown-4.1.4/feeluown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-21 15:53:37.000000 feeluown-4.1.4/feeluown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-05-21 15:53:38.000000 feeluown-4.1.4/feeluown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:53:37.000000 feeluown-4.1.4/feeluown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-21 15:53:37.000000 feeluown-4.1.4/feeluown.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-21 15:53:37.000000 feeluown-4.1.4/feeluown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 15:53:37.000000 feeluown-4.1.4/feeluown.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-21 15:53:38.112632 feeluown-4.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-21 15:53:36.000000 feeluown-4.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.678654 feeluown-4.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-06-03 14:56:36.000000 feeluown-4.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-06-03 14:56:39.678654 feeluown-4.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-06-03 14:56:36.000000 feeluown-4.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.642654 feeluown-4.1.5/feeluown/
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      158 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.646654 feeluown-4.1.5/feeluown/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/app/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/app/gui_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/app/mixed_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/app/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/app/once_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/app/server_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.646654 feeluown-4.1.5/feeluown/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/cli/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4208 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.646654 feeluown-4.1.5/feeluown/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/entry_points/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/entry_points/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/entry_points/run_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/entry_points/run_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/excs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.646654 feeluown-4.1.5/feeluown/fuoexec/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/fuoexec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/fuoexec/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/fuoexec/fuoexec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/fuoexec/signal_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.650653 feeluown-4.1.5/feeluown/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.638654 feeluown-4.1.5/feeluown/gui/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.650653 feeluown-4.1.5/feeluown/gui/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/icons/already_download.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/icons/already_downloaded_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/icons/cur_playlist.png
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/icons/cur_playlist_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/icons/download.png
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/icons/download_dark.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)   303153 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/icons/feeluown.icns
+-rw-r--r--   0 runner    (1001) docker     (127)   112526 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/icons/feeluown.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    35773 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/icons/feeluown.png
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/icons/like.png
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/icons/like_checked.png
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/icons/like_checked_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/icons/like_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/icons/tray-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/icons/tray-light.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.654654 feeluown-4.1.5/feeluown/gui/assets/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/themes/common.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/themes/dark.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/themes/light.qss
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/assets/themes/macos_dark.colors
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/base_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.654654 feeluown-4.1.5/feeluown/gui/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/components/avatar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/components/btns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/components/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/components/line_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/components/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/components/nowplaying.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/components/player_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/components/player_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/components/playlist_btn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/components/song_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/components/volume_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/drawers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20692 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/hotkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/mimedata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.654654 feeluown-4.1.5/feeluown/gui/page_containers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/page_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/page_containers/scroll_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20407 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/page_containers/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.658654 feeluown-4.1.5/feeluown/gui/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/pages/coll_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/pages/homepage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/pages/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/pages/my_fav.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/pages/provider_home.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/pages/recently_played.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/pages/recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/pages/recommendation_daily_songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/pages/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/pages/song_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/pages/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/pages/toplist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/provider_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/tips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/tray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.658654 feeluown-4.1.5/feeluown/gui/uimain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/uimain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/uimain/floating_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/uimain/lyric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/uimain/nowplaying_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/uimain/page_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/uimain/player_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/uimain/playlist_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13716 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/uimain/sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/uimain/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.658654 feeluown-4.1.5/feeluown/gui/uimodels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/uimodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/uimodels/my_music.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/uimodels/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/uimodels/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.662654 feeluown-4.1.5/feeluown/gui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/accordion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/comment_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/cover_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/frameless.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17511 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/img_card_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/lyric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/magicbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/messageline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/mpv_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/my_music.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/playlist_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/progress_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/selfpaint_btn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/separator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/size_grip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/song_minicard_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27444 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/statusline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.662654 feeluown-4.1.5/feeluown/gui/widgets/statusline_items/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/statusline_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/statusline_items/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/statusline_items/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/tabbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/table_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/textbtn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/textlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/volume_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/gui/widgets/weblogin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.666653 feeluown-4.1.5/feeluown/library/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/library/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/library/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/library/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/library/excs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/library/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/library/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/library/model_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/library/model_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/library/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/library/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/library/provider_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/library/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.666653 feeluown-4.1.5/feeluown/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/local/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/local/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/local/provider_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/local/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/local/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79978 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/mpv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.666653 feeluown-4.1.5/feeluown/nowplaying/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/nowplaying/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.666653 feeluown-4.1.5/feeluown/nowplaying/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/nowplaying/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/nowplaying/linux/introspect.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/nowplaying/linux/mpris2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/nowplaying/macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/nowplaying/nowplaying.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.670654 feeluown-4.1.5/feeluown/player/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/player/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/player/base_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/player/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/player/fm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/player/lyric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/player/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/player/mpvplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25849 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/player/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/player/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/player/recently_played.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.670654 feeluown-4.1.5/feeluown/pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/pyinstaller/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/pyinstaller/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.670654 feeluown-4.1.5/feeluown/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/serializers/_plain_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/serializers/json_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/serializers/model_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/serializers/objs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/serializers/plain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/serializers/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/serializers/typename.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.674654 feeluown-4.1.5/feeluown/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/data_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.674654 feeluown-4.1.5/feeluown/server/dslv1/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/dslv1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/dslv1/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/dslv1/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/dslv1/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/dslv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/excs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.674654 feeluown-4.1.5/feeluown/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/handlers/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/handlers/excs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/handlers/exec_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/handlers/handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/handlers/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/handlers/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/handlers/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/handlers/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/handlers/set_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/handlers/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/handlers/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/handlers/sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.674654 feeluown-4.1.5/feeluown/server/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/pubsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/pubsub/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/pubsub/publishers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.674654 feeluown-4.1.5/feeluown/server/rpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/server/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.674654 feeluown-4.1.5/feeluown/uimodels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/uimodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/uimodels/my_music.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/uimodels/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/uimodels/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.678654 feeluown-4.1.5/feeluown/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/utils/aio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/utils/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/utils/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/utils/lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/utils/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12691 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/utils/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/utils/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13634 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/utils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/utils/typing_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54535 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/utils/yt_dlp_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.678654 feeluown-4.1.5/feeluown/webserver/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/webserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/webserver/jsonrpc_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-06-03 14:56:36.000000 feeluown-4.1.5/feeluown/webserver/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:39.642654 feeluown-4.1.5/feeluown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-06-03 14:56:39.000000 feeluown-4.1.5/feeluown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-06-03 14:56:39.000000 feeluown-4.1.5/feeluown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:56:39.000000 feeluown-4.1.5/feeluown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-06-03 14:56:39.000000 feeluown-4.1.5/feeluown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-06-03 14:56:39.000000 feeluown-4.1.5/feeluown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 14:56:39.000000 feeluown-4.1.5/feeluown.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-06-03 14:56:39.678654 feeluown-4.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-06-03 14:56:36.000000 feeluown-4.1.5/setup.py
```

### Comparing `feeluown-4.1.4/LICENSE` & `feeluown-4.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/PKG-INFO` & `feeluown-4.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feeluown
-Version: 4.1.4
+Version: 4.1.5
 Summary: *nix music player
 Home-page: https://github.com/feeluown/FeelUOwn
 Author: feeluown
 Author-email: yinshaowen241@gmail.com
 License: GPL-3.0
 Description: ## FeelUOwn - feel your own
         
@@ -44,16 +44,16 @@
         
         # macOS（也可以下载打包好的二进制）
         brew tap feeluown/feeluown
         brew install feeluown --with-battery # 安装 FeelUOwn 以及扩展
         feeluown genicon                     # 在桌面生成 FeelUOwn 图标
         ```
         
-        Windows 用户可以在 Release 页面下载预打包好的二进制。
-        Gentoo, NixOS, Debian 等 Linux 发行版也支持使用其系统包管理器安装！
+        Windows 和 macOS 用户可以在 Release 页面下载预打包好的二进制。
+        Gentoo, NixOS, Debian, openSUSE 等 Linux 发行版也支持使用其系统包管理器安装！
         详情可以参考文档：https://feeluown.readthedocs.io/ ，
         也欢迎你加入开发者/用户[交流群](https://t.me/joinchat/H7k12hG5HYsGy7RVvK_Dwg)。
         
         ### 免责声明
         
         FeelUown（以下简称“本软件”）是一个个人媒体资源播放工具。本软件提供的所有功能和资料
         不得用于任何商业用途。用户可以自由选择是否使用本产品提供的软件。如果用户下载、安装、
```

### Comparing `feeluown-4.1.4/README.md` & `feeluown-4.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 
 # macOS（也可以下载打包好的二进制）
 brew tap feeluown/feeluown
 brew install feeluown --with-battery # 安装 FeelUOwn 以及扩展
 feeluown genicon                     # 在桌面生成 FeelUOwn 图标
 ```
 
-Windows 用户可以在 Release 页面下载预打包好的二进制。
-Gentoo, NixOS, Debian 等 Linux 发行版也支持使用其系统包管理器安装！
+Windows 和 macOS 用户可以在 Release 页面下载预打包好的二进制。
+Gentoo, NixOS, Debian, openSUSE 等 Linux 发行版也支持使用其系统包管理器安装！
 详情可以参考文档：https://feeluown.readthedocs.io/ ，
 也欢迎你加入开发者/用户[交流群](https://t.me/joinchat/H7k12hG5HYsGy7RVvK_Dwg)。
 
 ### 免责声明
 
 FeelUown（以下简称“本软件”）是一个个人媒体资源播放工具。本软件提供的所有功能和资料
 不得用于任何商业用途。用户可以自由选择是否使用本产品提供的软件。如果用户下载、安装、
```

### Comparing `feeluown-4.1.4/feeluown/__init__.py` & `feeluown-4.1.5/feeluown/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 import logging.config
 
 from .consts import LOG_FILE
 
 
-__version__ = '4.1.4'
+__version__ = '4.1.5'
 
 
 dict_config = {
     'version': 1,
     'disable_existing_loggers': False,
     'formatters': {
         'standard': {
```

### Comparing `feeluown-4.1.4/feeluown/app/app.py` & `feeluown-4.1.5/feeluown/app/app.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/app/cli_app.py` & `feeluown-4.1.5/feeluown/app/cli_app.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/app/config.py` & `feeluown-4.1.5/feeluown/app/config.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/app/gui_app.py` & `feeluown-4.1.5/feeluown/app/gui_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -111,19 +111,26 @@
     def apply_state(self, state):
         super().apply_state(state)
         coll_library = self.coll_mgr.get_coll_library()
         self.browser.goto(page=f'/colls/{coll_library.identifier}')
 
         gui = state.get('gui', {})
         lyric = gui.get('lyric', {})
+        local_storage = gui.get('browser', {}).get('local_storage', {})
+        self.browser.local_storage = local_storage
         self.ui.lyric_window.apply_state(lyric)
 
     def dump_state(self):
         state = super().dump_state()
-        state['gui'] = {'lyric': self.ui.lyric_window.dump_state()}
+        state['gui'] = {
+            'lyric': self.ui.lyric_window.dump_state(),
+            'browser': {
+                'local_storage': self.browser.local_storage
+            }
+        }
         return state
 
     def closeEvent(self, _):
         if not self.config.ENABLE_TRAY:
             self.exit()
 
     def mouseReleaseEvent(self, e):
```

### Comparing `feeluown-4.1.4/feeluown/app/server_app.py` & `feeluown-4.1.5/feeluown/app/server_app.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/argparser.py` & `feeluown-4.1.5/feeluown/argparser.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/cli/cli.py` & `feeluown-4.1.5/feeluown/cli/cli.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/cli/install.py` & `feeluown-4.1.5/feeluown/cli/install.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/collection.py` & `feeluown-4.1.5/feeluown/collection.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/config.py` & `feeluown-4.1.5/feeluown/config.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/entry_points/base.py` & `feeluown-4.1.5/feeluown/entry_points/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/entry_points/run.py` & `feeluown-4.1.5/feeluown/entry_points/run.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/entry_points/run_app.py` & `feeluown-4.1.5/feeluown/entry_points/run_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,27 +129,29 @@
         if not sentinal.done():
             sentinal.set_result(0)
 
     app.about_to_shutdown.connect(shutdown, weak=False)
 
     # GUI state must be load before running app, otherwise, it does not take effects.
     app.load_and_apply_state()
+    logger.info("Load app last state...")
 
     # App can exit in several ways.
     #
     # GUI mode:
     # 1. QApplication.quit. QApplication.quit can be called under several circumstances
     #    1. User press CMD-Q on macOS.
     #    2. User clicks the tray icon exit button.
     # 2. SIGTERM is received.
     #
     # Daemon mode:
     # 1. Ctrl-C
     # 2. SIGTERM
     app.run()
+    logger.info("App started")
     app.started.emit(app)
 
     await sentinal
 
     Signal.teardown_aio_support()
```

### Comparing `feeluown-4.1.4/feeluown/excs.py` & `feeluown-4.1.5/feeluown/excs.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/fuoexec/functions.py` & `feeluown-4.1.5/feeluown/fuoexec/functions.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/fuoexec/fuoexec.py` & `feeluown-4.1.5/feeluown/fuoexec/fuoexec.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/fuoexec/signal_manager.py` & `feeluown-4.1.5/feeluown/fuoexec/signal_manager.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/icons/already_download.png` & `feeluown-4.1.5/feeluown/gui/assets/icons/already_download.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/icons/already_downloaded_dark.png` & `feeluown-4.1.5/feeluown/gui/assets/icons/already_downloaded_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/icons/cur_playlist.png` & `feeluown-4.1.5/feeluown/gui/assets/icons/cur_playlist.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/icons/cur_playlist_dark.png` & `feeluown-4.1.5/feeluown/gui/assets/icons/cur_playlist_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/icons/download.png` & `feeluown-4.1.5/feeluown/gui/assets/icons/download.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/icons/download_dark.png` & `feeluown-4.1.5/feeluown/gui/assets/icons/download_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/icons/feeluown.icns` & `feeluown-4.1.5/feeluown/gui/assets/icons/feeluown.icns`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/icons/feeluown.ico` & `feeluown-4.1.5/feeluown/gui/assets/icons/feeluown.ico`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/icons/feeluown.png` & `feeluown-4.1.5/feeluown/gui/assets/icons/feeluown.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/icons/like.png` & `feeluown-4.1.5/feeluown/gui/assets/icons/like.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/icons/like_checked.png` & `feeluown-4.1.5/feeluown/gui/assets/icons/like_checked.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/icons/like_checked_dark.png` & `feeluown-4.1.5/feeluown/gui/assets/icons/like_checked_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/icons/like_dark.png` & `feeluown-4.1.5/feeluown/gui/assets/icons/like_dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/icons/tray-dark.png` & `feeluown-4.1.5/feeluown/gui/assets/icons/tray-dark.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/icons/tray-light.png` & `feeluown-4.1.5/feeluown/gui/assets/icons/tray-light.png`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/themes/common.qss` & `feeluown-4.1.5/feeluown/gui/assets/themes/common.qss`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/themes/dark.qss` & `feeluown-4.1.5/feeluown/gui/assets/themes/dark.qss`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/themes/light.qss` & `feeluown-4.1.5/feeluown/gui/assets/themes/light.qss`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/assets/themes/macos_dark.colors` & `feeluown-4.1.5/feeluown/gui/assets/themes/macos_dark.colors`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/base_renderer.py` & `feeluown-4.1.5/feeluown/gui/base_renderer.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/browser.py` & `feeluown-4.1.5/feeluown/gui/browser.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/components/__init__.py` & `feeluown-4.1.5/feeluown/gui/components/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/components/avatar.py` & `feeluown-4.1.5/feeluown/gui/components/avatar.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/components/btns.py` & `feeluown-4.1.5/feeluown/gui/components/btns.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/components/collections.py` & `feeluown-4.1.5/feeluown/gui/components/collections.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/components/line_song.py` & `feeluown-4.1.5/feeluown/gui/components/line_song.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/components/menu.py` & `feeluown-4.1.5/feeluown/gui/components/menu.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/components/nowplaying.py` & `feeluown-4.1.5/feeluown/gui/components/nowplaying.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/components/player_playlist.py` & `feeluown-4.1.5/feeluown/gui/components/player_playlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/components/player_progress.py` & `feeluown-4.1.5/feeluown/gui/components/player_progress.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/components/playlist_btn.py` & `feeluown-4.1.5/feeluown/gui/components/playlist_btn.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/components/song_tag.py` & `feeluown-4.1.5/feeluown/gui/components/song_tag.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/consts.py` & `feeluown-4.1.5/feeluown/gui/consts.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/debug.py` & `feeluown-4.1.5/feeluown/gui/debug.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/drawers.py` & `feeluown-4.1.5/feeluown/gui/drawers.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/helpers.py` & `feeluown-4.1.5/feeluown/gui/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -617,14 +617,15 @@
 
 
 def esc_hide_widget(widget):
     QShortcut(QKeySequence.Cancel, widget).activated.connect(widget.hide)
 
 
 # https://ethanschoonover.com/solarized/
+# Do not change the existing colors if they are used by some widgets/components.
 SOLARIZED_COLORS = {
     'yellow':    '#b58900',
     'orange':    '#cb4b16',
     'red':       '#dc322f',
     'magenta':   '#d33682',
     'violet':    '#6c71c4',
     'blue':      '#268bd2',
```

### Comparing `feeluown-4.1.4/feeluown/gui/hotkey.py` & `feeluown-4.1.5/feeluown/gui/hotkey.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/image.py` & `feeluown-4.1.5/feeluown/gui/image.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/mimedata.py` & `feeluown-4.1.5/feeluown/gui/mimedata.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/page_containers/scroll_area.py` & `feeluown-4.1.5/feeluown/gui/page_containers/scroll_area.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/page_containers/table.py` & `feeluown-4.1.5/feeluown/gui/page_containers/table.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/pages/coll_mixed.py` & `feeluown-4.1.5/feeluown/gui/pages/coll_mixed.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/pages/homepage.py` & `feeluown-4.1.5/feeluown/gui/pages/homepage.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/pages/model.py` & `feeluown-4.1.5/feeluown/gui/pages/model.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/pages/my_fav.py` & `feeluown-4.1.5/feeluown/gui/pages/my_fav.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/pages/provider_home.py` & `feeluown-4.1.5/feeluown/gui/pages/provider_home.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/pages/recently_played.py` & `feeluown-4.1.5/feeluown/gui/pages/recently_played.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/pages/recommendation.py` & `feeluown-4.1.5/feeluown/gui/pages/recommendation.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/pages/recommendation_daily_songs.py` & `feeluown-4.1.5/feeluown/gui/pages/recommendation_daily_songs.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/pages/search.py` & `feeluown-4.1.5/feeluown/gui/pages/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,98 +1,114 @@
+from datetime import datetime
 from PyQt5.QtWidgets import QAbstractItemView, QFrame, QVBoxLayout
 
 from feeluown.library import SearchType
 from feeluown.gui.page_containers.table import TableContainer, Renderer
 from feeluown.gui.page_containers.scroll_area import ScrollArea
 from feeluown.gui.widgets.img_card_list import ImgCardListDelegate
 from feeluown.gui.widgets.songs import SongsTableView, ColumnsMode
 from feeluown.gui.base_renderer import TabBarRendererMixin
 from feeluown.gui.helpers import BgTransparentMixin
 from feeluown.gui.widgets.magicbox import KeySourceIn, KeyType
 from feeluown.gui.widgets.header import LargeHeader, MidHeader
 from feeluown.gui.widgets.accordion import Accordion
+from feeluown.gui.widgets.labels import MessageLabel
 from feeluown.utils.reader import create_reader
+from feeluown.utils.router import Request
+from feeluown.app.gui_app import GuiApp
 
 Tabs = [('歌曲', SearchType.so),
         ('专辑', SearchType.al),
         ('歌手', SearchType.ar),
         ('歌单', SearchType.pl),
         ('视频', SearchType.vi)]
 
 
-async def render(req, **kwargs):  # pylint: disable=too-many-locals,too-many-branches
+def get_tab_idx(search_type):
+    for i, tab in enumerate(Tabs):
+        if tab[1] == search_type:
+            return i
+    raise ValueError("unknown search type")
+
+
+def get_source_in(req: Request):
+    source_in = req.query.get('source_in', None)
+    if source_in is not None:
+        source_in = source_in.split(',')
+    else:
+        source_in = None
+    return source_in
+
+
+async def render(req: Request, **kwargs):
     """/search handler
 
     :type app: feeluown.app.App
     """
+    # pylint: disable=too-many-locals,too-many-branches
     q = req.query.get('q', '')
     if not q:
         return
 
-    source_in = req.query.get('source_in', None)
+    app: 'GuiApp' = req.ctx['app']
+    source_in = get_source_in(req)
     search_type = SearchType(req.query.get('type', SearchType.so.value))
-    if source_in is not None:
-        source_in = source_in.split(',')
-    else:
-        source_in = None
-
-    app = req.ctx['app']
 
     body = Body()
     view = View(app, q)
     body.setWidget(view)
     app.ui.right_panel.set_body(body)
 
-    tab_index = 0
-    for i, tab in enumerate(Tabs):
-        if tab[1] == search_type:
-            tab_index = i
-            break
-
+    tab_index = get_tab_idx(search_type)
+    succeed = 0
+    start = datetime.now()
     is_first = True  # Is first search result.
+    view.hint.show_msg('正在搜索...')
     async for result in app.library.a_search(
             q, type_in=search_type, source_in=source_in):
-        if result is not None:
-            table_container = TableContainer(app, view.accordion)
-            table_container.layout().setContentsMargins(0, 0, 0, 0)
-
-            # HACK: set fixed row for tables.
-            # pylint: disable=protected-access
-            for table in table_container._tables:
-                assert isinstance(table, QAbstractItemView)
-                delegate = table.itemDelegate()
-                if isinstance(delegate, ImgCardListDelegate):
-                    # FIXME: set fixed_row_count in better way.
-                    table._fixed_row_count = 2  # type: ignore[attr-defined]
-                    delegate.update_settings("card_min_width", 100)
-                elif isinstance(table, SongsTableView):
-                    table._fixed_row_count = 8
-                    table._row_height = table.verticalHeader().defaultSectionSize()
-
-            renderer = SearchResultRenderer(q, tab_index, source_in=source_in)
-            await table_container.set_renderer(renderer)
-            _, search_type, attrname, show_handler = renderer.tabs[tab_index]
-            objects = getattr(result, attrname) or []
-            if not objects:  # Result is empty.
-                continue
-
-            if search_type is SearchType.so:
-                show_handler(  # type: ignore[operator]
-                    create_reader(objects), columns_mode=ColumnsMode.playlist)
-            else:
-                show_handler(create_reader(objects))  # type: ignore[operator]
-            source = objects[0].source
-            provider = app.library.get(source)
-            provider_name = provider.name
-            if is_first is False:
-                table_container.hide()
-            view.accordion.add_section(MidHeader(provider_name), table_container, 6, 12)
-            renderer.meta_widget.hide()
-            renderer.toolbar.hide()
-            is_first = False
+        table_container = TableContainer(app, view.accordion)
+        table_container.layout().setContentsMargins(0, 0, 0, 0)
+
+        # HACK: set fixed row for tables.
+        # pylint: disable=protected-access
+        for table in table_container._tables:
+            assert isinstance(table, QAbstractItemView)
+            delegate = table.itemDelegate()
+            if isinstance(delegate, ImgCardListDelegate):
+                # FIXME: set fixed_row_count in better way.
+                table._fixed_row_count = 2  # type: ignore[attr-defined]
+                delegate.update_settings("card_min_width", 140)
+            elif isinstance(table, SongsTableView):
+                table._fixed_row_count = 8
+                table._row_height = table.verticalHeader().defaultSectionSize()
+
+        renderer = SearchResultRenderer(q, tab_index, source_in=source_in)
+        await table_container.set_renderer(renderer)
+        _, search_type, attrname, show_handler = renderer.tabs[tab_index]
+        objects = getattr(result, attrname) or []
+        if not objects:  # Result is empty.
+            continue
+
+        succeed += 1
+        if search_type is SearchType.so:
+            show_handler(  # type: ignore[operator]
+                create_reader(objects), columns_mode=ColumnsMode.playlist)
+        else:
+            show_handler(create_reader(objects))  # type: ignore[operator]
+        source = objects[0].source
+        provider = app.library.get(source)
+        provider_name = provider.name
+        if is_first is False:
+            table_container.hide()
+        view.accordion.add_section(MidHeader(provider_name), table_container, 6, 12)
+        renderer.meta_widget.hide()
+        renderer.toolbar.hide()
+        is_first = False
+    time_cost = (datetime.now() - start).total_seconds()
+    view.hint.show_msg(f'搜索完成，共有 {succeed} 个有效的结果，花费 {time_cost:.2f}s')
 
 
 class SearchResultRenderer(Renderer, TabBarRendererMixin):
     def __init__(self, q, tab_index, source_in=None):
         self.q = q
         self.tab_index = tab_index
         self.source_in = source_in
@@ -129,17 +145,20 @@
 class View(QFrame, BgTransparentMixin):
     def __init__(self, app, q):
         super().__init__()
 
         self._app = app
 
         self.title = LargeHeader(f'搜索“{q}”')
+        self.hint = MessageLabel()
         self.accordion = Accordion()
 
         self._layout = QVBoxLayout(self)
         self._layout.setContentsMargins(20, 0, 20, 0)
         self._layout.setSpacing(0)
         self._layout.addSpacing(30)
         self._layout.addWidget(self.title)
         self._layout.addSpacing(10)
+        self._layout.addWidget(self.hint)
+        self._layout.addSpacing(10)
         self._layout.addWidget(self.accordion)
         self._layout.addStretch(0)
```

### Comparing `feeluown-4.1.4/feeluown/gui/pages/song_explore.py` & `feeluown-4.1.5/feeluown/gui/pages/song_explore.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/pages/toplist.py` & `feeluown-4.1.5/feeluown/gui/pages/toplist.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/provider_ui.py` & `feeluown-4.1.5/feeluown/gui/provider_ui.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/theme.py` & `feeluown-4.1.5/feeluown/gui/theme.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/tips.py` & `feeluown-4.1.5/feeluown/gui/tips.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/tray.py` & `feeluown-4.1.5/feeluown/gui/tray.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/ui.py` & `feeluown-4.1.5/feeluown/gui/ui.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/uimain/floating_box.py` & `feeluown-4.1.5/feeluown/gui/uimain/floating_box.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/uimain/lyric.py` & `feeluown-4.1.5/feeluown/gui/uimain/lyric.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/uimain/nowplaying_overlay.py` & `feeluown-4.1.5/feeluown/gui/uimain/nowplaying_overlay.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/uimain/page_view.py` & `feeluown-4.1.5/feeluown/gui/uimain/page_view.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/uimain/player_bar.py` & `feeluown-4.1.5/feeluown/gui/uimain/player_bar.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/uimain/playlist_overlay.py` & `feeluown-4.1.5/feeluown/gui/uimain/playlist_overlay.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/uimain/sidebar.py` & `feeluown-4.1.5/feeluown/gui/uimain/sidebar.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/uimain/toolbar.py` & `feeluown-4.1.5/feeluown/gui/uimain/toolbar.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/uimodels/my_music.py` & `feeluown-4.1.5/feeluown/gui/uimodels/my_music.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/uimodels/playlist.py` & `feeluown-4.1.5/feeluown/gui/uimodels/playlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/watch.py` & `feeluown-4.1.5/feeluown/gui/watch.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/accordion.py` & `feeluown-4.1.5/feeluown/gui/widgets/accordion.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/comment_list.py` & `feeluown-4.1.5/feeluown/gui/widgets/comment_list.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/cover_label.py` & `feeluown-4.1.5/feeluown/gui/widgets/cover_label.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/frameless.py` & `feeluown-4.1.5/feeluown/gui/widgets/frameless.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/header.py` & `feeluown-4.1.5/feeluown/gui/widgets/header.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/img_card_list.py` & `feeluown-4.1.5/feeluown/gui/widgets/img_card_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,17 @@
     QBrush, QPainter, QTextOption, QFontMetrics
 )
 from PyQt5.QtWidgets import (
     QAbstractItemDelegate, QListView, QFrame,
 )
 
 from feeluown.utils import aio
-from feeluown.library import AlbumModel, AlbumType
+from feeluown.library import AlbumModel, AlbumType, PlaylistModel, VideoModel
 from feeluown.utils.reader import wrap
+from feeluown.utils.utils import int_to_human_readable
 from feeluown.library import reverse
 from feeluown.gui.helpers import (
     ItemViewNoScrollMixin, resize_font, ReaderFetchMoreMixin, painter_save,
     secondary_text_color
 )
 
 logger = logging.getLogger(__name__)
@@ -121,14 +122,16 @@
             return color
         elif role == Qt.DisplayRole:
             return item.name_display
         elif role == Qt.UserRole:
             return item
         elif role == Qt.WhatsThisRole:
             return self.source_name_map.get(item.source, item.source)
+        elif role == Qt.ToolTipRole:
+            return item.name
         return None
 
 
 class ImgCardListDelegate(QAbstractItemDelegate):
     """
     Card layout should be like the following::
 
@@ -372,15 +375,23 @@
 class VideoCardListModel(ImgCardListModel):
     def data(self, index, role):
         offset = index.row()
         if not index.isValid() or offset >= len(self._items):
             return None
         video = self._items[offset]
         if role == Qt.DisplayRole:
-            return video.title_display
+            return video.title
+        elif role == Qt.ToolTipRole:
+            return video.title
+        elif (
+            role == Qt.WhatsThisRole
+            and isinstance(video, VideoModel)
+            and video.play_count > 0
+        ):
+            return f'► {int_to_human_readable(video.play_count)}'
         return super().data(index, role)
 
 
 class VideoCardListDelegate(ImgCardListDelegate):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -397,15 +408,28 @@
 
     def on_activated(self, index):
         video = index.data(Qt.UserRole)
         self.play_video_needed.emit(video)
 
 
 class PlaylistCardListModel(ImgCardListModel):
-    pass
+    def data(self, index, role):
+        offset = index.row()
+        if not index.isValid() or offset >= len(self._items):
+            return None
+
+        playlist = self._items[offset]
+        if (
+            role == Qt.WhatsThisRole
+            and isinstance(playlist, PlaylistModel)
+            and playlist.play_count > 0
+        ):
+            count = int_to_human_readable(playlist.play_count)
+            return f'► {count}'
+        return super().data(index, role)
 
 
 class PlaylistCardListDelegate(ImgCardListDelegate):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.as_circle = False
```

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/labels.py` & `feeluown-4.1.5/feeluown/gui/widgets/labels.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from PyQt5.QtCore import QTime, Qt
 from PyQt5.QtWidgets import QLabel, QSizePolicy
 
 from feeluown.utils.utils import parse_ms
-from feeluown.gui.helpers import elided_text
+from feeluown.gui.helpers import elided_text, SOLARIZED_COLORS
 
 
 def format_second(s):
     """Format mileseconds to text
 
     >>> format_second(1)
     '00:01'
@@ -68,7 +68,32 @@
         self._app = app
 
         self.setAlignment(Qt.AlignCenter)
         self._app.player_pos_per300ms.changed.connect(self.on_position_changed)
 
     def on_position_changed(self, position):
         self.setText(format_second(position or 0))
+
+
+class MessageLabel(QLabel):
+    """Show warning/error message.
+    """
+    INFO = 'info'
+    ERROR = 'error'
+
+    def __init__(self, text='', level=None, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.setTextFormat(Qt.RichText)
+        self.show_msg(text, level)
+
+    def show_msg(self, text, level=None):
+        if level == MessageLabel.ERROR:
+            hint = '错误提示：'
+            color = 'red'
+        elif level == MessageLabel.INFO:
+            hint = '️提示：'
+            color = SOLARIZED_COLORS['blue']
+        else:
+            hint = '️'
+            color = SOLARIZED_COLORS['blue']
+        self.setText(f"<span style='color: {color};'>{hint}{text}<span>")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/login.py` & `feeluown-4.1.5/feeluown/gui/widgets/login.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/lyric.py` & `feeluown-4.1.5/feeluown/gui/widgets/lyric.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/magicbox.py` & `feeluown-4.1.5/feeluown/gui/widgets/magicbox.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/messageline.py` & `feeluown-4.1.5/feeluown/gui/widgets/messageline.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/meta.py` & `feeluown-4.1.5/feeluown/gui/widgets/meta.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/mpv_.py` & `feeluown-4.1.5/feeluown/gui/widgets/mpv_.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/my_music.py` & `feeluown-4.1.5/feeluown/gui/widgets/my_music.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/playlist_button.py` & `feeluown-4.1.5/feeluown/gui/widgets/playlist_button.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/playlists.py` & `feeluown-4.1.5/feeluown/gui/widgets/playlists.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/progress_slider.py` & `feeluown-4.1.5/feeluown/gui/widgets/progress_slider.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/provider.py` & `feeluown-4.1.5/feeluown/gui/widgets/provider.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/selfpaint_btn.py` & `feeluown-4.1.5/feeluown/gui/widgets/selfpaint_btn.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/separator.py` & `feeluown-4.1.5/feeluown/gui/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/settings.py` & `feeluown-4.1.5/feeluown/gui/widgets/settings.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/song_minicard_list.py` & `feeluown-4.1.5/feeluown/gui/widgets/song_minicard_list.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/songs.py` & `feeluown-4.1.5/feeluown/gui/widgets/songs.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/statusline.py` & `feeluown-4.1.5/feeluown/gui/widgets/statusline.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/statusline_items/notify.py` & `feeluown-4.1.5/feeluown/gui/widgets/statusline_items/notify.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/statusline_items/plugin.py` & `feeluown-4.1.5/feeluown/gui/widgets/statusline_items/plugin.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/tabbar.py` & `feeluown-4.1.5/feeluown/gui/widgets/tabbar.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/table_toolbar.py` & `feeluown-4.1.5/feeluown/gui/widgets/table_toolbar.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/textlist.py` & `feeluown-4.1.5/feeluown/gui/widgets/textlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/video.py` & `feeluown-4.1.5/feeluown/gui/widgets/video.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/volume_button.py` & `feeluown-4.1.5/feeluown/gui/widgets/volume_button.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/gui/widgets/weblogin.py` & `feeluown-4.1.5/feeluown/gui/widgets/weblogin.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/library/__init__.py` & `feeluown-4.1.5/feeluown/library/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/library/base.py` & `feeluown-4.1.5/feeluown/library/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/library/collection.py` & `feeluown-4.1.5/feeluown/library/collection.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/library/flags.py` & `feeluown-4.1.5/feeluown/library/flags.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/library/library.py` & `feeluown-4.1.5/feeluown/library/library.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/library/model_protocol.py` & `feeluown-4.1.5/feeluown/library/model_protocol.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/library/model_state.py` & `feeluown-4.1.5/feeluown/library/model_state.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/library/models.py` & `feeluown-4.1.5/feeluown/library/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -338,14 +338,17 @@
 class ArtistModel(BriefArtistModel, BaseNormalModel):
     meta: Any = ModelMeta.create(ModelType.artist, is_normal=True)
     name: str
     pic_url: str
     aliases: List[str]
     hot_songs: List[BriefSongModel]
     description: str
+    song_count: int = -1
+    album_count: int = -1
+    mv_count: int = -1
 
 
 class AlbumModel(BriefAlbumModel, BaseNormalModel):
     """
     .. versionadded:: 3.8.12
         The `song_count` field.
     """
@@ -383,28 +386,38 @@
 
 class VideoModel(BriefVideoModel, BaseNormalModel):
     meta: Any = ModelMeta.create(ModelType.video, is_normal=True)
     title: str
     artists: List[BriefArtistModel]
     duration: int
     cover: str
+    play_count: int = -1  # -1 means unknown
+    released: str = ''  # publish date. format: 2000-12-27
 
     def model_post_init(self, _):
         super().model_post_init(_)
         self.artists_name = fmt_artists(self.artists)
         self.duration_ms = get_duration_ms(self.duration)
 
 
 class PlaylistModel(BriefPlaylistModel, BaseNormalModel):
     meta: Any = ModelMeta.create(ModelType.playlist, is_normal=True)
     # Since modelv1 playlist does not have creator field, it is set to optional.
     creator: Optional[BriefUserModel] = None
     name: str
     cover: str
     description: str
+    play_count: int = -1  # -1 means unknown
+    created: str = ''  # format: 2000-12-27
+    updated: str = ''  # format: 2000-12-27
+
+    def model_post_init(self, _):
+        super().model_post_init(_)
+        if self.creator is not None:
+            self.creator_name = self.creator.name
 
 
 class SimpleSearchResult(_BaseModel):
     q: str
     songs: List[TSong] = []
     albums: List[TAlbum] = []
     artists: List[TArtist] = []
```

### Comparing `feeluown-4.1.4/feeluown/library/provider.py` & `feeluown-4.1.5/feeluown/library/provider.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/library/provider_protocol.py` & `feeluown-4.1.5/feeluown/library/provider_protocol.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/library/uri.py` & `feeluown-4.1.5/feeluown/library/uri.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/local/__init__.py` & `feeluown-4.1.5/feeluown/local/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/local/db.py` & `feeluown-4.1.5/feeluown/local/db.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/local/provider.py` & `feeluown-4.1.5/feeluown/local/provider.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/local/provider_ui.py` & `feeluown-4.1.5/feeluown/local/provider_ui.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/local/schemas.py` & `feeluown-4.1.5/feeluown/local/schemas.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/local/ui.py` & `feeluown-4.1.5/feeluown/local/ui.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/media.py` & `feeluown-4.1.5/feeluown/media.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/mpv.py` & `feeluown-4.1.5/feeluown/mpv.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/nowplaying/__init__.py` & `feeluown-4.1.5/feeluown/nowplaying/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/nowplaying/linux/__init__.py` & `feeluown-4.1.5/feeluown/nowplaying/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/nowplaying/linux/introspect.xml` & `feeluown-4.1.5/feeluown/nowplaying/linux/introspect.xml`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/nowplaying/linux/mpris2.py` & `feeluown-4.1.5/feeluown/nowplaying/linux/mpris2.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/nowplaying/macos.py` & `feeluown-4.1.5/feeluown/nowplaying/macos.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/nowplaying/nowplaying.py` & `feeluown-4.1.5/feeluown/nowplaying/nowplaying.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/player/__init__.py` & `feeluown-4.1.5/feeluown/player/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/player/base_player.py` & `feeluown-4.1.5/feeluown/player/base_player.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/player/delegate.py` & `feeluown-4.1.5/feeluown/player/delegate.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/player/fm.py` & `feeluown-4.1.5/feeluown/player/fm.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/player/lyric.py` & `feeluown-4.1.5/feeluown/player/lyric.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/player/metadata.py` & `feeluown-4.1.5/feeluown/player/metadata.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/player/mpvplayer.py` & `feeluown-4.1.5/feeluown/player/mpvplayer.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/player/playlist.py` & `feeluown-4.1.5/feeluown/player/playlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/player/radio.py` & `feeluown-4.1.5/feeluown/player/radio.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/player/recently_played.py` & `feeluown-4.1.5/feeluown/player/recently_played.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/plugin.py` & `feeluown-4.1.5/feeluown/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,14 +94,16 @@
 
         names = [self.name]
         # Currently, plugin name looks like fuo_xxx and xxx is the real name.
         # User maye want to define config like app.xxx.X=Y,
         # instead of app.fuo_xxx.X=Y.
         if self.name.startswith('fuo_'):
             names.append(self.name[4:])
+        elif self.name.startswith('feeluown_'):
+            names.append(self.name[9:])
 
         # Define a subconfig(namespace) for plugin so that plugin can
         # define its own configuration fields.
         for name in names:
             config.deffield(name,
                             type_=Config,
                             default=myconfig,
```

### Comparing `feeluown-4.1.4/feeluown/serializers/__init__.py` & `feeluown-4.1.5/feeluown/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/serializers/_plain_formatter.py` & `feeluown-4.1.5/feeluown/serializers/_plain_formatter.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/serializers/base.py` & `feeluown-4.1.5/feeluown/serializers/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/serializers/json_.py` & `feeluown-4.1.5/feeluown/serializers/json_.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/serializers/model_helpers.py` & `feeluown-4.1.5/feeluown/serializers/model_helpers.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/serializers/objs.py` & `feeluown-4.1.5/feeluown/serializers/objs.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/serializers/plain.py` & `feeluown-4.1.5/feeluown/serializers/plain.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/serializers/python.py` & `feeluown-4.1.5/feeluown/serializers/python.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/serializers/typename.py` & `feeluown-4.1.5/feeluown/serializers/typename.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/__init__.py` & `feeluown-4.1.5/feeluown/server/__init__.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/data_structure.py` & `feeluown-4.1.5/feeluown/server/data_structure.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/dslv1/codegen.py` & `feeluown-4.1.5/feeluown/server/dslv1/codegen.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/dslv1/lexer.py` & `feeluown-4.1.5/feeluown/server/dslv1/lexer.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/dslv1/parser.py` & `feeluown-4.1.5/feeluown/server/dslv1/parser.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/dslv2.py` & `feeluown-4.1.5/feeluown/server/dslv2.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/excs.py` & `feeluown-4.1.5/feeluown/server/excs.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/handlers/base.py` & `feeluown-4.1.5/feeluown/server/handlers/base.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/handlers/exec_.py` & `feeluown-4.1.5/feeluown/server/handlers/exec_.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/handlers/handle.py` & `feeluown-4.1.5/feeluown/server/handlers/handle.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/handlers/help.py` & `feeluown-4.1.5/feeluown/server/handlers/help.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/handlers/player.py` & `feeluown-4.1.5/feeluown/server/handlers/player.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/handlers/playlist.py` & `feeluown-4.1.5/feeluown/server/handlers/playlist.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/handlers/search.py` & `feeluown-4.1.5/feeluown/server/handlers/search.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/handlers/show.py` & `feeluown-4.1.5/feeluown/server/handlers/show.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/handlers/sub.py` & `feeluown-4.1.5/feeluown/server/handlers/sub.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/protocol.py` & `feeluown-4.1.5/feeluown/server/protocol.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/pubsub/gateway.py` & `feeluown-4.1.5/feeluown/server/pubsub/gateway.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/pubsub/publishers.py` & `feeluown-4.1.5/feeluown/server/pubsub/publishers.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/server/server.py` & `feeluown-4.1.5/feeluown/server/server.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/task.py` & `feeluown-4.1.5/feeluown/task.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/utils/aio.py` & `feeluown-4.1.5/feeluown/utils/aio.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/utils/audio.py` & `feeluown-4.1.5/feeluown/utils/audio.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/utils/cache.py` & `feeluown-4.1.5/feeluown/utils/cache.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/utils/dispatch.py` & `feeluown-4.1.5/feeluown/utils/dispatch.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/utils/lang.py` & `feeluown-4.1.5/feeluown/utils/lang.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/utils/patch.py` & `feeluown-4.1.5/feeluown/utils/patch.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/utils/reader.py` & `feeluown-4.1.5/feeluown/utils/reader.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/utils/request.py` & `feeluown-4.1.5/feeluown/utils/request.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/utils/router.py` & `feeluown-4.1.5/feeluown/utils/router.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/utils/sync.py` & `feeluown-4.1.5/feeluown/utils/sync.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/utils/utils.py` & `feeluown-4.1.5/feeluown/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,7 +257,15 @@
             raise ValueError("list.remove(x): x not in list")
         idx = self._map[item]
         self.pop(idx)
 
     def clear(self):
         self._map.clear()
         super().clear()
+
+
+def int_to_human_readable(i):
+    if i >= 100000000:
+        return f'{i / 100000000:.1f}亿'
+    elif i >= 10000:
+        return f'{i / 10000:.1f}万'
+    return i
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `feeluown-4.1.4/feeluown/utils/yt_dlp_cookies.py` & `feeluown-4.1.5/feeluown/utils/yt_dlp_cookies.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/version.py` & `feeluown-4.1.5/feeluown/version.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/webserver/jsonrpc_.py` & `feeluown-4.1.5/feeluown/webserver/jsonrpc_.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown/webserver/server.py` & `feeluown-4.1.5/feeluown/webserver/server.py`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/feeluown.egg-info/PKG-INFO` & `feeluown-4.1.5/feeluown.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feeluown
-Version: 4.1.4
+Version: 4.1.5
 Summary: *nix music player
 Home-page: https://github.com/feeluown/FeelUOwn
 Author: feeluown
 Author-email: yinshaowen241@gmail.com
 License: GPL-3.0
 Description: ## FeelUOwn - feel your own
         
@@ -44,16 +44,16 @@
         
         # macOS（也可以下载打包好的二进制）
         brew tap feeluown/feeluown
         brew install feeluown --with-battery # 安装 FeelUOwn 以及扩展
         feeluown genicon                     # 在桌面生成 FeelUOwn 图标
         ```
         
-        Windows 用户可以在 Release 页面下载预打包好的二进制。
-        Gentoo, NixOS, Debian 等 Linux 发行版也支持使用其系统包管理器安装！
+        Windows 和 macOS 用户可以在 Release 页面下载预打包好的二进制。
+        Gentoo, NixOS, Debian, openSUSE 等 Linux 发行版也支持使用其系统包管理器安装！
         详情可以参考文档：https://feeluown.readthedocs.io/ ，
         也欢迎你加入开发者/用户[交流群](https://t.me/joinchat/H7k12hG5HYsGy7RVvK_Dwg)。
         
         ### 免责声明
         
         FeelUown（以下简称“本软件”）是一个个人媒体资源播放工具。本软件提供的所有功能和资料
         不得用于任何商业用途。用户可以自由选择是否使用本产品提供的软件。如果用户下载、安装、
```

### Comparing `feeluown-4.1.4/feeluown.egg-info/SOURCES.txt` & `feeluown-4.1.5/feeluown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/setup.cfg` & `feeluown-4.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `feeluown-4.1.4/setup.py` & `feeluown-4.1.5/setup.py`

 * *Files identical despite different names*

