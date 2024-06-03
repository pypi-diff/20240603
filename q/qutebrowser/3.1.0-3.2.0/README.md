# Comparing `tmp/qutebrowser-3.1.0.tar.gz` & `tmp/qutebrowser-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qutebrowser-3.1.0.tar", last modified: Fri Dec  8 15:32:17 2023, max compression
+gzip compressed data, was "qutebrowser-3.2.0.tar", last modified: Mon Jun  3 14:43:35 2024, max compression
```

## Comparing `qutebrowser-3.1.0.tar` & `qutebrowser-3.2.0.tar`

### file list

```diff
@@ -1,955 +1,958 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.655451 qutebrowser-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15731 2023-12-08 15:32:17.655451 qutebrowser-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14402 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/README.asciidoc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.519451 qutebrowser-3.1.0/doc/
--rw-r--r--   0 runner    (1001) docker     (127)   233200 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/doc/changelog.asciidoc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.519451 qutebrowser-3.1.0/doc/img/
--rw-r--r--   0 runner    (1001) docker     (127)   708315 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/doc/img/cheatsheet-big.png
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/doc/img/cheatsheet-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    36391 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/doc/img/completion.png
--rw-r--r--   0 runner    (1001) docker     (127)    34786 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/doc/img/downloads.png
--rw-r--r--   0 runner    (1001) docker     (127)    46347 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/doc/img/hints.png
--rw-r--r--   0 runner    (1001) docker     (127)    34604 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/doc/img/main.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.519451 qutebrowser-3.1.0/doc/img/sponsors/
--rw-r--r--   0 runner    (1001) docker     (127)    11046 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/doc/img/sponsors/hsr.png
--rw-r--r--   0 runner    (1001) docker     (127)    33193 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/doc/img/sponsors/macstadium.png
--rw-r--r--   0 runner    (1001) docker     (127)     8222 2023-12-08 15:32:13.000000 qutebrowser-3.1.0/doc/qutebrowser.1
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/doc/qutebrowser.1.asciidoc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.523451 qutebrowser-3.1.0/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.523451 qutebrowser-3.1.0/misc/apparmor/
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/apparmor/usr.bin.qutebrowser
--rw-r--r--   0 runner    (1001) docker     (127)   179325 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/cheatsheet.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/org.qutebrowser.qutebrowser.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/org.qutebrowser.qutebrowser.desktop
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.527452 qutebrowser-3.1.0/misc/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-check-manifest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-check-manifest.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      839 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-dev.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-docs.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      540 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-flake8.txt
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-flake8.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-mypy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-mypy.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyinstaller.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyinstaller.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pylint.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pylint.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-5.15.2.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-5.15.2.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-5.15.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-5.15.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-5.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-5.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-6.2.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-6.2.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-6.3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-6.3.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-6.4.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-6.4.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-6.5.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-6.5.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-6.6.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-6.6.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-6.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt-6.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyqt.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyroma.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-pyroma.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-qutebrowser.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      578 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-sphinx.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-sphinx.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-tests-bleeding.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-tests.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-tox.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-tox.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-vulture.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-vulture.txt-raw
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-yamllint.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/requirements/requirements-yamllint.txt-raw
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.531452 qutebrowser-3.1.0/misc/userscripts/
--rw-r--r--   0 runner    (1001) docker     (127)     6635 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     5025 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/add-nextcloud-bookmarks
--rwxr-xr-x   0 runner    (1001) docker     (127)     3912 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/add-nextcloud-cookbook
--rwxr-xr-x   0 runner    (1001) docker     (127)     5821 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/cast
--rwxr-xr-x   0 runner    (1001) docker     (127)     1405 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/dmenu_qutebrowser
--rwxr-xr-x   0 runner    (1001) docker     (127)     1579 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/format_json
--rwxr-xr-x   0 runner    (1001) docker     (127)     2162 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/getbib
--rwxr-xr-x   0 runner    (1001) docker     (127)     4270 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/kodi
--rwxr-xr-x   0 runner    (1001) docker     (127)     3747 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/open_download
--rwxr-xr-x   0 runner    (1001) docker     (127)      899 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/openfeeds
--rwxr-xr-x   0 runner    (1001) docker     (127)    13375 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/password_fill
--rwxr-xr-x   0 runner    (1001) docker     (127)      253 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/qr
--rwxr-xr-x   0 runner    (1001) docker     (127)     4806 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/qute-1pass
--rwxr-xr-x   0 runner    (1001) docker     (127)    10480 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/qute-bitwarden
--rwxr-xr-x   0 runner    (1001) docker     (127)     8673 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/qute-keepass
--rwxr-xr-x   0 runner    (1001) docker     (127)    14941 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/qute-keepassxc
--rwxr-xr-x   0 runner    (1001) docker     (127)     6714 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/qute-lastpass
--rwxr-xr-x   0 runner    (1001) docker     (127)    12079 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/qute-pass
--rwxr-xr-x   0 runner    (1001) docker     (127)     1755 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/qutedmenu
--rwxr-xr-x   0 runner    (1001) docker     (127)     1946 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/readability
--rwxr-xr-x   0 runner    (1001) docker     (127)     5442 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/readability-js
--rwxr-xr-x   0 runner    (1001) docker     (127)      938 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/ripbang
--rwxr-xr-x   0 runner    (1001) docker     (127)     3031 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/rss
--rwxr-xr-x   0 runner    (1001) docker     (127)     1359 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/taskadd
--rwxr-xr-x   0 runner    (1001) docker     (127)     1550 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/tor_identity
--rwxr-xr-x   0 runner    (1001) docker     (127)     5092 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/misc/userscripts/view_in_mpv
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.531452 qutebrowser-3.1.0/qutebrowser/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.535452 qutebrowser-3.1.0/qutebrowser/api/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/api/apitypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7945 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/api/cmdutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/api/downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/api/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/api/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/api/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/api/qtutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20493 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.539451 qutebrowser-3.1.0/qutebrowser/browser/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47968 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/browsertab.py
--rw-r--r--   0 runner    (1001) docker     (127)    75641 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    49166 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/downloadview.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/eventfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18626 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/greasemonkey.py
--rw-r--r--   0 runner    (1001) docker     (127)    43912 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/hints.py
--rw-r--r--   0 runner    (1001) docker     (127)    17758 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7761 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/navigate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.539451 qutebrowser-3.1.0/qutebrowser/browser/network/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11848 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/network/pac.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/network/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7763 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/pdfjs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22716 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/qtnetworkdownloads.py
--rw-r--r--   0 runner    (1001) docker     (127)    19725 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/qutescheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    19909 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/signalfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/urlmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16564 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webelem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.539451 qutebrowser-3.1.0/qutebrowser/browser/webengine/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webengine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webengine/certificateerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webengine/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)    14405 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webengine/darkmode.py
--rw-r--r--   0 runner    (1001) docker     (127)     9470 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webengine/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    45018 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webengine/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webengine/spell.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webengine/tabhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webengine/webenginedownloads.py
--rw-r--r--   0 runner    (1001) docker     (127)    10521 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webengine/webengineelem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webengine/webengineinspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webengine/webenginequtescheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    22735 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webengine/webenginesettings.py
--rw-r--r--   0 runner    (1001) docker     (127)    63864 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webengine/webenginetab.py
--rw-r--r--   0 runner    (1001) docker     (127)    14119 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webengine/webview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.543451 qutebrowser-3.1.0/qutebrowser/browser/webkit/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/certificateerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/http.py
--rw-r--r--   0 runner    (1001) docker     (127)    20002 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/mhtml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.543451 qutebrowser-3.1.0/qutebrowser/browser/webkit/network/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/network/filescheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    17225 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/network/networkmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/network/networkreply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/network/webkitqutescheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/tabhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/webkitelem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/webkithistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/webkitinspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/webkitsettings.py
--rw-r--r--   0 runner    (1001) docker     (127)    39859 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/webkittab.py
--rw-r--r--   0 runner    (1001) docker     (127)    22561 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/webpage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8092 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/browser/webkit/webview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.543451 qutebrowser-3.1.0/qutebrowser/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/commands/argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/commands/cmdexc.py
--rw-r--r--   0 runner    (1001) docker     (127)    22413 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/commands/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/commands/runners.py
--rw-r--r--   0 runner    (1001) docker     (127)    15624 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/commands/userscripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.547452 qutebrowser-3.1.0/qutebrowser/completion/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/completion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12552 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/completion/completer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/completion/completiondelegate.py
--rw-r--r--   0 runner    (1001) docker     (127)    17515 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/completion/completionwidget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.547452 qutebrowser-3.1.0/qutebrowser/completion/models/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/completion/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/completion/models/completionmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/completion/models/configmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/completion/models/filepathcategory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/completion/models/histcategory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/completion/models/listcategory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/completion/models/miscmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/completion/models/urlmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/completion/models/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.547452 qutebrowser-3.1.0/qutebrowser/components/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/components/adblockcommands.py
--rw-r--r--   0 runner    (1001) docker     (127)    12360 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/components/braveadblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/components/caretcommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     9902 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/components/hostblock.py
--rw-r--r--   0 runner    (1001) docker     (127)    13770 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/components/misccommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     9709 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/components/readlinecommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/components/scrollcommands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.547452 qutebrowser-3.1.0/qutebrowser/components/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/components/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/components/utils/blockutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/components/zoomcommands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.551452 qutebrowser-3.1.0/qutebrowser/config/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24260 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/config/configcache.py
--rw-r--r--   0 runner    (1001) docker     (127)    19542 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/config/configcommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/config/configdata.py
--rw-r--r--   0 runner    (1001) docker     (127)   113728 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/config/configdata.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/config/configexc.py
--rw-r--r--   0 runner    (1001) docker     (127)    39763 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/config/configfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/config/configinit.py
--rw-r--r--   0 runner    (1001) docker     (127)    64724 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/config/configtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12219 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/config/configutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15191 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/config/qtargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/config/stylesheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9286 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/config/websettings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.551452 qutebrowser-3.1.0/qutebrowser/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/extensions/interceptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/extensions/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-08 15:32:17.000000 qutebrowser-3.1.0/qutebrowser/git-commit-id
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.555451 qutebrowser-3.1.0/qutebrowser/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/back.html
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/bindings.html
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/bookmarks.html
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/dirbrowser.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.555451 qutebrowser-3.1.0/qutebrowser/html/doc/
--rw-r--r--   0 runner    (1001) docker     (127)   360260 2023-12-08 15:32:05.000000 qutebrowser-3.1.0/qutebrowser/html/doc/changelog.html
--rw-r--r--   0 runner    (1001) docker     (127)   177952 2023-12-08 15:32:12.000000 qutebrowser-3.1.0/qutebrowser/html/doc/commands.html
--rw-r--r--   0 runner    (1001) docker     (127)    53744 2023-12-08 15:32:11.000000 qutebrowser-3.1.0/qutebrowser/html/doc/configuring.html
--rw-r--r--   0 runner    (1001) docker     (127)    75683 2023-12-08 15:32:06.000000 qutebrowser-3.1.0/qutebrowser/html/doc/contributing.html
--rw-r--r--   0 runner    (1001) docker     (127)    57671 2023-12-08 15:32:03.000000 qutebrowser-3.1.0/qutebrowser/html/doc/faq.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.559451 qutebrowser-3.1.0/qutebrowser/html/doc/img/
--rw-r--r--   0 runner    (1001) docker     (127)   708315 2023-12-08 15:32:12.000000 qutebrowser-3.1.0/qutebrowser/html/doc/img/cheatsheet-big.png
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2023-12-08 15:32:12.000000 qutebrowser-3.1.0/qutebrowser/html/doc/img/cheatsheet-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    25157 2023-12-08 15:32:07.000000 qutebrowser-3.1.0/qutebrowser/html/doc/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    46416 2023-12-08 15:32:06.000000 qutebrowser-3.1.0/qutebrowser/html/doc/install.html
--rw-r--r--   0 runner    (1001) docker     (127)    26683 2023-12-08 15:32:06.000000 qutebrowser-3.1.0/qutebrowser/html/doc/quickstart.html
--rw-r--r--   0 runner    (1001) docker     (127)   340303 2023-12-08 15:32:09.000000 qutebrowser-3.1.0/qutebrowser/html/doc/settings.html
--rw-r--r--   0 runner    (1001) docker     (127)    29686 2023-12-08 15:32:07.000000 qutebrowser-3.1.0/qutebrowser/html/doc/stacktrace.html
--rw-r--r--   0 runner    (1001) docker     (127)    27176 2023-12-08 15:32:06.000000 qutebrowser-3.1.0/qutebrowser/html/doc/userscripts.html
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/error.html
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/history.html
--rw-r--r--   0 runner    (1001) docker     (127)    37521 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/license.html
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/log.html
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/no_pdfjs.html
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/pre.html
--rw-r--r--   0 runner    (1001) docker     (127)      556 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/process.html
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/settings.html
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/startpage.html
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/styled.html
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/tabs.html
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/version.html
--rw-r--r--   0 runner    (1001) docker     (127)      875 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/warning-qt5.html
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/warning-sessions.html
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/html/warning-webkit.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.559451 qutebrowser-3.1.0/qutebrowser/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     6426 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-128x128.png
--rw-r--r--   0 runner    (1001) docker     (127)      856 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-24x24.png
--rw-r--r--   0 runner    (1001) docker     (127)    13690 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-256x256.png
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-48x48.png
--rw-r--r--   0 runner    (1001) docker     (127)    30109 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-64x64.png
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-96x96.png
--rw-r--r--   0 runner    (1001) docker     (127)   131549 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-all.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15990 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)   196205 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/icons/qutebrowser.icns
--rw-r--r--   0 runner    (1001) docker     (127)   115490 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/icons/qutebrowser.ico
--rw-r--r--   0 runner    (1001) docker     (127)    16018 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/icons/qutebrowser.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/icons/qutebrowser.xpm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.559451 qutebrowser-3.1.0/qutebrowser/img/
--rw-r--r--   0 runner    (1001) docker     (127)    58370 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/img/broken_qutebrowser_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    23799 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/img/file.svg
--rw-r--r--   0 runner    (1001) docker     (127)    22869 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/img/folder.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.563451 qutebrowser-3.1.0/qutebrowser/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)    49901 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/javascript/caret.js
--rw-r--r--   0 runner    (1001) docker     (127)      292 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/javascript/global_wrapper.js
--rw-r--r--   0 runner    (1001) docker     (127)     7847 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/javascript/greasemonkey_wrapper.js
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/javascript/history.js
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/javascript/pac_utils.js
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/javascript/position_caret.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.563451 qutebrowser-3.1.0/qutebrowser/javascript/quirks/
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/javascript/quirks/array_at.user.js
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/javascript/quirks/discord.user.js
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/javascript/quirks/googledocs.user.js
--rw-r--r--   0 runner    (1001) docker     (127)      874 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/javascript/quirks/string_replaceall.user.js
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/javascript/quirks/whatsapp_web.user.js
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/javascript/scroll.js
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/javascript/stylesheet.js
--rw-r--r--   0 runner    (1001) docker     (127)    12704 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/javascript/webelem.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.563451 qutebrowser-3.1.0/qutebrowser/keyinput/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/keyinput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13956 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/keyinput/basekeyparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/keyinput/eventfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)    25987 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/keyinput/keyutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/keyinput/macros.py
--rw-r--r--   0 runner    (1001) docker     (127)    17408 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/keyinput/modeman.py
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/keyinput/modeparsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.567452 qutebrowser-3.1.0/qutebrowser/mainwindow/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28104 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/messageview.py
--rw-r--r--   0 runner    (1001) docker     (127)    37168 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.567452 qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/backforward.py
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/clock.py
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/keystring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/percentage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/searchmatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/tabindex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/textbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/url.py
--rw-r--r--   0 runner    (1001) docker     (127)    43996 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/tabbedbrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)    38092 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/tabwidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/mainwindow/windowundo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.571452 qutebrowser-3.1.0/qutebrowser/misc/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/autoupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)    17398 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/backendproblem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/binparsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/checkpyver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/cmdhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/consolewidget.py
--rw-r--r--   0 runner    (1001) docker     (127)    25317 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/crashdialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    16525 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/crashsignal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/debugcachestats.py
--rw-r--r--   0 runner    (1001) docker     (127)    12053 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/earlyinit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/elf.py
--rw-r--r--   0 runner    (1001) docker     (127)    15687 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/guiprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    19762 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/ipc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/keyhintwidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/lineparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15522 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/miscwidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/msgbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/nativeeventfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/pakjoy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10888 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/quitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/savemanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    24623 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/split.py
--rw-r--r--   0 runner    (1001) docker     (127)    20676 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/misc/utilcmds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.575451 qutebrowser-3.1.0/qutebrowser/qt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/_core_pyqtproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/dbus.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/machinery.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/opengl.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/printsupport.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/qml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/sip.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/webenginecore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/webenginewidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/webkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/webkitwidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qt/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10132 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/qutebrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.575451 qutebrowser-3.1.0/qutebrowser/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12321 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/docutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/javascript.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)    20930 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    11821 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/objreg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/qtlog.py
--rw-r--r--   0 runner    (1001) docker     (127)    22478 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/qtutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    11940 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/standarddir.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/testfile
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/urlmatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    21146 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/urlutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16311 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/usertypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    26624 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37418 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.655451 qutebrowser-3.1.0/qutebrowser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15731 2023-12-08 15:32:17.000000 qutebrowser-3.1.0/qutebrowser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32100 2023-12-08 15:32:17.000000 qutebrowser-3.1.0/qutebrowser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 15:32:17.000000 qutebrowser-3.1.0/qutebrowser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-08 15:32:17.000000 qutebrowser-3.1.0/qutebrowser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-08 15:32:17.000000 qutebrowser-3.1.0/qutebrowser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-08 15:32:17.000000 qutebrowser-3.1.0/qutebrowser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 15:32:13.000000 qutebrowser-3.1.0/qutebrowser.egg-info/zip-safe
--rwxr-xr-x   0 runner    (1001) docker     (127)      307 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/qutebrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.579451 qutebrowser-3.1.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/scripts/cycle-inputs.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     8150 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/scripts/dictcli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5440 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/scripts/hist_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/scripts/hostblock_blame.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11263 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/scripts/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/scripts/keytester.py
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/scripts/link_pyqt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19825 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/scripts/mkvenv.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      537 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/scripts/open_url_in_instance.sh
--rw-r--r--   0 runner    (1001) docker     (127)      916 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/scripts/opengl_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/scripts/setupcommon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.579451 qutebrowser-3.1.0/scripts/testbrowser/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1226 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/scripts/testbrowser/testbrowser_webengine.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1176 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/scripts/testbrowser/testbrowser_webkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 15:32:17.655451 qutebrowser-3.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3309 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.579451 qutebrowser-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.579451 qutebrowser-3.1.0/tests/end2end/
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.587452 qutebrowser-3.1.0/tests/end2end/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.587452 qutebrowser-3.1.0/tests/end2end/data/backforward/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/backforward/1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/backforward/2.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/backforward/3.txt
--rw-r--r--   0 runner    (1001) docker     (127)   257960 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/blocked-hosts.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.587452 qutebrowser-3.1.0/tests/end2end/data/blocking/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/blocking/external_logo.html
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/blocking/qutebrowser-adblock
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/blocking/qutebrowser-hosts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.587452 qutebrowser-3.1.0/tests/end2end/data/brave-adblock/
--rw-r--r--   0 runner    (1001) docker     (127)    15313 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/brave-adblock/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/brave-adblock/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/brave-adblock/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)  1279186 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/brave-adblock/ublock-matches.tsv.gz
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/caret.html
--rw-r--r--   0 runner    (1001) docker     (127)      790 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/click_element.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.591452 qutebrowser-3.1.0/tests/end2end/data/crashers/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/crashers/installedapp.html
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/crashers/webrtc.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.591452 qutebrowser-3.1.0/tests/end2end/data/darkmode/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/darkmode/blank.html
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/darkmode/mathml-display.html
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/darkmode/mathml-inline.html
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/darkmode/mathml.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/darkmode/prefers-color-scheme.html
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/darkmode/yellow.html
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/data_link.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.591452 qutebrowser-3.1.0/tests/end2end/data/downloads/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/download with no title.html
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/download with spaces.bin
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/download.bin
--rw-r--r--   0 runner    (1001) docker     (127)        2 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/download2.bin
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/downloads.html
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/issue1243.html
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/issue1535.html
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/issue1725.html
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/issue2134.html
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/issue2298.html
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/issue889.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.511452 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.595451 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/Background.png
--rw-r--r--   0 runner    (1001) docker     (127)    17035 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/Banner.png
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/DYK.png
--rw-r--r--   0 runner    (1001) docker     (127)      511 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/Inline.png
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/base.css
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/complex.html
--rw-r--r--   0 runner    (1001) docker     (127)    54939 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/complex.mht
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/external-in-extern.css
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/not-css.qss
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/requests
--rw-r--r--   0 runner    (1001) docker     (127)      434 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/script.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.595451 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/simple/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/simple/requests
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/simple/simple.html
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/simple/simple.mht
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/qutebrowser.png
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/downloads/ä-issue908.bin
--rw-r--r--   0 runner    (1001) docker     (127)   593611 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/easylist.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)   144367 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/easyprivacy.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/editor.html
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/email_address.html
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/fileselect.html
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hello.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hello2.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hello3.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hinting.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.595451 qutebrowser-3.1.0/tests/end2end/data/hints/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.599451 qutebrowser-3.1.0/tests/end2end/data/hints/ace/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/ace/ace.html
--rw-r--r--   0 runner    (1001) docker     (127)   661179 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/ace/ace.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.599451 qutebrowser-3.1.0/tests/end2end/data/hints/angular1/
--rw-r--r--   0 runner    (1001) docker     (127)   167131 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/angular1/angular.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    13147 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/benchmark.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.599451 qutebrowser-3.1.0/tests/end2end/data/hints/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)   198313 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/bootstrap/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)      537 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/bootstrap/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/buttons.html
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/custom_group.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.599451 qutebrowser-3.1.0/tests/end2end/data/hints/html/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/html/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/html/angular1.html
--rw-r--r--   0 runner    (1001) docker     (127)      444 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/html/click_handler.html
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/html/invisible.html
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/html/javascript.html
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/html/nested_block_style.html
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/html/nested_formatting_tags.html
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/html/nested_table_style.html
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/html/simple.html
--rw-r--r--   0 runner    (1001) docker     (127)      262 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/html/tabindex-negative.html
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/html/target_blank_js.html
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/html/with_spaces.html
--rw-r--r--   0 runner    (1001) docker     (127)      772 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/html/wrapped.html
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/html/wrapped_button.html
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/html/zoom_precision.html
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/iframe.html
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/iframe_button.html
--rw-r--r--   0 runner    (1001) docker     (127)      249 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/iframe_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/iframe_scroll.html
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/iframe_target.html
--rw-r--r--   0 runner    (1001) docker     (127)      926 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/input.html
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/issue1186.html
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/issue1393.html
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/issue3711.html
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/issue3711_frame.html
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/link_blank.html
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/link_inject.html
--rw-r--r--   0 runner    (1001) docker     (127)      872 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/link_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/link_span.html
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/number.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/rapid.html
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/hints/short_dict.html
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/iframe_search.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.511452 qutebrowser-3.1.0/tests/end2end/data/insert_mode_settings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.603451 qutebrowser-3.1.0/tests/end2end/data/insert_mode_settings/html/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/insert_mode_settings/html/autofocus.html
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/insert_mode_settings/html/input.html
--rw-r--r--   0 runner    (1001) docker     (127)      562 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/insert_mode_settings/html/textarea.html
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/invalid_link.html
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/invalid_resource.html
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/issue2569.html
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/issue4011.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.603451 qutebrowser-3.1.0/tests/end2end/data/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/javascript/consolelog.html
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/javascript/enabled.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.603451 qutebrowser-3.1.0/tests/end2end/data/javascript/img/
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/javascript/img/big.png
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/javascript/img/padded.png
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/javascript/img/padded2.png
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/javascript/img/rgb.png
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/javascript/img/rgba.png
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/javascript/localstorage.html
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/javascript/notifications.html
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/javascript/window_open.html
--rw-r--r--   0 runner    (1001) docker     (127)      728 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/javascript/windowsize.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.603451 qutebrowser-3.1.0/tests/end2end/data/keyinput/
--rw-r--r--   0 runner    (1001) docker     (127)      722 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/keyinput/log.html
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/l33t.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/long_load.html
--rw-r--r--   0 runner    (1001) docker     (127)      487 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/marks.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.603451 qutebrowser-3.1.0/tests/end2end/data/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/misc/hello.txt.html
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/misc/jseval.html
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/misc/jseval_file.js
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/misc/pyeval_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/misc/qutescheme_csrf.html
--rw-r--r--   0 runner    (1001) docker     (127)    16667 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/misc/test.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/misc/xhr_headers.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.607452 qutebrowser-3.1.0/tests/end2end/data/navigate/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/navigate/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/navigate/multilinelinks.html
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/navigate/next.html
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/navigate/prev.html
--rw-r--r--   0 runner    (1001) docker     (127)      291 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/navigate/rel.html
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/navigate/rel_nofollow.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.607452 qutebrowser-3.1.0/tests/end2end/data/navigate/sub/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/navigate/sub/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.607452 qutebrowser-3.1.0/tests/end2end/data/numbers/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/10.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/11.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/12.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/13.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/14.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/15.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/16.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/17.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/18.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/19.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/2.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/3.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/4.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/5.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/6.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/7.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/8.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/numbers/9.txt
--rw-r--r--   0 runner    (1001) docker     (127)      878 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/paste_primary.html
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/prefers_reduced_motion.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.607452 qutebrowser-3.1.0/tests/end2end/data/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/prompt/geolocation.html
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/prompt/jsalert.html
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/prompt/jsconfirm.html
--rw-r--r--   0 runner    (1001) docker     (127)      544 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/prompt/jsprompt.html
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/prompt/notifications.html
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/prompt/script.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/reload.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.611451 qutebrowser-3.1.0/tests/end2end/data/scroll/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/scroll/no_doctype.html
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/scroll/position_absolute.html
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/scroll/simple.html
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/search.html
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/search_select.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.611451 qutebrowser-3.1.0/tests/end2end/data/service-worker/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/service-worker/data.json
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/service-worker/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/service-worker/worker.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.611451 qutebrowser-3.1.0/tests/end2end/data/sessions/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/sessions/history_replace_state.html
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/sessions/snowman.html
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/smart.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.611451 qutebrowser-3.1.0/tests/end2end/data/ssl/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/ssl/cert.csr
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/ssl/cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/ssl/key.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/ssl/privkey.pem
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/title with spaces.html
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/title.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.611451 qutebrowser-3.1.0/tests/end2end/data/userscripts/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/userscripts/echo.bat
--rwxr-xr-x   0 runner    (1001) docker     (127)       71 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/userscripts/echo_hint_text
--rwxr-xr-x   0 runner    (1001) docker     (127)      194 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/userscripts/hello_if_count
--rwxr-xr-x   0 runner    (1001) docker     (127)       54 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/userscripts/open_current_url
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/userscripts/open_current_url.bat
--rwxr-xr-x   0 runner    (1001) docker     (127)      343 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/userscripts/stdinclose.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/words.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/data/äöü.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.619451 qutebrowser-3.1.0/tests/end2end/features/
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/backforward.feature
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/caret.feature
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/completion.feature
--rw-r--r--   0 runner    (1001) docker     (127)    25370 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    34700 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/downloads.feature
--rw-r--r--   0 runner    (1001) docker     (127)    12203 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/editor.feature
--rw-r--r--   0 runner    (1001) docker     (127)    28200 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/hints.feature
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/history.feature
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/invoke.feature
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/javascript.feature
--rw-r--r--   0 runner    (1001) docker     (127)     8009 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/keyinput.feature
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/marks.feature
--rw-r--r--   0 runner    (1001) docker     (127)    25182 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/misc.feature
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/navigate.feature
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/notifications.feature
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/open.feature
--rw-r--r--   0 runner    (1001) docker     (127)    10623 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/private.feature
--rw-r--r--   0 runner    (1001) docker     (127)    22477 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/prompts.feature
--rw-r--r--   0 runner    (1001) docker     (127)    12980 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/qutescheme.feature
--rw-r--r--   0 runner    (1001) docker     (127)    12723 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/scroll.feature
--rw-r--r--   0 runner    (1001) docker     (127)    16142 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/search.feature
--rw-r--r--   0 runner    (1001) docker     (127)    15515 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/sessions.feature
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/spawn.feature
--rw-r--r--   0 runner    (1001) docker     (127)    66742 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/tabs.feature
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_backforward_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_caret_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_completion_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_downloads_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_editor_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_hints_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_history_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_invoke_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_javascript_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_keyinput_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_marks_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_misc_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_navigate_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_notifications_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_open_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_private_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_prompts_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_qutescheme_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_scroll_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_search_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_sessions_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_spawn_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_tabs_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_urlmarks_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_utilcmds_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_yankpaste_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/test_zoom_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/urlmarks.feature
--rw-r--r--   0 runner    (1001) docker     (127)     6817 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/utilcmds.feature
--rw-r--r--   0 runner    (1001) docker     (127)    14772 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/yankpaste.feature
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/features/zoom.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.623451 qutebrowser-3.1.0/tests/end2end/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     8909 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/fixtures/notificationserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    38108 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/fixtures/quteprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/fixtures/test_quteprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/fixtures/test_testprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/fixtures/test_webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    17025 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/fixtures/testprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     6777 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/fixtures/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/fixtures/webserver_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/fixtures/webserver_sub_ssl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.623451 qutebrowser-3.1.0/tests/end2end/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/misc/test_runners_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.623451 qutebrowser-3.1.0/tests/end2end/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/templates/headers-link.html
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/templates/https-iframe.html
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/templates/https-script.html
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/test_adblock_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/test_dirbrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/test_hints_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/test_insert_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    35750 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/test_invocations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/end2end/test_mhtml_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.623451 qutebrowser-3.1.0/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)    22370 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/helpers/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/helpers/logfail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/helpers/messagemock.py
--rw-r--r--   0 runner    (1001) docker     (127)    19749 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/helpers/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/helpers/test_helper_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/helpers/test_logfail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/helpers/test_stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8840 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/helpers/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.623451 qutebrowser-3.1.0/tests/manual/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.623451 qutebrowser-3.1.0/tests/manual/completion/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/manual/completion/changing_title.html
--rw-r--r--   0 runner    (1001) docker     (127)      363 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/manual/files.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.623451 qutebrowser-3.1.0/tests/manual/hints/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/manual/hints/find_implementation.html
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/manual/hints/hide_unmatched_rapid_hints.html
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/manual/hints/issue824.html
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/manual/hints/issue925.html
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/manual/hints/other.html
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/manual/hints/zoom.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.623451 qutebrowser-3.1.0/tests/manual/history/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/manual/history/visited.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.623451 qutebrowser-3.1.0/tests/manual/js/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/manual/js/jsalert_multiline.html
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/manual/js/jsconfirm.html
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/manual/js/jsprompt.html
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/manual/mouse.html
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/test_conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.627452 qutebrowser-3.1.0/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.627452 qutebrowser-3.1.0/tests/unit/api/
--rw-r--r--   0 runner    (1001) docker     (127)    17408 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/api/test_cmdutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.627452 qutebrowser-3.1.0/tests/unit/browser/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/test_browsertab.py
--rw-r--r--   0 runner    (1001) docker     (127)    16004 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/test_caret.py
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/test_downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/test_downloadview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/test_hints.py
--rw-r--r--   0 runner    (1001) docker     (127)    22503 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/test_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/test_navigate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8654 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/test_pdfjs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10737 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/test_qutescheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/test_signalfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/test_urlmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.627452 qutebrowser-3.1.0/tests/unit/browser/webengine/
--rw-r--r--   0 runner    (1001) docker     (127)     9230 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webengine/test_darkmode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webengine/test_spell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webengine/test_webengine_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webengine/test_webenginedownloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webengine/test_webengineinterceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webengine/test_webenginesettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8194 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webengine/test_webenginetab.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webengine/test_webview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.631451 qutebrowser-3.1.0/tests/unit/browser/webkit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.631451 qutebrowser-3.1.0/tests/unit/browser/webkit/http/
--rw-r--r--   0 runner    (1001) docker     (127)    35615 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webkit/http/test_content_disposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webkit/http/test_http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.631451 qutebrowser-3.1.0/tests/unit/browser/webkit/network/
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webkit/network/test_filescheme.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webkit/network/test_networkmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webkit/network/test_networkreply.py
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webkit/network/test_pac.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webkit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webkit/test_certificateerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webkit/test_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9503 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webkit/test_mhtml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webkit/test_tabhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webkit/test_webkit_view.py
--rw-r--r--   0 runner    (1001) docker     (127)    34619 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webkit/test_webkitelem.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/browser/webkit/test_webkitsettings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.631451 qutebrowser-3.1.0/tests/unit/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/commands/test_argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/commands/test_cmdexc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/commands/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/commands/test_userscripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.631451 qutebrowser-3.1.0/tests/unit/completion/
--rw-r--r--   0 runner    (1001) docker     (127)    14395 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/completion/test_completer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/completion/test_completiondelegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/completion/test_completionmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/completion/test_completionwidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/completion/test_histcategory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/completion/test_listcategory.py
--rw-r--r--   0 runner    (1001) docker     (127)    51679 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/completion/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.635451 qutebrowser-3.1.0/tests/unit/components/
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/components/test_blockutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15792 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/components/test_braveadblock.py
--rw-r--r--   0 runner    (1001) docker     (127)    19813 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/components/test_hostblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/components/test_misccommands.py
--rw-r--r--   0 runner    (1001) docker     (127)    12684 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/components/test_readlinecommands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.635451 qutebrowser-3.1.0/tests/unit/config/
--rw-r--r--   0 runner    (1001) docker     (127)    31855 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/config/test_configcache.py
--rw-r--r--   0 runner    (1001) docker     (127)    34845 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/config/test_configcommands.py
--rw-r--r--   0 runner    (1001) docker     (127)    10356 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/config/test_configdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/config/test_configexc.py
--rw-r--r--   0 runner    (1001) docker     (127)    56473 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/config/test_configfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    16567 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/config/test_configinit.py
--rw-r--r--   0 runner    (1001) docker     (127)    73447 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/config/test_configtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/config/test_configutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24245 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/config/test_qtargs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13708 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/config/test_qtargs_locale_workaround.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/config/test_stylesheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/config/test_websettings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.635451 qutebrowser-3.1.0/tests/unit/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/extensions/test_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.635451 qutebrowser-3.1.0/tests/unit/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.635451 qutebrowser-3.1.0/tests/unit/javascript/position_caret/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/position_caret/invisible.html
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/position_caret/scrolled_down.html
--rw-r--r--   0 runner    (1001) docker     (127)      888 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/position_caret/scrolled_down_img.html
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/position_caret/simple.html
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/position_caret/test_position_caret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.639451 qutebrowser-3.1.0/tests/unit/javascript/stylesheet/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/stylesheet/green.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/stylesheet/none.css
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/stylesheet/simple.html
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/stylesheet/simple.xml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/stylesheet/simple_bg_set_red.html
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/stylesheet/test_appendchild.js
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/stylesheet/test_stylesheet_js.py
--rw-r--r--   0 runner    (1001) docker     (127)    18856 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/test_greasemonkey.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/test_js_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/javascript/test_js_quirks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.639451 qutebrowser-3.1.0/tests/unit/keyinput/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/keyinput/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    23998 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/keyinput/key_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14627 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/keyinput/test_basekeyparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/keyinput/test_bindingtrie.py
--rw-r--r--   0 runner    (1001) docker     (127)    26299 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/keyinput/test_keyutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/keyinput/test_modeman.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/keyinput/test_modeparsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.639451 qutebrowser-3.1.0/tests/unit/mainwindow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.639451 qutebrowser-3.1.0/tests/unit/mainwindow/statusbar/
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/mainwindow/statusbar/test_backforward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/mainwindow/statusbar/test_percentage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/mainwindow/statusbar/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/mainwindow/statusbar/test_tabindex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/mainwindow/statusbar/test_textbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/mainwindow/statusbar/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     9015 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/mainwindow/test_messageview.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/mainwindow/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/mainwindow/test_tabbedbrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/mainwindow/test_tabwidget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.643451 qutebrowser-3.1.0/tests/unit/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_autoupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_checkpyver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_cmdhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_crashdialog.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_earlyinit.py
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_elf.py
--rw-r--r--   0 runner    (1001) docker     (127)    17984 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_guiprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    29392 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_ipc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7118 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_keyhints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_lineparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_miscwidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_msgbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    15481 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_pakjoy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_pastebin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11668 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_split_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (127)    16839 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/test_utilcmds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.643451 qutebrowser-3.1.0/tests/unit/misc/userscripts/
--rw-r--r--   0 runner    (1001) docker     (127)    12682 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/misc/userscripts/test_qute_lastpass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.643451 qutebrowser-3.1.0/tests/unit/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.515452 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.643451 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/chrome/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/chrome/bookmarks
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/chrome/config_py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.643451 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/chrome/input/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/chrome/input/Bookmarks
--rw-r--r--   0 runner    (1001) docker     (127)    63488 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/chrome/input/Web Data
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/chrome/quickmarks
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.647451 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/html/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/html/bookmarks
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/html/config_py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/html/input
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/html/quickmarks
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.647451 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/mozilla/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/mozilla/bookmarks
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/mozilla/config_py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.647451 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/mozilla/input/
--rw-r--r--   0 runner    (1001) docker     (127)  5242880 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/mozilla/input/places.sqlite
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/importer_sample/mozilla/quickmarks
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/test_dictcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/test_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/scripts/test_problemmatchers.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    15897 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/test_qt_machinery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/test_qutebrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.655451 qutebrowser-3.1.0/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/overflow_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/test_javascript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/test_jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)    12825 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/test_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/test_qtlog.py
--rw-r--r--   0 runner    (1001) docker     (127)    40750 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/test_qtutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    17424 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/test_standarddir.py
--rw-r--r--   0 runner    (1001) docker     (127)    24710 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/test_urlmatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    30313 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/test_urlutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    36379 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51792 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:32:17.655451 qutebrowser-3.1.0/tests/unit/utils/usertypes/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/usertypes/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/usertypes/test_neighborlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/usertypes/test_question.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2023-12-08 15:31:12.000000 qutebrowser-3.1.0/tests/unit/utils/usertypes/test_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.145003 qutebrowser-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15731 2024-06-03 14:43:35.145003 qutebrowser-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/README.asciidoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.009001 qutebrowser-3.2.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)   235336 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/doc/changelog.asciidoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.009001 qutebrowser-3.2.0/doc/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   708315 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/doc/img/cheatsheet-big.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/doc/img/cheatsheet-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36391 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/doc/img/completion.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34786 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/doc/img/downloads.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46347 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/doc/img/hints.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34604 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/doc/img/main.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.009001 qutebrowser-3.2.0/doc/img/sponsors/
+-rw-r--r--   0 runner    (1001) docker     (127)    11046 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/doc/img/sponsors/hsr.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33193 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/doc/img/sponsors/macstadium.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-06-03 14:43:31.000000 qutebrowser-3.2.0/doc/qutebrowser.1
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/doc/qutebrowser.1.asciidoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.009001 qutebrowser-3.2.0/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.009001 qutebrowser-3.2.0/misc/apparmor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/apparmor/usr.bin.qutebrowser
+-rw-r--r--   0 runner    (1001) docker     (127)   179325 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/cheatsheet.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/org.qutebrowser.qutebrowser.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/org.qutebrowser.qutebrowser.desktop
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.017001 qutebrowser-3.2.0/misc/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-check-manifest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-check-manifest.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-dev.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-docs.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-flake8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-flake8.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-mypy.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyinstaller.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyinstaller.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pylint.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pylint.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-5.15.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-5.15.2.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-5.15.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-5.15.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-5.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-6.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-6.2.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-6.3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-6.3.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-6.4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-6.4.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-6.5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-6.5.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-6.6.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-6.6.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-6.7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-6.7.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-6.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt-6.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyqt.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyroma.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-pyroma.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-qutebrowser.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-sphinx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-sphinx.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-tests-bleeding.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-tests.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-tox.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-tox.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-vulture.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-vulture.txt-raw
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-yamllint.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/requirements/requirements-yamllint.txt-raw
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.021001 qutebrowser-3.2.0/misc/userscripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5025 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/add-nextcloud-bookmarks
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3912 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/add-nextcloud-cookbook
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5821 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/cast
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1405 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/dmenu_qutebrowser
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1579 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/format_json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2162 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/getbib
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4270 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/kodi
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3747 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/open_download
+-rwxr-xr-x   0 runner    (1001) docker     (127)      899 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/openfeeds
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13375 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/password_fill
+-rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/qr
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4806 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/qute-1pass
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10480 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/qute-bitwarden
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8673 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/qute-keepass
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14941 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/qute-keepassxc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6714 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/qute-lastpass
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12079 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/qute-pass
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1755 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/qutedmenu
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1946 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/readability
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5442 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/readability-js
+-rwxr-xr-x   0 runner    (1001) docker     (127)      938 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/ripbang
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3031 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/rss
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1359 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/taskadd
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1560 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/tor_identity
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5092 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/misc/userscripts/view_in_mpv
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.025002 qutebrowser-3.2.0/qutebrowser/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.025002 qutebrowser-3.2.0/qutebrowser/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/api/apitypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/api/cmdutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/api/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/api/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/api/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/api/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/api/qtutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20654 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.029002 qutebrowser-3.2.0/qutebrowser/browser/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48397 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/browsertab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75704 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49166 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/downloadview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/eventfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18626 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/greasemonkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43912 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/hints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17758 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7761 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/navigate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.029002 qutebrowser-3.2.0/qutebrowser/browser/network/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/network/pac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/network/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/pdfjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22730 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/qtnetworkdownloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19771 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/qutescheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19909 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/signalfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/urlmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16760 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webelem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.033002 qutebrowser-3.2.0/qutebrowser/browser/webengine/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webengine/certificateerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webengine/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15224 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webengine/darkmode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9470 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webengine/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45018 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webengine/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webengine/spell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webengine/tabhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webengine/webenginedownloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webengine/webengineelem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webengine/webengineinspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webengine/webenginequtescheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23004 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webengine/webenginesettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63929 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webengine/webenginetab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14060 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webengine/webview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.033002 qutebrowser-3.2.0/qutebrowser/browser/webkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/certificateerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/httpheaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20002 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/mhtml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.033002 qutebrowser-3.2.0/qutebrowser/browser/webkit/network/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/network/filescheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17225 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/network/networkmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/network/networkreply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/network/webkitqutescheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/tabhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/webkitelem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/webkithistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/webkitinspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/webkitsettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39859 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/webkittab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22582 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/webpage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/browser/webkit/webview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.037002 qutebrowser-3.2.0/qutebrowser/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/commands/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/commands/cmdexc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22413 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/commands/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/commands/runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/commands/userscripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.037002 qutebrowser-3.2.0/qutebrowser/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/completion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12564 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/completion/completer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/completion/completiondelegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17480 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/completion/completionwidget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.037002 qutebrowser-3.2.0/qutebrowser/completion/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/completion/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/completion/models/completionmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/completion/models/configmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/completion/models/filepathcategory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/completion/models/histcategory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/completion/models/listcategory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/completion/models/miscmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/completion/models/urlmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/completion/models/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.037002 qutebrowser-3.2.0/qutebrowser/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/components/adblockcommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12360 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/components/braveadblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/components/caretcommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9902 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/components/hostblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13770 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/components/misccommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/components/readlinecommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/components/scrollcommands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.041002 qutebrowser-3.2.0/qutebrowser/components/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/components/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/components/utils/blockutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/components/zoomcommands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.041002 qutebrowser-3.2.0/qutebrowser/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24283 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/config/configcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19542 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/config/configcommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/config/configdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113898 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/config/configdata.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/config/configexc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39763 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/config/configfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/config/configinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64724 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/config/configtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/config/configutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15191 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/config/qtargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/config/stylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9257 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/config/websettings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.041002 qutebrowser-3.2.0/qutebrowser/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/extensions/interceptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/extensions/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 14:43:34.000000 qutebrowser-3.2.0/qutebrowser/git-commit-id
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.045002 qutebrowser-3.2.0/qutebrowser/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/back.html
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/bindings.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/bookmarks.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/dirbrowser.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.049002 qutebrowser-3.2.0/qutebrowser/html/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)   363289 2024-06-03 14:43:23.000000 qutebrowser-3.2.0/qutebrowser/html/doc/changelog.html
+-rw-r--r--   0 runner    (1001) docker     (127)   177952 2024-06-03 14:43:28.000000 qutebrowser-3.2.0/qutebrowser/html/doc/commands.html
+-rw-r--r--   0 runner    (1001) docker     (127)    53744 2024-06-03 14:43:27.000000 qutebrowser-3.2.0/qutebrowser/html/doc/configuring.html
+-rw-r--r--   0 runner    (1001) docker     (127)    75683 2024-06-03 14:43:24.000000 qutebrowser-3.2.0/qutebrowser/html/doc/contributing.html
+-rw-r--r--   0 runner    (1001) docker     (127)    57671 2024-06-03 14:43:21.000000 qutebrowser-3.2.0/qutebrowser/html/doc/faq.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.049002 qutebrowser-3.2.0/qutebrowser/html/doc/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   708315 2024-06-03 14:43:31.000000 qutebrowser-3.2.0/qutebrowser/html/doc/img/cheatsheet-big.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-06-03 14:43:31.000000 qutebrowser-3.2.0/qutebrowser/html/doc/img/cheatsheet-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25157 2024-06-03 14:43:25.000000 qutebrowser-3.2.0/qutebrowser/html/doc/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    46379 2024-06-03 14:43:25.000000 qutebrowser-3.2.0/qutebrowser/html/doc/install.html
+-rw-r--r--   0 runner    (1001) docker     (127)    26683 2024-06-03 14:43:24.000000 qutebrowser-3.2.0/qutebrowser/html/doc/quickstart.html
+-rw-r--r--   0 runner    (1001) docker     (127)   340541 2024-06-03 14:43:31.000000 qutebrowser-3.2.0/qutebrowser/html/doc/settings.html
+-rw-r--r--   0 runner    (1001) docker     (127)    29686 2024-06-03 14:43:25.000000 qutebrowser-3.2.0/qutebrowser/html/doc/stacktrace.html
+-rw-r--r--   0 runner    (1001) docker     (127)    27176 2024-06-03 14:43:25.000000 qutebrowser-3.2.0/qutebrowser/html/doc/userscripts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/history.html
+-rw-r--r--   0 runner    (1001) docker     (127)    37521 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/license.html
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/log.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/no_pdfjs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/pre.html
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/process.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/settings.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/startpage.html
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/styled.html
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/tabs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/version.html
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/warning-qt5.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/warning-sessions.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/html/warning-webkit.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.053002 qutebrowser-3.2.0/qutebrowser/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-24x24.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13690 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-256x256.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30109 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (127)   131549 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15990 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   196205 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/icons/qutebrowser.icns
+-rw-r--r--   0 runner    (1001) docker     (127)   115490 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/icons/qutebrowser.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    16018 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/icons/qutebrowser.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/icons/qutebrowser.xpm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.053002 qutebrowser-3.2.0/qutebrowser/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    58370 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/img/broken_qutebrowser_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23799 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/img/file.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    22869 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/img/folder.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.053002 qutebrowser-3.2.0/qutebrowser/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)    50851 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/javascript/caret.js
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/javascript/global_wrapper.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/javascript/greasemonkey_wrapper.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/javascript/history.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/javascript/pac_utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/javascript/position_caret.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.053002 qutebrowser-3.2.0/qutebrowser/javascript/quirks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/javascript/quirks/array_at.user.js
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/javascript/quirks/discord.user.js
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/javascript/quirks/googledocs.user.js
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/javascript/quirks/string_replaceall.user.js
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/javascript/quirks/whatsapp_web.user.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/javascript/scroll.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/javascript/stylesheet.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/javascript/webelem.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.057002 qutebrowser-3.2.0/qutebrowser/keyinput/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/keyinput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/keyinput/basekeyparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/keyinput/eventfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26045 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/keyinput/keyutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/keyinput/macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17408 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/keyinput/modeman.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/keyinput/modeparsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.057002 qutebrowser-3.2.0/qutebrowser/mainwindow/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28104 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/messageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37168 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.057002 qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/backforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/keystring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/percentage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/searchmatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/tabindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/textbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43950 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/tabbedbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38101 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/tabwidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/mainwindow/windowundo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.061002 qutebrowser-3.2.0/qutebrowser/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/autoupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17398 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/backendproblem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/binparsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/checkpyver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/cmdhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/consolewidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25317 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/crashdialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17230 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/crashsignal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/debugcachestats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12053 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/earlyinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15687 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/guiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19992 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/keyhintwidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/lineparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15522 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/miscwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/msgbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/nativeeventfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/pakjoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10888 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/quitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/savemanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24623 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20676 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/misc/utilcmds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.065002 qutebrowser-3.2.0/qutebrowser/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/_core_pyqtproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/dbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/machinery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/opengl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/printsupport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/qml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/sip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/webenginecore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/webenginewidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/webkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/webkitwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qt/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10191 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/qutebrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.069002 qutebrowser-3.2.0/qutebrowser/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/docutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20983 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11821 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/objreg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/qtlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22833 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/qtutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/standarddir.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/testfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/urlmatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/urlutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/usertypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26741 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40595 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.145003 qutebrowser-3.2.0/qutebrowser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15731 2024-06-03 14:43:34.000000 qutebrowser-3.2.0/qutebrowser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32242 2024-06-03 14:43:34.000000 qutebrowser-3.2.0/qutebrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:43:34.000000 qutebrowser-3.2.0/qutebrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-03 14:43:34.000000 qutebrowser-3.2.0/qutebrowser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-06-03 14:43:34.000000 qutebrowser-3.2.0/qutebrowser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 14:43:34.000000 qutebrowser-3.2.0/qutebrowser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:43:32.000000 qutebrowser-3.2.0/qutebrowser.egg-info/zip-safe
+-rwxr-xr-x   0 runner    (1001) docker     (127)      307 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/qutebrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.069002 qutebrowser-3.2.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/scripts/cycle-inputs.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8150 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/scripts/dictcli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5440 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/scripts/hist_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/scripts/hostblock_blame.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11264 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/scripts/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/scripts/keytester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/scripts/link_pyqt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19825 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/scripts/mkvenv.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/scripts/open_url_in_instance.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/scripts/opengl_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/scripts/setupcommon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.069002 qutebrowser-3.2.0/scripts/testbrowser/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1226 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/scripts/testbrowser/testbrowser_webengine.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1176 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/scripts/testbrowser/testbrowser_webkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:43:35.145003 qutebrowser-3.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3309 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.069002 qutebrowser-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.073002 qutebrowser-3.2.0/tests/end2end/
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.077002 qutebrowser-3.2.0/tests/end2end/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.077002 qutebrowser-3.2.0/tests/end2end/data/backforward/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/backforward/1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/backforward/2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/backforward/3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   257960 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/blocked-hosts.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.077002 qutebrowser-3.2.0/tests/end2end/data/blocking/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/blocking/external_logo.html
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/blocking/qutebrowser-adblock
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/blocking/qutebrowser-hosts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.077002 qutebrowser-3.2.0/tests/end2end/data/brave-adblock/
+-rw-r--r--   0 runner    (1001) docker     (127)    15313 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/brave-adblock/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/brave-adblock/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/brave-adblock/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1279186 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/brave-adblock/ublock-matches.tsv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/caret.html
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/click_element.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.081002 qutebrowser-3.2.0/tests/end2end/data/crashers/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/crashers/installedapp.html
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/crashers/webrtc.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.081002 qutebrowser-3.2.0/tests/end2end/data/darkmode/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/darkmode/blank.html
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/darkmode/mathml-display.html
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/darkmode/mathml-inline.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/darkmode/mathml.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/darkmode/prefers-color-scheme.html
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/darkmode/yellow.html
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/data_link.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.081002 qutebrowser-3.2.0/tests/end2end/data/downloads/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/download with no title.html
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/download with spaces.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/download.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/download2.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/downloads.html
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/issue1243.html
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/issue1535.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/issue1725.html
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/issue2134.html
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/issue2298.html
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/issue889.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.001001 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.085002 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/Background.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17035 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/Banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/DYK.png
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/Inline.png
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/complex.html
+-rw-r--r--   0 runner    (1001) docker     (127)    54939 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/complex.mht
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/external-in-extern.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/not-css.qss
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/requests
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/script.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.085002 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/simple/requests
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/simple/simple.html
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/simple/simple.mht
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/qutebrowser.png
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/downloads/ä-issue908.bin
+-rw-r--r--   0 runner    (1001) docker     (127)   593611 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/easylist.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   144367 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/easyprivacy.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/editor.html
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/email_address.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/fileselect.html
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hello.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hello2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hello3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hinting.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.089002 qutebrowser-3.2.0/tests/end2end/data/hints/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.089002 qutebrowser-3.2.0/tests/end2end/data/hints/ace/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/ace/ace.html
+-rw-r--r--   0 runner    (1001) docker     (127)   661179 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/ace/ace.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.089002 qutebrowser-3.2.0/tests/end2end/data/hints/angular1/
+-rw-r--r--   0 runner    (1001) docker     (127)   167131 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/angular1/angular.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13147 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/benchmark.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.089002 qutebrowser-3.2.0/tests/end2end/data/hints/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)   198313 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/bootstrap/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/bootstrap/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/buttons.html
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/custom_group.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.093002 qutebrowser-3.2.0/tests/end2end/data/hints/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/html/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/html/angular1.html
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/html/click_handler.html
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/html/invisible.html
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/html/javascript.html
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/html/nested_block_style.html
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/html/nested_formatting_tags.html
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/html/nested_table_style.html
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/html/simple.html
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/html/tabindex-negative.html
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/html/target_blank_js.html
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/html/with_spaces.html
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/html/wrapped.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/html/wrapped_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/html/zoom_precision.html
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/iframe.html
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/iframe_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/iframe_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/iframe_scroll.html
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/iframe_target.html
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/input.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/issue1186.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/issue1393.html
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/issue3711.html
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/issue3711_frame.html
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/link_blank.html
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/link_inject.html
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/link_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/link_span.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/number.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/rapid.html
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/hints/short_dict.html
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/iframe_search.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.001001 qutebrowser-3.2.0/tests/end2end/data/insert_mode_settings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.093002 qutebrowser-3.2.0/tests/end2end/data/insert_mode_settings/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/insert_mode_settings/html/autofocus.html
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/insert_mode_settings/html/input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/insert_mode_settings/html/textarea.html
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/invalid_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/invalid_resource.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/issue2569.html
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/issue4011.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.093002 qutebrowser-3.2.0/tests/end2end/data/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/javascript/consolelog.html
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/javascript/enabled.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.093002 qutebrowser-3.2.0/tests/end2end/data/javascript/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/javascript/img/big.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/javascript/img/padded.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/javascript/img/padded2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/javascript/img/rgb.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/javascript/img/rgba.png
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/javascript/localstorage.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/javascript/notifications.html
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/javascript/window_open.html
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/javascript/windowsize.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.093002 qutebrowser-3.2.0/tests/end2end/data/keyinput/
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/keyinput/log.html
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/l33t.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/long_load.html
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/marks.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.093002 qutebrowser-3.2.0/tests/end2end/data/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/misc/hello.txt.html
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/misc/jseval.html
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/misc/jseval_file.js
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/misc/pyeval_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/misc/qutescheme_csrf.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16667 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/misc/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/misc/xhr_headers.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.097003 qutebrowser-3.2.0/tests/end2end/data/navigate/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/navigate/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/navigate/multilinelinks.html
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/navigate/next.html
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/navigate/prev.html
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/navigate/rel.html
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/navigate/rel_nofollow.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.097003 qutebrowser-3.2.0/tests/end2end/data/navigate/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/navigate/sub/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.097003 qutebrowser-3.2.0/tests/end2end/data/numbers/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/13.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/14.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/15.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/16.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/17.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/18.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/19.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/6.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/numbers/9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/paste_primary.html
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/prefers_reduced_motion.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.101003 qutebrowser-3.2.0/tests/end2end/data/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/prompt/geolocation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/prompt/jsalert.html
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/prompt/jsconfirm.html
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/prompt/jsprompt.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/prompt/notifications.html
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/prompt/script.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/reload.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.101003 qutebrowser-3.2.0/tests/end2end/data/scroll/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/scroll/no_doctype.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/scroll/position_absolute.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/scroll/simple.html
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/search_select.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.101003 qutebrowser-3.2.0/tests/end2end/data/service-worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/service-worker/data.json
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/service-worker/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/service-worker/worker.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.101003 qutebrowser-3.2.0/tests/end2end/data/sessions/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/sessions/history_replace_state.html
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/sessions/snowman.html
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/smart.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.101003 qutebrowser-3.2.0/tests/end2end/data/ssl/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/ssl/cert.csr
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/ssl/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/ssl/key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/ssl/privkey.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/title with spaces.html
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/title.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.101003 qutebrowser-3.2.0/tests/end2end/data/userscripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/userscripts/echo.bat
+-rwxr-xr-x   0 runner    (1001) docker     (127)       71 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/userscripts/echo_hint_text
+-rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/userscripts/hello_if_count
+-rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/userscripts/open_current_url
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/userscripts/open_current_url.bat
+-rwxr-xr-x   0 runner    (1001) docker     (127)      343 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/userscripts/stdinclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/data/äöü.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.109003 qutebrowser-3.2.0/tests/end2end/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/backforward.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/caret.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/completion.feature
+-rw-r--r--   0 runner    (1001) docker     (127)    25751 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34730 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/downloads.feature
+-rw-r--r--   0 runner    (1001) docker     (127)    12295 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/editor.feature
+-rw-r--r--   0 runner    (1001) docker     (127)    28266 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/hints.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/history.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/invoke.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/javascript.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/keyinput.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/marks.feature
+-rw-r--r--   0 runner    (1001) docker     (127)    25155 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/misc.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/navigate.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/notifications.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/open.feature
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/private.feature
+-rw-r--r--   0 runner    (1001) docker     (127)    22476 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/prompts.feature
+-rw-r--r--   0 runner    (1001) docker     (127)    12980 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/qutescheme.feature
+-rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/scroll.feature
+-rw-r--r--   0 runner    (1001) docker     (127)    16142 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/search.feature
+-rw-r--r--   0 runner    (1001) docker     (127)    15515 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/sessions.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/spawn.feature
+-rw-r--r--   0 runner    (1001) docker     (127)    66742 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/tabs.feature
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_backforward_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_caret_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_completion_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_downloads_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_editor_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_hints_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_history_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_invoke_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_javascript_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_keyinput_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_marks_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_misc_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_navigate_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_notifications_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_open_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_private_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_prompts_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_qutescheme_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_scroll_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_search_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_sessions_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_spawn_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_tabs_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_urlmarks_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_utilcmds_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_yankpaste_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/test_zoom_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/urlmarks.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/utilcmds.feature
+-rw-r--r--   0 runner    (1001) docker     (127)    14772 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/yankpaste.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/features/zoom.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.113003 qutebrowser-3.2.0/tests/end2end/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/fixtures/notificationserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39022 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/fixtures/quteprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/fixtures/test_quteprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/fixtures/test_testprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/fixtures/test_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17025 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/fixtures/testprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/fixtures/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/fixtures/webserver_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/fixtures/webserver_sub_ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.113003 qutebrowser-3.2.0/tests/end2end/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/misc/test_runners_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.113003 qutebrowser-3.2.0/tests/end2end/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/templates/headers-link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/templates/https-iframe.html
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/templates/https-script.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/test_adblock_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/test_dirbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/test_hints_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/test_insert_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35808 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/test_invocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/end2end/test_mhtml_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.113003 qutebrowser-3.2.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)    22370 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/helpers/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/helpers/logfail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/helpers/messagemock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19749 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/helpers/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/helpers/test_helper_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/helpers/test_logfail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/helpers/test_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/helpers/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.113003 qutebrowser-3.2.0/tests/manual/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.113003 qutebrowser-3.2.0/tests/manual/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/manual/completion/changing_title.html
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/manual/files.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.113003 qutebrowser-3.2.0/tests/manual/hints/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/manual/hints/find_implementation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/manual/hints/hide_unmatched_rapid_hints.html
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/manual/hints/issue824.html
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/manual/hints/issue925.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/manual/hints/other.html
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/manual/hints/zoom.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.113003 qutebrowser-3.2.0/tests/manual/history/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/manual/history/visited.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.113003 qutebrowser-3.2.0/tests/manual/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/manual/js/jsalert_multiline.html
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/manual/js/jsconfirm.html
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/manual/js/jsprompt.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/manual/mouse.html
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/test_conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.117003 qutebrowser-3.2.0/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.117003 qutebrowser-3.2.0/tests/unit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    17408 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/api/test_cmdutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.117003 qutebrowser-3.2.0/tests/unit/browser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/test_browsertab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16289 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/test_caret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/test_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/test_downloadview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/test_hints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22503 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/test_navigate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/test_pdfjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/test_qutescheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/test_signalfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/test_urlmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.117003 qutebrowser-3.2.0/tests/unit/browser/webengine/
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webengine/test_darkmode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webengine/test_spell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webengine/test_webengine_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webengine/test_webenginedownloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webengine/test_webengineinterceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webengine/test_webenginesettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webengine/test_webenginetab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webengine/test_webview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.121003 qutebrowser-3.2.0/tests/unit/browser/webkit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.121003 qutebrowser-3.2.0/tests/unit/browser/webkit/http/
+-rw-r--r--   0 runner    (1001) docker     (127)    35650 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webkit/http/test_content_disposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webkit/http/test_httpheaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.121003 qutebrowser-3.2.0/tests/unit/browser/webkit/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webkit/network/test_filescheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webkit/network/test_networkmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webkit/network/test_networkreply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webkit/network/test_pac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webkit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webkit/test_certificateerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webkit/test_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webkit/test_mhtml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webkit/test_tabhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webkit/test_webkit_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34619 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webkit/test_webkitelem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/browser/webkit/test_webkitsettings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.121003 qutebrowser-3.2.0/tests/unit/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/commands/test_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/commands/test_cmdexc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/commands/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/commands/test_userscripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.121003 qutebrowser-3.2.0/tests/unit/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)    14404 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/completion/test_completer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/completion/test_completiondelegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/completion/test_completionmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/completion/test_completionwidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/completion/test_histcategory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/completion/test_listcategory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51791 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/completion/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.125003 qutebrowser-3.2.0/tests/unit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/components/test_blockutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15792 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/components/test_braveadblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/components/test_hostblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/components/test_misccommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12684 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/components/test_readlinecommands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.125003 qutebrowser-3.2.0/tests/unit/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    31855 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/config/test_configcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34904 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/config/test_configcommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/config/test_configdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/config/test_configexc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56506 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/config/test_configfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16567 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/config/test_configinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73568 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/config/test_configtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/config/test_configutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24245 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/config/test_qtargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/config/test_qtargs_locale_workaround.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/config/test_stylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/config/test_websettings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.125003 qutebrowser-3.2.0/tests/unit/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/extensions/test_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.125003 qutebrowser-3.2.0/tests/unit/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.129003 qutebrowser-3.2.0/tests/unit/javascript/position_caret/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/position_caret/invisible.html
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/position_caret/scrolled_down.html
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/position_caret/scrolled_down_img.html
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/position_caret/simple.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/position_caret/test_position_caret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.129003 qutebrowser-3.2.0/tests/unit/javascript/stylesheet/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/stylesheet/green.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/stylesheet/none.css
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/stylesheet/simple.html
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/stylesheet/simple.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/stylesheet/simple_bg_set_red.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/stylesheet/test_appendchild.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/stylesheet/test_stylesheet_js.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18856 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/test_greasemonkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/test_js_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/javascript/test_js_quirks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.129003 qutebrowser-3.2.0/tests/unit/keyinput/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/keyinput/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23998 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/keyinput/key_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/keyinput/test_basekeyparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/keyinput/test_bindingtrie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26299 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/keyinput/test_keyutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/keyinput/test_modeman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/keyinput/test_modeparsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.129003 qutebrowser-3.2.0/tests/unit/mainwindow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.129003 qutebrowser-3.2.0/tests/unit/mainwindow/statusbar/
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/mainwindow/statusbar/test_backforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/mainwindow/statusbar/test_percentage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/mainwindow/statusbar/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/mainwindow/statusbar/test_tabindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/mainwindow/statusbar/test_textbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/mainwindow/statusbar/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/mainwindow/test_messageview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/mainwindow/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/mainwindow/test_tabbedbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/mainwindow/test_tabwidget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.133003 qutebrowser-3.2.0/tests/unit/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_autoupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_checkpyver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_cmdhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_crashdialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_crashsignal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_earlyinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18051 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_guiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29392 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_ipc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_keyhints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_lineparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_miscwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_msgbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_pakjoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_split_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16839 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/test_utilcmds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.133003 qutebrowser-3.2.0/tests/unit/misc/userscripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    12682 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/misc/userscripts/test_qute_lastpass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.133003 qutebrowser-3.2.0/tests/unit/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.005001 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.137003 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/chrome/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/chrome/bookmarks
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/chrome/config_py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.137003 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/chrome/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/chrome/input/Bookmarks
+-rw-r--r--   0 runner    (1001) docker     (127)    63488 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/chrome/input/Web Data
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/chrome/quickmarks
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.137003 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/html/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/html/bookmarks
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/html/config_py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/html/input
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/html/quickmarks
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.137003 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/mozilla/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/mozilla/bookmarks
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/mozilla/config_py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.137003 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/mozilla/input/
+-rw-r--r--   0 runner    (1001) docker     (127)  5242880 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/mozilla/input/places.sqlite
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/importer_sample/mozilla/quickmarks
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/test_dictcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/test_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/scripts/test_problemmatchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15963 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/test_qt_machinery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/test_qutebrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.145003 qutebrowser-3.2.0/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/overflow_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/test_javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/test_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/test_qtlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41708 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/test_qtutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17424 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/test_standarddir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24710 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/test_urlmatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30313 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/test_urlutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36379 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54449 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:43:35.145003 qutebrowser-3.2.0/tests/unit/utils/usertypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/usertypes/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/usertypes/test_neighborlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/usertypes/test_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-06-03 14:42:42.000000 qutebrowser-3.2.0/tests/unit/utils/usertypes/test_timer.py
```

### Comparing `qutebrowser-3.1.0/LICENSE` & `qutebrowser-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/MANIFEST.in` & `qutebrowser-3.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/PKG-INFO` & `qutebrowser-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qutebrowser
-Version: 3.1.0
+Version: 3.2.0
 Summary: A keyboard-driven, vim-like browser based on Python and Qt.
 Home-page: https://www.qutebrowser.org/
 Author: Florian Bruhin
 Author-email: mail@qutebrowser.org
 License: GPL
 Keywords: pyqt browser web qt webkit qtwebkit qtwebengine
 Classifier: Development Status :: 5 - Production/Stable
@@ -169,15 +169,15 @@
 https://github.com/sponsors/The-Compiler/[GitHub Sponsors page] for more
 information. Depending on your sign-up date and how long you keep a certain
 level, you can get qutebrowser t-shirts, stickers and more!
 
 GitHub Sponsors allows for one-time donations (using the buttons next to "Select a
 tier") as well as custom amounts. **For currencies other than Euro or Swiss Francs, this
 is the preferred donation method.** GitHub uses https://stripe.com/[Stripe] to accept
-payment via credit carts without any fees. Billing via PayPal is available as well, with
+payment via credit cards without any fees. Billing via PayPal is available as well, with
 less fees than a direct PayPal transaction.
 
 Alternatively, the following donation methods are available -- note that
 eligibility for swag (shirts/stickers/etc.) is handled on a case-by-case basis
 for those, please mailto:mail@qutebrowser.org[get in touch] for details.
 
 * https://liberapay.com/The-Compiler[Liberapay], which can handle payments
```

### Comparing `qutebrowser-3.1.0/README.asciidoc` & `qutebrowser-3.2.0/README.asciidoc`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 https://github.com/sponsors/The-Compiler/[GitHub Sponsors page] for more
 information. Depending on your sign-up date and how long you keep a certain
 level, you can get qutebrowser t-shirts, stickers and more!
 
 GitHub Sponsors allows for one-time donations (using the buttons next to "Select a
 tier") as well as custom amounts. **For currencies other than Euro or Swiss Francs, this
 is the preferred donation method.** GitHub uses https://stripe.com/[Stripe] to accept
-payment via credit carts without any fees. Billing via PayPal is available as well, with
+payment via credit cards without any fees. Billing via PayPal is available as well, with
 less fees than a direct PayPal transaction.
 
 Alternatively, the following donation methods are available -- note that
 eligibility for swag (shirts/stickers/etc.) is handled on a case-by-case basis
 for those, please mailto:mail@qutebrowser.org[get in touch] for details.
 
 * https://liberapay.com/The-Compiler[Liberapay], which can handle payments
```

### Comparing `qutebrowser-3.1.0/doc/changelog.asciidoc` & `qutebrowser-3.2.0/doc/changelog.asciidoc`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,68 @@
 // `Added` for new features.
 // `Changed` for changes in existing functionality.
 // `Deprecated` for once-stable features removed in upcoming releases.
 // `Removed` for deprecated features removed in this release.
 // `Fixed` for any bug fixes.
 // `Security` to invite users to upgrade in case of vulnerabilities.
 
+[[v3.2.0]]
+v3.2.0 (2024-06-03)
+-------------------
+
+Deprecated
+~~~~~~~~~~
+
+- This will be the last feature release supporting macOS 11 Big Sur.
+  Starting with qutebrowser v3.3.0, macOS 12 Monterey will be the oldest
+  supported version.
+
+Added
+~~~~~
+
+- When qutebrowser receives a SIGHUP it will now reload any config.py file
+  in use (same as the `:config-source` command does). (#8108)
+- The Chromium security patch version is now shown in the backend string in
+  `--version` and `:version`. This reflects the latest Chromium version that
+  security fixes have been backported to the base QtWebEngine version from.
+  (#7187)
+
+Changed
+~~~~~~~
+
+- Windows and macOS releases now ship with Qt 6.7.1, which is based on Chromium
+  118.0.5993.220 with security patches up to 124.0.6367.202.
+- With QtWebEngine 6.7+, the `colors.webpage.darkmode.enabled` setting can now
+  be changed at runtime and supports URL patterns (#8182).
+- A few more completions will now match search terms in any order:
+  `:quickmark-*`, `:bookmark-*`, `:tab-take` and `:tab-select` (for the quick
+  and bookmark categories). (#7955)
+- Elements with an ARIA `role="switch"` now get hints (toggle switches like
+  e.g. on cookie banners).
+- The `tor_identity` userscript now validates that the -c|--control-port
+  argument value is an int. (#8162)
+
+Fixed
+~~~~~
+
+- `input.insert_mode.auto_load` sometimes not triggering due to a race
+  condition. (#8145)
+- Worked around qutebrowser quitting when closing a KDE file dialog due to a Qt
+  bug. (#8143)
+- Trying to use qutebrowser after it's been deleted/moved on disk (e.g. after a
+  Python upgrade) should now not crash anymore.
+- When the QtWebEngine resources dir couldn't be found, qutebrowser now doesn't
+  crash anymore (but QtWebEngine still might).
+- Fixed a rare crash in the completion widget when there was no selection model
+  when we went to clear that, probably when leaving a mode. (#7901)
+- Worked around a minor issue around QTimers on Windows where the IPC server
+  could close the socket early. (#8191)
+- The latest PDF.js release (v4.2.67) is now supported when backed by
+  QtWebEngine 6.6+ (#8170)
+
 [[v3.1.0]]
 v3.1.0 (2023-12-08)
 -------------------
 
 Removed
 ~~~~~~~
 
@@ -3627,15 +3681,15 @@
 - When the key config isn't writable, we now show an error instead of crashing.
 - Fixed crash when unbinding an unbound key in the key config.
 - Fixed crash when using `:debug-log-filter` when `--filter` wasn't given on startup.
 - Fixed crash with some invalid setting values.
 - Continuing a search after clearing it now works correctly.
 - The tabbar and completion should now be more consistently and correctly
   styled with various system styles.
-- Applying styiles in `qt5ct` now shouldn't crash anymore.
+- Applying styles in `qt5ct` now shouldn't crash anymore.
 - The validation for colors in stylesheets is now less strict,
   allowing for all valid Qt values.
 - `data:` URLs now aren't added to the history anymore.
 - Accidentally starting with Python 2 now shows a proper error message again.
 - For some people, running some userscripts crashed - this should now be fixed.
 - Various other rare crashes should now be fixed.
 - The settings documentation was truncated with v0.10.1 which should now be
```

### Comparing `qutebrowser-3.1.0/doc/img/cheatsheet-big.png` & `qutebrowser-3.2.0/doc/img/cheatsheet-big.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/doc/img/cheatsheet-small.png` & `qutebrowser-3.2.0/doc/img/cheatsheet-small.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/doc/img/completion.png` & `qutebrowser-3.2.0/doc/img/completion.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/doc/img/downloads.png` & `qutebrowser-3.2.0/doc/img/downloads.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/doc/img/hints.png` & `qutebrowser-3.2.0/doc/img/hints.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/doc/img/main.png` & `qutebrowser-3.2.0/doc/img/main.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/doc/img/sponsors/hsr.png` & `qutebrowser-3.2.0/doc/img/sponsors/hsr.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/doc/img/sponsors/macstadium.png` & `qutebrowser-3.2.0/doc/img/sponsors/macstadium.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/doc/qutebrowser.1` & `qutebrowser-3.2.0/doc/qutebrowser.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '\" t
 .\"     Title: qutebrowser
 .\"    Author: [see the "AUTHOR" section]
 .\" Generator: DocBook XSL Stylesheets v1.79.1 <http://docbook.sf.net/>
-.\"      Date: 12/08/2023
+.\"      Date: 06/03/2024
 .\"    Manual: qutebrowser manpage
 .\"    Source: qutebrowser
 .\"  Language: English
 .\"
-.TH "QUTEBROWSER" "1" "12/08/2023" "qutebrowser" "qutebrowser manpage"
+.TH "QUTEBROWSER" "1" "06/03/2024" "qutebrowser" "qutebrowser manpage"
 .\" -----------------------------------------------------------------
 .\" * Define some portability stuff
 .\" -----------------------------------------------------------------
 .\" ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 .\" http://bugs.debian.org/507673
 .\" http://lists.gnu.org/archive/html/groff/2009-02/msg00013.html
 .\" ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `qutebrowser-3.1.0/doc/qutebrowser.1.asciidoc` & `qutebrowser-3.2.0/doc/qutebrowser.1.asciidoc`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/Makefile` & `qutebrowser-3.2.0/misc/Makefile`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/apparmor/usr.bin.qutebrowser` & `qutebrowser-3.2.0/misc/apparmor/usr.bin.qutebrowser`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/cheatsheet.svg` & `qutebrowser-3.2.0/misc/cheatsheet.svg`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/org.qutebrowser.qutebrowser.appdata.xml` & `qutebrowser-3.2.0/misc/org.qutebrowser.qutebrowser.appdata.xml`

 * *Files 1% similar despite different names*

#### Comparing `qutebrowser-3.1.0/misc/org.qutebrowser.qutebrowser.appdata.xml` & `qutebrowser-3.2.0/misc/org.qutebrowser.qutebrowser.appdata.xml`

```diff
@@ -37,14 +37,15 @@
   <url type="faq">https://qutebrowser.org/doc/faq.html</url>
   <url type="help">https://qutebrowser.org/doc/help/</url>
   <url type="bugtracker">https://github.com/qutebrowser/qutebrowser/issues/</url>
   <url type="donation">https://github.com/qutebrowser/qutebrowser#donating</url>
   <content_rating type="oars-1.1"/>
   <releases>
     <!-- Add new releases here -->
+    <release version="3.2.0" date="2024-06-03"/>
     <release version="3.1.0" date="2023-12-08"/>
     <release version="3.0.2" date="2023-10-19"/>
     <release version="3.0.1" date="2023-10-19"/>
     <release version="3.0.0" date="2023-08-18"/>
     <release version="2.5.4" date="2023-03-13"/>
     <release version="2.5.3" date="2023-02-17"/>
     <release version="2.5.2" date="2022-06-22"/>
```

### Comparing `qutebrowser-3.1.0/misc/org.qutebrowser.qutebrowser.desktop` & `qutebrowser-3.2.0/misc/org.qutebrowser.qutebrowser.desktop`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/requirements/README.md` & `qutebrowser-3.2.0/misc/requirements/README.md`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/requirements/requirements-qutebrowser.txt-raw` & `qutebrowser-3.2.0/misc/requirements/requirements-qutebrowser.txt-raw`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # pyobjc-core
 # pyobjc-framework-Cocoa
 #@ add: # Unpinned due to recompile_requirements.py limitations
 #@ add: pyobjc-core ; sys_platform=="darwin"  
 #@ add: pyobjc-framework-Cocoa ; sys_platform=="darwin"
 
 ## stdlib backports
-importlib-resources
+importlib_resources
 
 ## Optional dependencies
 Pygments  # For :view-source --pygments or on QtWebKit
 colorama  # Colored log output on Windows
 adblock  # Improved adblocking
 
-#@ markers: importlib-resources python_version=="3.8.*"
+#@ markers: importlib_resources python_version=="3.8.*"
```

### Comparing `qutebrowser-3.1.0/misc/requirements/requirements-tests-bleeding.txt` & `qutebrowser-3.2.0/misc/requirements/requirements-tests-bleeding.txt`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/requirements/requirements-tests.txt` & `qutebrowser-3.2.0/misc/requirements/requirements-tests.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 # This file is automatically generated by scripts/dev/recompile_requirements.py
 
-attrs==23.1.0
-beautifulsoup4==4.12.2
-blinker==1.7.0
-certifi==2023.11.17
+attrs==23.2.0
+beautifulsoup4==4.12.3
+blinker==1.8.2
+certifi==2024.6.2
 charset-normalizer==3.3.2
-cheroot==10.0.0
+cheroot==10.0.1
 click==8.1.7
-coverage==7.3.2
-exceptiongroup==1.2.0
-execnet==2.0.2
-filelock==3.13.1
-Flask==3.0.0
-hunter==3.6.1
-hypothesis==6.91.0
-idna==3.6
-importlib-metadata==7.0.0
+coverage==7.5.3
+exceptiongroup==1.2.1
+execnet==2.1.1
+filelock==3.14.0
+Flask==3.0.3
+hunter==3.7.0
+hypothesis==6.103.0
+idna==3.7
+importlib_metadata==7.1.0
 iniconfig==2.0.0
-itsdangerous==2.1.2
-jaraco.functools==4.0.0
-# Jinja2==3.1.2
-Mako==1.3.0
+itsdangerous==2.2.0
+jaraco.functools==4.0.1
+# Jinja2==3.1.4
+Mako==1.3.5
 manhole==1.8.0
-# MarkupSafe==2.1.3
-more-itertools==10.1.0
-packaging==23.2
-parse==1.20.0
+# MarkupSafe==2.1.5
+more-itertools==10.2.0
+packaging==24.0
+parse==1.20.1
 parse-type==0.6.2
-pluggy==1.3.0
+pluggy==1.5.0
 py-cpuinfo==9.0.0
-Pygments==2.17.2
-pytest==7.4.3
-pytest-bdd==7.0.1
+Pygments==2.18.0
+pytest==8.2.1
+pytest-bdd==7.1.2
 pytest-benchmark==4.0.0
-pytest-cov==4.1.0
+pytest-cov==5.0.0
 pytest-instafail==0.5.0
-pytest-mock==3.12.0
-pytest-qt==4.2.0
+pytest-mock==3.14.0
+pytest-qt==4.4.0
 pytest-repeat==0.9.3
-pytest-rerunfailures==13.0
-pytest-xdist==3.5.0
+pytest-rerunfailures==14.0
+pytest-xdist==3.6.1
 pytest-xvfb==3.0.0
 PyVirtualDisplay==3.0
-requests==2.31.0
-requests-file==1.5.1
+requests==2.32.3
+requests-file==2.1.0
 six==1.16.0
 sortedcontainers==2.4.0
 soupsieve==2.5
-tldextract==5.1.1
-toml==0.10.2
+tldextract==5.1.2
 tomli==2.0.1
-typing_extensions==4.8.0
-urllib3==2.1.0
-vulture==2.10
-Werkzeug==3.0.1
-zipp==3.17.0
+typing_extensions==4.12.1
+urllib3==2.2.1
+vulture==2.11
+Werkzeug==3.0.3
+zipp==3.19.1
```

### Comparing `qutebrowser-3.1.0/misc/requirements/requirements-tests.txt-raw` & `qutebrowser-3.2.0/misc/requirements/requirements-tests.txt-raw`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/README.md` & `qutebrowser-3.2.0/misc/userscripts/README.md`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/add-nextcloud-bookmarks` & `qutebrowser-3.2.0/misc/userscripts/add-nextcloud-bookmarks`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/add-nextcloud-cookbook` & `qutebrowser-3.2.0/misc/userscripts/add-nextcloud-cookbook`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/cast` & `qutebrowser-3.2.0/misc/userscripts/cast`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/dmenu_qutebrowser` & `qutebrowser-3.2.0/misc/userscripts/dmenu_qutebrowser`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/format_json` & `qutebrowser-3.2.0/misc/userscripts/format_json`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/getbib` & `qutebrowser-3.2.0/misc/userscripts/getbib`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/kodi` & `qutebrowser-3.2.0/misc/userscripts/kodi`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/open_download` & `qutebrowser-3.2.0/misc/userscripts/open_download`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/openfeeds` & `qutebrowser-3.2.0/misc/userscripts/openfeeds`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/password_fill` & `qutebrowser-3.2.0/misc/userscripts/password_fill`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/qute-1pass` & `qutebrowser-3.2.0/misc/userscripts/qute-1pass`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/qute-bitwarden` & `qutebrowser-3.2.0/misc/userscripts/qute-bitwarden`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/qute-keepass` & `qutebrowser-3.2.0/misc/userscripts/qute-keepass`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/qute-keepassxc` & `qutebrowser-3.2.0/misc/userscripts/qute-keepassxc`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/qute-lastpass` & `qutebrowser-3.2.0/misc/userscripts/qute-lastpass`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/qute-pass` & `qutebrowser-3.2.0/misc/userscripts/qute-pass`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/qutedmenu` & `qutebrowser-3.2.0/misc/userscripts/qutedmenu`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/readability` & `qutebrowser-3.2.0/misc/userscripts/readability`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/readability-js` & `qutebrowser-3.2.0/misc/userscripts/readability-js`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/ripbang` & `qutebrowser-3.2.0/misc/userscripts/ripbang`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/rss` & `qutebrowser-3.2.0/misc/userscripts/rss`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/taskadd` & `qutebrowser-3.2.0/misc/userscripts/taskadd`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/misc/userscripts/tor_identity` & `qutebrowser-3.2.0/misc/userscripts/tor_identity`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             f.write('message-error "Failed to import stem."')
     else:
         print('Failed to import stem.')
 
 
 if __name__ == '__main__':
     parser = ArgumentParser(prog='tor_identity')
-    parser.add_argument('-c', '--control-port', default=9051,
+    parser.add_argument('-c', '--control-port', type=int, default=9051,
                         help='Tor control port (default 9051).')
     parser.add_argument('-p', '--password', type=str, default=None,
                         help='Tor control port password.')
     args = parser.parse_args()
 
     with Controller.from_port(port=args.control_port) as controller:
         controller.authenticate(args.password)
```

### Comparing `qutebrowser-3.1.0/misc/userscripts/view_in_mpv` & `qutebrowser-3.2.0/misc/userscripts/view_in_mpv`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/pytest.ini` & `qutebrowser-3.2.0/pytest.ini`

 * *Files 10% similar despite different names*

```diff
@@ -57,16 +57,25 @@
     # Qt 6.5 debug build
     # WORKAROUND for https://www.riverbankcomputing.com/pipermail/pyqt/2023-March/045215.html
     ^QObject::connect: Connecting from COMPAT signal \(QSocketNotifier::activated\(int\)\)$
     # Randomly started showing up on Qt 5.15.2
     ^QBackingStore::endPaint\(\) called with active painter; did you forget to destroy it or call QPainter::end\(\) on it\?$
     # Qt 6.5 after system update, from qt-qt.accessibility.atspi
     Error in contacting registry: "org\.freedesktop\.DBus\.Error\.Disconnected" "Not connected to D-Bus server"
+    # Seen in Qt 6.6.2 on CI, https://github.com/qutebrowser/qutebrowser/pull/8106#issuecomment-1952320663
+    ^QDBusConnection: couldn't handle call to Notify, no slot matched
+    ^QDBusConnection: couldn't handle call to CloseNotification, no slot matched
+    # Qt 6.7
+    ^Path override failed for key base::DIR_APP_DICTIONARIES and path '.*/qtwebengine_dictionaries'
+    # Sometime the above message gets printed twice at the same time and the messages get interleaved.
+    # The last part of the outer message gets bumped down to a line on its own, so hopefully this
+    # catches that. And we don't see any other weird permutations of this.
+    ^[^ ]*qtwebengine_dictionaries'$
+    # Qt 5 on Archlinux
+    ^QSslSocket: cannot resolve .*
 xfail_strict = true
 filterwarnings =
     error
     default:Test process .* failed to terminate!:UserWarning
-    # Python 3.12: https://github.com/jendrikseipp/vulture/issues/314
-    ignore:ast\.Str is deprecated and will be removed in Python 3\.14; use ast\.Constant instead:DeprecationWarning:vulture\.core
-    # Python 3.12: https://github.com/ionelmc/pytest-benchmark/issues/240
+    # Python 3.12: https://github.com/ionelmc/pytest-benchmark/issues/240 (fixed but not released)
     ignore:(datetime\.)?datetime\.utcnow\(\) is deprecated and scheduled for removal in a future version\. Use timezone-aware objects to represent datetimes in UTC. (datetime\.)?datetime\.now\(datetime\.UTC\)\.:DeprecationWarning:pytest_benchmark\.utils
 faulthandler_timeout = 90
```

### Comparing `qutebrowser-3.1.0/qutebrowser/api/apitypes.py` & `qutebrowser-3.2.0/qutebrowser/api/apitypes.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/api/cmdutils.py` & `qutebrowser-3.2.0/qutebrowser/api/cmdutils.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/api/config.py` & `qutebrowser-3.2.0/qutebrowser/api/config.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/api/downloads.py` & `qutebrowser-3.2.0/qutebrowser/api/downloads.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/api/hook.py` & `qutebrowser-3.2.0/qutebrowser/api/hook.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/api/interceptor.py` & `qutebrowser-3.2.0/qutebrowser/api/interceptor.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/app.py` & `qutebrowser-3.2.0/qutebrowser/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,17 @@
 def init(*, args: argparse.Namespace) -> None:
     """Initialize everything."""
     log.init.debug("Starting init...")
 
     crashsignal.crash_handler.init_faulthandler()
 
     objects.qapp.setQuitOnLastWindowClosed(False)
+    # WORKAROUND for KDE file dialogs / QEventLoopLocker quitting:
+    # https://bugreports.qt.io/browse/QTBUG-124386
+    objects.qapp.setQuitLockEnabled(False)
     quitter.instance.shutting_down.connect(QApplication.closeAllWindows)
 
     _init_icon()
 
     loader.init()
     loader.load_components()
     try:
```

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/browsertab.py` & `qutebrowser-3.2.0/qutebrowser/browser/browsertab.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import functools
 import dataclasses
 from typing import (cast, TYPE_CHECKING, Any, Callable, Iterable, List, Optional,
                     Sequence, Set, Type, Union, Tuple)
 
 from qutebrowser.qt import machinery
 from qutebrowser.qt.core import (pyqtSignal, pyqtSlot, QUrl, QObject, QSizeF, Qt,
-                          QEvent, QPoint, QRect)
+                          QEvent, QPoint, QRect, QTimer)
 from qutebrowser.qt.gui import QKeyEvent, QIcon, QPixmap
 from qutebrowser.qt.widgets import QApplication, QWidget
 from qutebrowser.qt.printsupport import QPrintDialog, QPrinter
 from qutebrowser.qt.network import QNetworkAccessManager
 
 if TYPE_CHECKING:
     from qutebrowser.qt.webkit import QWebHistory, QWebHistoryItem
@@ -898,15 +898,21 @@
             if elem is None:
                 log.webview.debug("No focused element!")
                 return
             if elem.is_editable():
                 modeman.enter(self._tab.win_id, usertypes.KeyMode.insert,
                               'load finished', only_if_normal=True)
 
-        self._tab.elements.find_focused(_auto_insert_mode_cb)
+        # There seems to be a race between loadFinished being called,
+        # and the autoload attribute on websites actually focusing anything.
+        # Thus, we delay this by a bit. Locally, a delay of 13ms caused no races
+        # with 5000 test reruns (even with simultaneous CPU stress testing),
+        # so 65ms should be a safe bet and still not be too noticeable.
+        QTimer.singleShot(
+            65, lambda: self._tab.elements.find_focused(_auto_insert_mode_cb))
 
     def clear_ssl_errors(self) -> None:
         raise NotImplementedError
 
     def networkaccessmanager(self) -> Optional[QNetworkAccessManager]:
         """Get the QNetworkAccessManager for this tab.
```

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/commands.py` & `qutebrowser-3.2.0/qutebrowser/browser/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -944,14 +944,16 @@
             active_win = QApplication.activeWindow()
             if active_win is None:
                 # Not sure how you enter a command without an active window...
                 raise cmdutils.CommandError(
                     "No window specified and couldn't find active window!")
             assert isinstance(active_win, mainwindow.MainWindow), active_win
             win_id = active_win.win_id
+        else:
+            raise utils.Unreachable(index_parts)
 
         if win_id not in objreg.window_registry:
             raise cmdutils.CommandError(
                 "There's no window with id {}!".format(win_id))
 
         tabbed_browser = objreg.get('tabbed-browser', scope='window',
                                     window=win_id)
```

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/downloads.py` & `qutebrowser-3.2.0/qutebrowser/browser/downloads.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/downloadview.py` & `qutebrowser-3.2.0/qutebrowser/browser/downloadview.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/eventfilter.py` & `qutebrowser-3.2.0/qutebrowser/browser/eventfilter.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/greasemonkey.py` & `qutebrowser-3.2.0/qutebrowser/browser/greasemonkey.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/hints.py` & `qutebrowser-3.2.0/qutebrowser/browser/hints.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/history.py` & `qutebrowser-3.2.0/qutebrowser/browser/history.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/inspector.py` & `qutebrowser-3.2.0/qutebrowser/browser/inspector.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/navigate.py` & `qutebrowser-3.2.0/qutebrowser/browser/navigate.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/network/pac.py` & `qutebrowser-3.2.0/qutebrowser/browser/network/pac.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/network/proxy.py` & `qutebrowser-3.2.0/qutebrowser/browser/network/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # SPDX-FileCopyrightText: Florian Bruhin (The Compiler) <mail@qutebrowser.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Handling of proxies."""
 
+from typing import Optional
+
 from qutebrowser.qt.core import QUrl, pyqtSlot
 from qutebrowser.qt.network import QNetworkProxy, QNetworkProxyFactory
 
 from qutebrowser.config import config, configtypes
 from qutebrowser.utils import message, usertypes, urlutils, utils, qtutils
 from qutebrowser.misc import objects
 from qutebrowser.browser.network import pac
 
 
-application_factory = None
+application_factory: Optional["ProxyFactory"] = None
 
 
 def init():
     """Set the application wide proxy factory."""
     global application_factory
     application_factory = ProxyFactory()
     QNetworkProxyFactory.setApplicationProxyFactory(application_factory)
```

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/pdfjs.py` & `qutebrowser-3.2.0/qutebrowser/browser/pdfjs.py`

 * *Files 13% similar despite different names*

```diff
@@ -65,28 +65,45 @@
     html = html.replace(
         '<head>',
         '<head>\n<script>window.Response = undefined;</script>\n'
     )
     return html
 
 
+def _generate_polyfills():
+    return """
+        if (typeof Promise.withResolvers === 'undefined') {
+            Promise.withResolvers = function () {
+                let resolve, reject
+                const promise = new Promise((res, rej) => {
+                    resolve = res
+                    reject = rej
+                })
+                return { promise, resolve, reject }
+            }
+        }
+    """
+
+
 def _generate_pdfjs_script(filename):
     """Generate the script that shows the pdf with pdf.js.
 
     Args:
         filename: The name of the file to open.
     """
     url = QUrl('qute://pdfjs/file')
     url_query = QUrlQuery()
     url_query.addQueryItem('filename', filename)
     url.setQuery(url_query)
 
     js_url = javascript.to_js(url.toString(urlutils.FormatOption.ENCODED))
 
     return jinja.js_environment.from_string("""
+        {{ polyfills }}
+
         document.addEventListener("DOMContentLoaded", function() {
             if (typeof window.PDFJS !== 'undefined') {
                 // v1.x
                 window.PDFJS.verbosity = window.PDFJS.VERBOSITY_LEVELS.info;
             } else {
                 // v2.x+
                 const options = window.PDFViewerApplicationOptions;
@@ -100,15 +117,15 @@
                 // v1.6+
                 window.PDFViewerApplication.open({
                     url: {{ url }},
                     originalUrl: {{ url }}
                 });
             }
         });
-    """).render(url=js_url)
+    """).render(url=js_url, polyfills=_generate_polyfills())
 
 
 def get_pdfjs_res_and_path(path):
     """Get a pdf.js resource in binary format.
 
     Returns a (content, path) tuple, where content is the file content and path
     is the path where the file was found. If path is None, the bundled version
@@ -144,14 +161,22 @@
             content = resources.read_file_binary(res_path)
         except FileNotFoundError:
             raise PDFJSNotFound(path) from None
         except OSError as e:
             log.misc.warning("OSError while reading PDF.js file: {}".format(e))
             raise PDFJSNotFound(path) from None
 
+    if path == "build/pdf.worker.mjs":
+        content = b"\n".join(
+            [
+                _generate_polyfills().encode("ascii"),
+                content,
+            ]
+        )
+
     return content, file_path
 
 
 def get_pdfjs_res(path):
     """Get a pdf.js resource in binary format.
 
     Args:
```

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/qtnetworkdownloads.py` & `qutebrowser-3.2.0/qutebrowser/browser/qtnetworkdownloads.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from qutebrowser.qt.widgets import QApplication
 from qutebrowser.qt.network import QNetworkRequest, QNetworkReply, QNetworkAccessManager
 
 from qutebrowser.config import config, websettings
 from qutebrowser.utils import message, usertypes, log, urlutils, utils, debug, objreg, qtlog
 from qutebrowser.misc import quitter
 from qutebrowser.browser import downloads
-from qutebrowser.browser.webkit import http
+from qutebrowser.browser.webkit import httpheaders
 from qutebrowser.browser.webkit.network import networkmanager
 
 
 @dataclasses.dataclass
 class _RetryInfo:
 
     request: QNetworkRequest
@@ -120,15 +120,15 @@
             log.downloads.debug(f"File position at error: {pos}")
             try:
                 self.fileobj.close()
             except OSError:
                 log.downloads.exception("Error while closing file object")
 
             if pos == 0:
-                # Emtpy remaining file
+                # Empty remaining file
                 filename = self._get_open_filename()
                 log.downloads.debug(f"Removing empty file at {filename}")
                 try:
                     os.remove(filename)
                 except OSError:
                     log.downloads.exception("Error while removing empty file")
 
@@ -529,15 +529,15 @@
         Return:
             The created DownloadItem.
         """
         if not suggested_filename:
             try:
                 suggested_filename = target.suggested_filename()
             except downloads.NoFilenameError:
-                _, suggested_filename = http.parse_content_disposition(reply)
+                _, suggested_filename = httpheaders.parse_content_disposition(reply)
         log.downloads.debug("fetch: {} -> {}".format(reply.url(),
                                                      suggested_filename))
         download = DownloadItem(reply, manager=self)
         self._init_item(download, auto_remove, suggested_filename)
 
         if download.cancel_for_origin():
             return download
```

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/qutescheme.py` & `qutebrowser-3.2.0/qutebrowser/browser/qutescheme.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 from qutebrowser.utils import (version, utils, jinja, log, message, docutils,
                                resources, objreg, standarddir)
 from qutebrowser.misc import guiprocess, quitter
 from qutebrowser.qt import sip
 
 
 pyeval_output = ":pyeval was never called"
-csrf_token = None
+csrf_token: Optional[str] = None
 
 
-_HANDLERS = {}
+_HANDLERS: Dict[str, "_HandlerCallable"] = {}
 
 
 class Error(Exception):
 
     """Exception for generic errors on a qute:// page."""
```

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/shared.py` & `qutebrowser-3.2.0/qutebrowser/browser/shared.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/signalfilter.py` & `qutebrowser-3.2.0/qutebrowser/browser/signalfilter.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/urlmarks.py` & `qutebrowser-3.2.0/qutebrowser/browser/urlmarks.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webelem.py` & `qutebrowser-3.2.0/qutebrowser/browser/webelem.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,18 +351,22 @@
 
         events = [
             QMouseEvent(QEvent.Type.MouseMove, pos, Qt.MouseButton.NoButton, Qt.MouseButton.NoButton, Qt.KeyboardModifier.NoModifier),
             QMouseEvent(QEvent.Type.MouseButtonPress, pos, button, button, modifiers),
             QMouseEvent(QEvent.Type.MouseButtonRelease, pos, button, Qt.MouseButton.NoButton, modifiers),
         ]
 
-        for evt in events:
-            self._tab.send_event(evt)
+        def _send_events_after_delay() -> None:
+            """Delay clicks to workaround timing issue in e2e tests on 6.7."""
+            for evt in events:
+                self._tab.send_event(evt)
 
-        QTimer.singleShot(0, self._move_text_cursor)
+            QTimer.singleShot(0, self._move_text_cursor)
+
+        QTimer.singleShot(10, _send_events_after_delay)
 
     def _click_editable(self, click_target: usertypes.ClickTarget) -> None:
         """Fake a click on an editable input field."""
         raise NotImplementedError
 
     def _click_js(self, click_target: usertypes.ClickTarget) -> None:
         """Fake a click by using the JS .click() method."""
```

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webengine/certificateerror.py` & `qutebrowser-3.2.0/qutebrowser/browser/webengine/certificateerror.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webengine/cookies.py` & `qutebrowser-3.2.0/qutebrowser/browser/webengine/cookies.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webengine/darkmode.py` & `qutebrowser-3.2.0/qutebrowser/browser/webengine/darkmode.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,39 +109,49 @@
   https://chromium-review.googlesource.com/c/chromium/src/+/3821841
 
 Qt 6.6
 ------
 
 - New alternative image classifier:
   https://chromium-review.googlesource.com/c/chromium/src/+/3987823
+
+Qt 6.7
+------
+
+Enabling dark mode can now be done at runtime via QWebEngineSettings.
 """
 
 import os
 import copy
 import enum
 import dataclasses
 import collections
 from typing import (Any, Iterator, Mapping, MutableMapping, Optional, Set, Tuple, Union,
                     Sequence, List)
 
 from qutebrowser.config import config
 from qutebrowser.utils import usertypes, utils, log, version
 
+# Note: We *cannot* initialize QtWebEngine (even implicitly) in here, but checking for
+# the enum attribute seems to be okay.
+from qutebrowser.qt.webenginecore import QWebEngineSettings
+
 
 _BLINK_SETTINGS = 'blink-settings'
 
 
 class Variant(enum.Enum):
 
     """A dark mode variant."""
 
     qt_515_2 = enum.auto()
     qt_515_3 = enum.auto()
     qt_64 = enum.auto()
     qt_66 = enum.auto()
+    qt_67 = enum.auto()
 
 
 # Mapping from a colors.webpage.darkmode.algorithm setting value to
 # Chromium's DarkModeInversionAlgorithm enum values.
 _ALGORITHMS = {
     # 0: kOff (not exposed)
     # 1: kSimpleInvertForTesting (not exposed)
@@ -183,19 +193,14 @@
 }
 
 _BOOLS = {
     True: 'true',
     False: 'false',
 }
 
-_INT_BOOLS = {
-    True: '1',
-    False: '0',
-}
-
 
 @dataclasses.dataclass
 class _Setting:
 
     """A single dark mode setting."""
 
     option: str
@@ -256,34 +261,33 @@
         Yields tuples which contain the Chromium setting key (e.g. 'blink-settings' or
         'dark-mode-settings') and the corresponding _Settings object.
         """
         for setting in self._settings:
             switch = self._switch_names.get(setting.option, self._switch_names[None])
             yield switch, setting.with_prefix(self.prefix)
 
-    def copy_with(self, attr: str, value: Any) -> '_Definition':
-        """Get a new _Definition object with a changed attribute.
-
-        NOTE: This does *not* copy the settings list. Both objects will reference the
-        same (immutable) tuple.
-        """
-        new = copy.copy(self)
-        setattr(new, attr, value)
-        return new
-
     def copy_add_setting(self, setting: _Setting) -> '_Definition':
         """Get a new _Definition object with an additional setting."""
         new = copy.copy(self)
         new._settings = self._settings + (setting,)  # pylint: disable=protected-access
         return new
 
+    def copy_remove_setting(self, name: str) -> '_Definition':
+        """Get a new _Definition object with a setting removed."""
+        new = copy.copy(self)
+        filtered_settings = tuple(s for s in self._settings if s.option != name)
+        if len(filtered_settings) == len(self._settings):
+            raise ValueError(f"Setting {name} not found in {self}")
+        new._settings = filtered_settings  # pylint: disable=protected-access
+        return new
+
     def copy_replace_setting(self, option: str, chromium_key: str) -> '_Definition':
         """Get a new _Definition object with `old` replaced by `new`.
 
-        If `old` is not in the settings list, return the old _Definition object.
+        If `old` is not in the settings list, raise ValueError.
         """
         new = copy.deepcopy(self)
 
         for setting in new._settings:  # pylint: disable=protected-access
             if setting.option == option:
                 setting.chromium_key = chromium_key
                 return new
@@ -328,14 +332,16 @@
 }
 _DEFINITIONS[Variant.qt_64] = _DEFINITIONS[Variant.qt_515_3].copy_replace_setting(
     'threshold.foreground', 'ForegroundBrightnessThreshold',
 )
 _DEFINITIONS[Variant.qt_66] = _DEFINITIONS[Variant.qt_64].copy_add_setting(
     _Setting('policy.images', 'ImageClassifierPolicy', _IMAGE_CLASSIFIERS),
 )
+# Qt 6.7: Enabled is now handled dynamically via QWebEngineSettings
+_DEFINITIONS[Variant.qt_67] = _DEFINITIONS[Variant.qt_66].copy_remove_setting('enabled')
 
 
 _SettingValType = Union[str, usertypes.Unset]
 _PREFERRED_COLOR_SCHEME_DEFINITIONS: MutableMapping[Variant, Mapping[_SettingValType, str]] = {
     Variant.qt_515_2: {
         # 0: no-preference (not exposed)
         "dark": "1",
@@ -363,15 +369,22 @@
     env_var = os.environ.get('QUTE_DARKMODE_VARIANT')
     if env_var is not None:
         try:
             return Variant[env_var]
         except KeyError:
             log.init.warning(f"Ignoring invalid QUTE_DARKMODE_VARIANT={env_var}")
 
-    if versions.webengine >= utils.VersionNumber(6, 6):
+    if (
+        # We need a PyQt 6.7 as well with the API available, otherwise we can't turn on
+        # dark mode later in webenginesettings.py.
+        versions.webengine >= utils.VersionNumber(6, 7) and
+        hasattr(QWebEngineSettings.WebAttribute, 'ForceDarkMode')
+    ):
+        return Variant.qt_67
+    elif versions.webengine >= utils.VersionNumber(6, 6):
         return Variant.qt_66
     elif versions.webengine >= utils.VersionNumber(6, 4):
         return Variant.qt_64
     elif (versions.webengine == utils.VersionNumber(5, 15, 2) and
             versions.chromium_major == 87):
         # WORKAROUND for Gentoo packaging something newer as 5.15.2...
         return Variant.qt_515_3
```

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webengine/interceptor.py` & `qutebrowser-3.2.0/qutebrowser/browser/webengine/interceptor.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webengine/notification.py` & `qutebrowser-3.2.0/qutebrowser/browser/webengine/notification.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webengine/spell.py` & `qutebrowser-3.2.0/qutebrowser/browser/webengine/spell.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webengine/tabhistory.py` & `qutebrowser-3.2.0/qutebrowser/browser/webengine/tabhistory.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webengine/webenginedownloads.py` & `qutebrowser-3.2.0/qutebrowser/browser/webengine/webenginedownloads.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webengine/webengineelem.py` & `qutebrowser-3.2.0/qutebrowser/browser/webengine/webengineelem.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webengine/webengineinspector.py` & `qutebrowser-3.2.0/qutebrowser/browser/webengine/webengineinspector.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webengine/webenginequtescheme.py` & `qutebrowser-3.2.0/qutebrowser/browser/webengine/webenginequtescheme.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webengine/webenginesettings.py` & `qutebrowser-3.2.0/qutebrowser/browser/webengine/webenginesettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # The default QWebEngineProfile
 default_profile = cast(QWebEngineProfile, None)
 # The QWebEngineProfile used for private (off-the-record) windows
 private_profile: Optional[QWebEngineProfile] = None
 # The global WebEngineSettings object
 _global_settings = cast('WebEngineSettings', None)
 
-parsed_user_agent = None
+parsed_user_agent: Optional[websettings.UserAgent] = None
 
 _qute_scheme_handler = cast(webenginequtescheme.QuteSchemeHandler, None)
 _req_interceptor = cast('interceptor.RequestInterceptor', None)
 _download_manager = cast(webenginedownloads.DownloadManager, None)
 
 
 class _SettingsWrapper:
@@ -144,20 +144,28 @@
         'content.dns_prefetch':
             Attr(QWebEngineSettings.WebAttribute.DnsPrefetchEnabled),
 
         'tabs.favicons.show':
             Attr(QWebEngineSettings.WebAttribute.AutoLoadIconsForPage,
                  converter=lambda val: val != 'never'),
     }
-    try:
-        _ATTRIBUTES['content.canvas_reading'] = Attr(
-            QWebEngineSettings.WebAttribute.ReadingFromCanvasEnabled)  # type: ignore[attr-defined,unused-ignore]
-    except AttributeError:
-        # Added in QtWebEngine 6.6
-        pass
+
+    if machinery.IS_QT6:
+        try:
+            _ATTRIBUTES['content.canvas_reading'] = Attr(
+                QWebEngineSettings.WebAttribute.ReadingFromCanvasEnabled)
+        except AttributeError:
+            # Added in QtWebEngine 6.6
+            pass
+        try:
+            _ATTRIBUTES['colors.webpage.darkmode.enabled'] = Attr(
+                QWebEngineSettings.WebAttribute.ForceDarkMode)
+        except AttributeError:
+            # Added in QtWebEngine 6.7
+            pass
 
     _FONT_SIZES = {
         'fonts.web.size.minimum':
             QWebEngineSettings.FontSize.MinimumFontSize,
         'fonts.web.size.minimum_logical':
             QWebEngineSettings.FontSize.MinimumLogicalFontSize,
         'fonts.web.size.default':
```

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webengine/webenginetab.py` & `qutebrowser-3.2.0/qutebrowser/browser/webengine/webenginetab.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import struct
 import functools
 import dataclasses
 import re
 import html as html_utils
 from typing import cast, Union, Optional
 
-from qutebrowser.qt.core import (pyqtSignal, pyqtSlot, Qt, QPoint, QPointF, QTimer, QUrl,
+from qutebrowser.qt.core import (pyqtSignal, pyqtSlot, Qt, QPoint, QPointF, QUrl,
                           QObject, QByteArray)
 from qutebrowser.qt.network import QAuthenticator
 from qutebrowser.qt.webenginecore import QWebEnginePage, QWebEngineScript, QWebEngineHistory
 
 from qutebrowser.config import config
 from qutebrowser.browser import browsertab, eventfilter, shared, webelem, greasemonkey
 from qutebrowser.browser.webengine import (webview, webengineelem, tabhistory,
@@ -288,14 +288,16 @@
     _tab: 'WebEngineTab'
 
     def _flags(self):
         """Get flags to pass to JS."""
         flags = set()
         if utils.is_windows:
             flags.add('windows')
+        if 'caret' in objects.debug_flags:
+            flags.add('debug')
         return list(flags)
 
     @pyqtSlot(usertypes.KeyMode)
     def _on_mode_entered(self, mode):
         if mode != usertypes.KeyMode.caret:
             return
 
@@ -810,15 +812,15 @@
     def __init__(self, tab, parent=None):
         super().__init__(tab, parent)
         self._overridden = False
 
         # Implements the intended two-second delay specified at
         # https://doc.qt.io/archives/qt-5.14/qwebenginepage.html#recentlyAudibleChanged
         delay_ms = 2000
-        self._silence_timer = QTimer(self)
+        self._silence_timer = usertypes.Timer(self)
         self._silence_timer.setSingleShot(True)
         self._silence_timer.setInterval(delay_ms)
 
     def _connect_signals(self):
         page = self._widget.page()
         page.audioMutedChanged.connect(self.muted_changed)
         page.recentlyAudibleChanged.connect(self._delayed_recently_audible_changed)
@@ -1471,17 +1473,17 @@
             self.data.netrc_used = True
             netrc_success = shared.netrc_authentication(url, authenticator)
 
         if not netrc_success:
             log.network.debug("Asking for credentials")
             answer = shared.authentication_required(
                 url, authenticator, abort_on=[self.abort_questions])
-        if not netrc_success and answer is None:
-            log.network.debug("Aborting auth")
-            sip.assign(authenticator, QAuthenticator())
+            if answer is None:
+                log.network.debug("Aborting auth")
+                sip.assign(authenticator, QAuthenticator())
 
     @pyqtSlot()
     def _on_load_started(self):
         """Clear search when a new load is started if needed."""
         # WORKAROUND for
         # https://bugreports.qt.io/browse/QTBUG-61506
         # (seems to be back in later Qt versions as well)
```

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webengine/webview.py` & `qutebrowser-3.2.0/qutebrowser/browser/webengine/webview.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,17 +234,15 @@
     def __init__(self, *, theme_color, profile, parent=None):
         super().__init__(profile, parent)
         self._is_shutting_down = False
         self._theme_color = theme_color
         self._set_bg_color()
         config.instance.changed.connect(self._set_bg_color)
         if machinery.IS_QT6:
-            self.certificateError.connect(  # pylint: disable=no-member
-                self._handle_certificate_error
-            )
+            self.certificateError.connect(self._handle_certificate_error)
             # Qt 5: Overridden method instead of signal
 
     @config.change_filter('colors.webpage.bg')
     def _set_bg_color(self):
         col = config.val.colors.webpage.bg
         if col is None:
             col = self._theme_color
```

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/cache.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/cache.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/certificateerror.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/certificateerror.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/cookies.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/cookies.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/http.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/httpheaders.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/mhtml.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/mhtml.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/network/filescheme.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/network/filescheme.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/network/networkmanager.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/network/networkmanager.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/network/networkreply.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/network/networkreply.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/network/webkitqutescheme.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/network/webkitqutescheme.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/tabhistory.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/tabhistory.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/webkitelem.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/webkitelem.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/webkithistory.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/webkithistory.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/webkitinspector.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/webkitinspector.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/webkitsettings.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/webkitsettings.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/webkittab.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/webkittab.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/webpage.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/webpage.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from qutebrowser.qt.printsupport import QPrintDialog
 # pylint: disable=no-name-in-module
 from qutebrowser.qt.webkitwidgets import QWebPage, QWebFrame
 # pylint: enable=no-name-in-module
 
 from qutebrowser.config import websettings, config
 from qutebrowser.browser import pdfjs, shared, downloads, greasemonkey
-from qutebrowser.browser.webkit import http
+from qutebrowser.browser.webkit import httpheaders
 from qutebrowser.browser.webkit.network import networkmanager
 from qutebrowser.utils import message, usertypes, log, jinja, objreg
 from qutebrowser.qt import sip
 
 
 class BrowserPage(QWebPage):
 
@@ -259,22 +259,22 @@
 
         Most likely this will mean we need to download the reply, but we
         correct for some common errors the server do.
 
         At some point we might want to implement the MIME Sniffing standard
         here: https://mimesniff.spec.whatwg.org/
         """
-        inline, suggested_filename = http.parse_content_disposition(reply)
+        inline, suggested_filename = httpheaders.parse_content_disposition(reply)
         download_manager = objreg.get('qtnetwork-download-manager')
         if not inline:
             # Content-Disposition: attachment -> force download
             download_manager.fetch(reply,
                                    suggested_filename=suggested_filename)
             return
-        mimetype, _rest = http.parse_content_type(reply)
+        mimetype, _rest = httpheaders.parse_content_type(reply)
         if mimetype == 'image/jpg':
             # Some servers (e.g. the LinkedIn CDN) send a non-standard
             # image/jpg (instead of image/jpeg, defined in RFC 1341 section
             # 7.5). If this is the case, we force displaying with a corrected
             # mimetype.
             if reply.isFinished():
                 self.display_content(reply, 'image/jpeg')
```

### Comparing `qutebrowser-3.1.0/qutebrowser/browser/webkit/webview.py` & `qutebrowser-3.2.0/qutebrowser/browser/webkit/webview.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/commands/__init__.py` & `qutebrowser-3.2.0/qutebrowser/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/commands/argparser.py` & `qutebrowser-3.2.0/qutebrowser/commands/argparser.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/commands/cmdexc.py` & `qutebrowser-3.2.0/qutebrowser/commands/cmdexc.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/commands/command.py` & `qutebrowser-3.2.0/qutebrowser/commands/command.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/commands/parser.py` & `qutebrowser-3.2.0/qutebrowser/commands/parser.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/commands/runners.py` & `qutebrowser-3.2.0/qutebrowser/commands/runners.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Module containing command managers (SearchRunner and CommandRunner)."""
 
 import traceback
 import re
 import contextlib
-from typing import TYPE_CHECKING, Callable, Dict, Iterator, Mapping, MutableMapping
+from typing import TYPE_CHECKING, Callable, Dict, Tuple, Iterator, Mapping, MutableMapping
 
 from qutebrowser.qt.core import pyqtSlot, QUrl, QObject
 
 from qutebrowser.api import cmdutils
 from qutebrowser.commands import cmdexc, parser
 from qutebrowser.utils import message, objreg, qtutils, usertypes, utils
 from qutebrowser.keyinput import macros, modeman
 
 if TYPE_CHECKING:
     from qutebrowser.mainwindow import tabbedbrowser
 _ReplacementFunction = Callable[['tabbedbrowser.TabbedBrowser'], str]
 
 
-last_command = {}
+last_command: Dict[usertypes.KeyMode, Tuple[str, int]] = {}
 
 
 def _url(tabbed_browser):
     """Convenience method to get the current url."""
     try:
         return tabbed_browser.current_url()
     except qtutils.QtValueError as e:
```

### Comparing `qutebrowser-3.1.0/qutebrowser/commands/userscripts.py` & `qutebrowser-3.2.0/qutebrowser/commands/userscripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,14 @@
         self._kwargs = kwargs
 
         try:
             with tempfile.NamedTemporaryFile(delete=False) as handle:
                 self._filepath = handle.name
         except OSError as e:
             message.error("Error while creating tempfile: {}".format(e))
-            return
 
 
 class Error(Exception):
 
     """Base class for userscript exceptions."""
```

### Comparing `qutebrowser-3.1.0/qutebrowser/completion/completer.py` & `qutebrowser-3.2.0/qutebrowser/completion/completer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Completer attached to a CompletionView."""
 
 import dataclasses
 from typing import TYPE_CHECKING
 
-from qutebrowser.qt.core import pyqtSlot, QObject, QTimer
+from qutebrowser.qt.core import pyqtSlot, QObject
 
 from qutebrowser.config import config
 from qutebrowser.commands import parser, cmdexc
 from qutebrowser.misc import objects, split
-from qutebrowser.utils import log, utils, debug, objreg
+from qutebrowser.utils import log, utils, debug, objreg, usertypes
 from qutebrowser.completion.models import miscmodels
 from qutebrowser.completion import completionwidget
 if TYPE_CHECKING:
     from qutebrowser.browser import browsertab
 
 
 @dataclasses.dataclass
@@ -45,15 +45,15 @@
         _last_before_cursor: The prior value of before_cursor.
     """
 
     def __init__(self, *, cmd, win_id, parent=None):
         super().__init__(parent)
         self._cmd = cmd
         self._win_id = win_id
-        self._timer = QTimer()
+        self._timer = usertypes.Timer()
         self._timer.setSingleShot(True)
         self._timer.setInterval(0)
         self._timer.timeout.connect(self._update_completion)
         self._last_cursor_pos = -1
         self._last_text = None
         self._last_before_cursor = None
         self._cmd.update_completion.connect(self.schedule_completion_update)
```

### Comparing `qutebrowser-3.1.0/qutebrowser/completion/completiondelegate.py` & `qutebrowser-3.2.0/qutebrowser/completion/completiondelegate.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/completion/completionwidget.py` & `qutebrowser-3.2.0/qutebrowser/completion/completionwidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,15 +410,15 @@
         if config.val.completion.shrink:
             self.update_geometry.emit()
 
     @pyqtSlot()
     def on_clear_completion_selection(self):
         """Clear the selection model when an item is activated."""
         self.hide()
-        selmod = self._selection_model()
+        selmod = self.selectionModel()
         if selmod is not None:
             selmod.clearSelection()
             selmod.clearCurrentIndex()
 
     def sizeHint(self):
         """Get the completion size according to the config."""
         # Get the configured height/percentage.
@@ -433,16 +433,15 @@
         # Shrink to content size if needed and shrinking is enabled
         if config.val.completion.shrink:
             bar = self.horizontalScrollBar()
             assert bar is not None
             contents_height = (
                 self.viewportSizeHint().height() +
                 bar.sizeHint().height())
-            if contents_height <= height:
-                height = contents_height
+            height = min(height, contents_height)
         # The width isn't really relevant as we're expanding anyways.
         return QSize(-1, height)
 
     def selectionChanged(self, selected, deselected):
         """Extend selectionChanged to call completers selection_changed."""
         if not self._active:
             return
```

### Comparing `qutebrowser-3.1.0/qutebrowser/completion/models/completionmodel.py` & `qutebrowser-3.2.0/qutebrowser/completion/models/completionmodel.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/completion/models/configmodel.py` & `qutebrowser-3.2.0/qutebrowser/completion/models/configmodel.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/completion/models/filepathcategory.py` & `qutebrowser-3.2.0/qutebrowser/completion/models/filepathcategory.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/completion/models/histcategory.py` & `qutebrowser-3.2.0/qutebrowser/completion/models/histcategory.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/completion/models/listcategory.py` & `qutebrowser-3.2.0/qutebrowser/completion/models/listcategory.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,18 +44,21 @@
         Args:
             val: The value to set.
         """
         if len(val) > 5000:  # avoid crash on huge search terms (#5973)
             log.completion.warning(f"Trimming {len(val)}-char pattern to 5000")
             val = val[:5000]
         self._pattern = val
-        val = re.sub(r' +', r' ', val)  # See #1919
-        val = re.escape(val)
-        val = val.replace(r'\ ', '.*')
-        rx = QRegularExpression(val, QRegularExpression.PatternOption.CaseInsensitiveOption)
+
+        # Positive lookahead per search term. This means that all search terms must
+        # be matched but they can be matched anywhere in the string, so they can be
+        # in any order. For example "foo bar" -> "(?=.*foo)(?=.*bar)"
+        re_pattern = "^" + "".join(f"(?=.*{re.escape(term)})" for term in val.split())
+
+        rx = QRegularExpression(re_pattern, QRegularExpression.PatternOption.CaseInsensitiveOption)
         qtutils.ensure_valid(rx)
         self.setFilterRegularExpression(rx)
         self.invalidate()
         sortcol = 0
         self.sort(sortcol)
 
     def lessThan(self, lindex, rindex):
```

### Comparing `qutebrowser-3.1.0/qutebrowser/completion/models/miscmodels.py` & `qutebrowser-3.2.0/qutebrowser/completion/models/miscmodels.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/completion/models/urlmodel.py` & `qutebrowser-3.2.0/qutebrowser/completion/models/urlmodel.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/completion/models/util.py` & `qutebrowser-3.2.0/qutebrowser/completion/models/util.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/components/adblockcommands.py` & `qutebrowser-3.2.0/qutebrowser/components/adblockcommands.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/components/braveadblock.py` & `qutebrowser-3.2.0/qutebrowser/components/braveadblock.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/components/caretcommands.py` & `qutebrowser-3.2.0/qutebrowser/components/caretcommands.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/components/hostblock.py` & `qutebrowser-3.2.0/qutebrowser/components/hostblock.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/components/misccommands.py` & `qutebrowser-3.2.0/qutebrowser/components/misccommands.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/components/readlinecommands.py` & `qutebrowser-3.2.0/qutebrowser/components/readlinecommands.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/components/scrollcommands.py` & `qutebrowser-3.2.0/qutebrowser/components/scrollcommands.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/components/utils/blockutils.py` & `qutebrowser-3.2.0/qutebrowser/components/utils/blockutils.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/components/zoomcommands.py` & `qutebrowser-3.2.0/qutebrowser/components/zoomcommands.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/config/config.py` & `qutebrowser-3.2.0/qutebrowser/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # An easy way to access the config from other code via config.val.foo
 val = cast('ConfigContainer', None)
 instance = cast('Config', None)
 key_instance = cast('KeyConfig', None)
 cache = cast('configcache.ConfigCache', None)
 
 # Keeping track of all change filters to validate them later.
-change_filters = []
+change_filters: List["change_filter"] = []
 
 # Sentinel
 UNSET = object()
 
 
 class change_filter:  # noqa: N801,N806 pylint: disable=invalid-name
```

### Comparing `qutebrowser-3.1.0/qutebrowser/config/configcache.py` & `qutebrowser-3.2.0/qutebrowser/config/configcache.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/config/configcommands.py` & `qutebrowser-3.2.0/qutebrowser/config/configcommands.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/config/configdata.py` & `qutebrowser-3.2.0/qutebrowser/config/configdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Module attributes:
 
 DATA: A dict of Option objects after init() has been called.
 """
 
 from typing import (Any, Dict, Iterable, List, Mapping, MutableMapping, Optional,
-                    Sequence, Tuple, Union, cast)
+                    Sequence, Tuple, Union, NoReturn, cast)
 import functools
 import dataclasses
 
 from qutebrowser.config import configtypes
 from qutebrowser.utils import usertypes, qtutils, utils, resources
 from qutebrowser.misc import debugcachestats
 
@@ -53,15 +53,15 @@
         deleted: A list of option names which have been removed.
     """
 
     renamed: Dict[str, str] = dataclasses.field(default_factory=dict)
     deleted: List[str] = dataclasses.field(default_factory=list)
 
 
-def _raise_invalid_node(name: str, what: str, node: Any) -> None:
+def _raise_invalid_node(name: str, what: str, node: Any) -> NoReturn:
     """Raise an exception for an invalid configdata YAML node.
 
     Args:
         name: The name of the setting being parsed.
         what: The name of the thing being parsed.
         node: The invalid node.
     """
@@ -90,14 +90,15 @@
         valid_values = kwargs.get('valid_values', None)
         if valid_values is not None:
             kwargs['valid_values'] = configtypes.ValidValues(*valid_values)
     else:
         _raise_invalid_node(name, 'type', node)
 
     try:
+        # pylint: disable=possibly-used-before-assignment
         typ = getattr(configtypes, type_name)
     except AttributeError:
         raise AttributeError("Did not find type {} for {}".format(
             type_name, name))
 
     # Parse sub-types
     try:
```

### Comparing `qutebrowser-3.1.0/qutebrowser/config/configdata.yml` & `qutebrowser-3.2.0/qutebrowser/config/configdata.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1780,14 +1780,15 @@
       - '[onclick]'
       - '[onmousedown]'
       - '[role="link"]'
       - '[role="option"]'
       - '[role="button"]'
       - '[role="tab"]'
       - '[role="checkbox"]'
+      - '[role="switch"]'
       - '[role="menuitem"]'
       - '[role="menuitemcheckbox"]'
       - '[role="menuitemradio"]'
       - '[role="treeitem"]'
       - '[aria-haspopup]'
       - '[ng-click]'
       - '[ngClick]'
@@ -3267,28 +3268,31 @@
 
 colors.webpage.darkmode.enabled:
   default: false
   type: Bool
   desc: >-
     Render all web contents using a dark theme.
 
+    On QtWebEngine < 6.7, this setting requires a restart and does not support
+    URL patterns, only the global setting is applied.
+
     Example configurations from Chromium's `chrome://flags`:
 
     - "With simple HSL/CIELAB/RGB-based inversion": Set
       `colors.webpage.darkmode.algorithm` accordingly, and
       set `colors.webpage.darkmode.policy.images` to `never`.
 
     - "With selective image inversion": qutebrowser default settings.
-  restart: true
+  supports_pattern: true
   backend: QtWebEngine
 
 colors.webpage.darkmode.algorithm:
   default: lightness-cielab
   desc: >-
-    Which algorithm to use for modifying how colors are rendered with darkmode.
+    Which algorithm to use for modifying how colors are rendered with dark mode.
 
     The `lightness-cielab` value was added with QtWebEngine 5.14 and is treated
     like `lightness-hsl` with older QtWebEngine versions.
   type:
     name: String
     valid_values:
       - lightness-cielab: Modify colors by converting them to CIELAB color
```

### Comparing `qutebrowser-3.1.0/qutebrowser/config/configexc.py` & `qutebrowser-3.2.0/qutebrowser/config/configexc.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/config/configfiles.py` & `qutebrowser-3.2.0/qutebrowser/config/configfiles.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/config/configinit.py` & `qutebrowser-3.2.0/qutebrowser/config/configinit.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Initialization of the configuration."""
 
 import argparse
 import os.path
 import sys
+from typing import Optional
 
 from qutebrowser.qt.widgets import QMessageBox
 
 from qutebrowser.api import config as configapi
 from qutebrowser.config import (config, configdata, configfiles, configtypes,
                                 configexc, configcommands, stylesheet, qtargs)
 from qutebrowser.utils import objreg, usertypes, log, standarddir, message
 from qutebrowser.config import configcache
 from qutebrowser.misc import msgbox, objects, savemanager
 
 
 # Error which happened during init, so we can show a message box.
-_init_errors = None
+_init_errors: Optional[configexc.ConfigFileErrors] = None
 
 
 def early_init(args: argparse.Namespace) -> None:
     """Initialize the part of the config which works without a QApplication."""
     configdata.init()
 
     yaml_config = configfiles.YamlConfig()
```

### Comparing `qutebrowser-3.1.0/qutebrowser/config/configtypes.py` & `qutebrowser-3.2.0/qutebrowser/config/configtypes.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/config/configutils.py` & `qutebrowser-3.2.0/qutebrowser/config/configutils.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/config/qtargs.py` & `qutebrowser-3.2.0/qutebrowser/config/qtargs.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/config/stylesheet.py` & `qutebrowser-3.2.0/qutebrowser/config/stylesheet.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/config/websettings.py` & `qutebrowser-3.2.0/qutebrowser/config/websettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,15 @@
     """Clear cookies, cache and related data for private browsing sessions."""
     if objects.backend == usertypes.Backend.QtWebEngine:
         from qutebrowser.browser.webengine import webenginesettings
         webenginesettings.init_private_profile()
     elif objects.backend == usertypes.Backend.QtWebKit:
         from qutebrowser.browser.webkit import cookies
         assert cookies.ram_cookie_jar is not None
-        cookies.ram_cookie_jar.setAllCookies([])  # type: ignore[unreachable]
+        cookies.ram_cookie_jar.setAllCookies([])
     else:
         raise utils.Unreachable(objects.backend)
 
 
 @pyqtSlot()
 def shutdown() -> None:
     """Shut down QWeb(Engine)Settings."""
```

### Comparing `qutebrowser-3.1.0/qutebrowser/extensions/interceptors.py` & `qutebrowser-3.2.0/qutebrowser/extensions/interceptors.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/extensions/loader.py` & `qutebrowser-3.2.0/qutebrowser/extensions/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from qutebrowser import components
 from qutebrowser.config import config
 from qutebrowser.utils import log, standarddir
 from qutebrowser.misc import objects
 
 
 # ModuleInfo objects for all loaded plugins
-_module_infos = []
+_module_infos: List["ModuleInfo"] = []
 
 InitHookType = Callable[['InitContext'], None]
 ConfigChangedHookType = Callable[[], None]
 
 
 @dataclasses.dataclass
 class InitContext:
```

### Comparing `qutebrowser-3.1.0/qutebrowser/html/back.html` & `qutebrowser-3.2.0/qutebrowser/html/back.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/base.html` & `qutebrowser-3.2.0/qutebrowser/html/base.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/bindings.html` & `qutebrowser-3.2.0/qutebrowser/html/bindings.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/bookmarks.html` & `qutebrowser-3.2.0/qutebrowser/html/bookmarks.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/dirbrowser.html` & `qutebrowser-3.2.0/qutebrowser/html/dirbrowser.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/changelog.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/changelog.html`

 * *Files 0% similar despite different names*

#### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/changelog.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/changelog.html`

```diff
@@ -807,14 +807,144 @@
               , though minor
 breaking changes (such as renamed commands) can happen in minor releases.
             </p>
           </div>
         </div>
       </div>
       <div class="sect1">
+        <h2 id="v3.2.0">v3.2.0 (2024-06-03)</h2>
+        <div class="sectionbody">
+          <div class="sect2">
+            <h3 id="_deprecated">Deprecated</h3>
+            <div class="ulist">
+              <ul>
+                <li>
+                  <p>This will be the last feature release supporting macOS 11 Big Sur.
+  Starting with qutebrowser v3.3.0, macOS 12 Monterey will be the oldest
+  supported version.</p>
+                </li>
+              </ul>
+            </div>
+          </div>
+          <div class="sect2">
+            <h3 id="_added">Added</h3>
+            <div class="ulist">
+              <ul>
+                <li>
+                  <p>
+                    When qutebrowser receives a SIGHUP it will now reload any config.py file
+  in use (same as the
+                    <code>:config-source</code>
+                    command does). (#8108)
+                  </p>
+                </li>
+                <li>
+                  <p>
+                    The Chromium security patch version is now shown in the backend string in
+                    <code>--version</code>
+                    and
+                    <code>:version</code>
+                    . This reflects the latest Chromium version that
+  security fixes have been backported to the base QtWebEngine version from.
+  (#7187)
+                  </p>
+                </li>
+              </ul>
+            </div>
+          </div>
+          <div class="sect2">
+            <h3 id="_changed">Changed</h3>
+            <div class="ulist">
+              <ul>
+                <li>
+                  <p>Windows and macOS releases now ship with Qt 6.7.1, which is based on Chromium
+  118.0.5993.220 with security patches up to 124.0.6367.202.</p>
+                </li>
+                <li>
+                  <p>
+                    With QtWebEngine 6.7+, the
+                    <code>colors.webpage.darkmode.enabled</code>
+                    setting can now
+  be changed at runtime and supports URL patterns (#8182).
+                  </p>
+                </li>
+                <li>
+                  <p>
+                    A few more completions will now match search terms in any order:
+                    <code>:quickmark-*</code>
+                    ,
+                    <code>:bookmark-*</code>
+                    ,
+                    <code>:tab-take</code>
+                    and
+                    <code>:tab-select</code>
+                    (for the quick
+  and bookmark categories). (#7955)
+                  </p>
+                </li>
+                <li>
+                  <p>
+                    Elements with an ARIA
+                    <code>role=&quot;switch&quot;</code>
+                    now get hints (toggle switches like
+  e.g. on cookie banners).
+                  </p>
+                </li>
+                <li>
+                  <p>
+                    The
+                    <code>tor_identity</code>
+                    userscript now validates that the -c|--control-port
+  argument value is an int. (#8162)
+                  </p>
+                </li>
+              </ul>
+            </div>
+          </div>
+          <div class="sect2">
+            <h3 id="_fixed">Fixed</h3>
+            <div class="ulist">
+              <ul>
+                <li>
+                  <p>
+                    <code>input.insert_mode.auto_load</code>
+                    sometimes not triggering due to a race
+  condition. (#8145)
+                  </p>
+                </li>
+                <li>
+                  <p>Worked around qutebrowser quitting when closing a KDE file dialog due to a Qt
+  bug. (#8143)</p>
+                </li>
+                <li>
+                  <p>Trying to use qutebrowser after it’s been deleted/moved on disk (e.g. after a
+  Python upgrade) should now not crash anymore.</p>
+                </li>
+                <li>
+                  <p>When the QtWebEngine resources dir couldn’t be found, qutebrowser now doesn’t
+  crash anymore (but QtWebEngine still might).</p>
+                </li>
+                <li>
+                  <p>Fixed a rare crash in the completion widget when there was no selection model
+  when we went to clear that, probably when leaving a mode. (#7901)</p>
+                </li>
+                <li>
+                  <p>Worked around a minor issue around QTimers on Windows where the IPC server
+  could close the socket early. (#8191)</p>
+                </li>
+                <li>
+                  <p>The latest PDF.js release (v4.2.67) is now supported when backed by
+  QtWebEngine 6.6+ (#8170)</p>
+                </li>
+              </ul>
+            </div>
+          </div>
+        </div>
+      </div>
+      <div class="sect1">
         <h2 id="v3.1.0">v3.1.0 (2023-12-08)</h2>
         <div class="sectionbody">
           <div class="sect2">
             <h3 id="_removed">Removed</h3>
             <div class="ulist">
               <ul>
                 <li>
@@ -828,15 +958,15 @@
                     got removed, following removals in Chromium.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_added">Added</h3>
+            <h3 id="_added_2">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     New
                     <code>smart-simple</code>
                     value for
@@ -854,15 +984,15 @@
   disabled by default, following a Chromium change.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed">Changed</h3>
+            <h3 id="_changed_2">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Upgraded the bundled Qt version to 6.6.1, based on Chromium 112. Note
   this is only relevant for the macOS/Windows releases, on Linux those will be
   upgraded via your distribution packages.</p>
                 </li>
@@ -887,15 +1017,15 @@
   and supports URL patterns.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed">Fixed</h3>
+            <h3 id="_fixed_2">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Some web pages jumping to the top when the statusbar is hidden or (with
   v3.0.x) when a prompt is hidden.</p>
                 </li>
                 <li>
@@ -934,15 +1064,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v3.0.2">v3.0.2 (2023-10-19)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_2">Fixed</h3>
+            <h3 id="_fixed_3">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Upgraded the bundled Qt version to 6.5.3. Note this is only relevant for the
   macOS/Windows releases, on Linux those will be upgraded via your distribution
   packages. This Qt patch release comes with
@@ -981,15 +1111,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v3.0.1">v3.0.1 (2023-10-19)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_3">Fixed</h3>
+            <h3 id="_fixed_4">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The &quot;restore video&quot; functionality of the
                     <code>view_in_mpv</code>
                     script works again on
@@ -1202,15 +1332,15 @@
   macOS (&lt; 11)/Windows (&lt; 10) versions were dropped. See the &quot;Removed&quot; section
   below for details.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_added_2">Added</h3>
+            <h3 id="_added_3">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>On invalid commands/settings with a similarly spelled match, qutebrowser now
   suggests the correct name in its error messages.</p>
                 </li>
                 <li>
@@ -1456,15 +1586,15 @@
                 <li>
                   <p>Support for 32-bit Windows is now dropped.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_2">Changed</h3>
+            <h3 id="_changed_3">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The qutebrowser icons got moved from
                     <code>icons/</code>
                     to
@@ -1754,15 +1884,15 @@
   a future release.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_4">Fixed</h3>
+            <h3 id="_fixed_5">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     When the devtools are clicked but
                     <code>input.insert_mode.auto_enter</code>
                     is set to
@@ -1882,15 +2012,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v2.5.4">v2.5.4 (2023-03-13)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_5">Fixed</h3>
+            <h3 id="_fixed_6">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Support SQLite with DQS (double quoted string) compile time option turned
   off.</p>
                 </li>
               </ul>
@@ -1898,15 +2028,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v2.5.3">v2.5.3 (2023-02-17)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_3">Added</h3>
+            <h3 id="_added_4">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     New
                     <code>array_at</code>
                     quirk, polyfilling the
@@ -1918,15 +2048,15 @@
   which is needed by various websites, but only natively available with Qt 6.2.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_6">Fixed</h3>
+            <h3 id="_fixed_7">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Crash when the adblock filter file can’t be read.</p>
                 </li>
                 <li>
                   <p>
@@ -1988,15 +2118,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v2.5.2">v2.5.2 (2022-06-22)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_7">Fixed</h3>
+            <h3 id="_fixed_8">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Packaging-related fixes:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -2058,15 +2188,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v2.5.1">v2.5.1 (2022-05-26)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_8">Fixed</h3>
+            <h3 id="_fixed_9">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The
                     <code>qute-pass</code>
                     userscript is marked as executable again.
@@ -2160,15 +2290,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v2.5.0">v2.5.0 (2022-04-01)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_deprecated">Deprecated</h3>
+            <h3 id="_deprecated_2">Deprecated</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     v2.5.x will be the last release of qutebrowser 2.
                     <strong>For the upcoming 3.0.0 release</strong>
                     , it’s planned to drop support for various
@@ -2227,15 +2357,15 @@
   OS path separator and ignoring spaces) instead.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_3">Changed</h3>
+            <h3 id="_changed_4">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Improved message if a spawned process wasn’t found and a Flatpak container is
   in use.</p>
                 </li>
                 <li>
@@ -2434,15 +2564,15 @@
                     by default.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_added_4">Added</h3>
+            <h3 id="_added_5">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     New
                     <code>input.match_counts</code>
                     option which allows to turn off count matching for
@@ -2515,15 +2645,15 @@
   filename prompt now.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_9">Fixed</h3>
+            <h3 id="_fixed_10">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     When
                     <code>search.incremental</code>
                     is disabled, searching using
@@ -2685,15 +2815,15 @@
                     for details.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_added_5">Added</h3>
+            <h3 id="_added_6">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     New
                     <code>content.blocking.hosts.block_subdomains</code>
                     setting which can be used to
@@ -2723,15 +2853,15 @@
                     .
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_10">Fixed</h3>
+            <h3 id="_fixed_11">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Switching tabs via mouse wheel scrolling now works properly on macOS. Set
                     <code>tabs.mousewheel_switching</code>
                     to false if you prefer the previous behavior.
@@ -2741,15 +2871,15 @@
                   <p>Speculative fix for a crash when closing qutebrowser while a systray
   notification is shown.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_4">Changed</h3>
+            <h3 id="_changed_5">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Typing in the filename prompt now filters matching directories.</p>
                 </li>
                 <li>
                   <p>
@@ -2822,15 +2952,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v2.3.1">v2.3.1 (2021-07-28)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_11">Fixed</h3>
+            <h3 id="_fixed_12">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Updated the workaround for Google Account log in claiming that this browser
   isn’t secure. For an equivalent workaround on older versions, run:
                     <code>:set -u https://accounts.google.com/* content.headers.user_agent &quot;Mozilla/5.0 ({os_info}; rv:90.0) Gecko/20100101 Firefox/90.0&quot;</code>
@@ -2859,15 +2989,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v2.3.0">v2.3.0 (2021-06-28)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_6">Added</h3>
+            <h3 id="_added_7">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     New
                     <code>content.prefers_reduced_motion</code>
                     setting to request websites to reduce
@@ -2882,15 +3012,15 @@
   selected items in filename prompts.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_5">Changed</h3>
+            <h3 id="_changed_6">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The hosts-based adblocker (using
                     <code>content.blocking.hosts.lists</code>
                     ) now also
@@ -2925,15 +3055,15 @@
                     points to).
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_12">Fixed</h3>
+            <h3 id="_fixed_13">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Crash on macOS 10.14+ when logging into Google accounts — the previous fix
   was incomplete due wrong information in Apple’s documentation.</p>
                 </li>
                 <li>
@@ -2957,15 +3087,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v2.2.3">v2.2.3 (2021-06-01)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_13">Fixed</h3>
+            <h3 id="_fixed_14">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Logging into Google accounts or sharing the camera on macOS 10.14+ crashed,
   which is now fixed.</p>
                 </li>
                 <li>
@@ -3056,15 +3186,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v2.2.2">v2.2.2 (2021-05-20)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_14">Fixed</h3>
+            <h3 id="_fixed_15">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>When awesomewm’s &quot;naughty&quot; notification daemon was used with a development
   version of AwesomeWM and an unknown version number, qutebrowser would crash
   when trying to parse the version string. This is now fixed.</p>
                 </li>
@@ -3099,30 +3229,30 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v2.2.1">v2.2.1 (2021-04-29)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_changed_6">Changed</h3>
+            <h3 id="_changed_7">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>When an error occurs in a notification presenter, qutebrowser now shows that
   error in the statusbar instead of just logging it.</p>
                 </li>
                 <li>
                   <p>New site-specific-quirk for Discord logging users out when using vertical
   tabs (yes, really)</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_15">Fixed</h3>
+            <h3 id="_fixed_16">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Certain errors from notification daemons are now displayed as non-fatal
   errors instead of qutebrowser crashing:</p>
                   <div class="ulist">
                     <ul>
@@ -3193,15 +3323,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v2.2.0">v2.2.0 (2021-04-13)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_deprecated_2">Deprecated</h3>
+            <h3 id="_deprecated_3">Deprecated</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Running qutebrowser with Qt 5.12.0 is now unsupported and logs a warning. It
   should still work - however, a workaround for issues with the Nvidia graphic
   driver was dropped. Newer Qt 5.12.x versions are still fully supported.</p>
                 </li>
@@ -3225,15 +3355,15 @@
                     instead.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_added_7">Added</h3>
+            <h3 id="_added_8">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     New dependency on the
                     <code>QtDBus</code>
                     module. If this requirement is an issue for you
@@ -3358,15 +3488,15 @@
   from).
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_7">Changed</h3>
+            <h3 id="_changed_8">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The
                     <code>content.ssl_strict</code>
                     setting got renamed to
@@ -3573,15 +3703,15 @@
                     .
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_16">Fixed</h3>
+            <h3 id="_fixed_17">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>When an editor exits with a != 0 exit status, the temporary editor file is now
   persisted. This already was the case when the editor crashed.</p>
                 </li>
                 <li>
@@ -3640,15 +3770,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v2.1.1">v2.1.1 (2021-04-01)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_8">Added</h3>
+            <h3 id="_added_9">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Site-specific quirk for krunker.io, which shows a &quot;Socket Error&quot; with
   qutebrowser’s default Accept-Language header. The workaround is equivalent to
   doing
@@ -3656,30 +3786,30 @@
                     .
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_8">Changed</h3>
+            <h3 id="_changed_9">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Clicking the
                     <em>x</em>
                     in the devtools window to hide it now also leaves insert
   mode.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_17">Fixed</h3>
+            <h3 id="_fixed_18">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>The workaround for black on (almost) black formula images in dark mode now
   also works with Qt 5.12 and 5.13.</p>
                 </li>
                 <li>
@@ -3875,15 +4005,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_added_9">Added</h3>
+            <h3 id="_added_10">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     New
                     <code>:screenshot</code>
                     command which can be used to screenshot the visible part of
@@ -3906,15 +4036,15 @@
                     userscript integrating with the KeePassXC browser API.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_9">Changed</h3>
+            <h3 id="_changed_10">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Initial support for QtWebEngine 5.15.3 and PyQt 5.15.3/.4</p>
                 </li>
                 <li>
                   <p>
@@ -4033,15 +4163,15 @@
   a user stylesheet.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_18">Fixed</h3>
+            <h3 id="_fixed_19">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     With QtWebEngine 5.15.3 and some locales, Chromium can’t start its
   subprocesses. As a result, qutebrowser only shows a blank page and logs
   &quot;Network service crashed, restarting service.&quot;.  This release adds a
@@ -4165,15 +4295,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v2.0.2">v2.0.2 (2021-02-04)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_19">Fixed</h3>
+            <h3 id="_fixed_20">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>When right-clicking an empty part of the downloads bar, qutebrowser v2.0.x
   would crash. This is now fixed.</p>
                 </li>
                 <li>
@@ -4307,15 +4437,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v2.0.1">v2.0.1 (2021-01-28)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_20">Fixed</h3>
+            <h3 id="_fixed_21">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     If qutebrowser was installed as a Python egg (similar to a .zip file, via
                     <code>setup.py install</code>
                     under certain conditions), a change in v2.0.0 caused it to
@@ -4344,15 +4474,15 @@
   restart of qutebrowser is shown instead.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_10">Changed</h3>
+            <h3 id="_changed_11">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The
                     <code>format_json</code>
                     userscript now uses sh instead of bash again.
@@ -4571,15 +4701,15 @@
                     ) is now removed.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_deprecated_3">Deprecated</h3>
+            <h3 id="_deprecated_4">Deprecated</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Several commands have been renamed for consistency and/or easier grouping of
   related commands. Their old names are still available, but deprecated and will
   be removed in qutebrowser v2.1.0.</p>
                   <div class="ulist">
@@ -4664,15 +4794,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_added_10">Added</h3>
+            <h3 id="_added_11">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>New settings for the ABP-based adblocker:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -4837,15 +4967,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_11">Changed</h3>
+            <h3 id="_changed_12">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     <code>config.py</code>
                     files now are required to have either
                     <code>config.load_autoconfig(False)</code>
@@ -5236,15 +5366,15 @@
                 <li>
                   <p>Various performance improvements, including for the startup time.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_21">Fixed</h3>
+            <h3 id="_fixed_22">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     With interpolated color settings (
                     <code>colors.tabs.indicator.*</code>
                     and
@@ -5356,15 +5486,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.14.1">v1.14.1 (2020-12-04)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_11">Added</h3>
+            <h3 id="_added_12">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     With v1.14.0, qutebrowser configures the main window to be transparent, so
   that it’s possible to configure a translucent tab- or statusbar. However, that
   change introduced various issues, such as performance degradation on some
@@ -5379,15 +5509,15 @@
                     to restore the behavior of v1.14.0.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_12">Changed</h3>
+            <h3 id="_changed_13">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Windows and macOS releases now ship Qt 5.15.2, which is based on
   Chromium 83.0.4103.122 with security fixes up to 86.0.4240.183. This includes
   CVE-2020-15999 in the bundled freetype library, which is known to be exploited
   in the wild. It also includes various other bugfixes/features compared to
@@ -5438,15 +5568,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_22">Fixed</h3>
+            <h3 id="_fixed_23">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Setting the
                     <code>content.headers.referer</code>
                     setting to
@@ -5667,15 +5797,15 @@
             <p>Furthermore, this release still only contains partial session support for QtWebEngine
 5.15. It’s still recommended to run against Qt 5.15 due to the security patches
 contained in it — for most users, the added workarounds seem to work out fine. A
 rewritten session support will be part of qutebrowser v2.0.0, tentatively planned for the
 end of the year or early 2021.</p>
           </div>
           <div class="sect2">
-            <h3 id="_changed_13">Changed</h3>
+            <h3 id="_changed_14">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The
                     <code>content.media_capture</code>
                     setting got split up into three more fine-grained
@@ -5876,15 +6006,15 @@
                     userscript now supports hint userscript mode.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_added_12">Added</h3>
+            <h3 id="_added_13">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     New argument
                     <code>strip</code>
                     for
@@ -5994,15 +6124,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_23">Fixed</h3>
+            <h3 id="_fixed_24">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     A URL pattern with a
                     <code>*.</code>
                     host was considered valid and matched all hosts.
@@ -6183,15 +6313,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.13.1">v1.13.1 (2020-07-17)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_24">Fixed</h3>
+            <h3 id="_fixed_25">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     With Qt 5.14, shared workers are now disabled. This works around a crash in
   QtWebEngine on certain sites (like the Epic Games Store or the Unreal Engine
   page). On older versions, you can get the same effect by doing
@@ -6283,15 +6413,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.13.0">v1.13.0 (2020-06-26)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_deprecated_4">Deprecated</h3>
+            <h3 id="_deprecated_5">Deprecated</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The
                     <code>:inspector</code>
                     command is deprecated and has been replaced by a new
@@ -6327,15 +6457,15 @@
                     should be used instead.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_14">Changed</h3>
+            <h3 id="_changed_15">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Changes to commands:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -6493,15 +6623,15 @@
                 <li>
                   <p>Small performance improvements.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_added_13">Added</h3>
+            <h3 id="_added_14">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>New settings:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -6600,15 +6730,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_25">Fixed</h3>
+            <h3 id="_fixed_26">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Crash when
                     <code>tabs.focus_stack_size</code>
                     is set to -1.
@@ -6737,15 +6867,15 @@
                     instead.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_added_14">Added</h3>
+            <h3 id="_added_15">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     New
                     <code>:debug-keytester</code>
                     command, which shows a &quot;key tester&quot; widget.
@@ -6797,15 +6927,15 @@
   a restart of qutebrowser.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_15">Changed</h3>
+            <h3 id="_changed_16">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Windows and macOS releases now ship Qt 5.15, which is based on Chromium
   80.0.3987.163 with security fixes up to 81.0.4044.138.</p>
                 </li>
                 <li>
@@ -6845,15 +6975,15 @@
                     now detaches a tab into a new private window.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_26">Fixed</h3>
+            <h3 id="_fixed_27">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Using
                     <code>:open -s</code>
                     now only rewrites
@@ -6945,15 +7075,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.11.0">v1.11.0 (2020-04-27)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_15">Added</h3>
+            <h3 id="_added_16">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>New settings:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -7031,15 +7161,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_16">Changed</h3>
+            <h3 id="_changed_17">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>First adaptions to Qt 5.15, including a stop-gap measure for session loading
   not working properly with it.</p>
                 </li>
                 <li>
@@ -7137,26 +7267,26 @@
                 <li>
                   <p>Minor performance improvements.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_deprecated_5">Deprecated</h3>
+            <h3 id="_deprecated_6">Deprecated</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>A warning about old Qt versions is now also shown with Qt 5.9 and 5.10, as
   support for Qt &lt; 5.11 will be dropped in qutebrowser v2.0.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_27">Fixed</h3>
+            <h3 id="_fixed_28">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     <code>unsafeWindow</code>
                     is now defined for Greasemonkey scripts with QtWebKit.
                   </p>
@@ -7213,26 +7343,26 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.10.2">v1.10.2 (2020-04-17)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_changed_17">Changed</h3>
+            <h3 id="_changed_18">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Windows and macOS releases now bundle Qt 5.14.2, including security fixes up
   to Chromium 80.0.3987.132.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_28">Fixed</h3>
+            <h3 id="_fixed_29">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>The WhatsApp workaround now also works when using WhatsApp in languages other
   than English.</p>
                 </li>
                 <li>
@@ -7247,15 +7377,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.10.1">v1.10.1 (2020-02-15)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_29">Fixed</h3>
+            <h3 id="_fixed_30">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Crash when saving data fails during shutdown (which was a regression
   introduced in v1.9.0).</p>
                 </li>
                 <li>
@@ -7278,15 +7408,15 @@
   displayed.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_18">Changed</h3>
+            <h3 id="_changed_19">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     When the Qt version changes (and also on the first start of v1.10.1 on Qt
   5.14), service workers registered by websites are now deleted. This is done
   as a workaround for QtWebEngine issues causing crashes when visiting pages
@@ -7327,15 +7457,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.10.0">v1.10.0 (2020-02-02)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_16">Added</h3>
+            <h3 id="_added_17">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     New
                     <code>colors.webpage.prefers_color_scheme_dark</code>
                     setting which allows forcing
@@ -7352,15 +7482,15 @@
   for all UI fonts.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_19">Changed</h3>
+            <h3 id="_changed_20">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The
                     <code>fonts.monospace</code>
                     setting has been removed and replaced by
@@ -7463,15 +7593,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_30">Fixed</h3>
+            <h3 id="_fixed_31">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>When quitting qutebrowser, components are now cleaned up differently. This
   should fix certain (rare) segmentation faults and exceptions when quitting,
   especially with the new exit scheme introduced in in PyQt5 5.13.1.</p>
                 </li>
@@ -7496,15 +7626,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.9.0">v1.9.0 (2020-01-08)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_17">Added</h3>
+            <h3 id="_added_18">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Initial support for Qt 5.14.</p>
                 </li>
                 <li>
                   <p>
@@ -7563,15 +7693,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_20">Changed</h3>
+            <h3 id="_changed_21">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>The macOS binaries now require macOS 10.13 High Sierra or newer. Support for
   macOS 10.12 Sierra has been dropped.</p>
                 </li>
                 <li>
@@ -7750,15 +7880,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_31">Fixed</h3>
+            <h3 id="_fixed_32">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Downloads (e.g. via
                     <code>:download</code>
                     ) now see the same user agent header as
@@ -7890,15 +8020,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.8.3">v1.8.3 (2019-12-05)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_32">Fixed</h3>
+            <h3 id="_fixed_33">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Segmentation fault introduced in v1.8.2 when a tab gets closed immediately
   after it has finished loading (e.g. with certain login flows).</p>
                 </li>
               </ul>
@@ -7906,27 +8036,27 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.8.2">v1.8.2 (2019-11-22)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_changed_21">Changed</h3>
+            <h3 id="_changed_22">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Windows/macOS releases now ship with Qt 5.12.6. This includes security fixes
   up to Chromium 77.0.3865.120 plus a security fix for CVE-2019-13720 from
   Chromium 78.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_33">Fixed</h3>
+            <h3 id="_fixed_34">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Unbinding keys via
                     <code>config.bind(key, None)</code>
                     accidentally worked in
@@ -7988,15 +8118,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.8.1">v1.8.1 (2019-09-27)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_changed_22">Changed</h3>
+            <h3 id="_changed_23">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>No code changes - this release only repackages the Windows/macOS
   releases due to issues with the v1.8.0 release.</p>
                 </li>
                 <li>
@@ -8019,15 +8149,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.8.0">v1.8.0 (2019-09-25)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_18">Added</h3>
+            <h3 id="_added_19">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>New userscripts:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -8045,15 +8175,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_23">Changed</h3>
+            <h3 id="_changed_24">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>The statusbar text for passthrough mode now shows all configured bindings to
   leave the mode, not only one.</p>
                 </li>
                 <li>
@@ -8150,15 +8280,15 @@
                     for details.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_34">Fixed</h3>
+            <h3 id="_fixed_35">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     <code>:config-write-py</code>
                     now correctly writes
                     <code>config.unbind(...)</code>
@@ -8240,15 +8370,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.7.0">v1.7.0 (2019-07-18)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_19">Added</h3>
+            <h3 id="_added_20">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>New settings:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -8373,15 +8503,15 @@
                 <li>
                   <p>Qt 5.13: Support for notifications (shown via system tray).</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_24">Changed</h3>
+            <h3 id="_changed_25">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Updated dependencies for Windows/macOS releases:</p>
                 </li>
                 <li>
                   <p>PyQt5 5.12.3 / PyQtWebEngine 5.12.1</p>
@@ -8565,15 +8695,15 @@
                   <p>Various performance improvements (e.g. for showing hints or the :open
   completion).</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_deprecated_6">Deprecated</h3>
+            <h3 id="_deprecated_7">Deprecated</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     <code>:yank markdown</code>
                     got deprecated, as
                     <code>:yank inline [{title}]({url})</code>
@@ -8581,15 +8711,15 @@
   be used instead.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_35">Fixed</h3>
+            <h3 id="_fixed_36">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Various QtWebEngine load signals are now handled differently, which should
   fix issues with insert mode being left while typing on sites like Google
   Translate.</p>
                 </li>
@@ -8653,15 +8783,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.6.3">v1.6.3 (2019-06-18)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_36">Fixed</h3>
+            <h3 id="_fixed_37">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Crash when hinting and changing/closing the tab before hints are displayed.</p>
                 </li>
                 <li>
                   <p>Crash on redirects with Qt 5.13.</p>
@@ -8687,26 +8817,26 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.6.2">v1.6.2 (2019-05-06)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_changed_25">Changed</h3>
+            <h3 id="_changed_26">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Windows/macOS releases now ship with Qt 5.12.3, which includes security fixes
   up to Chromium 73.0.3683.75.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_37">Fixed</h3>
+            <h3 id="_fixed_38">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Crash when SQL errors occur while using the completion.</p>
                 </li>
                 <li>
                   <p>Crash when cancelling a download prompt started in an already closed window.</p>
@@ -8728,27 +8858,27 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.6.1">v1.6.1 (2019-03-20)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_changed_26">Changed</h3>
+            <h3 id="_changed_27">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Windows/macOS releases now ship with Qt 5.12.2, which includes
   security fixes up to Chromium 72.0.3626.121 (including CVE-2019-5786
   which is known to be exploited in the wild).</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_38">Fixed</h3>
+            <h3 id="_fixed_39">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Crash when using
                     <code>:config-{dict,list}-{add,remove}</code>
                     with an invalid setting.
@@ -8780,15 +8910,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.6.0">v1.6.0 (2019-02-25)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_20">Added</h3>
+            <h3 id="_added_21">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>New settings:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -8881,15 +9011,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_27">Changed</h3>
+            <h3 id="_changed_28">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Various changes to the Windows and macOS builds:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -9029,15 +9159,15 @@
                   <p>Combining Qt 5.12 with an older PyQt can lead to issues, so a warning is
   now shown when starting qutebrowser with that combination.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_39">Fixed</h3>
+            <h3 id="_fixed_40">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Invalid world IDs now get rejected for
                     <code>:jseval</code>
                     and GreaseMonkey scripts.
@@ -9155,15 +9285,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.5.2">v1.5.2 (2018-10-26)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_changed_28">Changed</h3>
+            <h3 id="_changed_29">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The
                     <code>content.cookies.accept</code>
                     setting is now set to
@@ -9181,15 +9311,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.5.1">v1.5.1 (2018-10-10)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_40">Fixed</h3>
+            <h3 id="_fixed_41">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Flickering when opening/closing tabs (as soon as more than 10 are open) on
   some pages.</p>
                 </li>
                 <li>
@@ -9217,15 +9347,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.5.0">v1.5.0 (2018-10-03)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_21">Added</h3>
+            <h3 id="_added_22">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Rewritten PDF.js support:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -9333,15 +9463,15 @@
                     .
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_29">Changed</h3>
+            <h3 id="_changed_30">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Windows and macOS releases now bundle Python 3.7, PyQt 5.11.3 and Qt 5.11.2.
   QtWebEngine includes security fixes up to Chromium 68.0.3440.75 and
                     <a href="https://code.qt.io/cgit/qt/qtwebengine.git/tree/dist/changes-5.11.2/?h=v5.11.2">various other fixes</a>
@@ -9518,15 +9648,15 @@
                     now clears the URL query.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_41">Fixed</h3>
+            <h3 id="_fixed_42">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     <code>qute://</code>
                     pages now work properly on Qt 5.11.2
                   </p>
@@ -9598,15 +9728,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.4.2">v1.4.2 (2018-09-02)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_changed_30">Changed</h3>
+            <h3 id="_changed_31">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The
                     <code>content.xss_auditing</code>
                     setting is now enabled by default, to mirror
@@ -9617,15 +9747,15 @@
                   <p>Long URLs in the statusbar are now elided at the end rather than in the
   middle, to make sure the hostname is completely visible whenever possible.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_42">Fixed</h3>
+            <h3 id="_fixed_43">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Crash in Qt 5.7.1 when a website uses
                     <code>window.print()</code>
                     .
@@ -9706,15 +9836,15 @@
                     <a href="https://github.com/qutebrowser/qutebrowser/issues/4060">https://github.com/qutebrowser/qutebrowser/issues/4060</a>
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_43">Fixed</h3>
+            <h3 id="_fixed_44">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Rare crash when an error occurs in downloads.</p>
                 </li>
                 <li>
                   <p>Newlines are now stripped from the :version pastebin URL.</p>
@@ -9754,15 +9884,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.4.0">v1.4.0 (2018-07-03)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_22">Added</h3>
+            <h3 id="_added_23">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Support for the bundled
                     <code>sip</code>
                     module in PyQt 5.11 and other changes in
@@ -9917,15 +10047,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_31">Changed</h3>
+            <h3 id="_changed_32">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>The following settings now support URL patterns:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -10130,15 +10260,15 @@
                   <p>Greasemonkey scripts now support a &quot;@qute-js-world&quot; tag to run them in a
   different JavaScript context.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_44">Fixed</h3>
+            <h3 id="_fixed_45">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Various subtle keyboard focus issues.</p>
                 </li>
                 <li>
                   <p>
@@ -10211,15 +10341,15 @@
                     .
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_45">Fixed</h3>
+            <h3 id="_fixed_46">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Crash in a workaround for a Qt 5.11 bug in rare circumstances.</p>
                 </li>
                 <li>
                   <p>Workaround for a Qt bug which preserves searches between page loads.</p>
@@ -10238,15 +10368,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.3.2">v1.3.2 (2018-06-10)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_46">Fixed</h3>
+            <h3 id="_fixed_47">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>QtWebEngine: Improved workaround for a bug in Qt 5.11 where only the
   top/bottom half of the window is used.</p>
                 </li>
                 <li>
@@ -10271,15 +10401,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.3.1">v1.3.1 (2018-05-29)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_47">Fixed</h3>
+            <h3 id="_fixed_48">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Work around a bug in Qt 5.11 where only the top/bottom half of the window is used.
   This workaround is incomplete, but fixes the majority of the cases where this happens.</p>
                 </li>
                 <li>
@@ -10300,15 +10430,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.3.0">v1.3.0 (2018-05-03)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_23">Added</h3>
+            <h3 id="_added_24">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     New
                     <code>:scroll-to-anchor</code>
                     command to scroll to an anchor in the document.
@@ -10348,15 +10478,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_32">Changed</h3>
+            <h3 id="_changed_33">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     QtWebEngine: Support for JavaScript Shared Web Workers have been disabled on
   Qt versions older than 5.11 because of security issues in in Chromium.
   You can get the same effect in earlier versions via
@@ -10430,15 +10560,15 @@
   to debug instead of messages.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_48">Fixed</h3>
+            <h3 id="_fixed_49">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Using hints before a page is fully loaded is now possible again.</p>
                 </li>
                 <li>
                   <p>Selecting hints with the number keypad now works again.</p>
@@ -10564,15 +10694,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.2.1">v1.2.1 (2018-03-14)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_49">Fixed</h3>
+            <h3 id="_fixed_50">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>qutebrowser now starts properly when the PyQt5 QOpenGLFunctions package wasn’t
   found.</p>
                 </li>
                 <li>
@@ -10624,15 +10754,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.2.0">v1.2.0 (2018-03-09)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_24">Added</h3>
+            <h3 id="_added_25">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Initial implementation of per-domain settings:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -10845,15 +10975,15 @@
                     to cycle through inputs.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_33">Changed</h3>
+            <h3 id="_changed_34">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Complete refactoring of key input handling, with various effects:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -11013,15 +11143,15 @@
                     .
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_50">Fixed</h3>
+            <h3 id="_fixed_51">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>QtWebEngine bugfixes:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -11193,26 +11323,26 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.1.2">v1.1.2 (2018-03-01)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_changed_34">Changed</h3>
+            <h3 id="_changed_35">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Windows/macOS releases now bundle Qt 5.10.1 which includes security fixes from
   Chromium up to version 64.0.3282.140.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_51">Fixed</h3>
+            <h3 id="_fixed_52">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>QtWebEngine: Crash with Qt 5.10.1 when using :undo on some tabs.</p>
                 </li>
                 <li>
                   <p>Compatibility with Python 3.7</p>
@@ -11222,15 +11352,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.1.1">v1.1.1 (2018-01-20)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_52">Fixed</h3>
+            <h3 id="_fixed_53">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>The Makefile now actually works.</p>
                 </li>
                 <li>
                   <p>Fixed crashes with Qt 5.10 when closing a tab before it finished loading.</p>
@@ -11240,15 +11370,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.1.0">v1.1.0 (2018-01-15)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_25">Added</h3>
+            <h3 id="_added_26">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Initial support for Greasemonkey scripts. There are still some rough edges,
   but many scripts should already work.</p>
                 </li>
                 <li>
@@ -11490,15 +11620,15 @@
                     script to import history from Firefox/Chromium.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_35">Changed</h3>
+            <h3 id="_changed_36">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Some settings got renamed:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -11669,15 +11799,15 @@
   different colors for the three completion columns.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_53">Fixed</h3>
+            <h3 id="_fixed_54">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>More consistent sizing for favicons with vertical tabs.</p>
                 </li>
                 <li>
                   <p>
@@ -11778,15 +11908,15 @@
                 <li>
                   <p>Fixed a crash when clicking certain form elements with QtWebEngine.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_deprecated_7">Deprecated</h3>
+            <h3 id="_deprecated_8">Deprecated</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     <code>:tab-detach</code>
                     has been deprecated, as
                     <code>:tab-give</code>
@@ -11844,15 +11974,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.0.4">v1.0.4 (2017-11-28)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_54">Fixed</h3>
+            <h3 id="_fixed_55">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The
                     <code>qute://gpl</code>
                     page now works correctly again.
@@ -11882,15 +12012,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.0.3">v1.0.3 (2017-11-04)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_changed_36">Changed</h3>
+            <h3 id="_changed_37">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>macOS and Windows builds are now built with PyQt 5.9.1 and Qt 5.9.2, including
   various bugfixes, as well as security fixes from Chromium up to version
   61.0.3163.79.</p>
                 </li>
@@ -11901,15 +12031,15 @@
                   <p>The :open-editor command is now not hidden anymore as it’s also usable in
   normal mode.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_55">Fixed</h3>
+            <h3 id="_fixed_56">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Handle accessing a locked sqlite database gracefully</p>
                 </li>
                 <li>
                   <p>Abort pinned tab dialogs properly when a tab is closed e.g. by closing a
@@ -11926,15 +12056,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.0.2">v1.0.2 (2017-10-17)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_56">Fixed</h3>
+            <h3 id="_fixed_57">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Fix workaround for black screens or crashes with Nvidia cards</p>
                 </li>
                 <li>
                   <p>Handle a filesystem going read-only gracefully</p>
@@ -11963,30 +12093,30 @@
                     in the completion
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_37">Changed</h3>
+            <h3 id="_changed_38">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Nicer error messages and other minor improvements</p>
                 </li>
               </ul>
             </div>
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v1.0.1">v1.0.1 (2017-10-13)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_57">Fixed</h3>
+            <h3 id="_fixed_58">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Fixed starting after customizing
                     <code>fonts.tabs</code>
                     or
@@ -12100,15 +12230,15 @@
                     .
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_added_26">Added</h3>
+            <h3 id="_added_27">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     QtWebEngine: Spell checking support, see the
                     <code>spellcheck.languages</code>
                     setting.
@@ -12204,15 +12334,15 @@
                 <li>
                   <p>QtWebEngine: Support for proxy authentication.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_38">Changed</h3>
+            <h3 id="_changed_39">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Using
                     <code>:download</code>
                     now uses the page’s title as filename.
@@ -12385,15 +12515,15 @@
                     if QtWebEngine is used.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_added_27">Added</h3>
+            <h3 id="_added_28">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Private browsing is now implemented for QtWebEngine,
                     <strong>and changed its
   behavior</strong>
@@ -12502,15 +12632,15 @@
                   <p>(QtWebEngine) Proxy support with Qt 5.7.1 (already was supported for 5.8 and
   newer)</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_39">Changed</h3>
+            <h3 id="_changed_40">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     To prevent elaborate phishing attacks, the Punycode version (
                     <code>xn--*</code>
                     ) is now
@@ -12667,15 +12797,15 @@
                 <li>
                   <p>(QtWebKit) PAC now supports SOCKS5 as type.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_58">Fixed</h3>
+            <h3 id="_fixed_59">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>The macOS .dmg is now built against Qt 5.9 which fixes various
   important issues (such as not being able to type dead keys).</p>
                 </li>
                 <li>
@@ -12718,15 +12848,15 @@
                 </li>
                 <li>
                   <p>The tabbar and completion should now be more consistently and correctly
   styled with various system styles.</p>
                 </li>
                 <li>
                   <p>
-                    Applying styiles in
+                    Applying styles in
                     <code>qt5ct</code>
                     now shouldn’t crash anymore.
                   </p>
                 </li>
                 <li>
                   <p>The validation for colors in stylesheets is now less strict,
   allowing for all valid Qt values.</p>
@@ -12801,30 +12931,30 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.10.1">v0.10.1 (2017-03-08)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_changed_40">Changed</h3>
+            <h3 id="_changed_41">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     <code>--qt-arg</code>
                     and
                     <code>--qt-flag</code>
                     can now also be used to pass arguments to Chromium when using QtWebEngine.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_59">Fixed</h3>
+            <h3 id="_fixed_60">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>URLs are now redacted properly (username/password, and path/query for HTTPS) when using Proxy Autoconfig with QtWebKit</p>
                 </li>
                 <li>
                   <p>Crash when updating adblock lists with invalid UTF8-chars in them</p>
@@ -12855,15 +12985,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.10.0">v0.10.0 (2017-02-25)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_28">Added</h3>
+            <h3 id="_added_29">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Userscripts now have a new
                     <code>$QUTE_COMMANDLINE_TEXT</code>
                     environment variable, containing the current commandline contents
@@ -12962,15 +13092,15 @@
                 <li>
                   <p>macOS builds are back, and built with QtWebEngine</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_41">Changed</h3>
+            <h3 id="_changed_42">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>PyQt 5.7/Qt 5.7.1 is now required for the QtWebEngine backend</p>
                 </li>
                 <li>
                   <p>Scrolling with the scrollwheel while holding shift now scrolls sideways</p>
@@ -13063,15 +13193,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_60">Fixed</h3>
+            <h3 id="_fixed_61">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Various bugs with Qt 5.8 and QtWebEngine:</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -13178,15 +13308,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.9.1">v0.9.1 (2017-01-13)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_61">Fixed</h3>
+            <h3 id="_fixed_62">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Prevent websites from downloading files to a location outside of the download
   folder with QtWebEngine.</p>
                 </li>
               </ul>
@@ -13194,15 +13324,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.9.0">v0.9.0 (2016-12-28)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_29">Added</h3>
+            <h3 id="_added_30">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     <strong>New dependency:</strong>
                     qutebrowser now depends on the Qt QML module, which is
    packaged separately in some distributions (as Qt Declarative/QML/Quick).
@@ -13394,15 +13524,15 @@
                 <li>
                   <p>Support for PAC (proxy autoconfig) with QtWebKit</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_42">Changed</h3>
+            <h3 id="_changed_43">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Hints are now drawn natively in Qt instead of using web elements. This has a
   few implications for users:</p>
                   <div class="ulist">
                     <ul>
@@ -13875,15 +14005,15 @@
                     given.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_deprecated_8">Deprecated</h3>
+            <h3 id="_deprecated_9">Deprecated</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The
                     <code>:paste</code>
                     command got deprecated as
@@ -14000,15 +14130,15 @@
                     should be sufficient.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_62">Fixed</h3>
+            <h3 id="_fixed_63">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     <code>:undo</code>
                     now doesn’t undo tabs &quot;closed&quot; by
                     <code>:tab-detach</code>
@@ -14049,15 +14179,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.8.3">v0.8.3 (2016-11-05)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_63">Fixed</h3>
+            <h3 id="_fixed_64">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Fixed crash when doing
                     <code>:&lt;space&gt;&lt;enter&gt;</code>
                     , another corner-case introduced in v0.8.0
@@ -14122,15 +14252,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.8.2">v0.8.2 (2016-08-02)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_64">Fixed</h3>
+            <h3 id="_fixed_65">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Fixed
                     <code>general -&gt; private-browsing</code>
                     not being set correctly until a restart
@@ -14212,15 +14342,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.8.1">v0.8.1 (2016-07-27)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_65">Fixed</h3>
+            <h3 id="_fixed_66">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Fix crash when pressing enter without a command</p>
                 </li>
                 <li>
                   <p>Adjust error message to point out QtWebEngine is unsupported with the OS
@@ -14234,15 +14364,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.8.0">v0.8.0 (2016-07-26)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_30">Added</h3>
+            <h3 id="_added_31">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     New
                     <code>:repeat-command</code>
                     command (mapped to
@@ -14321,15 +14451,15 @@
   PDF without a dialog.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_43">Changed</h3>
+            <h3 id="_changed_44">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     <code>:scroll-perc</code>
                     now prefers a count over the argument given to it, which means
                     <code>gg</code>
@@ -14373,15 +14503,15 @@
   is given.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_66">Fixed</h3>
+            <h3 id="_fixed_67">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Compatibility with PyQt 5.7</p>
                 </li>
                 <li>
                   <p>Fixed some configuration values being lost when a config option gets removed
@@ -14437,15 +14567,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.7.0">v0.7.0 (2016-06-10)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_31">Added</h3>
+            <h3 id="_added_32">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     New
                     <code>:edit-url</code>
                     command to edit the URL in an external editor.
@@ -14549,15 +14679,15 @@
                     to hint text input fields.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_44">Changed</h3>
+            <h3 id="_changed_45">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>qutebrowser got a new (slightly updated) logo</p>
                 </li>
                 <li>
                   <p>
@@ -14674,15 +14804,15 @@
                     suffix to the timestamp field.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_67">Fixed</h3>
+            <h3 id="_fixed_68">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Fixed using
                     <code>:hint links spawn</code>
                     with flags - you can now use things like the
@@ -14780,15 +14910,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.6.2">v0.6.2 (2016-04-30)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_68">Fixed</h3>
+            <h3 id="_fixed_69">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Fixed crash when using
                     <code>:tab-{prev,next,focus}</code>
                     right after closing the last
@@ -14825,15 +14955,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.6.1">v0.6.1 (2016-04-10)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_69">Fixed</h3>
+            <h3 id="_fixed_70">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Fixed broken cheatsheet image which was missing from package</p>
                 </li>
                 <li>
                   <p>Fixed occasional crash when switching/disconnecting monitors</p>
@@ -14853,15 +14983,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.6.0">v0.6.0 (2016-04-04)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_32">Added</h3>
+            <h3 id="_added_33">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     New
                     <code>:buffer</code>
                     command to easily switch tabs by name. This is not bound to a
@@ -14938,15 +15068,15 @@
                     )
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_45">Changed</h3>
+            <h3 id="_changed_46">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Pasting multiple lines via
                     <code>:paste</code>
                     now opens each line in a new tab.
@@ -15013,15 +15143,15 @@
                     ).
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_70">Fixed</h3>
+            <h3 id="_fixed_71">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Fixed starting with -c &quot;&quot;.</p>
                 </li>
                 <li>
                   <p>Fixed crash when a tab is closed twice via javascript (e.g. Dropbox
@@ -15120,15 +15250,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.5.1">v0.5.1 (2016-01-18)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_71">Fixed</h3>
+            <h3 id="_fixed_72">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Fixed completion for various config values when using
                     <code>:set</code>
                     .
@@ -15146,15 +15276,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.5.0">v0.5.0 (2016-01-05)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_33">Added</h3>
+            <h3 id="_added_34">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Ability to preview PDFs using pdf.js in the browser if it’s installed. This
   is disabled by default and can be enabled using the
                     <code>content -&gt; pdfjs-enabled</code>
@@ -15352,15 +15482,15 @@
                     to change the alignment of tab titles.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_46">Changed</h3>
+            <h3 id="_changed_47">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The
                     <code>colors -&gt; tabs.bg/fg.selected</code>
                     option got split into
@@ -15483,15 +15613,15 @@
                 <li>
                   <p>A search engine name can now contain any non-space character, like dashes.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_deprecated_9">Deprecated</h3>
+            <h3 id="_deprecated_10">Deprecated</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     <code>:download-remove --all</code>
                     is now deprecated and
                     <code>:download-clear</code>
@@ -15552,15 +15682,15 @@
                     command (deprecated in v0.2.0)
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_72">Fixed</h3>
+            <h3 id="_fixed_73">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Fixed retrying of downloads which were started in a now closed tab.</p>
                 </li>
                 <li>
                   <p>
@@ -15647,15 +15777,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.4.1">v0.4.1 (2015-09-30)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_73">Fixed</h3>
+            <h3 id="_fixed_74">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Adjusted AppArmor config for the IPC changes in v0.4.0.</p>
                 </li>
                 <li>
                   <p>Fixed atime update frequency for IPC file.</p>
@@ -15699,15 +15829,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.4.0">v0.4.0 (2015-09-11)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_34">Added</h3>
+            <h3 id="_added_35">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>New bookmark functionality (similar to quickmarks without a name).</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -15812,15 +15942,15 @@
                     is now supported.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_47">Changed</h3>
+            <h3 id="_changed_48">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Some developer scripts got moved to
                     <code>scripts/dev/</code>
                   </p>
@@ -15898,15 +16028,15 @@
                 <li>
                   <p>Better support for Qt 5.5 and Python 3.5.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_74">Fixed</h3>
+            <h3 id="_fixed_75">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Fixed a bug where cookies were saved despite qutebrowser being started in
   private browsing mode.</p>
                 </li>
                 <li>
@@ -16016,15 +16146,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.3.0">v0.3.0 (2015-06-28)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_35">Added</h3>
+            <h3 id="_added_36">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     New commands
                     <code>:message-info</code>
                     ,
@@ -16216,15 +16346,15 @@
                 <li>
                   <p>Support for Qt 5.5 and tox 2.0</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_48">Changed</h3>
+            <h3 id="_changed_49">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     <strong>Breaking change for userscripts:</strong>
                     <code>QUTE_HTML</code>
                     and
@@ -16350,15 +16480,15 @@
                 <li>
                   <p>Sessions now store zoom/scroll-position separately for each entry.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_deprecated_10">Deprecated</h3>
+            <h3 id="_deprecated_11">Deprecated</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     <code>:scroll</code>
                     with two pixel-arguments is now deprecated -
                     <code>:scroll-px</code>
@@ -16384,15 +16514,15 @@
                 <li>
                   <p>Support for Qt installations without SSL support was dropped.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_75">Fixed</h3>
+            <h3 id="_fixed_76">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Scrolling should now work more reliably on some pages where arrow keys worked but
                     <code>hjkl</code>
                     didn’t.
@@ -16463,30 +16593,30 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.2.1">v0.2.1 (2015-04-19)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_fixed_76">Fixed</h3>
+            <h3 id="_fixed_77">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Added missing manpage (doc/qutebrowser.1.asciidoc) to archive.</p>
                 </li>
               </ul>
             </div>
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.2.0">v0.2.0 (2015-04-19)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_36">Added</h3>
+            <h3 id="_added_37">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Session support</p>
                   <div class="ulist">
                     <ul>
                       <li>
@@ -16952,15 +17082,15 @@
                     option.
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_changed_49">Changed</h3>
+            <h3 id="_changed_50">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Ignore quotes with maxsplit-commands (
                     <code>:open</code>
                     ,
@@ -17181,15 +17311,15 @@
                     </ul>
                   </div>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_deprecated_11">Deprecated</h3>
+            <h3 id="_deprecated_12">Deprecated</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The
                     <code>:run-userscript</code>
                     command - use
@@ -17249,15 +17379,15 @@
                     instead..
                   </p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_77">Fixed</h3>
+            <h3 id="_fixed_78">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Fix for cache never being used.</p>
                 </li>
                 <li>
                   <p>Fixed handling of key release events (e.g. for javascript) when holding a key and pressing a second one.</p>
@@ -17336,15 +17466,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.1.4">v0.1.4 (2015-03-19)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_changed_50">Changed</h3>
+            <h3 id="_changed_51">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     The Windows builds come with Qt 5.4.1 which has some
                     <a href="https://listi.jpberlin.de/pipermail/qutebrowser/2015-March/000054.html">related bugfixes</a>
                     .
@@ -17395,15 +17525,15 @@
                 <li>
                   <p>Remove debug console completing completely.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_78">Fixed</h3>
+            <h3 id="_fixed_79">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Ignore RuntimeError in
                     <code>mouserelease_insertmode</code>
                     .
@@ -17478,15 +17608,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.1.3">v0.1.3 (2015-02-12)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_changed_51">Changed</h3>
+            <h3 id="_changed_52">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Various small logging improvements.</p>
                 </li>
                 <li>
                   <p>
@@ -17502,15 +17632,15 @@
                 <li>
                   <p>Hide adblocked iframes.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_79">Fixed</h3>
+            <h3 id="_fixed_80">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Handle shutdown of page with prompt correctly.</p>
                 </li>
                 <li>
                   <p>fuzzy_url: handle invalid URLs with autosearch off</p>
@@ -17590,15 +17720,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.1.2">v0.1.2 (2015-01-09)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_changed_52">Changed</h3>
+            <h3 id="_changed_53">Changed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Uncheck sending of debug log by default when private browsing is on.</p>
                 </li>
                 <li>
                   <p>Add SSL info to version info.</p>
@@ -17613,15 +17743,15 @@
                 <li>
                   <p>Remove hosts-file.net from blocker default lists.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_80">Fixed</h3>
+            <h3 id="_fixed_81">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Fix rare exception when a key is pressed shortly after opening a window</p>
                 </li>
                 <li>
                   <p>
@@ -17684,15 +17814,15 @@
           </div>
         </div>
       </div>
       <div class="sect1">
         <h2 id="v0.1.1">v0.1.1 (2014-12-28)</h2>
         <div class="sectionbody">
           <div class="sect2">
-            <h3 id="_added_37">Added</h3>
+            <h3 id="_added_38">Added</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>Set window icon and add a qutebrowser.ico file for Windows.</p>
                 </li>
                 <li>
                   <p>Ask the user when downloading to an already existing file.</p>
@@ -17773,15 +17903,15 @@
                 <li>
                   <p>Clean up and temporarily disable alias completion.</p>
                 </li>
               </ul>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_fixed_81">Fixed</h3>
+            <h3 id="_fixed_82">Fixed</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>
                     Fix setting of
                     <code>QWebSettings</code>
                     (e.g. web fonts) with empty strings.
@@ -17912,11 +18042,11 @@
       </div>
     </div>
     <div id="footnotes">
       <hr/>
     </div>
     <div id="footer">
       <div id="footer-text">Last updated
- 2023-12-08 15:32:03 UTC</div>
+ 2024-06-03 14:43:21 UTC</div>
     </div>
   </body>
 </html>
```

### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/commands.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/commands.html`

 * *Files 0% similar despite different names*

#### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/commands.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/commands.html`

```diff
@@ -10254,11 +10254,11 @@
       </div>
     </div>
     <div id="footnotes">
       <hr/>
     </div>
     <div id="footer">
       <div id="footer-text">Last updated
- 2023-12-08 15:32:11 UTC</div>
+ 2024-06-03 14:43:27 UTC</div>
     </div>
   </body>
 </html>
```

### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/configuring.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/configuring.html`

 * *Files 0% similar despite different names*

#### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/configuring.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/configuring.html`

```diff
@@ -2226,11 +2226,11 @@
       </div>
     </div>
     <div id="footnotes">
       <hr/>
     </div>
     <div id="footer">
       <div id="footer-text">Last updated
- 2023-12-08 15:32:09 UTC</div>
+ 2024-06-03 14:43:25 UTC</div>
     </div>
   </body>
 </html>
```

### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/contributing.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/contributing.html`

 * *Files 0% similar despite different names*

#### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/contributing.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/contributing.html`

```diff
@@ -3140,11 +3140,11 @@
       </div>
     </div>
     <div id="footnotes">
       <hr/>
     </div>
     <div id="footer">
       <div id="footer-text">Last updated
- 2023-12-08 15:32:05 UTC</div>
+ 2024-06-03 14:43:23 UTC</div>
     </div>
   </body>
 </html>
```

### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/faq.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/faq.html`

 * *Files 0% similar despite different names*

#### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/faq.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/faq.html`

```diff
@@ -1737,15 +1737,15 @@
 for long enough, you can get some qutebrowser stickers!
             </p>
           </div>
           <div class="dlist">
             <dl>
               <dt class="hdlist1">Why GitHub Sponsors?</dt>
               <dd>
-                <p>GitHub Sponsors is a crowdfundign platform nicely integrated with
+                <p>GitHub Sponsors is a crowdfunding platform nicely integrated with
     qutebrowser’s existing GitHub page and a better offering than alternatives such
     as Patreon or Liberapay.</p>
                 <div class="paragraph">
                   <p>
                     It also offers a
                     <a href="https://help.github.com/en/github/supporting-the-open-source-community-with-github-sponsors/about-github-sponsors#about-the-github-sponsors-matching-fund">Matching Fund</a>
                     which matches all donations until a cap of $5000, which has already been
@@ -1993,11 +1993,11 @@
       </div>
     </div>
     <div id="footnotes">
       <hr/>
     </div>
     <div id="footer">
       <div id="footer-text">Last updated
- 2023-12-08 15:32:03 UTC</div>
+ 2024-06-03 14:43:21 UTC</div>
     </div>
   </body>
 </html>
```

### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/img/cheatsheet-big.png` & `qutebrowser-3.2.0/qutebrowser/html/doc/img/cheatsheet-big.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/img/cheatsheet-small.png` & `qutebrowser-3.2.0/qutebrowser/html/doc/img/cheatsheet-small.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/index.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/index.html`

 * *Files 1% similar despite different names*

#### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/index.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/index.html`

```diff
@@ -1004,11 +1004,11 @@
       </div>
     </div>
     <div id="footnotes">
       <hr/>
     </div>
     <div id="footer">
       <div id="footer-text">Last updated
- 2023-12-08 15:32:07 UTC</div>
+ 2024-06-03 14:43:25 UTC</div>
     </div>
   </body>
 </html>
```

### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/install.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/install.html`

 * *Files 1% similar despite different names*

#### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/install.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/install.html`

```diff
@@ -1347,17 +1347,15 @@
                   <td class="content">Due to GitHub limitations, you need to be signed in with a GitHub account
 to download the files.</td>
                 </tr>
               </table>
             </div>
           </div>
           <div class="sect2">
-            <h3 id="_a_href_https_chocolatey_org_packages_qutebrowser_chocolatey_package_a">
-              <a href="https://chocolatey.org/packages/qutebrowser">Chocolatey package</a>
-            </h3>
+            <h3 id="_package_managers">Package managers</h3>
             <div class="ulist">
               <ul>
                 <li>
                   <p>PackageManagement PowerShell module</p>
                 </li>
               </ul>
             </div>
@@ -1367,15 +1365,20 @@
                   <code>PS C:\&gt; Install-Package qutebrowser</code>
                 </pre>
               </div>
             </div>
             <div class="ulist">
               <ul>
                 <li>
-                  <p>Chocolatey’s client</p>
+                  <p>
+                    <a href="https://chocolatey.org/packages/qutebrowser">Chocolatey package</a>
+                    with
+                    <code>choco</code>
+                    :
+                  </p>
                 </li>
               </ul>
             </div>
             <div class="listingblock">
               <div class="content">
                 <pre>
                   <code>C:\&gt; choco install qutebrowser</code>
@@ -1803,11 +1806,11 @@
       </div>
     </div>
     <div id="footnotes">
       <hr/>
     </div>
     <div id="footer">
       <div id="footer-text">Last updated
- 2023-12-08 15:32:06 UTC</div>
+ 2024-06-03 14:43:25 UTC</div>
     </div>
   </body>
 </html>
```

### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/quickstart.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/quickstart.html`

 * *Files 1% similar despite different names*

#### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/quickstart.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/quickstart.html`

```diff
@@ -1089,11 +1089,11 @@
       </div>
     </div>
     <div id="footnotes">
       <hr/>
     </div>
     <div id="footer">
       <div id="footer-text">Last updated
- 2023-12-08 15:32:06 UTC</div>
+ 2024-06-03 14:43:24 UTC</div>
     </div>
   </body>
 </html>
```

### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/settings.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/settings.html`

 * *Files 0% similar despite different names*

#### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/settings.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/settings.html`

```diff
@@ -1868,15 +1868,15 @@
                 <tr>
                   <td align="left" valign="top">
                     <p class="table">
                       <a href="#colors.webpage.darkmode.algorithm">colors.webpage.darkmode.algorithm</a>
                     </p>
                   </td>
                   <td align="left" valign="top">
-                    <p class="table">Which algorithm to use for modifying how colors are rendered with darkmode.</p>
+                    <p class="table">Which algorithm to use for modifying how colors are rendered with dark mode.</p>
                   </td>
                 </tr>
                 <tr>
                   <td align="left" valign="top">
                     <p class="table">
                       <a href="#colors.webpage.darkmode.contrast">colors.webpage.darkmode.contrast</a>
                     </p>
@@ -8931,15 +8931,15 @@
               </p>
             </div>
           </div>
           <div class="sect2">
             <h3 id="colors.webpage.darkmode.algorithm">colors.webpage.darkmode.algorithm</h3>
             <div class="paragraph">
               <p>
-                Which algorithm to use for modifying how colors are rendered with darkmode.
+                Which algorithm to use for modifying how colors are rendered with dark mode.
 The
                 <code>lightness-cielab</code>
                 value was added with QtWebEngine 5.14 and is treated like
                 <code>lightness-hsl</code>
                 with older QtWebEngine versions.
               </p>
             </div>
@@ -9021,14 +9021,15 @@
             </div>
           </div>
           <div class="sect2">
             <h3 id="colors.webpage.darkmode.enabled">colors.webpage.darkmode.enabled</h3>
             <div class="paragraph">
               <p>
                 Render all web contents using a dark theme.
+On QtWebEngine &lt; 6.7, this setting requires a restart and does not support URL patterns, only the global setting is applied.
 Example configurations from Chromium’s
                 <code>chrome://flags</code>
                 :
 - &quot;With simple HSL/CIELAB/RGB-based inversion&quot;: Set
                 <code>colors.webpage.darkmode.algorithm</code>
                 accordingly, and
   set
@@ -9042,15 +9043,19 @@
               <ul>
                 <li>
                   <p>&quot;With selective image inversion&quot;: qutebrowser default settings.</p>
                 </li>
               </ul>
             </div>
             <div class="paragraph">
-              <p>This setting requires a restart.</p>
+              <p>
+                This setting supports
+                <a href="configuring.html#patterns">URL patterns</a>
+                .
+              </p>
             </div>
             <div class="paragraph">
               <p>This setting is only available with the QtWebEngine backend.</p>
             </div>
             <div class="paragraph">
               <p>
                 Type:
@@ -13853,14 +13858,19 @@
                       <li>
                         <p>
                           <code>[role=&quot;checkbox&quot;]</code>
                         </p>
                       </li>
                       <li>
                         <p>
+                          <code>[role=&quot;switch&quot;]</code>
+                        </p>
+                      </li>
+                      <li>
+                        <p>
                           <code>[role=&quot;menuitem&quot;]</code>
                         </p>
                       </li>
                       <li>
                         <p>
                           <code>[role=&quot;menuitemcheckbox&quot;]</code>
                         </p>
@@ -18342,11 +18352,11 @@
       </div>
     </div>
     <div id="footnotes">
       <hr/>
     </div>
     <div id="footer">
       <div id="footer-text">Last updated
- 2023-12-08 15:32:07 UTC</div>
+ 2024-06-03 14:43:28 UTC</div>
     </div>
   </body>
 </html>
```

### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/stacktrace.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/stacktrace.html`

 * *Files 0% similar despite different names*

#### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/stacktrace.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/stacktrace.html`

```diff
@@ -1170,11 +1170,11 @@
       </div>
     </div>
     <div id="footnotes">
       <hr/>
     </div>
     <div id="footer">
       <div id="footer-text">Last updated
- 2023-12-08 15:32:06 UTC</div>
+ 2024-06-03 14:43:25 UTC</div>
     </div>
   </body>
 </html>
```

### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/userscripts.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/userscripts.html`

 * *Files 1% similar despite different names*

#### Comparing `qutebrowser-3.1.0/qutebrowser/html/doc/userscripts.html` & `qutebrowser-3.2.0/qutebrowser/html/doc/userscripts.html`

```diff
@@ -1139,11 +1139,11 @@
       </div>
     </div>
     <div id="footnotes">
       <hr/>
     </div>
     <div id="footer">
       <div id="footer-text">Last updated
- 2023-12-08 15:32:06 UTC</div>
+ 2024-06-03 14:43:24 UTC</div>
     </div>
   </body>
 </html>
```

### Comparing `qutebrowser-3.1.0/qutebrowser/html/error.html` & `qutebrowser-3.2.0/qutebrowser/html/error.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/history.html` & `qutebrowser-3.2.0/qutebrowser/html/history.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/license.html` & `qutebrowser-3.2.0/qutebrowser/html/license.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/log.html` & `qutebrowser-3.2.0/qutebrowser/html/log.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/no_pdfjs.html` & `qutebrowser-3.2.0/qutebrowser/html/no_pdfjs.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/process.html` & `qutebrowser-3.2.0/qutebrowser/html/process.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/settings.html` & `qutebrowser-3.2.0/qutebrowser/html/settings.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/startpage.html` & `qutebrowser-3.2.0/qutebrowser/html/startpage.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/styled.html` & `qutebrowser-3.2.0/qutebrowser/html/styled.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/tabs.html` & `qutebrowser-3.2.0/qutebrowser/html/tabs.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/version.html` & `qutebrowser-3.2.0/qutebrowser/html/version.html`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 {% block style %}
 html { margin-left: 10px; }
 {% endblock %}
 
 {% block content %}
 {{ super() }}
 <h1>Version info</h1>
-<pre>{{ version }}</pre>
 <button onclick="paste_version()">Yank pastebin URL for version info</button>
+<pre>{{ version }}</pre>
 
 <h1>Copyright info</h1>
 <p>{{ copyright }}</p>
 <p>
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 {% extends "base.html" %} {% block script %} function paste_version() { const
 xhr = new XMLHttpRequest(); xhr.open("GET", "qute://pastebin-version");
 xhr.send(); } {% endblock %} {% block style %} html { margin-left: 10px; } {%
 endblock %} {% block content %} {{ super() }}
 ************ VVeerrssiioonn iinnffoo ************
-{{ version }}
 Yank pastebin URL for version info
+{{ version }}
 ************ CCooppyyrriigghhtt iinnffoo ************
 {{ copyright }}
 This program is free software: you can redistribute it and/or modify it under
 the terms of the GNU General Public License as published by the Free Software
 Foundation, either version 3 of the License, or (at your option) any later
 version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `qutebrowser-3.1.0/qutebrowser/html/warning-qt5.html` & `qutebrowser-3.2.0/qutebrowser/html/warning-qt5.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/warning-sessions.html` & `qutebrowser-3.2.0/qutebrowser/html/warning-sessions.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/html/warning-webkit.html` & `qutebrowser-3.2.0/qutebrowser/html/warning-webkit.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-128x128.png` & `qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-128x128.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-16x16.png` & `qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-16x16.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-24x24.png` & `qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-24x24.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-256x256.png` & `qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-256x256.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-32x32.png` & `qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-32x32.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-48x48.png` & `qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-48x48.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-512x512.png` & `qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-512x512.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-64x64.png` & `qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-64x64.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-96x96.png` & `qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-96x96.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-all.svg` & `qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-all.svg`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/icons/qutebrowser-favicon.svg` & `qutebrowser-3.2.0/qutebrowser/icons/qutebrowser-favicon.svg`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/icons/qutebrowser.icns` & `qutebrowser-3.2.0/qutebrowser/icons/qutebrowser.icns`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/icons/qutebrowser.ico` & `qutebrowser-3.2.0/qutebrowser/icons/qutebrowser.ico`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/icons/qutebrowser.svg` & `qutebrowser-3.2.0/qutebrowser/icons/qutebrowser.svg`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/icons/qutebrowser.xpm` & `qutebrowser-3.2.0/qutebrowser/icons/qutebrowser.xpm`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/img/broken_qutebrowser_logo.png` & `qutebrowser-3.2.0/qutebrowser/img/broken_qutebrowser_logo.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/img/file.svg` & `qutebrowser-3.2.0/qutebrowser/img/file.svg`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/img/folder.svg` & `qutebrowser-3.2.0/qutebrowser/img/folder.svg`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/javascript/caret.js` & `qutebrowser-3.2.0/qutebrowser/javascript/caret.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -733,14 +733,20 @@
     /**
      * Whether we're running on Windows.
      * @type {boolean}
      */
     CaretBrowsing.isWindows = null;
 
     /**
+     * Whether we should log debug outputs.
+     * @type {boolean}
+     */
+    CaretBrowsing.isDebug = null;
+
+    /**
      * The id returned by window.setInterval for our stopAnimation function, so
      * we can cancel it when we call stopAnimation again.
      * @type {number?}
      */
     CaretBrowsing.animationFunctionId = null;
 
     /**
@@ -1143,14 +1149,16 @@
 
     CaretBrowsing.move = function(direction, granularity, count = 1) {
         let action = "move";
         if (CaretBrowsing.selectionState !== CaretBrowsing.SelectionState.NONE) {
             action = "extend";
         }
 
+        CaretBrowsing.debug(`(move) ${action} ${count} ${granularity} ${direction}, selection ${CaretBrowsing.selectionState}`);
+
         for (let i = 0; i < count; i++) {
             if (CaretBrowsing.selectionState === CaretBrowsing.SelectionState.LINE) {
                 CaretBrowsing.updateLineSelection(direction, granularity);
             } else {
                 window.
                 getSelection().
                 modify(action, direction, granularity);
@@ -1173,14 +1181,16 @@
     };
 
     CaretBrowsing.moveToBlock = function(paragraph, boundary, count = 1) {
         let action = "move";
         if (CaretBrowsing.selectionState !== CaretBrowsing.SelectionState.NONE) {
             action = "extend";
         }
+        CaretBrowsing.debug(`(moveToBlock) ${action} paragraph ${paragraph}, boundary ${boundary}, count ${count}, selection ${CaretBrowsing.selectionState}`);
+
         for (let i = 0; i < count; i++) {
             window.
             getSelection().
             modify(action, paragraph, "paragraph");
 
             window.
             getSelection().
@@ -1189,14 +1199,15 @@
             if (CaretBrowsing.selectionState === CaretBrowsing.SelectionState.LINE) {
                 CaretBrowsing.selectLine();
             }
         }
     };
 
     CaretBrowsing.toggle = function(value) {
+        CaretBrowsing.debug(`(toggle) enabled ${CaretBrowsing.isEnabled}, force ${CaretBrowsing.forceEnabled}`);
         if (CaretBrowsing.forceEnabled) {
             CaretBrowsing.recreateCaretElement();
             return;
         }
 
         if (value === undefined) {
             CaretBrowsing.isEnabled = !CaretBrowsing.isEnabled;
@@ -1224,14 +1235,15 @@
     };
 
     /**
      * Update whether or not the caret is visible, based on whether caret browsing
      * is enabled and whether this window / iframe has focus.
      */
     CaretBrowsing.updateIsCaretVisible = function() {
+        CaretBrowsing.debug(`(updateIsCaretVisible) isEnabled ${CaretBrowsing.isEnabled}, isWindowFocused ${CaretBrowsing.isWindowFocused}, isCaretVisible ${CaretBrowsing.isCaretVisible}, caretElement ${CaretBrowsing.caretElement}`);
         CaretBrowsing.isCaretVisible =
             (CaretBrowsing.isEnabled && CaretBrowsing.isWindowFocused);
         if (CaretBrowsing.isCaretVisible && !CaretBrowsing.caretElement) {
             CaretBrowsing.setInitialCursor();
             CaretBrowsing.updateCaretOrSelection(true);
         } else if (!CaretBrowsing.isCaretVisible &&
             CaretBrowsing.caretElement) {
@@ -1267,14 +1279,20 @@
 
             CaretBrowsing.animationFunctionId = window.setTimeout(() => {
                 CaretBrowsing.startAnimation();
             }, 1000);
         }
     };
 
+    CaretBrowsing.debug = (text) => {
+        if (CaretBrowsing.isDebug) {
+            console.debug(`caret: ${text}`);
+        }
+    }
+
     CaretBrowsing.init = function() {
         CaretBrowsing.isWindowFocused = document.hasFocus();
 
         document.addEventListener("click", CaretBrowsing.onClick, false);
         window.addEventListener("focus", CaretBrowsing.onWindowFocus, false);
         window.addEventListener("blur", CaretBrowsing.onWindowBlur, false);
     };
@@ -1306,14 +1324,15 @@
         }
         CaretBrowsing.toggle();
         return CaretBrowsing.selectionState !== CaretBrowsing.SelectionState.NONE;
     };
 
     funcs.setFlags = (flags) => {
         CaretBrowsing.isWindows = flags.includes("windows");
+        CaretBrowsing.isDebug = flags.includes("debug");
     };
 
     funcs.disableCaret = () => {
         CaretBrowsing.toggle(false);
     };
 
     funcs.toggle = () => {
```

### Comparing `qutebrowser-3.1.0/qutebrowser/javascript/greasemonkey_wrapper.js` & `qutebrowser-3.2.0/qutebrowser/javascript/greasemonkey_wrapper.js`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/javascript/history.js` & `qutebrowser-3.2.0/qutebrowser/javascript/history.js`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/javascript/pac_utils.js` & `qutebrowser-3.2.0/qutebrowser/javascript/pac_utils.js`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/javascript/position_caret.js` & `qutebrowser-3.2.0/qutebrowser/javascript/position_caret.js`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/javascript/quirks/array_at.user.js` & `qutebrowser-3.2.0/qutebrowser/javascript/quirks/array_at.user.js`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/javascript/quirks/string_replaceall.user.js` & `qutebrowser-3.2.0/qutebrowser/javascript/quirks/string_replaceall.user.js`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/javascript/scroll.js` & `qutebrowser-3.2.0/qutebrowser/javascript/scroll.js`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/javascript/stylesheet.js` & `qutebrowser-3.2.0/qutebrowser/javascript/stylesheet.js`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/javascript/webelem.js` & `qutebrowser-3.2.0/qutebrowser/javascript/webelem.js`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/keyinput/basekeyparser.py` & `qutebrowser-3.2.0/qutebrowser/keyinput/basekeyparser.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/keyinput/eventfilter.py` & `qutebrowser-3.2.0/qutebrowser/keyinput/eventfilter.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/keyinput/keyutils.py` & `qutebrowser-3.2.0/qutebrowser/keyinput/keyutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from qutebrowser.qt import machinery
 from qutebrowser.qt.core import Qt, QEvent
 from qutebrowser.qt.gui import QKeySequence, QKeyEvent
 if machinery.IS_QT6:
     from qutebrowser.qt.core import QKeyCombination
 else:
-    QKeyCombination = None  # QKeyCombination was added in Qt 6
+    QKeyCombination: None = None  # QKeyCombination was added in Qt 6
 
 from qutebrowser.utils import utils, qtutils, debug
 
 
 class InvalidKeyError(Exception):
 
     """Raised when a key can't be represented by PyQt.
@@ -355,14 +355,16 @@
     def __post_init__(self) -> None:
         """Run some validation on the key/modifier values."""
         # This changed with Qt 6, and e.g. to_qt() relies on this.
         if machinery.IS_QT5:
             modifier_classes = (Qt.KeyboardModifier, Qt.KeyboardModifiers)
         elif machinery.IS_QT6:
             modifier_classes = Qt.KeyboardModifier
+        else:
+            raise utils.Unreachable()
         assert isinstance(self.key, Qt.Key), self.key
         assert isinstance(self.modifiers, modifier_classes), self.modifiers
 
         _assert_plain_key(self.key)
         _assert_plain_modifier(self.modifiers)
 
     def __repr__(self) -> str:
```

### Comparing `qutebrowser-3.1.0/qutebrowser/keyinput/macros.py` & `qutebrowser-3.2.0/qutebrowser/keyinput/macros.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/keyinput/modeman.py` & `qutebrowser-3.2.0/qutebrowser/keyinput/modeman.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/keyinput/modeparsers.py` & `qutebrowser-3.2.0/qutebrowser/keyinput/modeparsers.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/mainwindow.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/mainwindow.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/messageview.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/messageview.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Showing messages above the statusbar."""
 
 from typing import MutableSequence, Optional
 
-from qutebrowser.qt.core import pyqtSlot, pyqtSignal, QTimer, Qt
+from qutebrowser.qt.core import pyqtSlot, pyqtSignal, Qt
 from qutebrowser.qt.widgets import QWidget, QVBoxLayout, QLabel, QSizePolicy
 
 from qutebrowser.config import config, stylesheet
 from qutebrowser.utils import usertypes, message
 
 
 class Message(QLabel):
@@ -97,15 +97,15 @@
         super().__init__(parent)
         self._messages: MutableSequence[Message] = []
         self._vbox = QVBoxLayout(self)
         self._vbox.setContentsMargins(0, 0, 0, 0)
         self._vbox.setSpacing(0)
         self.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Fixed)
 
-        self._clear_timer = QTimer()
+        self._clear_timer = usertypes.Timer()
         self._clear_timer.timeout.connect(self.clear_messages)
         config.instance.changed.connect(self._set_clear_timer_interval)
 
         self._last_info = None
 
     @config.change_filter('messages.timeout')
     def _set_clear_timer_interval(self):
```

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/prompt.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/prompt.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/backforward.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/backforward.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/bar.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/bar.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/clock.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/clock.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # SPDX-FileCopyrightText: Florian Bruhin (The Compiler) <mail@qutebrowser.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Clock displayed in the statusbar."""
 from datetime import datetime
 
-from qutebrowser.qt.core import Qt, QTimer
+from qutebrowser.qt.core import Qt
 
 from qutebrowser.mainwindow.statusbar import textbase
+from qutebrowser.utils import usertypes
 
 
 class Clock(textbase.TextBase):
 
     """Shows current time and date in the statusbar."""
 
     UPDATE_DELAY = 500  # ms
 
     def __init__(self, parent=None):
         super().__init__(parent, elidemode=Qt.TextElideMode.ElideNone)
         self.format = ""
 
-        self.timer = QTimer(self)
+        self.timer = usertypes.Timer(self)
         self.timer.timeout.connect(self._show_time)
 
     def _show_time(self):
         """Set text to current time, using self.format as format-string."""
         self.setText(datetime.now().strftime(self.format))
 
     def hideEvent(self, event):
```

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/command.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/command.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/keystring.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/keystring.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/percentage.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/percentage.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/progress.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/progress.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/searchmatch.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/searchmatch.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/tabindex.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/tabindex.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/textbase.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/textbase.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/statusbar/url.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/statusbar/url.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/tabbedbrowser.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/tabbedbrowser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1007,43 +1007,43 @@
             browsertab.TerminationStatus.killed: "Renderer process was killed",
             browsertab.TerminationStatus.unknown: "Renderer process did not start",
         }
         msg = messages[status] + f" (status {code})"
 
         # WORKAROUND for https://bugreports.qt.io/browse/QTBUG-91715
         versions = version.qtwebengine_versions()
-        is_qtbug_91715 = (
+        if (
             status == browsertab.TerminationStatus.unknown and
             code == 1002 and
-            versions.webengine == utils.VersionNumber(5, 15, 3))
-
-        def show_error_page(html):
-            tab.set_html(html)
-            log.webview.error(msg)
-
-        if is_qtbug_91715:
+            versions.webengine == utils.VersionNumber(5, 15, 3)
+        ):
             log.webview.error(msg)
             log.webview.error('')
             log.webview.error(
                 'NOTE: If you see this and "Network service crashed, restarting '
                 'service.", please see:')
             log.webview.error('https://github.com/qutebrowser/qutebrowser/issues/6235')
             log.webview.error(
                 'You can set the "qt.workarounds.locale" setting in qutebrowser to '
                 'work around the issue.')
             log.webview.error(
                 'A proper fix is likely available in QtWebEngine soon (which is why '
                 'the workaround is disabled by default).')
             log.webview.error('')
-        else:
-            url_string = tab.url(requested=True).toDisplayString()
-            error_page = jinja.render(
-                'error.html', title="Error loading {}".format(url_string),
-                url=url_string, error=msg)
-            QTimer.singleShot(100, lambda: show_error_page(error_page))
+            return
+
+        def show_error_page(html):
+            tab.set_html(html)
+            log.webview.error(msg)
+
+        url_string = tab.url(requested=True).toDisplayString()
+        error_page = jinja.render(
+            'error.html', title="Error loading {}".format(url_string),
+            url=url_string, error=msg)
+        QTimer.singleShot(100, lambda: show_error_page(error_page))
 
     def resizeEvent(self, e):
         """Extend resizeEvent of QWidget to emit a resized signal afterwards.
 
         Args:
             e: The QResizeEvent
         """
```

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/tabwidget.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/tabwidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
     def __init__(self, win_id, parent=None):
         super().__init__(parent)
         self._win_id = win_id
         self._our_style = TabBarStyle()
         self.setStyle(self._our_style)
         self.setFocusPolicy(Qt.FocusPolicy.NoFocus)
         self.vertical = False
-        self._auto_hide_timer = QTimer()
+        self._auto_hide_timer = usertypes.Timer()
         self._auto_hide_timer.setSingleShot(True)
         self._auto_hide_timer.timeout.connect(self.maybe_hide)
         self._on_show_switching_delay_changed()
         self.setAutoFillBackground(True)
         # FIXME:mypy Is it a mypy bug that we need to specify bool here?
         # Otherwise, we get "Cannot determine type of "drag_in_progress" in
         # TabWidget._toggle_visibility below.
```

### Comparing `qutebrowser-3.1.0/qutebrowser/mainwindow/windowundo.py` & `qutebrowser-3.2.0/qutebrowser/mainwindow/windowundo.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/autoupdate.py` & `qutebrowser-3.2.0/qutebrowser/misc/autoupdate.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/backendproblem.py` & `qutebrowser-3.2.0/qutebrowser/misc/backendproblem.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/binparsing.py` & `qutebrowser-3.2.0/qutebrowser/misc/binparsing.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/checkpyver.py` & `qutebrowser-3.2.0/qutebrowser/misc/checkpyver.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/cmdhistory.py` & `qutebrowser-3.2.0/qutebrowser/misc/cmdhistory.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/consolewidget.py` & `qutebrowser-3.2.0/qutebrowser/misc/consolewidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Debugging console."""
 
 import sys
 import code
-from typing import MutableSequence
+from typing import MutableSequence, Optional
 
 from qutebrowser.qt.core import pyqtSignal, pyqtSlot, Qt
 from qutebrowser.qt.widgets import QTextEdit, QWidget, QVBoxLayout, QApplication
 from qutebrowser.qt.gui import QTextCursor
 
 from qutebrowser.config import stylesheet
 from qutebrowser.misc import cmdhistory, miscwidgets
 from qutebrowser.utils import utils, objreg
 
 
-console_widget = None
+console_widget: Optional["ConsoleWidget"] = None
 
 
 class ConsoleLineEdit(miscwidgets.CommandLineEdit):
 
     """A QLineEdit which executes entered code and provides a history.
 
     Attributes:
```

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/crashdialog.py` & `qutebrowser-3.2.0/qutebrowser/misc/crashdialog.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/crashsignal.py` & `qutebrowser-3.2.0/qutebrowser/misc/crashsignal.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 from typing import TYPE_CHECKING, Optional, MutableMapping, cast, List
 
 from qutebrowser.qt.core import (pyqtSlot, qInstallMessageHandler, QObject,
                           QSocketNotifier, QTimer, QUrl)
 from qutebrowser.qt.widgets import QApplication
 
 from qutebrowser.api import cmdutils
+from qutebrowser.config import configfiles, configexc
 from qutebrowser.misc import earlyinit, crashdialog, ipc, objects
-from qutebrowser.utils import usertypes, standarddir, log, objreg, debug, utils
+from qutebrowser.utils import usertypes, standarddir, log, objreg, debug, utils, message
 from qutebrowser.qt import sip
 if TYPE_CHECKING:
     from qutebrowser.misc import quitter
 
 
 @dataclasses.dataclass
 class ExceptionInfo:
@@ -318,27 +319,36 @@
         self._quitter = quitter
         self._notifier = None
         self._timer = usertypes.Timer(self, 'python_hacks')
         self._orig_handlers: MutableMapping[int, 'signal._HANDLER'] = {}
         self._activated = False
         self._orig_wakeup_fd: Optional[int] = None
 
+        self._handlers = {
+            signal.SIGINT: self.interrupt,
+            signal.SIGTERM: self.interrupt,
+        }
+        platform_dependant_handlers = {
+            "SIGHUP": self.reload_config,
+        }
+        for sig_str, handler in platform_dependant_handlers.items():
+            if hasattr(signal.Signals, sig_str):
+                self._handlers[signal.Signals[sig_str]] = handler
+
     def activate(self):
         """Set up signal handlers.
 
         On Windows this uses a QTimer to periodically hand control over to
         Python so it can handle signals.
 
         On Unix, it uses a QSocketNotifier with os.set_wakeup_fd to get
         notified.
         """
-        self._orig_handlers[signal.SIGINT] = signal.signal(
-            signal.SIGINT, self.interrupt)
-        self._orig_handlers[signal.SIGTERM] = signal.signal(
-            signal.SIGTERM, self.interrupt)
+        for sig, handler in self._handlers.items():
+            self._orig_handlers[sig] = signal.signal(sig, handler)
 
         if utils.is_posix and hasattr(signal, 'set_wakeup_fd'):
             # pylint: disable=import-error,no-member,useless-suppression
             import fcntl
             read_fd, write_fd = os.pipe()
             for fd in [read_fd, write_fd]:
                 flags = fcntl.fcntl(fd, fcntl.F_GETFL)
@@ -426,14 +436,23 @@
 
         This doesn't run *any* Qt cleanup and simply exits via Python.
         It will most likely lead to a segfault.
         """
         print("WHY ARE YOU DOING THIS TO ME? :(")
         sys.exit(128 + signum)
 
+    def reload_config(self, _signum, _frame):
+        """Reload the config."""
+        log.signals.info("SIGHUP received, reloading config.")
+        filename = standarddir.config_py()
+        try:
+            configfiles.read_config_py(filename)
+        except configexc.ConfigFileErrors as e:
+            message.error(str(e))
+
 
 def init(q_app: QApplication,
          args: argparse.Namespace,
          quitter: 'quitter.Quitter') -> None:
     """Initialize crash/signal handlers."""
     global crash_handler
     crash_handler = CrashHandler(
```

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/debugcachestats.py` & `qutebrowser-3.2.0/qutebrowser/misc/debugcachestats.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/earlyinit.py` & `qutebrowser-3.2.0/qutebrowser/misc/earlyinit.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/editor.py` & `qutebrowser-3.2.0/qutebrowser/misc/editor.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/elf.py` & `qutebrowser-3.2.0/qutebrowser/misc/elf.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
             )
         except UnicodeDecodeError as e:
             raise binparsing.ParseError(e)
 
     # Here it gets even more crazy: Sometimes, we don't have the full UA in one piece
     # in the string table somehow (?!). However, Qt 6.2 added a separate
     # qWebEngineChromiumVersion(), with PyQt wrappers following later. And *that*
-    # apperently stores the full version in the string table separately from the UA.
+    # apparently stores the full version in the string table separately from the UA.
     # As we clearly didn't have enough crazy heuristics yet so far, let's hunt for it!
 
     # We first get the partial Chromium version from the UA:
     match = re.search(pattern[:-4], data)  # without trailing literal \x00
     if match is None:
         raise binparsing.ParseError("No match in .rodata")
```

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/guiprocess.py` & `qutebrowser-3.2.0/qutebrowser/misc/guiprocess.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/httpclient.py` & `qutebrowser-3.2.0/qutebrowser/misc/httpclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import urllib.parse
 from typing import MutableMapping
 
 from qutebrowser.qt.core import pyqtSignal, QObject, QTimer
 from qutebrowser.qt.network import (QNetworkAccessManager, QNetworkRequest,
                              QNetworkReply)
 
-from qutebrowser.utils import qtlog
+from qutebrowser.utils import qtlog, usertypes
 
 
 class HTTPRequest(QNetworkRequest):
     """A QNetworkRquest that follows (secure) redirects by default."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -81,15 +81,15 @@
         self._handle_reply(reply)
 
     def _handle_reply(self, reply):
         """Handle a new QNetworkReply."""
         if reply.isFinished():
             self.on_reply_finished(reply)
         else:
-            timer = QTimer(self)
+            timer = usertypes.Timer(self)
             timer.setInterval(10000)
             timer.timeout.connect(reply.abort)
             timer.start()
             self._timers[reply] = timer
             reply.finished.connect(functools.partial(
                 self.on_reply_finished, reply))
```

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/ipc.py` & `qutebrowser-3.2.0/qutebrowser/misc/ipc.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 WRITE_TIMEOUT = 1000
 READ_TIMEOUT = 5000
 ATIME_INTERVAL = 5000 * 60  # 5 minutes
 PROTOCOL_VERSION = 1
 
 
 # The ipc server instance
-server = None
+server: Optional["IPCServer"] = None
 
 
 def _get_socketname_windows(basedir):
     """Get a socketname to use for Windows."""
     try:
         username = getpass.getuser()
     except ImportError:
@@ -387,14 +387,19 @@
         if self._socket is not None:
             self._timer.start()
 
     @pyqtSlot()
     def on_timeout(self):
         """Cancel the current connection if it was idle for too long."""
         assert self._socket is not None
+        if not self._timer.check_timeout_validity():
+            # WORKAROUND for https://bugreports.qt.io/browse/QTBUG-124496
+            log.ipc.debug("Ignoring early on_timeout call")
+            return
+
         log.ipc.error("IPC connection timed out "
                       "(socket 0x{:x}).".format(id(self._socket)))
         self._socket.disconnectFromServer()
         if self._socket is not None:  # pragma: no cover
             # on_socket_disconnected sets it to None
             self._socket.waitForDisconnected(CONNECT_TIMEOUT)
         if self._socket is not None:  # pragma: no cover
```

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/keyhintwidget.py` & `qutebrowser-3.2.0/qutebrowser/misc/keyhintwidget.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/lineparser.py` & `qutebrowser-3.2.0/qutebrowser/misc/lineparser.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/miscwidgets.py` & `qutebrowser-3.2.0/qutebrowser/misc/miscwidgets.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/msgbox.py` & `qutebrowser-3.2.0/qutebrowser/misc/msgbox.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/nativeeventfilter.py` & `qutebrowser-3.2.0/qutebrowser/misc/nativeeventfilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from qutebrowser.qt.core import QAbstractNativeEventFilter, QByteArray, qVersion
 
 from qutebrowser.misc import objects
 from qutebrowser.utils import log
 
 
 # Needs to be saved to avoid garbage collection
-_instance = None
+_instance: Optional["NativeEventFilter"] = None
 
 # Using C-style naming for C structures in this file
 # pylint: disable=invalid-name
 
 
 class xcb_ge_generic_event_t(ctypes.Structure):  # noqa: N801
     """See https://xcb.freedesktop.org/manual/structxcb__ge__generic__event__t.html.
```

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/objects.py` & `qutebrowser-3.2.0/qutebrowser/misc/objects.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/pakjoy.py` & `qutebrowser-3.2.0/qutebrowser/misc/pakjoy.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
     candidates = []
     qt_data_path = qtutils.library_path(qtutils.LibraryPath.data)
     if utils.is_mac:  # pragma: no cover
         # I'm not sure how to arrive at this path without hardcoding it
         # ourselves. importlib_resources("PyQt6.Qt6") can serve as a
         # replacement for the qtutils bit but it doesn't seem to help find the
-        # actuall Resources folder.
+        # actual Resources folder.
         candidates.append(
             qt_data_path / "lib" / "QtWebEngineCore.framework" / "Resources"
         )
 
     candidates += [
         qt_data_path / "resources",
         qt_data_path,
@@ -180,15 +180,17 @@
         pathlib.Path.home() / f".{objects.qapp.applicationName()}",
     ]
 
     for candidate in candidates:
         if (candidate / PAK_FILENAME).exists():
             return candidate
 
-    raise binparsing.ParseError("Couldn't find webengine resources dir")
+    candidates_str = "\n".join(f"    {p}" for p in candidates)
+    raise FileNotFoundError(
+        f"Couldn't find webengine resources dir, candidates:\n{candidates_str}")
 
 
 def copy_webengine_resources() -> Optional[pathlib.Path]:
     """Copy qtwebengine resources to local dir for patching."""
     resources_dir = _find_webengine_resources()
     work_dir = pathlib.Path(standarddir.cache()) / CACHE_DIR_NAME
```

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/pastebin.py` & `qutebrowser-3.2.0/qutebrowser/misc/pastebin.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/quitter.py` & `qutebrowser-3.2.0/qutebrowser/misc/quitter.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/savemanager.py` & `qutebrowser-3.2.0/qutebrowser/misc/savemanager.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/sessions.py` & `qutebrowser-3.2.0/qutebrowser/misc/sessions.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/split.py` & `qutebrowser-3.2.0/qutebrowser/misc/split.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/sql.py` & `qutebrowser-3.2.0/qutebrowser/misc/sql.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/throttle.py` & `qutebrowser-3.2.0/qutebrowser/misc/throttle.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/misc/utilcmds.py` & `qutebrowser-3.2.0/qutebrowser/misc/utilcmds.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/_core_pyqtproperty.py` & `qutebrowser-3.2.0/qutebrowser/qt/_core_pyqtproperty.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/core.py` & `qutebrowser-3.2.0/qutebrowser/qt/core.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/dbus.py` & `qutebrowser-3.2.0/qutebrowser/qt/dbus.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/gui.py` & `qutebrowser-3.2.0/qutebrowser/qt/gui.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/machinery.py` & `qutebrowser-3.2.0/qutebrowser/qt/machinery.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,29 +30,29 @@
 
 from qutebrowser.utils import log
 
 # Packagers: Patch the line below to enforce a Qt wrapper, e.g.:
 # sed -i 's/_WRAPPER_OVERRIDE = .*/_WRAPPER_OVERRIDE = "PyQt6"/' qutebrowser/qt/machinery.py
 #
 # Users: Set the QUTE_QT_WRAPPER environment variable to change the default wrapper.
-_WRAPPER_OVERRIDE = None
+_WRAPPER_OVERRIDE = None  # type: ignore[var-annotated]
 
 WRAPPERS = [
     "PyQt6",
     "PyQt5",
     # Needs more work
     # "PySide6",
 ]
 
 
 class Error(Exception):
     """Base class for all exceptions in this module."""
 
 
-class Unavailable(Error, ImportError):
+class Unavailable(Error, ModuleNotFoundError):
 
     """Raised when a module is unavailable with the given wrapper."""
 
     def __init__(self) -> None:
         super().__init__(f"Unavailable with {INFO.wrapper}")
 
 
@@ -164,17 +164,17 @@
     """Select a Qt wrapper.
 
     - If --qt-wrapper is given, use that.
     - Otherwise, if the QUTE_QT_WRAPPER environment variable is set, use that.
     - Otherwise, try the wrappers in WRAPPER in order (PyQt6 -> PyQt5)
     """
     # If any Qt wrapper has been imported before this, something strange might
-    # be happening.
+    # be happening. With PyInstaller, it imports the Qt bindings early.
     for name in WRAPPERS:
-        if name in sys.modules:
+        if name in sys.modules and not hasattr(sys, "frozen"):
             warnings.warn(f"{name} already imported", stacklevel=1)
 
     if args is not None and args.qt_wrapper is not None:
         assert args.qt_wrapper in WRAPPERS, args.qt_wrapper  # ensured by argparse
         return SelectionInfo(wrapper=args.qt_wrapper, reason=SelectionReason.cli)
 
     env_var = "QUTE_QT_WRAPPER"
@@ -186,15 +186,15 @@
             raise Error(
                 f"Unknown wrapper {env_wrapper} set via {env_var}, "
                 f"allowed: {', '.join(WRAPPERS)}"
             )
         return SelectionInfo(wrapper=env_wrapper, reason=SelectionReason.env)
 
     if _WRAPPER_OVERRIDE is not None:
-        assert _WRAPPER_OVERRIDE in WRAPPERS  # type: ignore[unreachable]
+        assert _WRAPPER_OVERRIDE in WRAPPERS
         return SelectionInfo(wrapper=_WRAPPER_OVERRIDE, reason=SelectionReason.override)
 
     return _autoselect_wrapper()
 
 
 # Values are set in init(). If you see a NameError here, it means something tried to
 # import Qt (or check for its availability) before machinery.init() was called.
```

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/network.py` & `qutebrowser-3.2.0/qutebrowser/qt/network.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/opengl.py` & `qutebrowser-3.2.0/qutebrowser/qt/opengl.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/printsupport.py` & `qutebrowser-3.2.0/qutebrowser/qt/printsupport.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/qml.py` & `qutebrowser-3.2.0/qutebrowser/qt/qml.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/sip.py` & `qutebrowser-3.2.0/qutebrowser/qt/sip.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/sql.py` & `qutebrowser-3.2.0/qutebrowser/qt/sql.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/test.py` & `qutebrowser-3.2.0/qutebrowser/qt/test.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/webenginecore.py` & `qutebrowser-3.2.0/qutebrowser/qt/webenginecore.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/webenginewidgets.py` & `qutebrowser-3.2.0/qutebrowser/qt/webenginewidgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 elif machinery.USE_PYQT6:
     from PyQt6.QtWebEngineWidgets import *
 else:
     raise machinery.UnknownWrapper()
 
 
 if machinery.IS_QT5:
+    # pylint: disable=undefined-variable
     # moved to WebEngineCore in Qt 6
     del QWebEngineSettings
     del QWebEngineProfile
     del QWebEngineDownloadItem
     del QWebEnginePage
     del QWebEngineCertificateError
     del QWebEngineScript
```

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/webkit.py` & `qutebrowser-3.2.0/qutebrowser/qt/webkit.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/webkitwidgets.py` & `qutebrowser-3.2.0/qutebrowser/qt/webkitwidgets.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/qt/widgets.py` & `qutebrowser-3.2.0/qutebrowser/qt/widgets.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,8 +22,9 @@
     from PyQt5.QtWidgets import *
 elif machinery.USE_PYQT6:
     from PyQt6.QtWidgets import *
 else:
     raise machinery.UnknownWrapper()
 
 if machinery.IS_QT5:
+    # pylint: disable=undefined-variable
     del QFileSystemModel  # moved to QtGui in Qt 6
```

### Comparing `qutebrowser-3.1.0/qutebrowser/qutebrowser.py` & `qutebrowser-3.2.0/qutebrowser/qutebrowser.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,20 +167,21 @@
         log-sensitive-keys: Log keypresses in passthrough modes.
         stack: Enable Chromium stack logging.
         chromium: Enable Chromium logging.
         wait-renderer-process: Wait for debugger in renderer process.
         avoid-chromium-init: Enable `--version` without initializing Chromium.
         werror: Turn Python warnings into errors.
         test-notification-service: Use the testing libnotify service.
+        caret: Enable debug logging for caret.js.
     """
     valid_flags = ['debug-exit', 'pdb-postmortem', 'no-sql-history',
                    'no-scroll-filtering', 'log-requests', 'log-cookies',
                    'log-scroll-pos', 'log-sensitive-keys', 'stack', 'chromium',
                    'wait-renderer-process', 'avoid-chromium-init', 'werror',
-                   'test-notification-service', 'log-qt-events']
+                   'test-notification-service', 'log-qt-events', 'caret']
 
     if flag in valid_flags:
         return flag
     else:
         raise argparse.ArgumentTypeError("Invalid debug flag - valid flags: {}"
                                          .format(', '.join(valid_flags)))
```

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/debug.py` & `qutebrowser-3.2.0/qutebrowser/utils/debug.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/docutils.py` & `qutebrowser-3.2.0/qutebrowser/utils/docutils.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/error.py` & `qutebrowser-3.2.0/qutebrowser/utils/error.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/javascript.py` & `qutebrowser-3.2.0/qutebrowser/utils/javascript.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/jinja.py` & `qutebrowser-3.2.0/qutebrowser/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/log.py` & `qutebrowser-3.2.0/qutebrowser/utils/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     colorama = None  # type: ignore[assignment]
 
 if TYPE_CHECKING:
     from qutebrowser.config import config as configmodule
 
 _log_inited = False
-_args = None
+_args: Optional[argparse.Namespace] = None
 
 COLORS = ['black', 'red', 'green', 'yellow', 'blue', 'purple', 'cyan', 'white']
 COLOR_ESCAPES = {color: '\033[{}m'.format(i)
                  for i, color in enumerate(COLORS, start=30)}
 RESET_ESCAPE = '\033[0m'
 
 
@@ -142,15 +142,15 @@
     'webelem', 'prompt', 'network', 'sql',
     'greasemonkey', 'extensions',
 ]
 
 
 ram_handler: Optional['RAMHandler'] = None
 console_handler: Optional[logging.Handler] = None
-console_filter = None
+console_filter: Optional["LogFilter"] = None
 
 
 def stub(suffix: str = '') -> None:
     """Show a STUB: message for the calling function."""
     try:
         function = inspect.stack()[1][3]
     except IndexError:  # pragma: no cover
```

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/message.py` & `qutebrowser-3.2.0/qutebrowser/utils/message.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/objreg.py` & `qutebrowser-3.2.0/qutebrowser/utils/objreg.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/qtlog.py` & `qutebrowser-3.2.0/qutebrowser/utils/qtlog.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import sys
 import traceback
 from typing import Iterator, Optional
 
 from qutebrowser.qt import core as qtcore
 from qutebrowser.utils import log
 
-_args = None
+_args: Optional[argparse.Namespace] = None
 
 
 def init(args: argparse.Namespace) -> None:
     """Install Qt message handler based on the argparse namespace passed."""
     global _args
     _args = args
     qtcore.qInstallMessageHandler(qt_message_handler)
```

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/qtutils.py` & `qutebrowser-3.2.0/qutebrowser/utils/qtutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,24 @@
         QDataStream.Status.Ok: "The data stream is operating normally.",
         QDataStream.Status.ReadPastEnd: ("The data stream has read past the end of "
                                   "the data in the underlying device."),
         QDataStream.Status.ReadCorruptData: "The data stream has read corrupt data.",
         QDataStream.Status.WriteFailed: ("The data stream cannot write to the "
                                   "underlying device."),
     }
+    if machinery.IS_QT6:
+        try:
+            status_to_str[QDataStream.Status.SizeLimitExceeded] = (
+                "The data stream cannot read or write the data because its size is larger "
+                "than supported by the current platform."
+            )
+        except AttributeError:
+            # Added in Qt 6.7
+            pass
+
     if stream.status() != QDataStream.Status.Ok:
         raise OSError(status_to_str[stream.status()])
 
 
 _QtSerializableType = Union[
     QObject,
     QByteArray,
@@ -732,8 +742,8 @@
 
     def remove_optional(obj: Optional[_T]) -> Optional[_T]:
         return obj
 
     def add_optional(obj: Optional[_T]) -> Optional[_T]:
         return obj
 
-    QT_NONE = None
+    QT_NONE: None = None
```

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/resources.py` & `qutebrowser-3.2.0/qutebrowser/utils/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """Resources related utilities."""
 
 import os.path
 import sys
 import contextlib
 import posixpath
 import pathlib
-from typing import Iterator, Iterable, Union
+from typing import Iterator, Iterable, Union, Dict
 
 
 # We cannot use the stdlib version on 3.8 because we need the files() API.
 if sys.version_info >= (3, 11):  # pragma: no cover
     # https://github.com/python/cpython/issues/90276
     import importlib.resources as importlib_resources
     from importlib.resources.abc import Traversable
@@ -21,15 +21,16 @@
     import importlib.resources as importlib_resources
     from importlib.abc import Traversable
 else:  # pragma: no cover
     import importlib_resources
     from importlib_resources.abc import Traversable
 
 import qutebrowser
-_cache = {}
+_cache: Dict[str, str] = {}
+_bin_cache: Dict[str, bytes] = {}
 
 
 _ResourceType = Union[Traversable, pathlib.Path]
 
 
 def _path(filename: str) -> _ResourceType:
     """Get a pathlib.Path object for a resource."""
@@ -84,14 +85,18 @@
             ('html', '.html'),
             ('javascript', '.js'),
             ('javascript/quirks', '.js'),
     ]:
         for name in _glob(resource_path, subdir, ext):
             _cache[name] = read_file(name)
 
+    for name in _glob(resource_path, 'img', '.png'):
+        # e.g. broken_qutebrowser_logo.png
+        _bin_cache[name] = read_file_binary(name)
+
 
 def read_file(filename: str) -> str:
     """Get the contents of a file contained with qutebrowser.
 
     Args:
         filename: The filename to open as string.
 
@@ -111,10 +116,13 @@
 
     Args:
         filename: The filename to open as string.
 
     Return:
         The file contents as a bytes object.
     """
+    if filename in _bin_cache:
+        return _bin_cache[filename]
+
     path = _path(filename)
     with _keyerror_workaround():
         return path.read_bytes()
```

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/standarddir.py` & `qutebrowser-3.2.0/qutebrowser/utils/standarddir.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 import os
 import os.path
 import sys
 import contextlib
 import enum
 import argparse
-from typing import Iterator, Optional
+from typing import Iterator, Optional, Dict
 
 from qutebrowser.qt.core import QStandardPaths
 from qutebrowser.qt.widgets import QApplication
 
 from qutebrowser.utils import log, debug, utils, version, qtutils
 
 # The cached locations
-_locations = {}
+_locations: Dict["_Location", str] = {}
 
 
 class _Location(enum.Enum):
 
     """A key for _locations."""
 
     config = enum.auto()
```

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/urlmatch.py` & `qutebrowser-3.2.0/qutebrowser/utils/urlmatch.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/urlutils.py` & `qutebrowser-3.2.0/qutebrowser/utils/urlutils.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/usertypes.py` & `qutebrowser-3.2.0/qutebrowser/utils/usertypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Custom useful data types."""
 
 import html
 import operator
 import enum
+import time
 import dataclasses
+import logging
 from typing import Optional, Sequence, TypeVar, Union
 
 from qutebrowser.qt.core import pyqtSignal, pyqtSlot, QObject, QTimer
 from qutebrowser.qt.core import QUrl
 
 from qutebrowser.utils import log, qtutils, utils
 
@@ -439,30 +441,66 @@
 
     Attributes:
         _name: The name of the timer.
     """
 
     def __init__(self, parent: QObject = None, name: str = None) -> None:
         super().__init__(parent)
+        self._start_time: Optional[float] = None
+        self.timeout.connect(self._validity_check_handler)
         if name is None:
             self._name = "unnamed"
         else:
             self.setObjectName(name)
             self._name = name
 
     def __repr__(self) -> str:
         return utils.get_repr(self, name=self._name)
 
+    @pyqtSlot()
+    def _validity_check_handler(self) -> None:
+        if not self.check_timeout_validity() and self._start_time is not None:
+            elapsed = time.monotonic() - self._start_time
+            level = logging.WARNING
+            if utils.is_windows and self._name == "ipc-timeout":
+                level = logging.DEBUG
+            log.misc.log(
+                level,
+                (
+                    f"Timer {self._name} (id {self.timerId()}) triggered too early: "
+                    f"interval {self.interval()} but only {elapsed:.3f}s passed"
+                )
+            )
+
+    def check_timeout_validity(self) -> bool:
+        """Check to see if the timeout signal was fired at the expected time.
+
+        WORKAROUND for https://bugreports.qt.io/browse/QTBUG-124496
+        """
+        if self._start_time is None:
+            # manual emission?
+            return True
+
+        elapsed = time.monotonic() - self._start_time
+        # Checking for half the interval is pretty arbitrary. In the bug case
+        # the timer typically fires immediately since the expiry event is
+        # already pending when it is created.
+        if elapsed < self.interval() / 1000 / 2:
+            return False
+
+        return True
+
     def setInterval(self, msec: int) -> None:
         """Extend setInterval to check for overflows."""
         qtutils.check_overflow(msec, 'int')
         super().setInterval(msec)
 
     def start(self, msec: int = None) -> None:
         """Extend start to check for overflows."""
+        self._start_time = time.monotonic()
         if msec is not None:
             qtutils.check_overflow(msec, 'int')
             super().start(msec)
         else:
             super().start()
```

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/utils.py` & `qutebrowser-3.2.0/qutebrowser/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import json
 import fnmatch
 import datetime
 import traceback
 import functools
 import contextlib
 import shlex
+import sysconfig
 import mimetypes
 from typing import (Any, Callable, IO, Iterator,
                     Optional, Sequence, Tuple, List, Type, Union,
                     TypeVar, Protocol)
 
 from qutebrowser.qt.core import QUrl, QVersionNumber, QRect, QPoint
 from qutebrowser.qt.gui import QClipboard, QDesktopServices
@@ -34,15 +35,15 @@
 except ImportError:  # pragma: no cover
     from yaml import (SafeLoader as YamlLoader,  # type: ignore[assignment]
                       SafeDumper as YamlDumper)
     YAML_C_EXT = False
 
 from qutebrowser.utils import log
 
-fake_clipboard = None
+fake_clipboard: Optional[str] = None
 log_clipboard = False
 
 is_mac = sys.platform.startswith('darwin')
 is_linux = sys.platform.startswith('linux')
 is_windows = sys.platform.startswith('win')
 is_posix = os.name == 'posix'
 
@@ -337,15 +338,15 @@
         retval = self._retval
 
         @functools.wraps(func)
         def wrapper(*args: Any, **kwargs: Any) -> Any:
             """Call the original function."""
             try:
                 return func(*args, **kwargs)
-            except BaseException:
+            except BaseException:  # noqa: B036
                 log.misc.exception("Error in {}".format(qualname(func)))
                 return retval
 
         return wrapper
 
 
 def is_enum(obj: Any) -> bool:
@@ -632,15 +633,15 @@
 
     Does nothing for other paths.
 
     Args:
         path: The path to expand.
     """
     # Usually, "E:" on Windows refers to the current working directory on drive
-    # E:\. The correct way to specifify drive E: is "E:\", but most users
+    # E:\. The correct way to specify drive E: is "E:\", but most users
     # probably don't use the "multiple working directories" feature and expect
     # "E:" and "E:\" to be equal.
     if re.fullmatch(r'[A-Z]:', path, re.IGNORECASE):
         return path + "\\"
     else:
         return path
 
@@ -662,15 +663,18 @@
                 # WORKAROUND for https://github.com/yaml/pyyaml/issues/168
                 raise yaml.YAMLError(e)
             raise
 
     end = datetime.datetime.now()
 
     delta = (end - start).total_seconds()
-    deadline = 10 if 'CI' in os.environ else 2
+    if "CI" in os.environ or sysconfig.get_config_var("Py_DEBUG"):
+        deadline = 10
+    else:
+        deadline = 2
     if delta > deadline:  # pragma: no cover
         log.misc.warning(
             "YAML load took unusually long, please report this at "
             "https://github.com/qutebrowser/qutebrowser/issues/2777\n"
             "duration: {}s\n"
             "PyYAML version: {}\n"
             "C extension: {}\n"
```

### Comparing `qutebrowser-3.1.0/qutebrowser/utils/version.py` & `qutebrowser-3.2.0/qutebrowser/utils/version.py`

 * *Files 21% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     """Information about the running distribution."""
 
     id: Optional[str]
     parsed: 'Distribution'
     pretty: str
 
 
-pastebin_url = None
+pastebin_url: Optional[str] = None
 
 
 class Distribution(enum.Enum):
 
     """A known Linux distribution.
 
     Usually lines up with ID=... in /etc/os-release.
@@ -482,15 +482,15 @@
     try:
         pdfjs_file, file_path = pdfjs.get_pdfjs_res_and_path(pdfjs.get_pdfjs_js_path())
     except pdfjs.PDFJSNotFound:
         return 'no'
     else:
         pdfjs_file = pdfjs_file.decode('utf-8')
         version_re = re.compile(
-            r"^ *(PDFJS\.version|(var|const) pdfjsVersion) = '(?P<version>[^']+)';$",
+            r"""^ *(PDFJS\.version|(var|const) pdfjsVersion) = ['"](?P<version>[^'"]+)['"];$""",
             re.MULTILINE)
 
         match = version_re.search(pdfjs_file)
         pdfjs_version = 'unknown' if not match else match.group('version')
         if file_path is None:
             file_path = 'bundled'
 
@@ -531,17 +531,30 @@
 class WebEngineVersions:
 
     """Version numbers for QtWebEngine and the underlying Chromium."""
 
     webengine: utils.VersionNumber
     chromium: Optional[str]
     source: str
+    chromium_security: Optional[str] = None
     chromium_major: Optional[int] = dataclasses.field(init=False)
 
-    _CHROMIUM_VERSIONS: ClassVar[Dict[utils.VersionNumber, str]] = {
+    _BASES: ClassVar[Dict[int, str]] = {
+        83: '83.0.4103.122',  # ~2020-06-24
+        87: '87.0.4280.144',  # ~2020-12-02
+        90: '90.0.4430.228',  # 2021-06-22
+        94: '94.0.4606.126',  # 2021-11-17
+        102: '102.0.5005.177',  # ~2022-05-24
+        # (.220 claimed by code, .181 claimed by CHROMIUM_VERSION)
+        108: '108.0.5359.220',  # ~2022-12-23
+        112: '112.0.5615.213',  # ~2023-04-18
+        118: '118.0.5993.220',  # ~2023-10-24
+    }
+
+    _CHROMIUM_VERSIONS: ClassVar[Dict[utils.VersionNumber, Tuple[str, Optional[str]]]] = {
         # ====== UNSUPPORTED =====
 
         # Qt 5.12: Chromium 69
         # (LTS)    69.0.3497.128 (~2018-09-11)
         #          5.12.10: Security fixes up to 86.0.4240.75 (2020-10-06)
 
         # Qt 5.13: Chromium 73
@@ -554,152 +567,185 @@
 
         # Qt 5.15: Chromium 80
         #          80.0.3987.163 (2020-04-02)
         #          5.15.0: Security fixes up to 81.0.4044.138 (2020-05-05)
         #          5.15.1: Security fixes up to 85.0.4183.83  (2020-08-25)
 
         # ====== SUPPORTED =====
-
-        # Qt 5.15.2: Chromium 83
-        #            83.0.4103.122           (~2020-06-24)
-        #            5.15.2: Security fixes up to 86.0.4240.183 (2020-11-02)
-        utils.VersionNumber(5, 15, 2): '83.0.4103.122',
-
-        # Qt 5.15.3: Chromium 87
-        #            87.0.4280.144           (~2020-12-02)
-        #            5.15.3: Security fixes up to 88.0.4324.150 (2021-02-04)
-        #            5.15.4: Security fixes up to ???
-        #            5.15.5: Security fixes up to ???
-        #            5.15.6: Security fixes up to ???
-        #            5.15.7: Security fixes up to 94.0.4606.61  (2021-09-24)
-        #            5.15.8: Security fixes up to 96.0.4664.110 (2021-12-13)
-        #            5.15.9: Security fixes up to 98.0.4758.102 (2022-02-14)
-        #            5.15.10: Security fixes up to ???
-        #            5.15.11: Security fixes up to ???
-        utils.VersionNumber(5, 15): '87.0.4280.144',  # >= 5.15.3
-
-        # Qt 6.2: Chromium 90
-        #         90.0.4430.228 (2021-06-22)
-        #         6.2.0: Security fixes up to 93.0.4577.63 (2021-08-31)
-        #         6.2.1: Security fixes up to 94.0.4606.61 (2021-09-24)
-        #         6.2.2: Security fixes up to 96.0.4664.45 (2021-11-15)
-        #         6.2.3: Security fixes up to 96.0.4664.45 (2021-11-15)
-        #         6.2.4: Security fixes up to 98.0.4758.102 (2022-02-14)
-        #         6.2.5: Security fixes up to ???
-        #         6.2.6: Security fixes up to ???
-        #         6.2.7: Security fixes up to ???
-        utils.VersionNumber(6, 2): '90.0.4430.228',
-
-        # Qt 6.3: Chromium 94
-        #         94.0.4606.126 (2021-11-17)
-        #         6.3.0: Security fixes up to 99.0.4844.84 (2022-03-25)
-        #         6.3.1: Security fixes up to 101.0.4951.64 (2022-05-10)
-        #         6.3.2: Security fixes up to 104.0.5112.81 (2022-08-01)
-        utils.VersionNumber(6, 3): '94.0.4606.126',
-
-        # Qt 6.4: Chromium 102
-        #         102.0.5005.177 (~2022-05-24)
-        #         6.4.0: Security fixes up to 104.0.5112.102 (2022-08-16)
-        #         6.4.1: Security fixes up to 107.0.5304.88 (2022-10-27)
-        #         6.4.2: Security fixes up to 108.0.5359.94 (2022-12-02)
-        #         6.4.3: Security fixes up to 110.0.5481.78 (2023-02-07)
-        utils.VersionNumber(6, 4): '102.0.5005.177',
-
-        # Qt 6.5: Chromium 108
-        #         108.0.5359.220 (~2022-12-23)
-        #         (.220 claimed by code, .181 claimed by CHROMIUM_VERSION)
-        #         6.5.0: Security fixes up to 110.0.5481.104 (2023-02-16)
-        #         6.5.1: Security fixes up to 112.0.5615.138 (2023-04-18)
-        #         6.5.2: Security fixes up to 114.0.5735.133 (2023-06-13)
-        utils.VersionNumber(6, 5): '108.0.5359.220',
-
-        # Qt 6.6: Chromium 112
-        #         112.0.5615.213 (~2023-04-18)
-        #         6.6.0: Security fixes up to 116.0.5845.110 (?) (2023-08-22)
-        utils.VersionNumber(6, 6): '112.0.5615.213',
+        #                               base         security
+        ## Qt 5.15
+        utils.VersionNumber(5, 15, 2): (_BASES[83], '86.0.4240.183'),  # 2020-11-02
+        utils.VersionNumber(5, 15): (_BASES[87], None),  # >= 5.15.3
+        utils.VersionNumber(5, 15, 3): (_BASES[87], '88.0.4324.150'),  # 2021-02-04
+        # 5.15.4 to 5.15.6: unknown security fixes
+        utils.VersionNumber(5, 15, 7): (_BASES[87], '94.0.4606.61'),  # 2021-09-24
+        utils.VersionNumber(5, 15, 8): (_BASES[87], '96.0.4664.110'),  # 2021-12-13
+        utils.VersionNumber(5, 15, 9): (_BASES[87], '98.0.4758.102'),  # 2022-02-14
+        utils.VersionNumber(5, 15, 10): (_BASES[87], '98.0.4758.102'),  # (?) 2022-02-14
+        utils.VersionNumber(5, 15, 11): (_BASES[87], '98.0.4758.102'),  # (?) 2022-02-14
+        utils.VersionNumber(5, 15, 12): (_BASES[87], '98.0.4758.102'),  # (?) 2022-02-14
+        utils.VersionNumber(5, 15, 13): (_BASES[87], '108.0.5359.124'),  # 2022-12-13
+        utils.VersionNumber(5, 15, 14): (_BASES[87], '113.0.5672.64'),  # 2023-05-02
+        # 5.15.15: unknown security fixes
+        utils.VersionNumber(5, 15, 16): (_BASES[87], '119.0.6045.123'),  # 2023-11-07
+        utils.VersionNumber(5, 15, 17): (_BASES[87], '123.0.6312.58'),  # 2024-03-19
+
+
+        ## Qt 6.2
+        utils.VersionNumber(6, 2): (_BASES[90], '93.0.4577.63'),  # 2021-08-31
+        utils.VersionNumber(6, 2, 1): (_BASES[90], '94.0.4606.61'),  # 2021-09-24
+        utils.VersionNumber(6, 2, 2): (_BASES[90], '96.0.4664.45'),  # 2021-11-15
+        utils.VersionNumber(6, 2, 3): (_BASES[90], '96.0.4664.45'),  # 2021-11-15
+        utils.VersionNumber(6, 2, 4): (_BASES[90], '98.0.4758.102'),  # 2022-02-14
+        # 6.2.5 / 6.2.6: unknown security fixes
+        utils.VersionNumber(6, 2, 7): (_BASES[90], '107.0.5304.110'),  # 2022-11-08
+        utils.VersionNumber(6, 2, 8): (_BASES[90], '111.0.5563.110'),  # 2023-03-21
+
+        ## Qt 6.3
+        utils.VersionNumber(6, 3): (_BASES[94], '99.0.4844.84'),  # 2022-03-25
+        utils.VersionNumber(6, 3, 1): (_BASES[94], '101.0.4951.64'),  # 2022-05-10
+        utils.VersionNumber(6, 3, 2): (_BASES[94], '104.0.5112.81'),  # 2022-08-01
+
+        ## Qt 6.4
+        utils.VersionNumber(6, 4): (_BASES[102], '104.0.5112.102'),  # 2022-08-16
+        utils.VersionNumber(6, 4, 1): (_BASES[102], '107.0.5304.88'),  # 2022-10-27
+        utils.VersionNumber(6, 4, 2): (_BASES[102], '108.0.5359.94'),  # 2022-12-02
+        utils.VersionNumber(6, 4, 3): (_BASES[102], '110.0.5481.78'),  # 2023-02-07
+
+        ## Qt 6.5
+        utils.VersionNumber(6, 5): (_BASES[108], '110.0.5481.104'),  # 2023-02-16
+        utils.VersionNumber(6, 5, 1): (_BASES[108], '112.0.5615.138'),  # 2023-04-18
+        utils.VersionNumber(6, 5, 2): (_BASES[108], '114.0.5735.133'),  # 2023-06-13
+        utils.VersionNumber(6, 5, 3): (_BASES[108], '117.0.5938.63'),  # 2023-09-12
+
+        ## Qt 6.6
+        utils.VersionNumber(6, 6): (_BASES[112], '117.0.5938.63'),  # 2023-09-12
+        utils.VersionNumber(6, 6, 1): (_BASES[112], '119.0.6045.123'),  # 2023-11-07
+        utils.VersionNumber(6, 6, 2): (_BASES[112], '121.0.6167.160'),  # 2024-02-06
+        utils.VersionNumber(6, 6, 3): (_BASES[112], '122.0.6261.128'),  # 2024-03-12
+
+        ## Qt 6.7
+        utils.VersionNumber(6, 7): (_BASES[118], '122.0.6261.128'),  # 2024-03-12
+        utils.VersionNumber(6, 7, 1): (_BASES[118], '124.0.6367.202'),  # ~2024-05-09
     }
 
     def __post_init__(self) -> None:
         """Set the major Chromium version."""
         if self.chromium is None:
             self.chromium_major = None
         else:
             self.chromium_major = int(self.chromium.split('.')[0])
 
     def __str__(self) -> str:
-        s = f'QtWebEngine {self.webengine}'
+        lines = [f'QtWebEngine {self.webengine}']
         if self.chromium is not None:
-            s += f', based on Chromium {self.chromium}'
-        if self.source != 'UA':
-            s += f' (from {self.source})'
-        return s
+            lines.append(f'  based on Chromium {self.chromium}')
+        if self.chromium_security is not None:
+            lines.append(f'  with security patches up to {self.chromium_security} (plus any distribution patches)')
+        lines.append(f'  (source: {self.source})')
+        return "\n".join(lines)
 
     @classmethod
     def from_ua(cls, ua: 'websettings.UserAgent') -> 'WebEngineVersions':
         """Get the versions parsed from a user agent.
 
-        This is the most reliable and "default" way to get this information (at least
-        until QtWebEngine adds an API for it). However, it needs a fully initialized
-        QtWebEngine, and we sometimes need this information before that is available.
+        This is the most reliable and "default" way to get this information for
+        older Qt versions that don't provide an API for it. However, it needs a
+        fully initialized QtWebEngine, and we sometimes need this information
+        before that is available.
         """
         assert ua.qt_version is not None, ua
+        webengine = utils.VersionNumber.parse(ua.qt_version)
+        chromium_inferred, chromium_security = cls._infer_chromium_version(webengine)
+        if ua.upstream_browser_version != chromium_inferred:  # pragma: no cover
+            # should never happen, but let's play it safe
+            log.misc.debug(
+                f"Chromium version mismatch: {ua.upstream_browser_version} (UA) != "
+                f"{chromium_inferred} (inferred)")
+            chromium_security = None
+
         return cls(
-            webengine=utils.VersionNumber.parse(ua.qt_version),
+            webengine=webengine,
             chromium=ua.upstream_browser_version,
+            chromium_security=chromium_security,
             source='UA',
         )
 
     @classmethod
     def from_elf(cls, versions: elf.Versions) -> 'WebEngineVersions':
         """Get the versions based on an ELF file.
 
         This only works on Linux, and even there, depends on various assumption on how
         QtWebEngine is built (e.g. that the version string is in the .rodata section).
 
         On Windows/macOS, we instead rely on from_pyqt, but especially on Linux, people
         sometimes mix and match Qt/QtWebEngine versions, so this is a more reliable
         (though hackish) way to get a more accurate result.
         """
+        webengine = utils.VersionNumber.parse(versions.webengine)
+        chromium_inferred, chromium_security = cls._infer_chromium_version(webengine)
+        if versions.chromium != chromium_inferred:  # pragma: no cover
+            # should never happen, but let's play it safe
+            log.misc.debug(
+                f"Chromium version mismatch: {versions.chromium} (ELF) != "
+                f"{chromium_inferred} (inferred)")
+            chromium_security = None
+
         return cls(
-            webengine=utils.VersionNumber.parse(versions.webengine),
+            webengine=webengine,
             chromium=versions.chromium,
+            chromium_security=chromium_security,
             source='ELF',
         )
 
     @classmethod
     def _infer_chromium_version(
             cls,
             pyqt_webengine_version: utils.VersionNumber,
-    ) -> Optional[str]:
-        """Infer the Chromium version based on the PyQtWebEngine version."""
-        chromium_version = cls._CHROMIUM_VERSIONS.get(pyqt_webengine_version)
+    ) -> Tuple[Optional[str], Optional[str]]:
+        """Infer the Chromium version based on the PyQtWebEngine version.
+
+        Returns:
+            A tuple of the Chromium version and the security patch version.
+        """
+        chromium_version, security_version = cls._CHROMIUM_VERSIONS.get(
+            pyqt_webengine_version, (None, None))
         if chromium_version is not None:
-            return chromium_version
+            return chromium_version, security_version
 
         # 5.15 patch versions change their QtWebEngine version, but no changes are
         # expected after 5.15.3 and 5.15.[01] are unsupported.
-        if pyqt_webengine_version == utils.VersionNumber(5, 15, 2):
-            minor_version = pyqt_webengine_version
-        else:
-            # e.g. 5.14.2 -> 5.14
-            minor_version = pyqt_webengine_version.strip_patch()
+        assert pyqt_webengine_version != utils.VersionNumber(5, 15, 2)
+
+        # e.g. 5.15.4 -> 5.15
+        # we ignore the security version as that one will have changed from .0
+        # and is thus unknown.
+        minor_version = pyqt_webengine_version.strip_patch()
+        chromium_ver, _security_ver = cls._CHROMIUM_VERSIONS.get(
+            minor_version, (None, None))
 
-        return cls._CHROMIUM_VERSIONS.get(minor_version)
+        return chromium_ver, None
 
     @classmethod
-    def from_api(cls, qtwe_version: str, chromium_version: Optional[str]) -> 'WebEngineVersions':
+    def from_api(
+        cls,
+        qtwe_version: str,
+        chromium_version: Optional[str],
+        chromium_security: Optional[str] = None,
+    ) -> 'WebEngineVersions':
         """Get the versions based on the exact versions.
 
         This is called if we have proper APIs to get the versions easily
         (Qt 6.2 with PyQt 6.3.1+).
         """
         parsed = utils.VersionNumber.parse(qtwe_version)
         return cls(
             webengine=parsed,
             chromium=chromium_version,
+            chromium_security=chromium_security,
             source='api',
         )
 
     @classmethod
     def from_webengine(
         cls,
         pyqt_webengine_qt_version: str,
@@ -708,17 +754,19 @@
         """Get the versions based on the PyQtWebEngine version.
 
         This is called if we don't want to fully initialize QtWebEngine (so
         from_ua isn't possible), we're not on Linux (or ELF parsing failed), but we have
         a PyQtWebEngine-Qt{,5} package from PyPI, so we could query its exact version.
         """
         parsed = utils.VersionNumber.parse(pyqt_webengine_qt_version)
+        chromium, chromium_security = cls._infer_chromium_version(parsed)
         return cls(
             webengine=parsed,
-            chromium=cls._infer_chromium_version(parsed),
+            chromium=chromium,
+            chromium_security=chromium_security,
             source=source,
         )
 
     @classmethod
     def from_pyqt(cls, pyqt_webengine_version: str, source: str = "PyQt") -> 'WebEngineVersions':
         """Get the versions based on the PyQtWebEngine version.
 
@@ -753,17 +801,20 @@
             # be using QtWebEngine 5.15.3 (87-based). For now, we play it safe, and only
             # do this kind of "downgrade" when we know we're using PyInstaller.
             frozen = hasattr(sys, 'frozen')
             log.misc.debug(f"PyQt5 >= 5.15.3, frozen {frozen}")
             if frozen:
                 parsed = utils.VersionNumber(5, 15, 2)
 
+        chromium, chromium_security = cls._infer_chromium_version(parsed)
+
         return cls(
             webengine=parsed,
-            chromium=cls._infer_chromium_version(parsed),
+            chromium=chromium,
+            chromium_security=chromium_security,
             source=source,
         )
 
 
 def qtwebengine_versions(*, avoid_init: bool = False) -> WebEngineVersions:
     """Get the QtWebEngine and Chromium version numbers.
 
@@ -792,19 +843,28 @@
             from qutebrowser.qt.webenginecore import (
                 qWebEngineVersion,
                 qWebEngineChromiumVersion,
             )
         except ImportError:
             pass  # Needs QtWebEngine 6.2+ with PyQtWebEngine 6.3.1+
         else:
+            try:
+                from qutebrowser.qt.webenginecore import (
+                    qWebEngineChromiumSecurityPatchVersion,
+                )
+                chromium_security = qWebEngineChromiumSecurityPatchVersion()
+            except ImportError:
+                chromium_security = None  # Needs QtWebEngine 6.3+
+
             qtwe_version = qWebEngineVersion()
             assert qtwe_version is not None
             return WebEngineVersions.from_api(
                 qtwe_version=qtwe_version,
                 chromium_version=qWebEngineChromiumVersion(),
+                chromium_security=chromium_security,
             )
 
     from qutebrowser.browser.webengine import webenginesettings
 
     if webenginesettings.parsed_user_agent is None and not avoid_init:
         webenginesettings.init_user_agent()
```

### Comparing `qutebrowser-3.1.0/qutebrowser.egg-info/PKG-INFO` & `qutebrowser-3.2.0/qutebrowser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qutebrowser
-Version: 3.1.0
+Version: 3.2.0
 Summary: A keyboard-driven, vim-like browser based on Python and Qt.
 Home-page: https://www.qutebrowser.org/
 Author: Florian Bruhin
 Author-email: mail@qutebrowser.org
 License: GPL
 Keywords: pyqt browser web qt webkit qtwebkit qtwebengine
 Classifier: Development Status :: 5 - Production/Stable
@@ -169,15 +169,15 @@
 https://github.com/sponsors/The-Compiler/[GitHub Sponsors page] for more
 information. Depending on your sign-up date and how long you keep a certain
 level, you can get qutebrowser t-shirts, stickers and more!
 
 GitHub Sponsors allows for one-time donations (using the buttons next to "Select a
 tier") as well as custom amounts. **For currencies other than Euro or Swiss Francs, this
 is the preferred donation method.** GitHub uses https://stripe.com/[Stripe] to accept
-payment via credit carts without any fees. Billing via PayPal is available as well, with
+payment via credit cards without any fees. Billing via PayPal is available as well, with
 less fees than a direct PayPal transaction.
 
 Alternatively, the following donation methods are available -- note that
 eligibility for swag (shirts/stickers/etc.) is handled on a case-by-case basis
 for those, please mailto:mail@qutebrowser.org[get in touch] for details.
 
 * https://liberapay.com/The-Compiler[Liberapay], which can handle payments
```

### Comparing `qutebrowser-3.1.0/qutebrowser.egg-info/SOURCES.txt` & `qutebrowser-3.2.0/qutebrowser.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 misc/requirements/requirements-pyqt-6.3.txt-raw
 misc/requirements/requirements-pyqt-6.4.txt
 misc/requirements/requirements-pyqt-6.4.txt-raw
 misc/requirements/requirements-pyqt-6.5.txt
 misc/requirements/requirements-pyqt-6.5.txt-raw
 misc/requirements/requirements-pyqt-6.6.txt
 misc/requirements/requirements-pyqt-6.6.txt-raw
+misc/requirements/requirements-pyqt-6.7.txt
+misc/requirements/requirements-pyqt-6.7.txt-raw
 misc/requirements/requirements-pyqt-6.txt
 misc/requirements/requirements-pyqt-6.txt-raw
 misc/requirements/requirements-pyqt.txt
 misc/requirements/requirements-pyqt.txt-raw
 misc/requirements/requirements-pyroma.txt
 misc/requirements/requirements-pyroma.txt-raw
 misc/requirements/requirements-qutebrowser.txt-raw
@@ -153,15 +155,15 @@
 qutebrowser/browser/webengine/webenginesettings.py
 qutebrowser/browser/webengine/webenginetab.py
 qutebrowser/browser/webengine/webview.py
 qutebrowser/browser/webkit/__init__.py
 qutebrowser/browser/webkit/cache.py
 qutebrowser/browser/webkit/certificateerror.py
 qutebrowser/browser/webkit/cookies.py
-qutebrowser/browser/webkit/http.py
+qutebrowser/browser/webkit/httpheaders.py
 qutebrowser/browser/webkit/mhtml.py
 qutebrowser/browser/webkit/tabhistory.py
 qutebrowser/browser/webkit/webkitelem.py
 qutebrowser/browser/webkit/webkithistory.py
 qutebrowser/browser/webkit/webkitinspector.py
 qutebrowser/browser/webkit/webkitsettings.py
 qutebrowser/browser/webkit/webkittab.py
@@ -712,15 +714,15 @@
 tests/unit/browser/webkit/test_cookies.py
 tests/unit/browser/webkit/test_mhtml.py
 tests/unit/browser/webkit/test_tabhistory.py
 tests/unit/browser/webkit/test_webkit_view.py
 tests/unit/browser/webkit/test_webkitelem.py
 tests/unit/browser/webkit/test_webkitsettings.py
 tests/unit/browser/webkit/http/test_content_disposition.py
-tests/unit/browser/webkit/http/test_http.py
+tests/unit/browser/webkit/http/test_httpheaders.py
 tests/unit/browser/webkit/network/test_filescheme.py
 tests/unit/browser/webkit/network/test_networkmanager.py
 tests/unit/browser/webkit/network/test_networkreply.py
 tests/unit/browser/webkit/network/test_pac.py
 tests/unit/commands/test_argparser.py
 tests/unit/commands/test_cmdexc.py
 tests/unit/commands/test_parser.py
@@ -785,14 +787,15 @@
 tests/unit/mainwindow/statusbar/test_tabindex.py
 tests/unit/mainwindow/statusbar/test_textbase.py
 tests/unit/mainwindow/statusbar/test_url.py
 tests/unit/misc/test_autoupdate.py
 tests/unit/misc/test_checkpyver.py
 tests/unit/misc/test_cmdhistory.py
 tests/unit/misc/test_crashdialog.py
+tests/unit/misc/test_crashsignal.py
 tests/unit/misc/test_earlyinit.py
 tests/unit/misc/test_editor.py
 tests/unit/misc/test_elf.py
 tests/unit/misc/test_guiprocess.py
 tests/unit/misc/test_ipc.py
 tests/unit/misc/test_keyhints.py
 tests/unit/misc/test_lineparser.py
```

### Comparing `qutebrowser-3.1.0/scripts/cycle-inputs.js` & `qutebrowser-3.2.0/scripts/cycle-inputs.js`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/scripts/dictcli.py` & `qutebrowser-3.2.0/scripts/dictcli.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/scripts/hist_importer.py` & `qutebrowser-3.2.0/scripts/hist_importer.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/scripts/hostblock_blame.py` & `qutebrowser-3.2.0/scripts/hostblock_blame.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/scripts/importer.py` & `qutebrowser-3.2.0/scripts/importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         'quickmark': {
             'bookmark': '{tag.string} {tag[href]}',
             'keyword': '{tag[shortcuturl]} {tag[href]}'
         }
     }
     bookmarks = []
     for typ in bookmark_types:
-        tags = soup.findAll(bookmark_query[typ])
+        tags = soup.find_all(bookmark_query[typ])
         for tag in tags:
             if typ == 'search':
                 tag['href'] = search_escape(tag['href']).replace('%s', '{}')
             if tag['href'] not in bookmarks:
                 bookmarks.append(
                     output_template[output_format][typ].format(tag=tag))
     for bookmark in bookmarks:
```

### Comparing `qutebrowser-3.1.0/scripts/link_pyqt.py` & `qutebrowser-3.2.0/scripts/link_pyqt.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/scripts/mkvenv.py` & `qutebrowser-3.2.0/scripts/mkvenv.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/scripts/open_url_in_instance.sh` & `qutebrowser-3.2.0/scripts/open_url_in_instance.sh`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/scripts/opengl_info.py` & `qutebrowser-3.2.0/scripts/opengl_info.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/scripts/setupcommon.py` & `qutebrowser-3.2.0/scripts/setupcommon.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/scripts/testbrowser/testbrowser_webengine.py` & `qutebrowser-3.2.0/scripts/testbrowser/testbrowser_webengine.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/scripts/testbrowser/testbrowser_webkit.py` & `qutebrowser-3.2.0/scripts/testbrowser/testbrowser_webkit.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/scripts/utils.py` & `qutebrowser-3.2.0/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/setup.py` & `qutebrowser-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/conftest.py` & `qutebrowser-3.2.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,19 +180,18 @@
         else:
             remaining_items.append(item)
 
     config.hook.pytest_deselected(items=deselected_items)
     items[:] = remaining_items
 
 
-def pytest_ignore_collect(path):
+def pytest_ignore_collect(collection_path: pathlib.Path) -> bool:
     """Ignore BDD tests if we're unable to run them."""
-    fspath = pathlib.Path(path)
     skip_bdd = hasattr(sys, 'frozen')
-    rel_path = fspath.relative_to(pathlib.Path(__file__).parent)
+    rel_path = collection_path.relative_to(pathlib.Path(__file__).parent)
     return rel_path == pathlib.Path('end2end') / 'features' and skip_bdd
 
 
 @pytest.fixture(scope='session')
 def qapp_args():
     """Make QtWebEngine unit tests run on older Qt versions + newer kernels."""
     if testutils.disable_seccomp_bpf_sandbox():
```

### Comparing `qutebrowser-3.1.0/tests/end2end/conftest.py` & `qutebrowser-3.2.0/tests/end2end/conftest.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/blocked-hosts.gz` & `qutebrowser-3.2.0/tests/end2end/data/blocked-hosts.gz`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/brave-adblock/LICENSE` & `qutebrowser-3.2.0/tests/end2end/data/brave-adblock/LICENSE`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/brave-adblock/README.md` & `qutebrowser-3.2.0/tests/end2end/data/brave-adblock/README.md`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/brave-adblock/generate.py` & `qutebrowser-3.2.0/tests/end2end/data/brave-adblock/generate.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/brave-adblock/ublock-matches.tsv.gz` & `qutebrowser-3.2.0/tests/end2end/data/brave-adblock/ublock-matches.tsv.gz`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/click_element.html` & `qutebrowser-3.2.0/tests/end2end/data/click_element.html`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,14 @@
         <title>quteprocess.click_element test</title>
     </head>
     <body>
         <span id='test' onclick='console.log("click_element clicked")'>Test Element</span>
         <span onclick='console.log("click_element special chars")'>"Don't", he shouted</span>
         <span>Duplicate</span>
         <span class='clickable' onclick='console.log("click_element CSS selector")'>Duplicate</span>
-        <form><input autofocus id='qute-input'></input></form>
+        <form><input id='qute-input' onfocus='console.log("qute-input focused")'></input></form>
         <a href="/data/hello.txt" id='link'>link</a>
         <span id='foo.bar' onclick='console.log("id with dot")'>ID with dot</span>
         <span style='position: absolute; left: 20px;top: 42px; width:10px; height:10px;'
               onclick='console.log("click_element position")'></span>
     </body>
 </html>
```

### Comparing `qutebrowser-3.1.0/tests/end2end/data/darkmode/mathml-display.html` & `qutebrowser-3.2.0/tests/end2end/data/darkmode/mathml-display.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/darkmode/mathml-inline.html` & `qutebrowser-3.2.0/tests/end2end/data/darkmode/mathml-inline.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/darkmode/mathml.svg` & `qutebrowser-3.2.0/tests/end2end/data/darkmode/mathml.svg`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/darkmode/prefers-color-scheme.html` & `qutebrowser-3.2.0/tests/end2end/data/darkmode/prefers-color-scheme.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/downloads/issue1725.html` & `qutebrowser-3.2.0/tests/end2end/data/downloads/issue1725.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/Banner.png` & `qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/Banner.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/DYK.png` & `qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/DYK.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/complex.html` & `qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/complex.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/complex.mht` & `qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/complex.mht`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/complex/favicon.png` & `qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/complex/favicon.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/downloads/mhtml/simple/simple.mht` & `qutebrowser-3.2.0/tests/end2end/data/downloads/mhtml/simple/simple.mht`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/downloads/qutebrowser.png` & `qutebrowser-3.2.0/tests/end2end/data/downloads/qutebrowser.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/easylist.txt.gz` & `qutebrowser-3.2.0/tests/end2end/data/easylist.txt.gz`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/easyprivacy.txt.gz` & `qutebrowser-3.2.0/tests/end2end/data/easyprivacy.txt.gz`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/fileselect.html` & `qutebrowser-3.2.0/tests/end2end/data/fileselect.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/ace/ace.js` & `qutebrowser-3.2.0/tests/end2end/data/hints/ace/ace.js`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/angular1/angular.min.js` & `qutebrowser-3.2.0/tests/end2end/data/hints/angular1/angular.min.js`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/benchmark.html` & `qutebrowser-3.2.0/tests/end2end/data/hints/benchmark.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/bootstrap/bootstrap.css` & `qutebrowser-3.2.0/tests/end2end/data/hints/bootstrap/bootstrap.css`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/bootstrap/checkbox.html` & `qutebrowser-3.2.0/tests/end2end/data/hints/bootstrap/checkbox.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/html/target_blank_js.html` & `qutebrowser-3.2.0/tests/end2end/data/hints/html/target_blank_js.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/html/wrapped.html` & `qutebrowser-3.2.0/tests/end2end/data/hints/html/wrapped.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/html/wrapped_button.html` & `qutebrowser-3.2.0/tests/end2end/data/hints/html/wrapped_button.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/html/zoom_precision.html` & `qutebrowser-3.2.0/tests/end2end/data/hints/html/zoom_precision.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/input.html` & `qutebrowser-3.2.0/tests/end2end/data/hints/input.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/issue1186.html` & `qutebrowser-3.2.0/tests/end2end/data/hints/issue1186.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/issue1393.html` & `qutebrowser-3.2.0/tests/end2end/data/hints/issue1393.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/link_inject.html` & `qutebrowser-3.2.0/tests/end2end/data/hints/link_inject.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/link_input.html` & `qutebrowser-3.2.0/tests/end2end/data/hints/link_input.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/number.html` & `qutebrowser-3.2.0/tests/end2end/data/hints/number.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/hints/short_dict.html` & `qutebrowser-3.2.0/tests/end2end/data/hints/short_dict.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/insert_mode_settings/html/autofocus.html` & `qutebrowser-3.2.0/tests/end2end/data/insert_mode_settings/html/input.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 <!DOCTYPE html>
 <html>
     <head>
         <meta charset="utf-8">
-        <title>Inputs Autofocus</title>
+        <title>Input</title>
         <script type="text/javascript">
           function setup_event_listener() {
-              var elem = document.getElementById('qute-input-autofocus');
+              var elem = document.getElementById('qute-input');
               console.log(elem);
               elem.addEventListener('input', function() {
                   console.log("contents: " + elem.value);
               });
           }
         </script>
     </head>
     <body onload="setup_event_listener()">
-      <p>Some text.</p>
-      <input id="qute-input-autofocus" type="text" autofocus value=""/>
-      <input id="qute-input-disabled" disabled="disabled" href="#"/>
+        <p>Some text.</p>
+        <input id="qute-input" type="text" value=""/>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1,2 +1,2 @@
 Some text.
-[                    ][                    ]
+[                    ]
```

### Comparing `qutebrowser-3.1.0/tests/end2end/data/insert_mode_settings/html/input.html` & `qutebrowser-3.2.0/tests/end2end/data/insert_mode_settings/html/textarea.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 <!DOCTYPE html>
 <html>
     <head>
         <meta charset="utf-8">
-        <title>Input</title>
+        <title>Textarea</title>
         <script type="text/javascript">
           function setup_event_listener() {
-              var elem = document.getElementById('qute-input');
-              console.log(elem);
+              var elem = document.getElementById('qute-textarea');
               elem.addEventListener('input', function() {
                   console.log("contents: " + elem.value);
               });
           }
         </script>
     </head>
     <body onload="setup_event_listener()">
         <p>Some text.</p>
-        <input id="qute-input" type="text" value=""/>
+        <textarea id="qute-textarea"></textarea>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1,2 +1 @@
 Some text.
-[                    ]
```

### Comparing `qutebrowser-3.1.0/tests/end2end/data/insert_mode_settings/html/textarea.html` & `qutebrowser-3.2.0/tests/end2end/data/insert_mode_settings/html/autofocus.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 <!DOCTYPE html>
 <html>
     <head>
         <meta charset="utf-8">
-        <title>Textarea</title>
+        <title>Inputs Autofocus</title>
         <script type="text/javascript">
           function setup_event_listener() {
-              var elem = document.getElementById('qute-textarea');
+              var elem = document.getElementById('qute-input-autofocus');
+              console.log(elem);
               elem.addEventListener('input', function() {
                   console.log("contents: " + elem.value);
               });
+              elem.addEventListener('focus', function() {
+                  console.log("autofocus element focused");
+              });
           }
         </script>
     </head>
     <body onload="setup_event_listener()">
-        <p>Some text.</p>
-        <textarea id="qute-textarea"></textarea>
+      <p>Some text.</p>
+      <input id="qute-input-autofocus" type="text" autofocus value=""/>
+      <input id="qute-input-disabled" disabled="disabled" href="#"/>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1 +1,2 @@
 Some text.
+[                    ][                    ]
```

### Comparing `qutebrowser-3.1.0/tests/end2end/data/issue2569.html` & `qutebrowser-3.2.0/tests/end2end/data/issue2569.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/javascript/img/big.png` & `qutebrowser-3.2.0/tests/end2end/data/javascript/img/big.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/javascript/img/padded.png` & `qutebrowser-3.2.0/tests/end2end/data/javascript/img/padded.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/javascript/img/padded2.png` & `qutebrowser-3.2.0/tests/end2end/data/javascript/img/padded2.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/javascript/img/rgb.png` & `qutebrowser-3.2.0/tests/end2end/data/javascript/img/rgb.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/javascript/img/rgba.png` & `qutebrowser-3.2.0/tests/end2end/data/javascript/img/rgba.png`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/javascript/localstorage.html` & `qutebrowser-3.2.0/tests/end2end/data/javascript/localstorage.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/javascript/notifications.html` & `qutebrowser-3.2.0/tests/end2end/data/javascript/notifications.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/javascript/window_open.html` & `qutebrowser-3.2.0/tests/end2end/data/javascript/window_open.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/javascript/windowsize.html` & `qutebrowser-3.2.0/tests/end2end/data/javascript/windowsize.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/keyinput/log.html` & `qutebrowser-3.2.0/tests/end2end/data/keyinput/log.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/misc/hello.txt.html` & `qutebrowser-3.2.0/tests/end2end/data/misc/hello.txt.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/misc/qutescheme_csrf.html` & `qutebrowser-3.2.0/tests/end2end/data/misc/qutescheme_csrf.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/misc/test.pdf` & `qutebrowser-3.2.0/tests/end2end/data/misc/test.pdf`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/misc/xhr_headers.html` & `qutebrowser-3.2.0/tests/end2end/data/misc/xhr_headers.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/paste_primary.html` & `qutebrowser-3.2.0/tests/end2end/data/paste_primary.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/prefers_reduced_motion.html` & `qutebrowser-3.2.0/tests/end2end/data/prefers_reduced_motion.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/prompt/geolocation.html` & `qutebrowser-3.2.0/tests/end2end/data/prompt/geolocation.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/prompt/jsprompt.html` & `qutebrowser-3.2.0/tests/end2end/data/prompt/jsprompt.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/prompt/notifications.html` & `qutebrowser-3.2.0/tests/end2end/data/prompt/notifications.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/scroll/no_doctype.html` & `qutebrowser-3.2.0/tests/end2end/data/scroll/no_doctype.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/scroll/position_absolute.html` & `qutebrowser-3.2.0/tests/end2end/data/scroll/position_absolute.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/scroll/simple.html` & `qutebrowser-3.2.0/tests/end2end/data/scroll/simple.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/search.html` & `qutebrowser-3.2.0/tests/end2end/data/search.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/ssl/cert.csr` & `qutebrowser-3.2.0/tests/end2end/data/ssl/cert.csr`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/ssl/cert.pem` & `qutebrowser-3.2.0/tests/end2end/data/ssl/cert.pem`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/ssl/key.pem` & `qutebrowser-3.2.0/tests/end2end/data/ssl/key.pem`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/data/ssl/privkey.pem` & `qutebrowser-3.2.0/tests/end2end/data/ssl/privkey.pem`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/backforward.feature` & `qutebrowser-3.2.0/tests/end2end/features/backforward.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/caret.feature` & `qutebrowser-3.2.0/tests/end2end/features/caret.feature`

 * *Files 4% similar despite different names*

```diff
@@ -30,19 +30,19 @@
         And I run :move-to-end-of-word
         And I run :yank selection --sel
         Then the message "3 chars yanked to primary selection" should be shown
         And the primary selection should contain "one"
 
     Scenario: :yank selection with --keep
         When I run :selection-toggle
-        And I run :move-to-end-of-word
+        And I run :move-to-next-word
         And I run :yank selection --keep
         And I run :move-to-end-of-word
         And I run :yank selection --keep
-        Then the message "3 chars yanked to clipboard" should be shown
+        Then the message "4 chars yanked to clipboard" should be shown
         And the message "7 chars yanked to clipboard" should be shown
         And the clipboard should contain "one two"
 
     # :selection-follow
 
     Scenario: :selection-follow with --tab (with JS)
         When I set content.javascript.enabled to true
```

### Comparing `qutebrowser-3.1.0/tests/end2end/features/completion.feature` & `qutebrowser-3.2.0/tests/end2end/features/completion.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/conftest.py` & `qutebrowser-3.2.0/tests/end2end/features/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -680,16 +680,23 @@
 @bdd.then("qutebrowser should quit")
 def should_quit(qtbot, quteproc):
     quteproc.wait_for_quit()
 
 
 def _get_scroll_values(quteproc):
     data = quteproc.get_session()
-    pos = data['windows'][0]['tabs'][0]['history'][-1]['scroll-pos']
-    return (pos['x'], pos['y'])
+
+    def get_active(things):
+        return next(thing for thing in things if thing.get("active"))
+
+    active_window = get_active(data["windows"])
+    active_tab = get_active(active_window["tabs"])
+    current_entry = get_active(active_tab["history"])
+    pos = current_entry["scroll-pos"]
+    return (pos["x"], pos["y"])
 
 
 @bdd.then(bdd.parsers.re(r"the page should be scrolled "
                          r"(?P<direction>horizontally|vertically)"))
 def check_scrolled(quteproc, direction):
     quteproc.wait_scroll_pos_changed()
     x, y = _get_scroll_values(quteproc)
@@ -748,7 +755,13 @@
     files = files.replace('(dirsep)', os.sep)
     args += files.split(' ')
     if output_type == "a temporary file":
         args += ['--file={}']
     fileselect_cmd = json.dumps([cmd, *args])
     quteproc.set_setting('fileselect.handler', 'external')
     quteproc.set_setting(f'fileselect.{kind}.command', fileselect_cmd)
+
+
+@bdd.then(bdd.parsers.parse("I run {command}"))
+def run_command_then(quteproc, command):
+    """Run a qutebrowser command."""
+    quteproc.send_cmd(command)
```

### Comparing `qutebrowser-3.1.0/tests/end2end/features/downloads.feature` & `qutebrowser-3.2.0/tests/end2end/features/downloads.feature`

 * *Files 0% similar despite different names*

```diff
@@ -708,7 +708,8 @@
 
     Scenario: Using :prompt-fileselect-external with other prompt
         When I open data/prompt/jsprompt.html
         And I run :click-element id button
         And I wait for "Asking question *" in the log
         And I run :prompt-fileselect-external
         Then the error "Can only launch external fileselect for FilenamePrompt, not LineEditPrompt" should be shown
+        And I run :mode-leave
```

### Comparing `qutebrowser-3.1.0/tests/end2end/features/editor.feature` & `qutebrowser-3.2.0/tests/end2end/features/editor.feature`

 * *Files 0% similar despite different names*

```diff
@@ -184,14 +184,16 @@
 
     Scenario: Edit a command to be empty
         When I run :cmd-set-text :
         When I setup a fake editor returning empty text
         And I run :cmd-edit
         Then the error "command must start with one of :/?" should be shown
         And "Leaving mode KeyMode.command *" should not be logged
+        And I run :mode-leave
+        And "Leaving mode KeyMode.command *" should be logged
 
     ## select single file
 
     Scenario: Select one file with single file command
         When I setup a fake single_file fileselector selecting "tests/end2end/data/numbers/1.txt" and writes to a temporary file
         And I open data/fileselect.html
         And I run :click-element id single_file
```

### Comparing `qutebrowser-3.1.0/tests/end2end/features/hints.feature` & `qutebrowser-3.2.0/tests/end2end/features/hints.feature`

 * *Files 0% similar despite different names*

```diff
@@ -275,14 +275,15 @@
         # The actual check is already done above
         Then no crash should happen
 
     Scenario: Using :hint-follow inside a scrolled iframe
         When I open data/hints/iframe_scroll.html
         And I wait for "* simple loaded" in the log
         And I hint with args "all normal" and follow a
+        And I wait for "Clicked non-editable element!" in the log
         And I run :scroll bottom
         And I hint with args "links normal" and follow a
         Then "navigation request: url http://localhost:*/data/hello2.txt (current http://localhost:*/data/hints/iframe_scroll.html), type link_clicked, *" should be logged
 
     Scenario: Opening a link inside a specific iframe
         When I open data/hints/iframe_target.html
         And I hint with args "links normal" and follow a
```

### Comparing `qutebrowser-3.1.0/tests/end2end/features/history.feature` & `qutebrowser-3.2.0/tests/end2end/features/history.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/invoke.feature` & `qutebrowser-3.2.0/tests/end2end/features/invoke.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/javascript.feature` & `qutebrowser-3.2.0/tests/end2end/features/javascript.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/keyinput.feature` & `qutebrowser-3.2.0/tests/end2end/features/keyinput.feature`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
     Scenario: :fake-key with an unparsable key
         When I run :fake-key <blub>
         Then the error "Could not parse '<blub>': Got invalid key!" should be shown
 
     Scenario: :fake-key sending key to the website
         When I open data/keyinput/log.html
+        And I wait 0.01s
         And I run :fake-key x
         Then the javascript message "key press: 88" should be logged
         And the javascript message "key release: 88" should be logged
 
     @no_xvfb @posix @qtwebengine_skip
     Scenario: :fake-key sending key to the website with other window focused
         When I open data/keyinput/log.html
@@ -44,20 +45,22 @@
         And I run :fake-key x
         And I run :devtools
         And I wait for "Focus object changed: <qutebrowser.browser.webkit.webview.WebView *>" in the log
         Then the error "No focused webview!" should be shown
 
     Scenario: :fake-key sending special key to the website
         When I open data/keyinput/log.html
+        And I wait 0.01s
         And I run :fake-key <Escape>
         Then the javascript message "key press: 27" should be logged
         And the javascript message "key release: 27" should be logged
 
     Scenario: :fake-key sending keychain to the website
         When I open data/keyinput/log.html
+        And I wait 0.01s
         And I run :fake-key x<greater>y<less>" "
         Then the javascript message "key press: 88" should be logged
         And the javascript message "key release: 88" should be logged
         And the javascript message "key press: 190" should be logged
         And the javascript message "key release: 190" should be logged
         And the javascript message "key press: 89" should be logged
         And the javascript message "key release: 89" should be logged
```

### Comparing `qutebrowser-3.1.0/tests/end2end/features/marks.feature` & `qutebrowser-3.2.0/tests/end2end/features/marks.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/misc.feature` & `qutebrowser-3.2.0/tests/end2end/features/misc.feature`

 * *Files 0% similar despite different names*

```diff
@@ -498,22 +498,21 @@
     Scenario: Clicking an element with non-integer position
         When I open data/click_element.html
         And I run :click-element position 20,42.001
         Then the error "String 20,42.001 does not match X,Y" should be shown
 
     Scenario: Clicking on focused element when there is none
         When I open data/click_element.html
-        # Need to loose focus on input element
-        And I run :click-element position 20,42
-        And I wait for the javascript message "click_element position"
         And I run :click-element focused
         Then the error "No element found with focus!" should be shown
 
     Scenario: Clicking on focused element
         When I open data/click_element.html
+        And I run :jseval document.getElementById("qute-input").focus()
+        And I wait for the javascript message "qute-input focused"
         And I run :click-element focused
         Then "Entering mode KeyMode.insert (reason: clicking input)" should be logged
 
     ## :command-history-{prev,next}
 
     Scenario: Calling previous command
         When I run :cmd-set-text :message-info blah
```

### Comparing `qutebrowser-3.1.0/tests/end2end/features/navigate.feature` & `qutebrowser-3.2.0/tests/end2end/features/navigate.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/notifications.feature` & `qutebrowser-3.2.0/tests/end2end/features/notifications.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/open.feature` & `qutebrowser-3.2.0/tests/end2end/features/open.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/private.feature` & `qutebrowser-3.2.0/tests/end2end/features/private.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/prompts.feature` & `qutebrowser-3.2.0/tests/end2end/features/prompts.feature`

 * *Files 0% similar despite different names*

```diff
@@ -409,15 +409,15 @@
         Then the json on the page should be:
             {
               "authenticated": true,
               "user": "user4"
             }
 
     @qtwebengine_skip
-    Scenario: Cancellling webpage authentication with QtWebKit
+    Scenario: Cancelling webpage authentication with QtWebKit
         When I open basic-auth/user6/password6 without waiting
         And I wait for a prompt
         And I run :mode-leave
         Then basic-auth/user6/password6 should be loaded
 
     # :prompt-accept with value argument
```

### Comparing `qutebrowser-3.1.0/tests/end2end/features/qutescheme.feature` & `qutebrowser-3.2.0/tests/end2end/features/qutescheme.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/scroll.feature` & `qutebrowser-3.2.0/tests/end2end/features/scroll.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/search.feature` & `qutebrowser-3.2.0/tests/end2end/features/search.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/sessions.feature` & `qutebrowser-3.2.0/tests/end2end/features/sessions.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/spawn.feature` & `qutebrowser-3.2.0/tests/end2end/features/spawn.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/tabs.feature` & `qutebrowser-3.2.0/tests/end2end/features/tabs.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_downloads_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_downloads_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_editor_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_editor_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_hints_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_hints_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_history_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_history_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_invoke_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_invoke_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_javascript_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_javascript_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_marks_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_marks_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_misc_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_misc_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_notifications_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_notifications_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_open_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_open_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_private_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_private_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_prompts_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_prompts_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_qutescheme_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_qutescheme_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_search_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_search_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_sessions_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_sessions_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_urlmarks_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_urlmarks_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/test_yankpaste_bdd.py` & `qutebrowser-3.2.0/tests/end2end/features/test_yankpaste_bdd.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/urlmarks.feature` & `qutebrowser-3.2.0/tests/end2end/features/urlmarks.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/utilcmds.feature` & `qutebrowser-3.2.0/tests/end2end/features/utilcmds.feature`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Feature: Miscellaneous utility commands exposed to the user.
 
     Background:
         Given I open data/scroll/simple.html
         And I run :tab-only
+        And I run :window-only
 
     ## :cmd-later
 
     Scenario: :cmd-later before
         When I run :cmd-later 500 scroll down
         Then the page should not be scrolled
         # wait for scroll to execute so we don't ruin our future
```

### Comparing `qutebrowser-3.1.0/tests/end2end/features/yankpaste.feature` & `qutebrowser-3.2.0/tests/end2end/features/yankpaste.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/features/zoom.feature` & `qutebrowser-3.2.0/tests/end2end/features/zoom.feature`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/fixtures/notificationserver.py` & `qutebrowser-3.2.0/tests/end2end/fixtures/notificationserver.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/fixtures/quteprocess.py` & `qutebrowser-3.2.0/tests/end2end/fixtures/quteprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,23 @@
 
         # Qt 6.6 on GitHub Actions
         (
             'libva error: vaGetDriverNameByIndex() failed with unknown libva error, '
             'driver_name = (null)'
         ),
         'libva error: vaGetDriverNames() failed with unknown libva error',
+
+        # Mesa 23.3
+        # See https://gitlab.freedesktop.org/mesa/mesa/-/issues/10293
+        'MESA: error: ZINK: vkCreateInstance failed (VK_ERROR_INCOMPATIBLE_DRIVER)',
+        'glx: failed to create drisw screen',
+        'failed to load driver: zink',
+        'DRI3 not available',
+        # Webkit on arch with a newer mesa
+        'MESA: error: ZINK: failed to load libvulkan.so.1',
     ]
     return any(testutils.pattern_match(pattern=pattern, value=message)
                for pattern in ignored_messages)
 
 
 def is_ignored_chromium_message(line):
     msg_re = re.compile(r"""
@@ -202,14 +211,24 @@
         # [5718:5718:0318/031330.803863:ERROR:interface_endpoint_client.cc(687)] Message 3 rejected by interface blink.mojom.Widget
         "Message * rejected by interface blink.mojom.Widget*",
 
         # GitHub Actions, Qt 6.6
         # [9895:9983:0904/043039.500565:ERROR:gpu_memory_buffer_support_x11.cc(49)]
         # dri3 extension not supported.
         "dri3 extension not supported.",
+
+        # Qt 6.7 debug build
+        # [44513:44717:0325/173456.146759:WARNING:render_message_filter.cc(144)]
+        # Could not find tid
+        "Could not find tid",
+
+        # [127693:127748:0325/230155.835421:WARNING:discardable_shared_memory_manager.cc(438)]
+        # Some MojoDiscardableSharedMemoryManagerImpls are still alive. They
+        # will be leaked.
+        "Some MojoDiscardableSharedMemoryManagerImpls are still alive. They will be leaked.",
     ]
     return any(testutils.pattern_match(pattern=pattern, value=message)
                for pattern in ignored_messages)
 
 
 class LogLine(testprocess.Line):
 
@@ -384,17 +403,19 @@
                 args = ['-bb', '-m', 'qutebrowser']
         return executable, args
 
     def _default_args(self):
         backend = 'webengine' if self.request.config.webengine else 'webkit'
         args = ['--debug', '--no-err-windows', '--temp-basedir',
                 '--json-logging', '--loglevel', 'vdebug',
-                '--backend', backend, '--debug-flag', 'no-sql-history',
-                '--debug-flag', 'werror', '--debug-flag',
-                'test-notification-service',
+                '--backend', backend,
+                '--debug-flag', 'no-sql-history',
+                '--debug-flag', 'werror',
+                '--debug-flag', 'test-notification-service',
+                '--debug-flag', 'caret',
                 '--qt-flag', 'disable-features=PaintHoldingCrossOrigin']
 
         if self.request.config.webengine and testutils.disable_seccomp_bpf_sandbox():
             args += testutils.DISABLE_SECCOMP_BPF_ARGS
 
         args.append('about:blank')
         return args
```

### Comparing `qutebrowser-3.1.0/tests/end2end/fixtures/test_quteprocess.py` & `qutebrowser-3.2.0/tests/end2end/fixtures/test_quteprocess.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/fixtures/test_testprocess.py` & `qutebrowser-3.2.0/tests/end2end/fixtures/test_testprocess.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/fixtures/test_webserver.py` & `qutebrowser-3.2.0/tests/end2end/fixtures/test_webserver.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/fixtures/testprocess.py` & `qutebrowser-3.2.0/tests/end2end/fixtures/testprocess.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/fixtures/webserver.py` & `qutebrowser-3.2.0/tests/end2end/fixtures/webserver.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import dataclasses
 from http import HTTPStatus
 
 import pytest
 from qutebrowser.qt.core import pyqtSignal, QUrl
 
 from end2end.fixtures import testprocess
+from helpers import testutils
 
 
 class Request(testprocess.Line):
 
     """A parsed line from the flask log output.
 
     Attributes:
@@ -107,14 +108,25 @@
     def __eq__(self, other):
         if isinstance(other, (Request, ExpectedRequest)):
             return self.verb == other.verb and self.path == other.path
         else:
             return NotImplemented
 
 
+def is_ignored_webserver_message(line: str) -> bool:
+    return testutils.pattern_match(
+        pattern=(
+            "Client ('127.0.0.1', *) lost * peer dropped the TLS connection suddenly, "
+            "during handshake: (1, '[SSL: SSLV3_ALERT_CERTIFICATE_UNKNOWN] * "
+            "alert certificate unknown (_ssl.c:*)')"
+        ),
+        value=line,
+    )
+
+
 class WebserverProcess(testprocess.Process):
 
     """Abstraction over a running Flask server process.
 
     Reads the log from its stdout and parses it.
 
     Signals:
@@ -147,15 +159,21 @@
     def _parse_line(self, line):
         self._log(line)
         started_re = re.compile(r' \* Running on https?://127\.0\.0\.1:{}/? '
                                 r'\(Press CTRL\+C to quit\)'.format(self.port))
         if started_re.fullmatch(line):
             self.ready.emit()
             return None
-        return Request(line)
+
+        try:
+            return Request(line)
+        except testprocess.InvalidLine:
+            if is_ignored_webserver_message(line):
+                return None
+            raise
 
     def _executable_args(self):
         if hasattr(sys, 'frozen'):
             executable = str(pathlib.Path(sys.executable).parent / self._script)
             args = []
         else:
             executable = sys.executable
```

### Comparing `qutebrowser-3.1.0/tests/end2end/fixtures/webserver_sub.py` & `qutebrowser-3.2.0/tests/end2end/fixtures/webserver_sub.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/fixtures/webserver_sub_ssl.py` & `qutebrowser-3.2.0/tests/end2end/fixtures/webserver_sub_ssl.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/misc/test_runners_e2e.py` & `qutebrowser-3.2.0/tests/end2end/misc/test_runners_e2e.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/test_adblock_e2e.py` & `qutebrowser-3.2.0/tests/end2end/test_adblock_e2e.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/test_dirbrowser.py` & `qutebrowser-3.2.0/tests/end2end/test_dirbrowser.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/test_hints_html.py` & `qutebrowser-3.2.0/tests/end2end/test_hints_html.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/end2end/test_insert_mode.py` & `qutebrowser-3.2.0/tests/end2end/test_insert_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
 
 @pytest.mark.parametrize('auto_load, background, insert_mode', [
     (False, False, False),  # auto_load disabled
     (True, False, True),  # enabled and foreground tab
     (True, True, False),  # background tab
 ])
-@pytest.mark.flaky
 def test_auto_load(quteproc, auto_load, background, insert_mode):
     quteproc.set_setting('input.insert_mode.auto_load', str(auto_load))
     url_path = 'data/insert_mode_settings/html/autofocus.html'
     quteproc.open_path(url_path, new_bg_tab=background)
 
     log_message = 'Entering mode KeyMode.insert (reason: *)'
     if insert_mode:
```

### Comparing `qutebrowser-3.1.0/tests/end2end/test_invocations.py` & `qutebrowser-3.2.0/tests/end2end/test_invocations.py`

 * *Files 1% similar despite different names*

```diff
@@ -901,14 +901,15 @@
             "PID namespaces": "Yes" if has_namespaces else "No",
             "Network namespaces": "Yes" if has_namespaces else "No",
 
             bpf_text: "Yes" if has_seccomp else "No",
             f"{bpf_text} supports TSYNC": "Yes" if has_seccomp else "No",
 
             f"{yama_text} (Broker)": "Yes" if has_yama else "No",
+            # pylint: disable-next=used-before-assignment
             f"{yama_text} (Non-broker)": "Yes" if has_yama_non_broker else "No",
         }
 
         assert header == "Sandbox Status"
         assert result == expected_result
 
         status = dict(line.split("\t") for line in lines)
```

### Comparing `qutebrowser-3.1.0/tests/end2end/test_mhtml_e2e.py` & `qutebrowser-3.2.0/tests/end2end/test_mhtml_e2e.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/helpers/fixtures.py` & `qutebrowser-3.2.0/tests/helpers/fixtures.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/helpers/logfail.py` & `qutebrowser-3.2.0/tests/helpers/logfail.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/helpers/messagemock.py` & `qutebrowser-3.2.0/tests/helpers/messagemock.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/helpers/stubs.py` & `qutebrowser-3.2.0/tests/helpers/stubs.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/helpers/test_helper_utils.py` & `qutebrowser-3.2.0/tests/helpers/test_helper_utils.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/helpers/test_logfail.py` & `qutebrowser-3.2.0/tests/helpers/test_logfail.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/helpers/test_stubs.py` & `qutebrowser-3.2.0/tests/helpers/test_stubs.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/helpers/testutils.py` & `qutebrowser-3.2.0/tests/helpers/testutils.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/manual/hints/find_implementation.html` & `qutebrowser-3.2.0/tests/manual/hints/find_implementation.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/manual/hints/hide_unmatched_rapid_hints.html` & `qutebrowser-3.2.0/tests/manual/hints/hide_unmatched_rapid_hints.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/manual/hints/other.html` & `qutebrowser-3.2.0/tests/manual/hints/other.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/manual/history/visited.html` & `qutebrowser-3.2.0/tests/manual/history/visited.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/manual/mouse.html` & `qutebrowser-3.2.0/tests/manual/mouse.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/test_conftest.py` & `qutebrowser-3.2.0/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/api/test_cmdutils.py` & `qutebrowser-3.2.0/tests/unit/api/test_cmdutils.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/test_browsertab.py` & `qutebrowser-3.2.0/tests/unit/browser/test_browsertab.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/test_caret.py` & `qutebrowser-3.2.0/tests/unit/browser/test_caret.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 """Tests for caret browsing mode."""
 
 import textwrap
 
 import pytest
 from qutebrowser.qt.core import QUrl
 
-from qutebrowser.utils import usertypes
+from qutebrowser.qt import machinery
+from qutebrowser.utils import utils, usertypes
 from qutebrowser.browser import browsertab
 
 
 @pytest.fixture
 def caret(web_tab, qtbot, mode_manager):
     web_tab.container.expose()
 
@@ -237,14 +238,21 @@
 class TestWord:
 
     def test_selecting_a_word(self, caret, selection):
         selection.toggle()
         caret.move_to_end_of_word()
         selection.check("one")
 
+    @pytest.mark.xfail(
+        machinery.IS_QT6 and utils.is_windows,
+        reason=(
+            "move-to-end-of-word is broken with Qt 6 and Windows: "
+            "https://github.com/qutebrowser/qutebrowser/issues/8146"
+        )
+    )
     def test_moving_to_end_and_selecting_a_word(self, caret, selection):
         caret.move_to_end_of_word()
         selection.toggle()
         caret.move_to_end_of_word()
         selection.check(" two")
 
     def test_moving_to_next_word_and_selecting_a_word(self, caret, selection):
```

### Comparing `qutebrowser-3.1.0/tests/unit/browser/test_downloads.py` & `qutebrowser-3.2.0/tests/unit/browser/test_downloads.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/test_downloadview.py` & `qutebrowser-3.2.0/tests/unit/browser/test_downloadview.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/test_hints.py` & `qutebrowser-3.2.0/tests/unit/browser/test_hints.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/test_history.py` & `qutebrowser-3.2.0/tests/unit/browser/test_history.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/test_inspector.py` & `qutebrowser-3.2.0/tests/unit/browser/test_inspector.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/test_navigate.py` & `qutebrowser-3.2.0/tests/unit/browser/test_navigate.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/test_notification.py` & `qutebrowser-3.2.0/tests/unit/browser/test_notification.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/test_pdfjs.py` & `qutebrowser-3.2.0/tests/unit/browser/test_pdfjs.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import os.path
 
 import pytest
 from qutebrowser.qt.core import QUrl
 
 from qutebrowser.browser import pdfjs
-from qutebrowser.utils import urlmatch
+from qutebrowser.utils import urlmatch, utils
 
 
 pytestmark = [pytest.mark.usefixtures('data_tmpdir')]
 
 
 @pytest.mark.parametrize('available, snippet', [
     (True, '<title>PDF.js viewer</title>'),
@@ -150,14 +150,16 @@
 
     if expected_name == 'one':
         expected = (b'text1', str(file1))
     elif expected_name == 'two':
         expected = (b'text2', str(file2))
     elif expected_name is None:
         expected = (None, None)
+    else:
+        raise utils.Unreachable(expected_name)
 
     assert pdfjs._read_from_system(str(tmpdir), names) == expected
 
 
 @pytest.fixture
 def unreadable_file(tmpdir):
     unreadable_file = tmpdir / 'unreadable'
```

### Comparing `qutebrowser-3.1.0/tests/unit/browser/test_qutescheme.py` & `qutebrowser-3.2.0/tests/unit/browser/test_qutescheme.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/test_shared.py` & `qutebrowser-3.2.0/tests/unit/browser/test_shared.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/test_signalfilter.py` & `qutebrowser-3.2.0/tests/unit/browser/test_signalfilter.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/test_urlmarks.py` & `qutebrowser-3.2.0/tests/unit/browser/test_urlmarks.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webengine/test_spell.py` & `qutebrowser-3.2.0/tests/unit/browser/webengine/test_spell.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webengine/test_webengine_cookies.py` & `qutebrowser-3.2.0/tests/unit/browser/webengine/test_webengine_cookies.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webengine/test_webenginedownloads.py` & `qutebrowser-3.2.0/tests/unit/browser/webengine/test_webenginedownloads.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webengine/test_webengineinterceptor.py` & `qutebrowser-3.2.0/tests/unit/browser/webengine/test_webengineinterceptor.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webengine/test_webenginesettings.py` & `qutebrowser-3.2.0/tests/unit/browser/webengine/test_webenginesettings.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webengine/test_webenginetab.py` & `qutebrowser-3.2.0/tests/unit/browser/webengine/test_webenginetab.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webengine/test_webview.py` & `qutebrowser-3.2.0/tests/unit/browser/webengine/test_webview.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webkit/http/test_content_disposition.py` & `qutebrowser-3.2.0/tests/unit/browser/webkit/http/test_content_disposition.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import logging
 
 import pytest
 
-from qutebrowser.browser.webkit import http
+from qutebrowser.browser.webkit import httpheaders
 
 
 DEFAULT_NAME = 'qutebrowser-download'
 _STDLIB_XFAIL = pytest.mark.xfail(reason="Not handled properly by Python stdlib")
 
 
 class HeaderChecker:
@@ -26,33 +26,33 @@
         self.caplog = caplog
         self.stubs = stubs
 
     def check_filename(self, header, filename, expected_inline=False):
         """Check if the passed header has the given filename."""
         reply = self.stubs.FakeNetworkReply(
             headers={'Content-Disposition': header})
-        cd_inline, cd_filename = http.parse_content_disposition(reply)
+        cd_inline, cd_filename = httpheaders.parse_content_disposition(reply)
         assert cd_filename is not None
         assert cd_filename == filename
         assert cd_inline == expected_inline
 
     def check_ignored(self, header):
         """Check if the passed header is ignored."""
         reply = self.stubs.FakeNetworkReply(
             headers={'Content-Disposition': header})
         with self.caplog.at_level(logging.ERROR, 'network'):
-            cd_inline, cd_filename = http.parse_content_disposition(reply)
+            cd_inline, cd_filename = httpheaders.parse_content_disposition(reply)
         assert cd_filename == DEFAULT_NAME
         assert cd_inline
 
     def check_unnamed(self, header):
         """Check if the passed header results in an unnamed attachment."""
         reply = self.stubs.FakeNetworkReply(
             headers={'Content-Disposition': header})
-        cd_inline, cd_filename = http.parse_content_disposition(reply)
+        cd_inline, cd_filename = httpheaders.parse_content_disposition(reply)
         assert cd_filename == DEFAULT_NAME
         assert not cd_inline
 
 
 @pytest.fixture
 def header_checker(caplog, stubs):
     """Fixture that provides a HeaderChecker class for tests"""
@@ -160,15 +160,15 @@
     def test_attonly(self, stubs):
         """'attachment' only.
 
         UA should offer to download the resource.
         """
         reply = stubs.FakeNetworkReply(
             headers={'Content-Disposition': 'attachment'})
-        cd_inline, cd_filename = http.parse_content_disposition(reply)
+        cd_inline, cd_filename = httpheaders.parse_content_disposition(reply)
         assert not cd_inline
         assert cd_filename == DEFAULT_NAME
 
     def test_attonlyquoted(self, header_checker):
         """'attachment' only, using double quotes
 
         This is invalid syntax, thus the header should be ignored.
```

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webkit/http/test_http.py` & `qutebrowser-3.2.0/tests/unit/browser/webkit/http/test_httpheaders.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # SPDX-FileCopyrightText: Florian Bruhin (The Compiler) <mail@qutebrowser.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-"""Tests for qutebrowser.browser.webkit.http."""
+"""Tests for qutebrowser.browser.webkit.httpheaders."""
 
 import logging
 
 import pytest
 import hypothesis
 from hypothesis import strategies
 from qutebrowser.qt.core import QUrl
 
-from qutebrowser.browser.webkit import http
+from qutebrowser.browser.webkit import httpheaders
 
 
 @pytest.mark.parametrize('url, expected', [
     # Filename in the URL
     ('http://example.com/path', 'path'),
     ('http://example.com/foo/path', 'path'),
     # No filename at all
     ('http://example.com', 'qutebrowser-download'),
     ('http://example.com/', 'qutebrowser-download'),
 ])
 def test_no_content_disposition(stubs, url, expected):
     reply = stubs.FakeNetworkReply(url=QUrl(url))
-    inline, filename = http.parse_content_disposition(reply)
+    inline, filename = httpheaders.parse_content_disposition(reply)
     assert inline
     assert filename == expected
 
 
 @pytest.mark.parametrize('value', [
     # https://github.com/python/cpython/issues/87112
     'inline; 0*²'.encode("iso-8859-1"),
@@ -36,16 +36,16 @@
     b'"',
     # https://github.com/python/cpython/issues/93010
     b'attachment; 0*00="foo"',
     # FIXME: Should probably have more tests if this is still relevant after
     # dropping QtWebKit.
 ])
 def test_parse_content_disposition_invalid(value):
-    with pytest.raises(http.ContentDispositionError):
-        http.ContentDisposition.parse(value)
+    with pytest.raises(httpheaders.ContentDispositionError):
+        httpheaders.ContentDisposition.parse(value)
 
 
 @pytest.mark.parametrize('template', [
     '{}',
     'attachment; filename="{}"',
     'inline; {}',
     'attachment; {}="foo"',
@@ -54,24 +54,24 @@
 ])
 @hypothesis.given(strategies.text(alphabet=[chr(x) for x in range(255)]))
 def test_parse_content_disposition_hypothesis(caplog, template, stubs, s):
     """Test parsing headers based on templates which hypothesis completes."""
     header = template.format(s)
     reply = stubs.FakeNetworkReply(headers={'Content-Disposition': header})
     with caplog.at_level(logging.ERROR, 'network'):
-        http.parse_content_disposition(reply)
+        httpheaders.parse_content_disposition(reply)
 
 
 @hypothesis.given(strategies.binary())
 def test_content_disposition_directly_hypothesis(s):
     """Test rfc6266 parsing directly with binary data."""
     try:
-        cd = http.ContentDisposition.parse(s)
+        cd = httpheaders.ContentDisposition.parse(s)
         cd.filename()
-    except http.ContentDispositionError:
+    except httpheaders.ContentDispositionError:
         pass
 
 
 @pytest.mark.parametrize('content_type, expected_mimetype, expected_rest', [
     (None, None, None),
     ('image/example', 'image/example', None),
     ('', '', None),
@@ -79,16 +79,16 @@
 ])
 def test_parse_content_type(stubs, content_type, expected_mimetype,
                             expected_rest):
     if content_type is None:
         reply = stubs.FakeNetworkReply()
     else:
         reply = stubs.FakeNetworkReply(headers={'Content-Type': content_type})
-    mimetype, rest = http.parse_content_type(reply)
+    mimetype, rest = httpheaders.parse_content_type(reply)
     assert mimetype == expected_mimetype
     assert rest == expected_rest
 
 
 @hypothesis.given(strategies.text())
 def test_parse_content_type_hypothesis(stubs, s):
     reply = stubs.FakeNetworkReply(headers={'Content-Type': s})
-    http.parse_content_type(reply)
+    httpheaders.parse_content_type(reply)
```

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webkit/network/test_filescheme.py` & `qutebrowser-3.2.0/tests/unit/browser/webkit/network/test_filescheme.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webkit/network/test_networkmanager.py` & `qutebrowser-3.2.0/tests/unit/browser/webkit/network/test_networkmanager.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webkit/network/test_networkreply.py` & `qutebrowser-3.2.0/tests/unit/browser/webkit/network/test_networkreply.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webkit/network/test_pac.py` & `qutebrowser-3.2.0/tests/unit/browser/webkit/network/test_pac.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webkit/test_cache.py` & `qutebrowser-3.2.0/tests/unit/browser/webkit/test_cache.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webkit/test_certificateerror.py` & `qutebrowser-3.2.0/tests/unit/browser/webkit/test_certificateerror.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,47 +14,48 @@
     def __init__(self, msg):
         self.msg = msg
 
     def errorString(self):
         return self.msg
 
 
-@pytest.mark.parametrize('errors, expected', [
+@pytest.mark.parametrize('error_factories, expected', [
     (
-        [QSslError(QSslError.SslError.UnableToGetIssuerCertificate)],
+        [lambda: QSslError(QSslError.SslError.UnableToGetIssuerCertificate)],
         ['<p>The issuer certificate could not be found</p>'],
     ),
     (
         [
-            QSslError(QSslError.SslError.UnableToGetIssuerCertificate),
-            QSslError(QSslError.SslError.UnableToDecryptCertificateSignature),
+            lambda: QSslError(QSslError.SslError.UnableToGetIssuerCertificate),
+            lambda: QSslError(QSslError.SslError.UnableToDecryptCertificateSignature),
         ],
         [
             '<ul>',
             '<li>The issuer certificate could not be found</li>',
             '<li>The certificate signature could not be decrypted</li>',
             '</ul>',
         ],
     ),
 
     (
-        [FakeError('Escaping test: <>')],
+        [lambda: FakeError('Escaping test: <>')],
         ['<p>Escaping test: &lt;&gt;</p>'],
     ),
     (
         [
-            FakeError('Escaping test 1: <>'),
-            FakeError('Escaping test 2: <>'),
+            lambda: FakeError('Escaping test 1: <>'),
+            lambda: FakeError('Escaping test 2: <>'),
         ],
         [
             '<ul>',
             '<li>Escaping test 1: &lt;&gt;</li>',
             '<li>Escaping test 2: &lt;&gt;</li>',
             '</ul>',
         ],
     ),
 ])
-def test_html(stubs, errors, expected):
+def test_html(stubs, error_factories, expected):
     reply = stubs.FakeNetworkReply(url=QUrl("https://example.com"))
+    errors = [factory() for factory in error_factories]
     wrapper = certificateerror.CertificateErrorWrapper(reply=reply, errors=errors)
     lines = [line.strip() for line in wrapper.html().splitlines() if line.strip()]
     assert lines == expected
```

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webkit/test_cookies.py` & `qutebrowser-3.2.0/tests/unit/browser/webkit/test_cookies.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webkit/test_mhtml.py` & `qutebrowser-3.2.0/tests/unit/browser/webkit/test_mhtml.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webkit/test_tabhistory.py` & `qutebrowser-3.2.0/tests/unit/browser/webkit/test_tabhistory.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/browser/webkit/test_webkitelem.py` & `qutebrowser-3.2.0/tests/unit/browser/webkit/test_webkitelem.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/commands/test_argparser.py` & `qutebrowser-3.2.0/tests/unit/commands/test_argparser.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/commands/test_cmdexc.py` & `qutebrowser-3.2.0/tests/unit/commands/test_cmdexc.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/commands/test_parser.py` & `qutebrowser-3.2.0/tests/unit/commands/test_parser.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/commands/test_userscripts.py` & `qutebrowser-3.2.0/tests/unit/commands/test_userscripts.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/completion/test_completer.py` & `qutebrowser-3.2.0/tests/unit/completion/test_completer.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     return CompletionWidgetStub()
 
 
 @pytest.fixture
 def completer_obj(qtbot, status_command_stub, config_stub, monkeypatch, stubs,
                   completion_widget_stub):
     """Create the completer used for testing."""
-    monkeypatch.setattr(completer, 'QTimer', stubs.InstaTimer)
+    monkeypatch.setattr(completer.usertypes, 'Timer', stubs.InstaTimer)
     config_stub.val.completion.show = 'auto'
     return completer.Completer(cmd=status_command_stub, win_id=0,
                                parent=completion_widget_stub)
 
 
 @pytest.fixture(autouse=True)
 def miscmodels_patch(mocker):
```

### Comparing `qutebrowser-3.1.0/tests/unit/completion/test_completiondelegate.py` & `qutebrowser-3.2.0/tests/unit/completion/test_completiondelegate.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/completion/test_completionmodel.py` & `qutebrowser-3.2.0/tests/unit/completion/test_completionmodel.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/completion/test_completionwidget.py` & `qutebrowser-3.2.0/tests/unit/completion/test_completionwidget.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Tests for the CompletionView Object."""
 
 from unittest import mock
 
 import pytest
-from qutebrowser.qt.core import QRect
+from qutebrowser.qt.core import QRect, QItemSelectionModel
 
 from qutebrowser.completion import completionwidget
 from qutebrowser.completion.models import completionmodel, listcategory
 from qutebrowser.api import cmdutils
 
 
 @pytest.fixture
@@ -281,14 +281,31 @@
                 not (quick_complete and len(rows) == 1))
     assert completionview.isVisible() == expected
     completionview.set_model(None)
     completionview.completion_item_focus('next')
     assert not completionview.isVisible()
 
 
+def test_completion_selection_clear_no_model(completionview):
+    completionview.show()
+    completionview.on_clear_completion_selection()
+    assert completionview.isVisible() is False
+
+
+def test_completion_selection_clear_with_model(completionview, mocker):
+    selmod = mock.Mock(spec=QItemSelectionModel)
+    mocker.patch.object(completionview, "selectionModel", return_value=selmod)
+    completionview.show()
+    completionview.on_clear_completion_selection()
+
+    assert completionview.isVisible() is False
+    selmod.clearSelection.assert_called_once()
+    selmod.clearCurrentIndex.assert_called_once()
+
+
 def test_completion_item_del(completionview, model):
     """Test that completion_item_del invokes delete_cur_item in the model."""
     func = mock.Mock(spec=[])
     cat = listcategory.ListCategory('', [('foo', 'bar')], delete_func=func)
     model.add_category(cat)
     completionview.set_model(model)
     completionview.completion_item_focus('next')
```

### Comparing `qutebrowser-3.1.0/tests/unit/completion/test_histcategory.py` & `qutebrowser-3.2.0/tests/unit/completion/test_histcategory.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/completion/test_listcategory.py` & `qutebrowser-3.2.0/tests/unit/completion/test_listcategory.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,19 @@
      [('foobar', ''), ('foobaz', ''), ('barfoo', '')],
      [('foobaz', ''), ('foobar', ''), ('barfoo', '')]),
 
     ('foo',
      [('foo', 'bar'), ('bar', 'foo'), ('bar', 'bar')],
      [('foo', 'bar'), ('bar', 'foo')],
      [('foo', 'bar'), ('bar', 'foo')]),
+
+    ('foo bar',
+     [('foobar', ''), ('barfoo', ''), ('foobaz', '')],
+     [('barfoo', ''), ('foobar', '')],
+     [('foobar', ''), ('barfoo', '')]),
 ])
 def test_set_pattern(pattern, before, after, after_nosort, model_validator):
     """Validate the filtering and sorting results of set_pattern."""
     cat = listcategory.ListCategory('Foo', before)
     model_validator.set_model(cat)
     cat.set_pattern(pattern)
     model_validator.validate(after)
```

### Comparing `qutebrowser-3.1.0/tests/unit/completion/test_models.py` & `qutebrowser-3.2.0/tests/unit/completion/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     pass
 
 from qutebrowser.misc import objects, guiprocess
 from qutebrowser.completion import completer
 from qutebrowser.completion.models import (
     configmodel, listcategory, miscmodels, urlmodel, filepathcategory)
 from qutebrowser.config import configdata, configtypes
-from qutebrowser.utils import usertypes
+from qutebrowser.utils import usertypes, utils
 from qutebrowser.mainwindow import tabbedbrowser
 
 
 def _check_completions(model, expected):
     """Check that a model contains the expected items in order.
 
     Args:
@@ -413,14 +413,16 @@
         monkeypatch.setenv('HOME', homedir)  # POSIX
         monkeypatch.setenv('USERPROFILE', homedir)  # Windows
         assert str(pathlib.Path.home()) == homedir
 
         base = '~'
         expected_1 = str(pathlib.Path('~') / 'file1.txt')
         expected_2 = str(pathlib.Path('~') / 'file2.txt')
+    else:
+        raise utils.Unreachable(method)
 
     config_stub.val.completion.open_categories = ['filesystem']
     model = urlmodel.url(info=info)
     model.set_pattern(base + os.sep)
     qtmodeltester.check(model)
 
     _check_completions(model, {
@@ -1306,30 +1308,31 @@
         'url': ['http://example.com/{}'.format(i) for i in r],
         'title': ['title{}'.format(i) for i in r]
     }
 
     web_history.completion.insert_batch(entries)
 
     quickmark_manager_stub.marks = collections.OrderedDict([
-        ('title{}'.format(i), 'example.com/{}'.format(i))
+        ('title{}'.format('a'*i), 'example.com/{}'.format(i))
         for i in range(1000)])
 
     bookmark_manager_stub.marks = collections.OrderedDict([
-        ('example.com/{}'.format(i), 'title{}'.format(i))
+        ('example.com/{}'.format('a'*i), 'title{}'.format(i))
         for i in range(1000)])
 
     def bench():
         model = urlmodel.url(info=info)
         model.set_pattern('')
         model.set_pattern('e')
         model.set_pattern('ex')
         model.set_pattern('ex ')
         model.set_pattern('ex 1')
         model.set_pattern('ex 12')
         model.set_pattern('ex 123')
+        model.set_pattern('zzzzz')  # no match
 
     benchmark(bench)
 
 
 @pytest.fixture
 def tab_with_history(fake_web_tab, tabbed_browser_stubs, info, monkeypatch):
     """Returns a fake tab with some fake history items."""
```

### Comparing `qutebrowser-3.1.0/tests/unit/components/test_blockutils.py` & `qutebrowser-3.2.0/tests/unit/components/test_blockutils.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/components/test_braveadblock.py` & `qutebrowser-3.2.0/tests/unit/components/test_braveadblock.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/components/test_hostblock.py` & `qutebrowser-3.2.0/tests/unit/components/test_hostblock.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/components/test_misccommands.py` & `qutebrowser-3.2.0/tests/unit/components/test_misccommands.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/components/test_readlinecommands.py` & `qutebrowser-3.2.0/tests/unit/components/test_readlinecommands.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/config/test_config.py` & `qutebrowser-3.2.0/tests/unit/config/test_config.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/config/test_configcache.py` & `qutebrowser-3.2.0/tests/unit/config/test_configcache.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/config/test_configcommands.py` & `qutebrowser-3.2.0/tests/unit/config/test_configcommands.py`

 * *Files 0% similar despite different names*

```diff
@@ -836,14 +836,16 @@
 
         Should show an error.
         """
         if command == 'bind':
             func = functools.partial(commands.bind, 0)
         elif command == 'unbind':
             func = commands.unbind
+        else:
+            raise utils.Unreachable(command)
 
         with pytest.raises(cmdutils.CommandError, match=expected):
             func(*args, **kwargs)
 
     @pytest.mark.parametrize('key', ['a', 'b', '<Ctrl-X>'])
     def test_bind_duplicate(self, commands, config_stub, key_config_stub, key):
         """Run ':bind' with a key which already has been bound.'.
```

### Comparing `qutebrowser-3.1.0/tests/unit/config/test_configdata.py` & `qutebrowser-3.2.0/tests/unit/config/test_configdata.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/config/test_configexc.py` & `qutebrowser-3.2.0/tests/unit/config/test_configexc.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/config/test_configfiles.py` & `qutebrowser-3.2.0/tests/unit/config/test_configfiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,14 +395,15 @@
 
         if insert:
             yaml.set_obj('tabs.show', 'never')
 
         yaml._save()
 
         if not insert and old_config is None:
+            data = {}   # unused
             lines = []
         else:
             data = autoconfig.read()
             lines = autoconfig.read_raw().splitlines()
 
             if insert:
                 assert lines[0].startswith(
```

### Comparing `qutebrowser-3.1.0/tests/unit/config/test_configinit.py` & `qutebrowser-3.2.0/tests/unit/config/test_configinit.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/config/test_configtypes.py` & `qutebrowser-3.2.0/tests/unit/config/test_configtypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1598,14 +1598,16 @@
                       fixed_keys=['one', 'two'])
             message = 'Expected keys .*'
         elif kind == 'required':
             d = klass(keytype=configtypes.String(),
                       valtype=configtypes.String(),
                       required_keys=['one', 'two'])
             message = 'Required keys .*'
+        else:
+            raise utils.Unreachable(kind)
 
         if ok:
             expectation = testutils.nop_contextmanager()
         else:
             expectation = pytest.raises(configexc.ValidationError,
                                         match=message)
 
@@ -1870,32 +1872,32 @@
 
 class TestProxy:
 
     @pytest.fixture
     def klass(self):
         return configtypes.Proxy
 
-    @pytest.mark.parametrize('val, expected', [
-        ('system', configtypes.SYSTEM_PROXY),
-        ('none', QNetworkProxy(QNetworkProxy.ProxyType.NoProxy)),
+    @pytest.mark.parametrize('val, expected_factory', [
+        ('system', lambda: configtypes.SYSTEM_PROXY),
+        ('none', lambda: QNetworkProxy(QNetworkProxy.ProxyType.NoProxy)),
         ('socks://example.com/',
-         QNetworkProxy(QNetworkProxy.ProxyType.Socks5Proxy, 'example.com')),
+         lambda: QNetworkProxy(QNetworkProxy.ProxyType.Socks5Proxy, 'example.com')),
         ('socks5://foo:bar@example.com:2323',
-         QNetworkProxy(QNetworkProxy.ProxyType.Socks5Proxy, 'example.com', 2323,
-                       'foo', 'bar')),
+         lambda: QNetworkProxy(
+             QNetworkProxy.ProxyType.Socks5Proxy, 'example.com', 2323, 'foo', 'bar')),
         ('pac+http://example.com/proxy.pac',
-         pac.PACFetcher(QUrl('pac+http://example.com/proxy.pac'))),
+         lambda: pac.PACFetcher(QUrl('pac+http://example.com/proxy.pac'))),
         ('pac+file:///tmp/proxy.pac',
-         pac.PACFetcher(QUrl('pac+file:///tmp/proxy.pac'))),
+         lambda: pac.PACFetcher(QUrl('pac+file:///tmp/proxy.pac'))),
     ])
-    def test_to_py_valid(self, klass, val, expected):
+    def test_to_py_valid(self, klass, val, expected_factory):
         actual = klass().to_py(val)
         if isinstance(actual, QNetworkProxy):
             actual = QNetworkProxy(actual)
-        assert actual == expected
+        assert actual == expected_factory()
 
     @pytest.mark.parametrize('val', [
         'blah',
         ':',  # invalid URL
         'ftp://example.com/',  # invalid scheme
     ])
     def test_to_py_invalid(self, klass, val):
```

### Comparing `qutebrowser-3.1.0/tests/unit/config/test_configutils.py` & `qutebrowser-3.2.0/tests/unit/config/test_configutils.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/config/test_qtargs.py` & `qutebrowser-3.2.0/tests/unit/config/test_qtargs.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/config/test_qtargs_locale_workaround.py` & `qutebrowser-3.2.0/tests/unit/config/test_qtargs_locale_workaround.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/config/test_stylesheet.py` & `qutebrowser-3.2.0/tests/unit/config/test_stylesheet.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/config/test_websettings.py` & `qutebrowser-3.2.0/tests/unit/config/test_websettings.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/extensions/test_loader.py` & `qutebrowser-3.2.0/tests/unit/extensions/test_loader.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/javascript/conftest.py` & `qutebrowser-3.2.0/tests/unit/javascript/conftest.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/javascript/position_caret/scrolled_down.html` & `qutebrowser-3.2.0/tests/unit/javascript/position_caret/scrolled_down.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/javascript/position_caret/scrolled_down_img.html` & `qutebrowser-3.2.0/tests/unit/javascript/position_caret/scrolled_down_img.html`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/javascript/position_caret/test_position_caret.py` & `qutebrowser-3.2.0/tests/unit/javascript/position_caret/test_position_caret.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/javascript/stylesheet/test_appendchild.js` & `qutebrowser-3.2.0/tests/unit/javascript/stylesheet/test_appendchild.js`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/javascript/stylesheet/test_stylesheet_js.py` & `qutebrowser-3.2.0/tests/unit/javascript/stylesheet/test_stylesheet_js.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/javascript/test_greasemonkey.py` & `qutebrowser-3.2.0/tests/unit/javascript/test_greasemonkey.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/javascript/test_js_execution.py` & `qutebrowser-3.2.0/tests/unit/javascript/test_js_execution.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/javascript/test_js_quirks.py` & `qutebrowser-3.2.0/tests/unit/javascript/test_js_quirks.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/keyinput/conftest.py` & `qutebrowser-3.2.0/tests/unit/keyinput/conftest.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/keyinput/key_data.py` & `qutebrowser-3.2.0/tests/unit/keyinput/key_data.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/keyinput/test_basekeyparser.py` & `qutebrowser-3.2.0/tests/unit/keyinput/test_basekeyparser.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/keyinput/test_bindingtrie.py` & `qutebrowser-3.2.0/tests/unit/keyinput/test_bindingtrie.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/keyinput/test_keyutils.py` & `qutebrowser-3.2.0/tests/unit/keyinput/test_keyutils.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/keyinput/test_modeman.py` & `qutebrowser-3.2.0/tests/unit/keyinput/test_modeman.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/keyinput/test_modeparsers.py` & `qutebrowser-3.2.0/tests/unit/keyinput/test_modeparsers.py`

 * *Files 8% similar despite different names*

```diff
@@ -111,35 +111,39 @@
                    bindings, keychain, prefix, hint, pyqt_enum_workaround):
         with pyqt_enum_workaround(keyutils.KeyParseError):
             keyparser.update_bindings(bindings)
 
         seq = keyutils.KeySequence.parse(keychain)
         assert len(seq) == 2
 
+        # pylint: disable-next=no-member
         match = keyparser.handle(seq[0].to_event())
         assert match == QKeySequence.SequenceMatch.PartialMatch
         assert hintmanager.keystr == prefix
 
+        # pylint: disable-next=no-member
         match = keyparser.handle(seq[1].to_event())
         assert match == QKeySequence.SequenceMatch.ExactMatch
         assert hintmanager.keystr == hint
 
     def test_match_key_mappings(self, config_stub, keyparser, hintmanager,
                                 pyqt_enum_workaround):
         with pyqt_enum_workaround(configexc.ValidationError):
             config_stub.val.bindings.key_mappings = {'α': 'a', 'σ': 's'}
         keyparser.update_bindings(['aa', 'as'])
 
         seq = keyutils.KeySequence.parse('ασ')
         assert len(seq) == 2
 
+        # pylint: disable-next=no-member
         match = keyparser.handle(seq[0].to_event())
         assert match == QKeySequence.SequenceMatch.PartialMatch
         assert hintmanager.keystr == 'a'
 
+        # pylint: disable-next=no-member
         match = keyparser.handle(seq[1].to_event())
         assert match == QKeySequence.SequenceMatch.ExactMatch
         assert hintmanager.keystr == 'as'
 
     def test_command(self, keyparser, config_stub, hintmanager, commandrunner):
         config_stub.val.bindings.commands = {
             'hint': {'abc': 'message-info abc'}
```

### Comparing `qutebrowser-3.1.0/tests/unit/mainwindow/statusbar/test_backforward.py` & `qutebrowser-3.2.0/tests/unit/mainwindow/statusbar/test_backforward.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/mainwindow/statusbar/test_percentage.py` & `qutebrowser-3.2.0/tests/unit/mainwindow/statusbar/test_percentage.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/mainwindow/statusbar/test_progress.py` & `qutebrowser-3.2.0/tests/unit/mainwindow/statusbar/test_progress.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/mainwindow/statusbar/test_tabindex.py` & `qutebrowser-3.2.0/tests/unit/mainwindow/statusbar/test_tabindex.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/mainwindow/statusbar/test_textbase.py` & `qutebrowser-3.2.0/tests/unit/mainwindow/statusbar/test_textbase.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/mainwindow/statusbar/test_url.py` & `qutebrowser-3.2.0/tests/unit/mainwindow/statusbar/test_url.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/mainwindow/test_messageview.py` & `qutebrowser-3.2.0/tests/unit/mainwindow/test_messageview.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/mainwindow/test_prompt.py` & `qutebrowser-3.2.0/tests/unit/mainwindow/test_prompt.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/mainwindow/test_tabwidget.py` & `qutebrowser-3.2.0/tests/unit/mainwindow/test_tabwidget.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_autoupdate.py` & `qutebrowser-3.2.0/tests/unit/misc/test_autoupdate.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_checkpyver.py` & `qutebrowser-3.2.0/tests/unit/misc/test_checkpyver.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_cmdhistory.py` & `qutebrowser-3.2.0/tests/unit/misc/test_cmdhistory.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_crashdialog.py` & `qutebrowser-3.2.0/tests/unit/misc/test_crashdialog.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_earlyinit.py` & `qutebrowser-3.2.0/tests/unit/misc/test_earlyinit.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_editor.py` & `qutebrowser-3.2.0/tests/unit/misc/test_editor.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_elf.py` & `qutebrowser-3.2.0/tests/unit/misc/test_elf.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_guiprocess.py` & `qutebrowser-3.2.0/tests/unit/misc/test_guiprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """Tests for qutebrowser.misc.guiprocess."""
 
 import sys
 import logging
 import signal
 
 import pytest
-from qutebrowser.qt.core import QProcess, QUrl
+from qutebrowser.qt.core import QProcess, QUrl, Qt
 
 from qutebrowser.misc import guiprocess
 from qutebrowser.utils import usertypes, utils, version
 from qutebrowser.api import cmdutils
 from qutebrowser.qt import sip
 
 
@@ -530,14 +530,15 @@
     assert str(proc) in [
         f"'{sys.executable}' -c 'import sys'",  # Sometimes sys.executable needs quoting
         f"{sys.executable} -c 'import sys'",
     ]
 
 
 def test_cleanup(proc, py_proc, qtbot):
+    proc._cleanup_timer.setTimerType(Qt.TimerType.CoarseTimer)
     proc._cleanup_timer.setInterval(100)
 
     with qtbot.wait_signal(proc._cleanup_timer.timeout):
         proc.start(*py_proc(""))
         assert proc.pid in guiprocess.all_processes
 
     assert guiprocess.all_processes[proc.pid] is None
```

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_ipc.py` & `qutebrowser-3.2.0/tests/unit/misc/test_ipc.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_keyhints.py` & `qutebrowser-3.2.0/tests/unit/misc/test_keyhints.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_lineparser.py` & `qutebrowser-3.2.0/tests/unit/misc/test_lineparser.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_miscwidgets.py` & `qutebrowser-3.2.0/tests/unit/misc/test_miscwidgets.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_msgbox.py` & `qutebrowser-3.2.0/tests/unit/misc/test_msgbox.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_objects.py` & `qutebrowser-3.2.0/tests/unit/misc/test_objects.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_pakjoy.py` & `qutebrowser-3.2.0/tests/unit/misc/test_pakjoy.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         """Test fallback path is used."""
         (fallback_path / pakjoy.PAK_FILENAME).touch()
         assert pakjoy._find_webengine_resources() == fallback_path
 
     def test_nowhere(self, fallback_path: pathlib.Path):
         """Test we raise if we can't find the resources."""
         with pytest.raises(
-            binparsing.ParseError, match="Couldn't find webengine resources dir"
+            FileNotFoundError, match="Couldn't find webengine resources dir, candidates:\n*"
         ):
             pakjoy._find_webengine_resources()
 
 
 def json_without_comments(bytestring):
     str_without_comments = "\n".join(
         [
```

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_pastebin.py` & `qutebrowser-3.2.0/tests/unit/misc/test_pastebin.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_sessions.py` & `qutebrowser-3.2.0/tests/unit/misc/test_sessions.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_split.py` & `qutebrowser-3.2.0/tests/unit/misc/test_split.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_split_hypothesis.py` & `qutebrowser-3.2.0/tests/unit/misc/test_split_hypothesis.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_sql.py` & `qutebrowser-3.2.0/tests/unit/misc/test_sql.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_throttle.py` & `qutebrowser-3.2.0/tests/unit/misc/test_throttle.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/test_utilcmds.py` & `qutebrowser-3.2.0/tests/unit/misc/test_utilcmds.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/misc/userscripts/test_qute_lastpass.py` & `qutebrowser-3.2.0/tests/unit/misc/userscripts/test_qute_lastpass.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/scripts/importer_sample/chrome/input/Bookmarks` & `qutebrowser-3.2.0/tests/unit/scripts/importer_sample/chrome/input/Bookmarks`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/scripts/importer_sample/chrome/input/Web Data` & `qutebrowser-3.2.0/tests/unit/scripts/importer_sample/chrome/input/Web Data`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/scripts/importer_sample/html/input` & `qutebrowser-3.2.0/tests/unit/scripts/importer_sample/html/input`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/scripts/importer_sample/mozilla/input/places.sqlite` & `qutebrowser-3.2.0/tests/unit/scripts/importer_sample/mozilla/input/places.sqlite`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/scripts/test_dictcli.py` & `qutebrowser-3.2.0/tests/unit/scripts/test_dictcli.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/scripts/test_importer.py` & `qutebrowser-3.2.0/tests/unit/scripts/test_importer.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/scripts/test_problemmatchers.py` & `qutebrowser-3.2.0/tests/unit/scripts/test_problemmatchers.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/test_app.py` & `qutebrowser-3.2.0/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/test_qt_machinery.py` & `qutebrowser-3.2.0/tests/unit/test_qt_machinery.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """Test qutebrowser.qt.machinery."""
 
 import re
 import sys
 import html
 import argparse
 import typing
-from typing import Any, Optional, List, Dict, Union
+from typing import Any, Optional, List, Dict, Union, Type
 import dataclasses
 
 import pytest
 
 from qutebrowser.qt import machinery
 
 
@@ -41,22 +41,22 @@
     for wrapper in machinery.WRAPPERS:
         monkeypatch.delitem(sys.modules, wrapper, raising=False)
     for var in MACHINERY_VARS:
         monkeypatch.delattr(machinery, var)
 
 
 @pytest.mark.parametrize(
-    "exception",
+    "exception, base",
     [
-        machinery.Unavailable(),
-        machinery.NoWrapperAvailableError(machinery.SelectionInfo()),
+        (machinery.Unavailable(), ModuleNotFoundError),
+        (machinery.NoWrapperAvailableError(machinery.SelectionInfo()), ImportError),
     ],
 )
-def test_importerror_exceptions(exception: Exception):
-    with pytest.raises(ImportError):
+def test_importerror_exceptions(exception: Exception, base: Type[Exception]):
+    with pytest.raises(base):
         raise exception
 
 
 def test_selectioninfo_set_module_error():
     info = machinery.SelectionInfo()
     info.set_module_error("PyQt5", ImportError("Python imploded"))
     assert info == machinery.SelectionInfo(
```

### Comparing `qutebrowser-3.1.0/tests/unit/test_qutebrowser.py` & `qutebrowser-3.2.0/tests/unit/test_qutebrowser.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/utils/overflow_test_cases.py` & `qutebrowser-3.2.0/tests/unit/utils/overflow_test_cases.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/utils/test_debug.py` & `qutebrowser-3.2.0/tests/unit/utils/test_debug.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/utils/test_error.py` & `qutebrowser-3.2.0/tests/unit/utils/test_error.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/utils/test_javascript.py` & `qutebrowser-3.2.0/tests/unit/utils/test_javascript.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/utils/test_jinja.py` & `qutebrowser-3.2.0/tests/unit/utils/test_jinja.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/utils/test_log.py` & `qutebrowser-3.2.0/tests/unit/utils/test_log.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/utils/test_qtlog.py` & `qutebrowser-3.2.0/tests/unit/utils/test_qtlog.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/utils/test_qtutils.py` & `qutebrowser-3.2.0/tests/unit/utils/test_qtutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,26 @@
     (QDataStream.Status.Ok, False, None),
     (QDataStream.Status.ReadPastEnd, True,
      "The data stream has read past the end of the data in the underlying device."),
     (QDataStream.Status.ReadCorruptData, True,
      "The data stream has read corrupt data."),
     (QDataStream.Status.WriteFailed, True,
      "The data stream cannot write to the underlying device."),
+    pytest.param(
+        getattr(QDataStream.Status, "SizeLimitExceeded", None),
+        True,
+        (
+            "The data stream cannot read or write the data because its size is larger "
+            "than supported by the current platform."
+        ),
+        marks=pytest.mark.skipif(
+            not hasattr(QDataStream.Status, "SizeLimitExceeded"),
+            reason="Added in Qt 6.7"
+        )
+    ),
 ])
 def test_check_qdatastream(status, raising, message):
     """Test check_qdatastream.
 
     Args:
         status: The status to set on the QDataStream we test with.
         raising: Whether check_qdatastream is expected to raise OSError.
@@ -222,18 +234,33 @@
     if raising:
         with pytest.raises(OSError, match=message):
             qtutils.check_qdatastream(stream)
     else:
         qtutils.check_qdatastream(stream)
 
 
-def test_qdatastream_status_count():
-    """Make sure no new members are added to QDataStream.Status."""
-    status_vals = testutils.enum_members(QDataStream, QDataStream.Status)
-    assert len(status_vals) == 4
+def test_qdatastream_status_members():
+    """Make sure no new members are added to QDataStream.Status.
+
+    If this fails, qtutils.check_qdatastream will need to be updated with the
+    respective error documentation.
+    """
+    status_vals = set(testutils.enum_members(QDataStream, QDataStream.Status).values())
+    expected = {
+        QDataStream.Status.Ok,
+        QDataStream.Status.ReadPastEnd,
+        QDataStream.Status.ReadCorruptData,
+        QDataStream.Status.WriteFailed,
+    }
+    try:
+        expected.add(QDataStream.Status.SizeLimitExceeded)
+    except AttributeError:
+        # Added in Qt 6.7
+        pass
+    assert status_vals == expected
 
 
 @pytest.mark.parametrize('color, expected', [
     (QColor('red'), 'rgba(255, 0, 0, 255)'),
     (QColor('blue'), 'rgba(0, 0, 255, 255)'),
     (QColor(1, 3, 5, 7), 'rgba(1, 3, 5, 7)'),
 ])
@@ -727,16 +754,18 @@
         if hasattr(os, 'SEEK_HOLE'):
             whence = os.SEEK_HOLE
         elif hasattr(os, 'SEEK_DATA'):
             whence = os.SEEK_DATA
         # pylint: enable=no-member,useless-suppression
         else:
             pytest.skip("Needs os.SEEK_HOLE or os.SEEK_DATA available.")
+
         pyqiodev.open(QIODevice.OpenModeFlag.ReadOnly)
         with pytest.raises(io.UnsupportedOperation):
+            # pylint: disable=possibly-used-before-assignment
             pyqiodev.seek(0, whence)
 
     @pytest.mark.flaky
     def test_qprocess(self, py_proc):
         """Test PyQIODevice with a QProcess which is non-sequential.
 
         This also verifies seek() and tell() behave as expected.
@@ -1085,21 +1114,21 @@
     def test_object_name(self):
         obj = QObject()
         obj.setObjectName("Tux")
         expected = f"<{self._py_repr(obj)}, objectName='Tux'>"
         assert qtutils.qobj_repr(obj) == expected
 
     def test_class_name(self):
-        obj = QTimer()
+        obj = QTimer()  # misc: ignore
         hidden = sip.cast(obj, QObject)
         expected = f"<{self._py_repr(hidden)}, className='QTimer'>"
         assert qtutils.qobj_repr(hidden) == expected
 
     def test_both(self):
-        obj = QTimer()
+        obj = QTimer()  # misc: ignore
         obj.setObjectName("Pomodoro")
         hidden = sip.cast(obj, QObject)
         expected = f"<{self._py_repr(hidden)}, objectName='Pomodoro', className='QTimer'>"
         assert qtutils.qobj_repr(hidden) == expected
 
     def test_rich_repr(self):
         class RichRepr(QObject):
```

### Comparing `qutebrowser-3.1.0/tests/unit/utils/test_resources.py` & `qutebrowser-3.2.0/tests/unit/utils/test_resources.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/utils/test_standarddir.py` & `qutebrowser-3.2.0/tests/unit/utils/test_standarddir.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/utils/test_urlmatch.py` & `qutebrowser-3.2.0/tests/unit/utils/test_urlmatch.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/utils/test_urlutils.py` & `qutebrowser-3.2.0/tests/unit/utils/test_urlutils.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/utils/test_utils.py` & `qutebrowser-3.2.0/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/utils/test_version.py` & `qutebrowser-3.2.0/tests/unit/utils/test_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -895,29 +895,53 @@
 
     @pytest.mark.parametrize('version, expected', [
         (
             version.WebEngineVersions(
                 webengine=utils.VersionNumber(5, 15, 2),
                 chromium=None,
                 source='UA'),
-            "QtWebEngine 5.15.2",
+            (
+                "QtWebEngine 5.15.2\n"
+                "  (source: UA)"
+            ),
         ),
         (
             version.WebEngineVersions(
                 webengine=utils.VersionNumber(5, 15, 2),
                 chromium='87.0.4280.144',
                 source='UA'),
-            "QtWebEngine 5.15.2, based on Chromium 87.0.4280.144",
+            (
+                "QtWebEngine 5.15.2\n"
+                "  based on Chromium 87.0.4280.144\n"
+                "  (source: UA)"
+            ),
         ),
         (
             version.WebEngineVersions(
                 webengine=utils.VersionNumber(5, 15, 2),
                 chromium='87.0.4280.144',
                 source='faked'),
-            "QtWebEngine 5.15.2, based on Chromium 87.0.4280.144 (from faked)",
+            (
+                "QtWebEngine 5.15.2\n"
+                "  based on Chromium 87.0.4280.144\n"
+                "  (source: faked)"
+            ),
+        ),
+        (
+            version.WebEngineVersions(
+                webengine=utils.VersionNumber(5, 15, 2),
+                chromium='87.0.4280.144',
+                chromium_security='9000.1',
+                source='faked'),
+            (
+                "QtWebEngine 5.15.2\n"
+                "  based on Chromium 87.0.4280.144\n"
+                "  with security patches up to 9000.1 (plus any distribution patches)\n"
+                "  (source: faked)"
+            ),
         ),
     ])
     def test_str(self, version, expected):
         assert str(version) == expected
 
     @pytest.mark.parametrize('version, expected', [
         (
@@ -946,45 +970,53 @@
             upstream_browser_version='83.0.4103.122',
             qt_key='QtWebEngine',
             qt_version='5.15.2',
         )
         expected = version.WebEngineVersions(
             webengine=utils.VersionNumber(5, 15, 2),
             chromium='83.0.4103.122',
+            chromium_security='86.0.4240.183',
             source='UA',
         )
         assert version.WebEngineVersions.from_ua(ua) == expected
 
     def test_from_elf(self):
         elf_version = elf.Versions(webengine='5.15.2', chromium='83.0.4103.122')
         expected = version.WebEngineVersions(
             webengine=utils.VersionNumber(5, 15, 2),
             chromium='83.0.4103.122',
+            chromium_security='86.0.4240.183',
             source='ELF',
         )
         assert version.WebEngineVersions.from_elf(elf_version) == expected
 
-    @pytest.mark.parametrize('pyqt_version, chromium_version', [
-        ('5.15.2', '83.0.4103.122'),
-        ('5.15.3', '87.0.4280.144'),
-        ('5.15.4', '87.0.4280.144'),
-        ('5.15.5', '87.0.4280.144'),
-        ('6.2.0', '90.0.4430.228'),
-        ('6.3.0', '94.0.4606.126'),
+    @pytest.mark.parametrize('pyqt_version, chromium_version, security_version', [
+        ('5.15.2', '83.0.4103.122', '86.0.4240.183'),
+        ('5.15.3', '87.0.4280.144', '88.0.4324.150'),
+        ('5.15.4', '87.0.4280.144', None),
+        ('5.15.5', '87.0.4280.144', None),
+        ('5.15.6', '87.0.4280.144', None),
+        ('5.15.7', '87.0.4280.144', '94.0.4606.61'),
+        ('6.2.0', '90.0.4430.228', '93.0.4577.63'),
+        ('6.2.99', '90.0.4430.228', None),
+        ('6.3.0', '94.0.4606.126', '99.0.4844.84'),
+        ('6.99.0', None, None),
     ])
-    def test_from_pyqt(self, freezer, pyqt_version, chromium_version):
-        if freezer and pyqt_version in ['5.15.3', '5.15.4', '5.15.5']:
+    def test_from_pyqt(self, freezer, pyqt_version, chromium_version, security_version):
+        if freezer and utils.VersionNumber(5, 15, 3) <= utils.VersionNumber.parse(pyqt_version) < utils.VersionNumber(6):
             chromium_version = '83.0.4103.122'
+            security_version = '86.0.4240.183'
             expected_pyqt_version = '5.15.2'
         else:
             expected_pyqt_version = pyqt_version
 
         expected = version.WebEngineVersions(
             webengine=utils.VersionNumber.parse(expected_pyqt_version),
             chromium=chromium_version,
+            chromium_security=security_version,
             source='PyQt',
         )
         assert version.WebEngineVersions.from_pyqt(pyqt_version) == expected
 
     def test_real_chromium_version(self, qapp):
         """Compare the inferred Chromium version with the real one."""
         try:
@@ -1020,14 +1052,47 @@
         inferred = versions.chromium
 
         webenginesettings.init_user_agent()
         real = webenginesettings.parsed_user_agent.upstream_browser_version
 
         assert inferred == real
 
+    def test_real_chromium_security_version(self, qapp):
+        """Check the API for reading the chromium security patch version."""
+        try:
+            from qutebrowser.qt.webenginecore import (
+                qWebEngineChromiumVersion,
+                qWebEngineChromiumSecurityPatchVersion,
+            )
+        except ImportError:
+            pytest.skip("Requires QtWebEngine 6.3+")
+
+        base = utils.VersionNumber.parse(qWebEngineChromiumVersion())
+        security = utils.VersionNumber.parse(qWebEngineChromiumSecurityPatchVersion())
+        assert security >= base
+
+    def test_chromium_security_version_dict(self, qapp):
+        """Check if we infer the QtWebEngine security version properly.
+
+        Note this test mostly tests that our overview in version.py (also
+        intended for human readers) is accurate. The code we call here is never
+        going to be called in real-life situations, as the API is available.
+        """
+        try:
+            from qutebrowser.qt.webenginecore import (
+                qWebEngineVersion,
+                qWebEngineChromiumSecurityPatchVersion,
+            )
+        except ImportError:
+            pytest.skip("Requires QtWebEngine 6.3+")
+
+        inferred = version.WebEngineVersions.from_webengine(
+            qWebEngineVersion(), source="API")
+        assert inferred.chromium_security == qWebEngineChromiumSecurityPatchVersion()
+
 
 class FakeQSslSocket:
 
     """Fake for the QSslSocket Qt class.
 
     Attributes:
         _version: What QSslSocket::sslLibraryVersionString() should return.
@@ -1290,15 +1355,15 @@
     if params.with_webkit:
         patches['qWebKitVersion'] = lambda: 'WEBKIT VERSION'
         patches['objects.backend'] = usertypes.Backend.QtWebKit
         substitutions['backend'] = 'new QtWebKit (WebKit WEBKIT VERSION)'
     else:
         monkeypatch.delattr(version, 'qtutils.qWebKitVersion', raising=False)
         patches['objects.backend'] = usertypes.Backend.QtWebEngine
-        substitutions['backend'] = 'QtWebEngine 1.2.3 (from faked)'
+        substitutions['backend'] = 'QtWebEngine 1.2.3\n  (source: faked)'
 
     if params.known_distribution:
         patches['distribution'] = lambda: version.DistributionInfo(
             parsed=version.Distribution.arch, pretty='LINUX DISTRIBUTION', id='arch')
         substitutions['linuxdist'] = ('\nLinux distribution: '
                                       'LINUX DISTRIBUTION (arch)')
         substitutions['osinfo'] = ''
```

### Comparing `qutebrowser-3.1.0/tests/unit/utils/usertypes/test_neighborlist.py` & `qutebrowser-3.2.0/tests/unit/utils/usertypes/test_neighborlist.py`

 * *Files identical despite different names*

### Comparing `qutebrowser-3.1.0/tests/unit/utils/usertypes/test_question.py` & `qutebrowser-3.2.0/tests/unit/utils/usertypes/test_question.py`

 * *Files identical despite different names*

