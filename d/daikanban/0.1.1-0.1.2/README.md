# Comparing `tmp/daikanban-0.1.1.tar.gz` & `tmp/daikanban-0.1.2.tar.gz`

## Comparing `daikanban-0.1.1.tar` & `daikanban-0.1.2.tar`

### file list

```diff
@@ -1,1589 +1,1590 @@
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 daikanban-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 daikanban-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     6952 2020-02-02 00:00:00.000000 daikanban-0.1.1/TODO.md
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 daikanban-0.1.1/ruff.toml
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 daikanban-0.1.1/summarize.sh
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/.lock
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/pyvenv.cfg
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/bin/activate
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/bin/activate.csh
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/bin/activate.fish
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/bin/activate.nu
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/bin/activate.ps1
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/bin/activate_this.py
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/bin/daikanban
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/bin/markdown-it
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/bin/pygmentize
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/bin/python -> /Users/jerm/.pyenv/versions/3.11.0/bin/python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/bin/python3.11 -> python
--rwxr-xr-x   0        0        0   120544 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/_time_machine.cpython-311-darwin.so
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/_virtualenv.pth
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/_virtualenv.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/six.py
--rw-r--r--   0        0        0   117599 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typing_extensions.py
--rw-r--r--   0        0        0    12151 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/annotated_types/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/annotated_types/py.typed
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/annotated_types/test_cases.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    12879 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/METADATA
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/WHEEL
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/__init__.py
--rw-r--r--   0        0        0    18744 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/_compat.py
--rw-r--r--   0        0        0    24069 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/_termui_impl.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/_textwrap.py
--rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/_winconsole.py
--rw-r--r--   0        0        0   114086 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/core.py
--rw-r--r--   0        0        0    18719 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/decorators.py
--rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/exceptions.py
--rw-r--r--   0        0        0     9706 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/formatting.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/globals.py
--rw-r--r--   0        0        0    19067 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/py.typed
--rw-r--r--   0        0        0    18460 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/shell_completion.py
--rw-r--r--   0        0        0    28324 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/termui.py
--rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/testing.py
--rw-r--r--   0        0        0    36391 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/types.py
--rw-r--r--   0        0        0    20298 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/utils.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/INSTALLER
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/LICENSE.rst
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/METADATA
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/WHEEL
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/top_level.txt
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/INSTALLER
--rw-r--r--   0        0        0    17158 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/METADATA
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/REQUESTED
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/WHEEL
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/billboard_art.txt
--rw-r--r--   0        0        0    39535 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/interface.py
--rwxr-xr-x   0        0        0     1012 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/main.py
--rw-r--r--   0        0        0    27508 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/model.py
--rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/prompt.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/score.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/settings.py
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/utils.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/INSTALLER
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/METADATA
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/WHEEL
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/__init__.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/_common.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/_version.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/easter.py
--rw-r--r--   0        0        0    24903 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/relativedelta.py
--rw-r--r--   0        0        0    66557 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/rrule.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/tzwin.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/utils.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/parser/__init__.py
--rw-r--r--   0        0        0    58796 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/parser/_parser.py
--rw-r--r--   0        0        0    13233 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/parser/isoparser.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/tz/__init__.py
--rw-r--r--   0        0        0    12977 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/tz/_common.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/tz/_factories.py
--rw-r--r--   0        0        0    62855 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/tz/tz.py
--rw-r--r--   0        0        0    12935 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/tz/win.py
--rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/zoneinfo/__init__.py
--rw-r--r--   0        0        0   156400 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/zoneinfo/dateutil-zoneinfo.tar.gz
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/zoneinfo/rebuild.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/_compat.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/_punycode.py
--rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/main.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/parser_block.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/parser_core.py
--rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/parser_inline.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/port.yaml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/py.typed
--rw-r--r--   0        0        0     9970 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/renderer.py
--rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/ruler.py
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/token.py
--rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/tree.py
--rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/cli/__init__.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/cli/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/common/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/common/entities.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/common/html_blocks.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/common/html_re.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/common/normalize_url.py
--rw-r--r--   0        0        0    10728 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/common/utils.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/helpers/__init__.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_destination.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_label.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_title.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/presets/__init__.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/presets/commonmark.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/presets/default.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/presets/zero.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/__init__.py
--rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/blockquote.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/code.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/fence.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/heading.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/hr.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/html_block.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/lheading.py
--rw-r--r--   0        0        0     9668 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/list.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/paragraph.py
--rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/reference.py
--rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/state_block.py
--rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/table.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_core/__init__.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_core/block.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_core/inline.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_core/linkify.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_core/normalize.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_core/replacements.py
--rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_core/smartquotes.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_core/state_core.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_core/text_join.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/__init__.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/autolink.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/backticks.py
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/balance_pairs.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/emphasis.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/entity.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/escape.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/fragments_join.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/html_inline.py
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/image.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/link.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/linkify.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/newline.py
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/state_inline.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/strikethrough.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/text.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE.markdown-it
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl/__init__.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl/_decode.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl/_encode.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl/_format.py
--rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl/_parse.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl/_url.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl/py.typed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/LICENSE
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/METADATA
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/REQUESTED
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/WHEEL
--rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/__version__.py
--rw-r--r--   0        0        0     8780 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/_helpers.py
--rwxr-xr-x   0        0        0   539840 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/_pendulum.cpython-311-darwin.so
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/_pendulum.pyi
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/constants.py
--rw-r--r--   0        0        0    24071 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/date.py
--rw-r--r--   0        0        0    42309 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/datetime.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/day.py
--rw-r--r--   0        0        0    14780 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/duration.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/exceptions.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/helpers.py
--rw-r--r--   0        0        0    13543 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/interval.py
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/py.typed
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/time.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/formatting/__init__.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/formatting/difference_formatter.py
--rw-r--r--   0        0        0    22499 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/formatting/formatter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/__init__.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/cs/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/cs/custom.py
--rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/cs/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/da/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/da/custom.py
--rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/da/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/de/__init__.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/de/custom.py
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/de/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/en/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/en/custom.py
--rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/en/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/en_gb/__init__.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/en_gb/custom.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/en_gb/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/en_us/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/en_us/custom.py
--rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/en_us/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/es/__init__.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/es/custom.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/es/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/fa/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/fa/custom.py
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/fa/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/fo/__init__.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/fo/custom.py
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/fo/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/fr/__init__.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/fr/custom.py
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/fr/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/he/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/he/custom.py
--rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/he/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/id/__init__.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/id/custom.py
--rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/id/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/it/__init__.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/it/custom.py
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/it/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/ja/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/ja/custom.py
--rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/ja/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/ko/__init__.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/ko/custom.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/ko/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/lt/__init__.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/lt/custom.py
--rw-r--r--   0        0        0     8342 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/lt/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/nb/__init__.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/nb/custom.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/nb/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/nl/__init__.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/nl/custom.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/nl/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/nn/__init__.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/nn/custom.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/nn/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/pl/__init__.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/pl/custom.py
--rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/pl/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/pt_br/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/pt_br/custom.py
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/pt_br/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/ru/__init__.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/ru/custom.py
--rw-r--r--   0        0        0     9529 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/ru/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/sk/__init__.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/sk/custom.py
--rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/sk/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/sv/__init__.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/sv/custom.py
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/sv/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/tr/__init__.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/tr/custom.py
--rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/tr/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/zh/__init__.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/zh/custom.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/zh/locale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/mixins/__init__.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/mixins/default.py
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/parsing/__init__.py
--rw-r--r--   0        0        0    13886 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/parsing/iso8601.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/parsing/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/testing/__init__.py
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/testing/traveller.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/tz/__init__.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/tz/exceptions.py
--rw-r--r--   0        0        0     8429 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/tz/local_timezone.py
--rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/tz/timezone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/tz/data/__init__.py
--rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/tz/data/windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/utils/__init__.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/utils/_compat.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/utils/_zoneinfo.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/METADATA
--rw-r--r--   0        0        0    10278 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/REQUESTED
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/license_files/LICENSE
--rw-r--r--   0        0        0    12780 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/__init__.py
--rw-r--r--   0        0        0    11913 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_migration.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/alias_generators.py
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/aliases.py
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/annotated_handlers.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/class_validators.py
--rw-r--r--   0        0        0    21493 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/color.py
--rw-r--r--   0        0        0    29141 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/config.py
--rw-r--r--   0        0        0    13450 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/dataclasses.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/datetime_parse.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/decorator.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/env_settings.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/error_wrappers.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/errors.py
--rw-r--r--   0        0        0    45930 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/fields.py
--rw-r--r--   0        0        0    14621 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/functional_serializers.py
--rw-r--r--   0        0        0    24313 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/functional_validators.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/generics.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/json.py
--rw-r--r--   0        0        0   102807 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/json_schema.py
--rw-r--r--   0        0        0    65892 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/main.py
--rw-r--r--   0        0        0    55131 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/mypy.py
--rw-r--r--   0        0        0    21225 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/networks.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/py.typed
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/root_model.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/schema.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/tools.py
--rw-r--r--   0        0        0    18104 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/type_adapter.py
--rw-r--r--   0        0        0    89607 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/types.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/typing.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/utils.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/validate_call_decorator.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/validators.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/version.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/warnings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/__init__.py
--rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_config.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_core_metadata.py
--rw-r--r--   0        0        0    24332 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_core_utils.py
--rw-r--r--   0        0        0     8481 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_dataclasses.py
--rw-r--r--   0        0        0    30627 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_decorators.py
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_decorators_v1.py
--rw-r--r--   0        0        0    26369 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_discriminated_union.py
--rw-r--r--   0        0        0    13184 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_fields.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_forward_ref.py
--rw-r--r--   0        0        0    98557 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_generate_schema.py
--rw-r--r--   0        0        0    22227 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_generics.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_git.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_internal_dataclass.py
--rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_known_annotated_metadata.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_mock_val_ser.py
--rw-r--r--   0        0        0    28114 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_model_construction.py
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_repr.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_schema_generation_shared.py
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_signature.py
--rw-r--r--   0        0        0    29085 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_std_types_schema.py
--rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_typing_extra.py
--rw-r--r--   0        0        0    12670 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_utils.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_validate_call.py
--rw-r--r--   0        0        0    10054 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/deprecated/__init__.py
--rw-r--r--   0        0        0     9871 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/deprecated/class_validators.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/deprecated/config.py
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/deprecated/copy_internals.py
--rw-r--r--   0        0        0    10778 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/deprecated/decorator.py
--rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/deprecated/json.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/deprecated/parse.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/deprecated/tools.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/plugin/__init__.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/plugin/_loader.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/plugin/_schema_validator.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/__init__.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/_hypothesis_plugin.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/annotated_types.py
--rw-r--r--   0        0        0    14595 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/class_validators.py
--rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/color.py
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/config.py
--rw-r--r--   0        0        0    18073 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/dataclasses.py
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/datetime_parse.py
--rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/decorator.py
--rw-r--r--   0        0        0    14039 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/env_settings.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/error_wrappers.py
--rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/errors.py
--rw-r--r--   0        0        0    50485 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/fields.py
--rw-r--r--   0        0        0    17805 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/generics.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/json.py
--rw-r--r--   0        0        0    44376 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/main.py
--rw-r--r--   0        0        0    38745 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/mypy.py
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/networks.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/py.typed
--rw-r--r--   0        0        0    47614 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/schema.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/tools.py
--rw-r--r--   0        0        0    35379 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/types.py
--rw-r--r--   0        0        0    18996 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/typing.py
--rw-r--r--   0        0        0    25809 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/utils.py
--rw-r--r--   0        0        0    21887 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/validators.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/version.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/INSTALLER
--rw-r--r--   0        0        0    85087 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/METADATA
--rw-r--r--   0        0        0     8852 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/REQUESTED
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/WHEEL
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core/__init__.py
--rwxr-xr-x   0        0        0  3955160 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core/_pydantic_core.cpython-311-darwin.so
--rw-r--r--   0        0        0    33290 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core/_pydantic_core.pyi
--rw-r--r--   0        0        0   134918 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core/core_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core/py.typed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/INSTALLER
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/METADATA
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/REQUESTED
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/WHEEL
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/license_files/LICENSE
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/__init__.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/__main__.py
--rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/filter.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatter.py
--rw-r--r--   0        0        0    35044 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/modeline.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/scanner.py
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/sphinxext.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/style.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/token.py
--rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/unistring.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/util.py
--rw-r--r--   0        0        0    40338 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/filters/__init__.py
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/__init__.py
--rwxr-xr-x   0        0        0     4176 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35640 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/html.py
--rw-r--r--   0        0        0    23116 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/img.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19303 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/other.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    12113 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/__init__.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_ada_builtins.py
--rw-r--r--   0        0        0    27287 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_asy_builtins.py
--rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_cl_builtins.py
--rw-r--r--   0        0        0   105182 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_cocoa_builtins.py
--rw-r--r--   0        0        0    18414 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_csound_builtins.py
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_css_builtins.py
--rw-r--r--   0        0        0    11883 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_julia_builtins.py
--rw-r--r--   0        0        0   134510 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_lasso_builtins.py
--rw-r--r--   0        0        0   108094 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_lilypond_builtins.py
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_lua_builtins.py
--rw-r--r--   0        0        0    68026 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    24713 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_mql_builtins.py
--rw-r--r--   0        0        0    25842 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_mysql_builtins.py
--rw-r--r--   0        0        0    49398 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_openedge_builtins.py
--rw-r--r--   0        0        0   107930 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_php_builtins.py
--rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_postgres_builtins.py
--rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_qlik_builtins.py
--rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_scheme_builtins.py
--rw-r--r--   0        0        0    52413 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_scilab_builtins.py
--rw-r--r--   0        0        0    26781 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_sourcemod_builtins.py
--rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_stan_builtins.py
--rw-r--r--   0        0        0    27227 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_stata_builtins.py
--rw-r--r--   0        0        0    15460 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_tsql_builtins.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_usd_builtins.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_vbscript_builtins.py
--rw-r--r--   0        0        0    57066 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_vim_builtins.py
--rw-r--r--   0        0        0    11676 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/actionscript.py
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ada.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/agile.py
--rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/algebra.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ambient.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/amdgpu.py
--rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ampl.py
--rw-r--r--   0        0        0    30766 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/apdlexer.py
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/apl.py
--rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/archetype.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/arrow.py
--rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/arturo.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/asc.py
--rw-r--r--   0        0        0    41243 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/asm.py
--rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/asn1.py
--rw-r--r--   0        0        0    19815 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/automation.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/bare.py
--rw-r--r--   0        0        0    27923 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/basic.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/bdd.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/berry.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/bibtex.py
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/blueprint.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/boa.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/bqn.py
--rw-r--r--   0        0        0    28112 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/business.py
--rw-r--r--   0        0        0    17946 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/c_cpp.py
--rw-r--r--   0        0        0    29206 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/c_like.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/capnproto.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/carbon.py
--rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/cddl.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/chapel.py
--rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/clean.py
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/comal.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/compiled.py
--rw-r--r--   0        0        0    50077 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/configs.py
--rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/console.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/cplint.py
--rw-r--r--   0        0        0    15757 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/crystal.py
--rw-r--r--   0        0        0    16994 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/csound.py
--rw-r--r--   0        0        0    25322 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/css.py
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/d.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/dalvik.py
--rw-r--r--   0        0        0    27032 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/data.py
--rw-r--r--   0        0        0     8099 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/dax.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/devicetree.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/diff.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/dns.py
--rw-r--r--   0        0        0    37623 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/dotnet.py
--rw-r--r--   0        0        0    36786 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/dsls.py
--rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/dylan.py
--rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ecl.py
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/eiffel.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/elm.py
--rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/elpi.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/email.py
--rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/erlang.py
--rw-r--r--   0        0        0    10396 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/esoteric.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ezhil.py
--rw-r--r--   0        0        0    19531 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/factor.py
--rw-r--r--   0        0        0    10197 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/fantom.py
--rw-r--r--   0        0        0     9646 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/felix.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/fift.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/floscript.py
--rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/forth.py
--rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/fortran.py
--rw-r--r--   0        0        0    26212 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/foxpro.py
--rw-r--r--   0        0        0    26914 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/freefem.py
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/func.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/functional.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/futhark.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/gcodelexer.py
--rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/gdscript.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/go.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/grammar_notation.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/graph.py
--rw-r--r--   0        0        0    39026 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/graphics.py
--rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/graphql.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/graphviz.py
--rwxr-xr-x   0        0        0     3991 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/gsql.py
--rw-r--r--   0        0        0    32898 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/haskell.py
--rw-r--r--   0        0        0    30976 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/haxe.py
--rw-r--r--   0        0        0    22520 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/hdl.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/hexdump.py
--rw-r--r--   0        0        0    20260 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/html.py
--rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/idl.py
--rw-r--r--   0        0        0    31658 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/igor.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/inferno.py
--rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/installers.py
--rw-r--r--   0        0        0    57119 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/int_fiction.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/iolang.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/j.py
--rw-r--r--   0        0        0    62859 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/javascript.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/jmespath.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/jslt.py
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/jsonnet.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/jsx.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/julia.py
--rw-r--r--   0        0        0    72929 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/jvm.py
--rw-r--r--   0        0        0    11406 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/kuin.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/kusto.py
--rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ldap.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/lean.py
--rw-r--r--   0        0        0     9753 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/lilypond.py
--rw-r--r--   0        0        0   144398 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/lisp.py
--rw-r--r--   0        0        0    32171 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/macaulay2.py
--rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/make.py
--rw-r--r--   0        0        0    60257 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/markup.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/math.py
--rw-r--r--   0        0        0   132852 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/matlab.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/maxima.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/meson.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/mime.py
--rw-r--r--   0        0        0    13810 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/minecraft.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/mips.py
--rw-r--r--   0        0        0    35315 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ml.py
--rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/modeling.py
--rw-r--r--   0        0        0    53073 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/modula2.py
--rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/monte.py
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/mosel.py
--rw-r--r--   0        0        0    63962 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ncl.py
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/nimrod.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/nit.py
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/nix.py
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/oberon.py
--rw-r--r--   0        0        0    22961 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/objective.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ooc.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/openscad.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/other.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/parasail.py
--rw-r--r--   0        0        0    25904 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/parsers.py
--rw-r--r--   0        0        0    30880 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/pascal.py
--rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/pawn.py
--rw-r--r--   0        0        0    39170 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/perl.py
--rw-r--r--   0        0        0    23252 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/phix.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/php.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/pointless.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/pony.py
--rw-r--r--   0        0        0    12677 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/praat.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/procfile.py
--rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/prolog.py
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/promql.py
--rw-r--r--   0        0        0     8748 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/prql.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ptx.py
--rw-r--r--   0        0        0    53400 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/python.py
--rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/q.py
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/qlik.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/qvt.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/r.py
--rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/rdf.py
--rw-r--r--   0        0        0    18248 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/rebol.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/resource.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ride.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/rita.py
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/rnc.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/roboconf.py
--rw-r--r--   0        0        0    18449 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/robotframework.py
--rw-r--r--   0        0        0    22672 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ruby.py
--rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/rust.py
--rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/sas.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/savi.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/scdoc.py
--rw-r--r--   0        0        0    70014 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/scripting.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/sgf.py
--rw-r--r--   0        0        0    36466 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/shell.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/sieve.py
--rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/slash.py
--rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/smalltalk.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/smithy.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/smv.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/snobol.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/solidity.py
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/sophia.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/special.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/spice.py
--rw-r--r--   0        0        0    42107 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/sql.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/srcinfo.py
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/stata.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/supercollider.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/tal.py
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/tcl.py
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/teal.py
--rw-r--r--   0        0        0    72610 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/templates.py
--rw-r--r--   0        0        0     9719 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/teraterm.py
--rw-r--r--   0        0        0    10767 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/testing.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/text.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/textedit.py
--rw-r--r--   0        0        0    15310 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/textfmts.py
--rw-r--r--   0        0        0    16659 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/theorem.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/thingsdb.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/tlb.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/tls.py
--rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/tnt.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/trafficscript.py
--rw-r--r--   0        0        0     8207 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/typoscript.py
--rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ul4.py
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/unicon.py
--rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/urbi.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/usd.py
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/varnish.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/verification.py
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/verifpal.py
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/vip.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/vyper.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/web.py
--rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/webassembly.py
--rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/webidl.py
--rw-r--r--   0        0        0    40549 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/webmisc.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/wgsl.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/whiley.py
--rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/wowtoc.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/wren.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/x10.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/xorg.py
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/yang.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/yara.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/zig.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/__init__.py
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/_mapping.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/abap.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/algol.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/algol_nu.py
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/arduino.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/autumn.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/borland.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/bw.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/colorful.py
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/default.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/dracula.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/emacs.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/friendly.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/friendly_grayscale.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/fruity.py
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/gh_dark.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/gruvbox.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/igor.py
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/inkpot.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/lightbulb.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/lilypond.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/lovelace.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/manni.py
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/material.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/monokai.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/murphy.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/native.py
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/nord.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/onedark.py
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/paraiso_dark.py
--rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/paraiso_light.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/pastie.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/perldoc.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/rainbow_dash.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/rrt.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/sas.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/solarized.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/staroffice.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/stata_dark.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/stata_light.py
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/tango.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/trac.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/vim.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/vs.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/xcode.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/zenburn.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/METADATA
--rw-r--r--   0        0        0    27426 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/REQUESTED
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/WHEEL
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/entry_points.txt
--rw-r--r--   0        0        0    10281 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/AUTHORS
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/INSTALLER
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/LICENSE
--rw-r--r--   0        0        0     8354 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/METADATA
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/REQUESTED
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/top_level.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/zip-safe
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse/VERSION
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse/__init__.py
--rw-r--r--   0        0        0     6654 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse/timeparse.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse/tests/__init__.py
--rw-r--r--   0        0        0    16386 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse/tests/testtimeparse.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/DESCRIPTION.rst
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/INSTALLER
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/METADATA
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/REQUESTED
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/WHEEL
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/top_level.txt
--rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/__init__.py
--rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/__main__.py
--rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_export_format.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_inspect.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_pick.py
--rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_timer.py
--rw-r--r--   0        0        0    22784 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_win32_console.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_windows.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_windows_renderer.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_wrap.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/abc.py
--rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/align.py
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/ansi.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/bar.py
--rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/box.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/cells.py
--rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/columns.py
--rw-r--r--   0        0        0    99101 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/constrain.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/containers.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/control.py
--rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/default_styles.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/diagnose.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/filesize.py
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/highlighter.py
--rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/json.py
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/jupyter.py
--rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/layout.py
--rw-r--r--   0        0        0    14271 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/live.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/live_render.py
--rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/logging.py
--rw-r--r--   0        0        0    26167 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/markdown.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/measure.py
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/pager.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/palette.py
--rw-r--r--   0        0        0    10705 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/panel.py
--rw-r--r--   0        0        0    35812 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/pretty.py
--rw-r--r--   0        0        0    59703 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/progress.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/progress_bar.py
--rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/prompt.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/py.typed
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/region.py
--rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/repr.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/rule.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/scope.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/screen.py
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/spinner.py
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/status.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/style.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/styled.py
--rw-r--r--   0        0        0    35367 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/syntax.py
--rw-r--r--   0        0        0    39644 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/terminal_theme.py
--rw-r--r--   0        0        0    47300 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/themes.py
--rw-r--r--   0        0        0    29529 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/traceback.py
--rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/tree.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/LICENSE
--rw-r--r--   0        0        0    18636 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/METADATA
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/WHEEL
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham/__init__.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham/_core.py
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham/nt.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham/posix/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham/posix/_core.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham/posix/proc.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham/posix/ps.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/INSTALLER
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/LICENSE
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/METADATA
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/REQUESTED
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/WHEEL
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/top_level.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/zip-safe
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/METADATA
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/REQUESTED
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/WHEEL
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/top_level.txt
--rw-r--r--   0        0        0    15939 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/time_machine/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/time_machine/py.typed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/LICENSE
--rw-r--r--   0        0        0    21388 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/METADATA
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/REQUESTED
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/WHEEL
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/__init__.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/_compat_utils.py
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/_completion_click7.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/_completion_click8.py
--rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/_completion_shared.py
--rw-r--r--   0        0        0    19743 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/_typing.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/colors.py
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/completion.py
--rw-r--r--   0        0        0    26545 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/core.py
--rw-r--r--   0        0        0    39310 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/main.py
--rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/models.py
--rw-r--r--   0        0        0    13401 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/py.typed
--rw-r--r--   0        0        0    23654 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/rich_utils.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/testing.py
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/utils.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/LICENSE
--rw-r--r--   0        0        0    14615 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/METADATA
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/WHEEL
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/METADATA
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/WHEEL
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/__init__.py
--rw-r--r--   0        0        0     9084 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zones
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/CET
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/CST6CDT
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Cuba
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/EET
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/EST
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/EST5EDT
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Egypt
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Eire
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Factory
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GB
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GB-Eire
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GMT
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GMT+0
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GMT-0
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GMT0
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Greenwich
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/HST
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Hongkong
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Iceland
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Iran
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Israel
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Jamaica
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Japan
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Kwajalein
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Libya
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/MET
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/MST
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/MST7MDT
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/NZ
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/NZ-CHAT
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Navajo
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/PRC
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/PST8PDT
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Poland
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Portugal
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/ROC
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/ROK
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Singapore
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Turkey
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/UCT
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/UTC
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Universal
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/W-SU
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/WET
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Zulu
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/__init__.py
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/iso3166.tab
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/leapseconds
--rw-r--r--   0        0        0   109388 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/tzdata.zi
--rw-r--r--   0        0        0    18846 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/zone.tab
--rw-r--r--   0        0        0    17582 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/zone1970.tab
--rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/zonenow.tab
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Abidjan
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Accra
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Addis_Ababa
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Algiers
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Asmara
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Asmera
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Bamako
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Bangui
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Banjul
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Bissau
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Blantyre
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Brazzaville
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Bujumbura
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Cairo
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Casablanca
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Ceuta
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Conakry
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Dakar
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Dar_es_Salaam
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Djibouti
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Douala
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/El_Aaiun
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Freetown
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Gaborone
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Harare
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Johannesburg
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Juba
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Kampala
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Khartoum
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Kigali
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Kinshasa
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Lagos
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Libreville
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Lome
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Luanda
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Lubumbashi
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Lusaka
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Malabo
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Maputo
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Maseru
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Mbabane
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Mogadishu
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Monrovia
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Nairobi
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Ndjamena
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Niamey
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Nouakchott
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Ouagadougou
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Porto-Novo
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Sao_Tome
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Timbuktu
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Tripoli
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Tunis
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Windhoek
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/__init__.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Adak
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Anchorage
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Anguilla
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Antigua
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Araguaina
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Aruba
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Asuncion
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Atikokan
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Atka
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Bahia
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Bahia_Banderas
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Barbados
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Belem
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Belize
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Blanc-Sablon
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Boa_Vista
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Bogota
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Boise
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Buenos_Aires
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cambridge_Bay
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Campo_Grande
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cancun
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Caracas
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Catamarca
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cayenne
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cayman
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Chicago
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Chihuahua
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Ciudad_Juarez
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Coral_Harbour
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cordoba
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Costa_Rica
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Creston
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cuiaba
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Curacao
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Danmarkshavn
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Dawson
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Dawson_Creek
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Denver
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Detroit
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Dominica
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Edmonton
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Eirunepe
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/El_Salvador
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Ensenada
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Fort_Nelson
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Fort_Wayne
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Fortaleza
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Glace_Bay
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Godthab
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Goose_Bay
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Grand_Turk
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Grenada
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Guadeloupe
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Guatemala
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Guayaquil
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Guyana
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Halifax
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Havana
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Hermosillo
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indianapolis
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Inuvik
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Iqaluit
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Jamaica
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Jujuy
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Juneau
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Knox_IN
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Kralendijk
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/La_Paz
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Lima
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Los_Angeles
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Louisville
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Lower_Princes
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Maceio
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Managua
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Manaus
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Marigot
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Martinique
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Matamoros
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Mazatlan
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Mendoza
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Menominee
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Merida
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Metlakatla
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Mexico_City
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Miquelon
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Moncton
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Monterrey
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Montevideo
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Montreal
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Montserrat
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nassau
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/New_York
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nipigon
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nome
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Noronha
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nuuk
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Ojinaga
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Panama
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Pangnirtung
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Paramaribo
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Phoenix
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Port-au-Prince
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Port_of_Spain
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Porto_Acre
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Porto_Velho
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Puerto_Rico
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Punta_Arenas
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Rainy_River
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Rankin_Inlet
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Recife
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Regina
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Resolute
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Rio_Branco
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Rosario
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Santa_Isabel
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Santarem
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Santiago
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Santo_Domingo
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Sao_Paulo
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Scoresbysund
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Shiprock
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Sitka
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/St_Barthelemy
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/St_Johns
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/St_Kitts
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/St_Lucia
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/St_Thomas
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/St_Vincent
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Swift_Current
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Tegucigalpa
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Thule
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Thunder_Bay
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Tijuana
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Toronto
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Tortola
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Vancouver
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Virgin
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Whitehorse
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Winnipeg
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Yakutat
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Yellowknife
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/__init__.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Buenos_Aires
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Catamarca
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/ComodRivadavia
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Cordoba
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Jujuy
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/La_Rioja
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Mendoza
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Rio_Gallegos
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Salta
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/San_Juan
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/San_Luis
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Tucuman
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Ushuaia
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/__init__.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Indianapolis
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Knox
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Marengo
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Petersburg
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Tell_City
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Vevay
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Vincennes
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Winamac
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/__init__.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Kentucky/Louisville
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Kentucky/Monticello
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Kentucky/__init__.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/North_Dakota/Beulah
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/North_Dakota/Center
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/North_Dakota/New_Salem
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/North_Dakota/__init__.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Casey
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Davis
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/DumontDUrville
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Macquarie
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Mawson
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/McMurdo
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Palmer
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Rothera
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/South_Pole
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Syowa
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Troll
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Vostok
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/__init__.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Arctic/Longyearbyen
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Arctic/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Aden
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Almaty
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Amman
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Anadyr
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Aqtau
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Aqtobe
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ashgabat
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ashkhabad
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Atyrau
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Baghdad
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Bahrain
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Baku
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Bangkok
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Barnaul
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Beirut
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Bishkek
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Brunei
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Calcutta
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Chita
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Choibalsan
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Chongqing
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Chungking
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Colombo
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Dacca
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Damascus
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Dhaka
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Dili
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Dubai
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Dushanbe
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Famagusta
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Gaza
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Harbin
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Hebron
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ho_Chi_Minh
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Hong_Kong
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Hovd
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Irkutsk
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Istanbul
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Jakarta
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Jayapura
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Jerusalem
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kabul
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kamchatka
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Karachi
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kashgar
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kathmandu
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Katmandu
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Khandyga
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kolkata
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Krasnoyarsk
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kuala_Lumpur
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kuching
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kuwait
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Macao
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Macau
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Magadan
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Makassar
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Manila
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Muscat
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Nicosia
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Novokuznetsk
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Novosibirsk
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Omsk
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Oral
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Phnom_Penh
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Pontianak
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Pyongyang
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Qatar
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Qostanay
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Qyzylorda
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Rangoon
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Riyadh
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Saigon
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Sakhalin
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Samarkand
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Seoul
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Shanghai
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Singapore
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Srednekolymsk
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Taipei
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tashkent
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tbilisi
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tehran
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tel_Aviv
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Thimbu
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Thimphu
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tokyo
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tomsk
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ujung_Pandang
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ulaanbaatar
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ulan_Bator
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Urumqi
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ust-Nera
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Vientiane
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Vladivostok
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Yakutsk
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Yangon
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Yekaterinburg
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Yerevan
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/__init__.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Azores
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Bermuda
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Canary
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Cape_Verde
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Faeroe
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Faroe
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Jan_Mayen
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Madeira
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Reykjavik
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/South_Georgia
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/St_Helena
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Stanley
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/__init__.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/ACT
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Adelaide
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Brisbane
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Broken_Hill
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Canberra
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Currie
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Darwin
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Eucla
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Hobart
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/LHI
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Lindeman
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Lord_Howe
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Melbourne
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/NSW
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/North
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Perth
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Queensland
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/South
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Sydney
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Tasmania
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Victoria
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/West
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Yancowinna
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/__init__.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Brazil/Acre
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Brazil/DeNoronha
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Brazil/East
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Brazil/West
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Brazil/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Atlantic
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Central
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Eastern
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Mountain
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Newfoundland
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Pacific
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Saskatchewan
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Yukon
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/__init__.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Chile/Continental
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Chile/EasterIsland
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Chile/__init__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+0
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+1
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+10
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+11
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+12
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+2
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+3
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+4
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+5
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+6
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+7
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+8
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+9
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-0
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-1
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-10
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-11
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-12
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-13
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-14
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-2
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-3
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-4
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-5
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-6
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-7
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-8
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-9
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT0
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/Greenwich
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/UCT
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/UTC
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/Universal
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/Zulu
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/__init__.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Amsterdam
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Andorra
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Astrakhan
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Athens
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Belfast
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Belgrade
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Berlin
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Bratislava
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Brussels
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Bucharest
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Budapest
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Busingen
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Chisinau
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Copenhagen
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Dublin
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Gibraltar
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Guernsey
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Helsinki
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Isle_of_Man
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Istanbul
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Jersey
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kaliningrad
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kiev
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kirov
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kyiv
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Lisbon
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Ljubljana
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/London
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Luxembourg
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Madrid
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Malta
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Mariehamn
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Minsk
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Monaco
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Moscow
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Nicosia
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Oslo
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Paris
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Podgorica
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Prague
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Riga
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Rome
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Samara
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/San_Marino
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Sarajevo
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Saratov
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Simferopol
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Skopje
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Sofia
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Stockholm
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Tallinn
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Tirane
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Tiraspol
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Ulyanovsk
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Uzhgorod
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Vaduz
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Vatican
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Vienna
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Vilnius
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Volgograd
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Warsaw
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Zagreb
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Zaporozhye
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Zurich
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Antananarivo
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Chagos
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Christmas
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Cocos
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Comoro
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Kerguelen
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Mahe
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Maldives
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Mauritius
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Mayotte
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Reunion
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/__init__.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Mexico/BajaNorte
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Mexico/BajaSur
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Mexico/General
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Mexico/__init__.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Apia
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Auckland
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Bougainville
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Chatham
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Chuuk
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Easter
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Efate
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Enderbury
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Fakaofo
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Fiji
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Funafuti
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Galapagos
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Gambier
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Guadalcanal
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Guam
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Honolulu
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Johnston
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Kanton
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Kiritimati
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Kosrae
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Kwajalein
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Majuro
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Marquesas
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Midway
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Nauru
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Niue
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Norfolk
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Noumea
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Pago_Pago
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Palau
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Pitcairn
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Pohnpei
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Ponape
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Port_Moresby
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Rarotonga
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Saipan
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Samoa
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Tahiti
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Tarawa
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Tongatapu
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Truk
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Wake
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Wallis
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Yap
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Alaska
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Aleutian
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Arizona
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Central
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/East-Indiana
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Eastern
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Hawaii
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Indiana-Starke
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Michigan
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Mountain
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Pacific
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Samoa
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/__init__.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/INSTALLER
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/LICENSE
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/LICENSE_APACHE
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/METADATA
--rw-r--r--   0        0        0    54836 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/REQUESTED
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/WHEEL
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/top_level.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 daikanban-0.1.1/daikanban/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 daikanban-0.1.1/daikanban/billboard_art.txt
--rw-r--r--   0        0        0    41319 2020-02-02 00:00:00.000000 daikanban-0.1.1/daikanban/interface.py
--rwxr-xr-x   0        0        0     1012 2020-02-02 00:00:00.000000 daikanban-0.1.1/daikanban/main.py
--rw-r--r--   0        0        0    30397 2020-02-02 00:00:00.000000 daikanban-0.1.1/daikanban/model.py
--rw-r--r--   0        0        0     5462 2020-02-02 00:00:00.000000 daikanban-0.1.1/daikanban/prompt.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 daikanban-0.1.1/daikanban/score.py
--rw-r--r--   0        0        0    10555 2020-02-02 00:00:00.000000 daikanban-0.1.1/daikanban/settings.py
--rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 daikanban-0.1.1/daikanban/utils.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 daikanban-0.1.1/doc/dkmarkdown.md
--rw-r--r--   0        0        0   864213 2020-02-02 00:00:00.000000 daikanban-0.1.1/doc/screenshot_v0_1_0.png
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 daikanban-0.1.1/doc/shell.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 daikanban-0.1.1/tests/test_interface.py
--rw-r--r--   0        0        0    24390 2020-02-02 00:00:00.000000 daikanban-0.1.1/tests/test_model.py
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 daikanban-0.1.1/tests/test_settings.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 daikanban-0.1.1/tests/test_utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 daikanban-0.1.1/.gitignore
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 daikanban-0.1.1/AUTHORS.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 daikanban-0.1.1/LICENSE
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 daikanban-0.1.1/README.md
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 daikanban-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 daikanban-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 daikanban-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 daikanban-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 daikanban-0.1.2/TODO.md
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 daikanban-0.1.2/ruff.toml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/.lock
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/pyvenv.cfg
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/bin/activate
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/bin/activate.csh
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/bin/activate.fish
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/bin/activate.nu
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/bin/activate.ps1
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/bin/activate_this.py
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/bin/daikanban
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/bin/markdown-it
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/bin/pygmentize
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/bin/python -> /Users/jerm/.pyenv/versions/3.11.0/bin/python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/bin/python3.11 -> python
+-rwxr-xr-x   0        0        0   120544 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/_time_machine.cpython-311-darwin.so
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/six.py
+-rw-r--r--   0        0        0   117599 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typing_extensions.py
+-rw-r--r--   0        0        0    12151 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/annotated_types/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/annotated_types/py.typed
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/annotated_types/test_cases.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0    12879 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/METADATA
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/__init__.py
+-rw-r--r--   0        0        0    18744 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/_compat.py
+-rw-r--r--   0        0        0    24069 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/_termui_impl.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/_textwrap.py
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/_winconsole.py
+-rw-r--r--   0        0        0   114086 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/core.py
+-rw-r--r--   0        0        0    18719 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/decorators.py
+-rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/exceptions.py
+-rw-r--r--   0        0        0     9706 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/formatting.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/globals.py
+-rw-r--r--   0        0        0    19067 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/py.typed
+-rw-r--r--   0        0        0    18460 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/shell_completion.py
+-rw-r--r--   0        0        0    28324 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/termui.py
+-rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/testing.py
+-rw-r--r--   0        0        0    36391 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/types.py
+-rw-r--r--   0        0        0    20298 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/utils.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/LICENSE.rst
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/METADATA
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/WHEEL
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/top_level.txt
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/INSTALLER
+-rw-r--r--   0        0        0    17158 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/METADATA
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/REQUESTED
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/WHEEL
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/billboard_art.txt
+-rw-r--r--   0        0        0    39535 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/interface.py
+-rwxr-xr-x   0        0        0     1012 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/main.py
+-rw-r--r--   0        0        0    27508 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/model.py
+-rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/prompt.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/score.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/settings.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/utils.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/__init__.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/_common.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/_version.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/easter.py
+-rw-r--r--   0        0        0    24903 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/relativedelta.py
+-rw-r--r--   0        0        0    66557 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/rrule.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/tzwin.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/utils.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/parser/__init__.py
+-rw-r--r--   0        0        0    58796 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/parser/_parser.py
+-rw-r--r--   0        0        0    13233 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/parser/isoparser.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/tz/__init__.py
+-rw-r--r--   0        0        0    12977 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/tz/_common.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/tz/_factories.py
+-rw-r--r--   0        0        0    62855 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/tz/tz.py
+-rw-r--r--   0        0        0    12935 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/tz/win.py
+-rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/zoneinfo/__init__.py
+-rw-r--r--   0        0        0   156400 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/zoneinfo/dateutil-zoneinfo.tar.gz
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/zoneinfo/rebuild.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/_compat.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/_punycode.py
+-rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/main.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/parser_block.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/parser_core.py
+-rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/parser_inline.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/port.yaml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/py.typed
+-rw-r--r--   0        0        0     9970 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/renderer.py
+-rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/ruler.py
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/token.py
+-rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/tree.py
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/cli/__init__.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/cli/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/common/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/common/entities.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/common/html_blocks.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/common/html_re.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/common/normalize_url.py
+-rw-r--r--   0        0        0    10728 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/common/utils.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/helpers/__init__.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_destination.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_label.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_title.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/presets/__init__.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/presets/commonmark.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/presets/default.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/presets/zero.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/__init__.py
+-rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/blockquote.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/code.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/fence.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/heading.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/hr.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/html_block.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/lheading.py
+-rw-r--r--   0        0        0     9668 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/list.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/paragraph.py
+-rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/reference.py
+-rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/state_block.py
+-rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/table.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_core/__init__.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_core/block.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_core/inline.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_core/linkify.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_core/normalize.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_core/replacements.py
+-rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_core/smartquotes.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_core/state_core.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_core/text_join.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/__init__.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/autolink.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/backticks.py
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/balance_pairs.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/emphasis.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/entity.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/escape.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/fragments_join.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/html_inline.py
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/image.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/link.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/linkify.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/newline.py
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/state_inline.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/strikethrough.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/text.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE.markdown-it
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl/__init__.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl/_decode.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl/_encode.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl/_format.py
+-rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl/_parse.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl/_url.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl/py.typed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/METADATA
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/REQUESTED
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/WHEEL
+-rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/__version__.py
+-rw-r--r--   0        0        0     8780 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/_helpers.py
+-rwxr-xr-x   0        0        0   539840 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/_pendulum.cpython-311-darwin.so
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/_pendulum.pyi
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/constants.py
+-rw-r--r--   0        0        0    24071 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/date.py
+-rw-r--r--   0        0        0    42309 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/datetime.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/day.py
+-rw-r--r--   0        0        0    14780 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/duration.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/exceptions.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/helpers.py
+-rw-r--r--   0        0        0    13543 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/interval.py
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/py.typed
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/time.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/formatting/__init__.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/formatting/difference_formatter.py
+-rw-r--r--   0        0        0    22499 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/formatting/formatter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/__init__.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/cs/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/cs/custom.py
+-rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/cs/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/da/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/da/custom.py
+-rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/da/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/de/__init__.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/de/custom.py
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/de/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/en/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/en/custom.py
+-rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/en/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/en_gb/__init__.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/en_gb/custom.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/en_gb/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/en_us/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/en_us/custom.py
+-rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/en_us/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/es/__init__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/es/custom.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/es/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/fa/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/fa/custom.py
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/fa/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/fo/__init__.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/fo/custom.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/fo/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/fr/__init__.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/fr/custom.py
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/fr/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/he/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/he/custom.py
+-rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/he/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/id/__init__.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/id/custom.py
+-rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/id/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/it/__init__.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/it/custom.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/it/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/ja/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/ja/custom.py
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/ja/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/ko/__init__.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/ko/custom.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/ko/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/lt/__init__.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/lt/custom.py
+-rw-r--r--   0        0        0     8342 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/lt/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/nb/__init__.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/nb/custom.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/nb/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/nl/__init__.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/nl/custom.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/nl/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/nn/__init__.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/nn/custom.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/nn/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/pl/__init__.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/pl/custom.py
+-rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/pl/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/pt_br/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/pt_br/custom.py
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/pt_br/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/ru/__init__.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/ru/custom.py
+-rw-r--r--   0        0        0     9529 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/ru/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/sk/__init__.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/sk/custom.py
+-rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/sk/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/sv/__init__.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/sv/custom.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/sv/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/tr/__init__.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/tr/custom.py
+-rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/tr/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/zh/__init__.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/zh/custom.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/zh/locale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/mixins/__init__.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/mixins/default.py
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/parsing/__init__.py
+-rw-r--r--   0        0        0    13886 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/parsing/iso8601.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/parsing/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/testing/__init__.py
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/testing/traveller.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/tz/__init__.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/tz/exceptions.py
+-rw-r--r--   0        0        0     8429 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/tz/local_timezone.py
+-rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/tz/timezone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/tz/data/__init__.py
+-rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/tz/data/windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/utils/__init__.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/utils/_compat.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/utils/_zoneinfo.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0    10278 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/license_files/LICENSE
+-rw-r--r--   0        0        0    12780 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/__init__.py
+-rw-r--r--   0        0        0    11913 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_migration.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/alias_generators.py
+-rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/aliases.py
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/annotated_handlers.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/class_validators.py
+-rw-r--r--   0        0        0    21493 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/color.py
+-rw-r--r--   0        0        0    29141 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/config.py
+-rw-r--r--   0        0        0    13450 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/dataclasses.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/datetime_parse.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/decorator.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/env_settings.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/error_wrappers.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/errors.py
+-rw-r--r--   0        0        0    45930 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/fields.py
+-rw-r--r--   0        0        0    14621 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/functional_serializers.py
+-rw-r--r--   0        0        0    24313 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/functional_validators.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/generics.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/json.py
+-rw-r--r--   0        0        0   102807 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/json_schema.py
+-rw-r--r--   0        0        0    65892 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/main.py
+-rw-r--r--   0        0        0    55131 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/mypy.py
+-rw-r--r--   0        0        0    21225 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/networks.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/py.typed
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/root_model.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/schema.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/tools.py
+-rw-r--r--   0        0        0    18104 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/type_adapter.py
+-rw-r--r--   0        0        0    89607 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/types.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/typing.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/utils.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/validate_call_decorator.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/validators.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/version.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/warnings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/__init__.py
+-rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_config.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_core_metadata.py
+-rw-r--r--   0        0        0    24332 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_core_utils.py
+-rw-r--r--   0        0        0     8481 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_dataclasses.py
+-rw-r--r--   0        0        0    30627 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_decorators.py
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_decorators_v1.py
+-rw-r--r--   0        0        0    26369 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_discriminated_union.py
+-rw-r--r--   0        0        0    13184 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_fields.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_forward_ref.py
+-rw-r--r--   0        0        0    98557 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_generate_schema.py
+-rw-r--r--   0        0        0    22227 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_generics.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_git.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_internal_dataclass.py
+-rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_known_annotated_metadata.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_mock_val_ser.py
+-rw-r--r--   0        0        0    28114 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_model_construction.py
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_repr.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_schema_generation_shared.py
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_signature.py
+-rw-r--r--   0        0        0    29085 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_std_types_schema.py
+-rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_typing_extra.py
+-rw-r--r--   0        0        0    12670 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_utils.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_validate_call.py
+-rw-r--r--   0        0        0    10054 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/deprecated/__init__.py
+-rw-r--r--   0        0        0     9871 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/deprecated/class_validators.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/deprecated/config.py
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/deprecated/copy_internals.py
+-rw-r--r--   0        0        0    10778 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/deprecated/decorator.py
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/deprecated/json.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/deprecated/parse.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/deprecated/tools.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/plugin/__init__.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/plugin/_loader.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/plugin/_schema_validator.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/__init__.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/_hypothesis_plugin.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/annotated_types.py
+-rw-r--r--   0        0        0    14595 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/class_validators.py
+-rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/color.py
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/config.py
+-rw-r--r--   0        0        0    18073 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/dataclasses.py
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/datetime_parse.py
+-rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/decorator.py
+-rw-r--r--   0        0        0    14039 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/env_settings.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/error_wrappers.py
+-rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/errors.py
+-rw-r--r--   0        0        0    50485 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/fields.py
+-rw-r--r--   0        0        0    17805 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/generics.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/json.py
+-rw-r--r--   0        0        0    44376 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/main.py
+-rw-r--r--   0        0        0    38745 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/mypy.py
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/networks.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/py.typed
+-rw-r--r--   0        0        0    47614 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/schema.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/tools.py
+-rw-r--r--   0        0        0    35379 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/types.py
+-rw-r--r--   0        0        0    18996 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/typing.py
+-rw-r--r--   0        0        0    25809 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/utils.py
+-rw-r--r--   0        0        0    21887 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/validators.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/version.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/INSTALLER
+-rw-r--r--   0        0        0    85087 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/METADATA
+-rw-r--r--   0        0        0     8852 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/REQUESTED
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/WHEEL
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core/__init__.py
+-rwxr-xr-x   0        0        0  3955160 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core/_pydantic_core.cpython-311-darwin.so
+-rw-r--r--   0        0        0    33290 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core/_pydantic_core.pyi
+-rw-r--r--   0        0        0   134918 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core/core_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core/py.typed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/INSTALLER
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/METADATA
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/REQUESTED
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/WHEEL
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/license_files/LICENSE
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/__init__.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/__main__.py
+-rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/filter.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatter.py
+-rw-r--r--   0        0        0    35044 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/modeline.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/scanner.py
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/style.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/token.py
+-rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/unistring.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/util.py
+-rw-r--r--   0        0        0    40338 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/__init__.py
+-rwxr-xr-x   0        0        0     4176 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35640 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/html.py
+-rw-r--r--   0        0        0    23116 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/img.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19303 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    12113 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_ada_builtins.py
+-rw-r--r--   0        0        0    27287 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_asy_builtins.py
+-rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_cl_builtins.py
+-rw-r--r--   0        0        0   105182 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_cocoa_builtins.py
+-rw-r--r--   0        0        0    18414 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_csound_builtins.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_css_builtins.py
+-rw-r--r--   0        0        0    11883 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_julia_builtins.py
+-rw-r--r--   0        0        0   134510 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_lasso_builtins.py
+-rw-r--r--   0        0        0   108094 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_lilypond_builtins.py
+-rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_lua_builtins.py
+-rw-r--r--   0        0        0    68026 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    24713 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_mql_builtins.py
+-rw-r--r--   0        0        0    25842 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_mysql_builtins.py
+-rw-r--r--   0        0        0    49398 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_openedge_builtins.py
+-rw-r--r--   0        0        0   107930 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_php_builtins.py
+-rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_postgres_builtins.py
+-rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_qlik_builtins.py
+-rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_scheme_builtins.py
+-rw-r--r--   0        0        0    52413 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_scilab_builtins.py
+-rw-r--r--   0        0        0    26781 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_sourcemod_builtins.py
+-rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_stan_builtins.py
+-rw-r--r--   0        0        0    27227 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_stata_builtins.py
+-rw-r--r--   0        0        0    15460 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_tsql_builtins.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_usd_builtins.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_vbscript_builtins.py
+-rw-r--r--   0        0        0    57066 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_vim_builtins.py
+-rw-r--r--   0        0        0    11676 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/actionscript.py
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ada.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/agile.py
+-rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/algebra.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ambient.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/amdgpu.py
+-rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ampl.py
+-rw-r--r--   0        0        0    30766 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/apdlexer.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/apl.py
+-rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/archetype.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/arrow.py
+-rw-r--r--   0        0        0    11417 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/arturo.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/asc.py
+-rw-r--r--   0        0        0    41243 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/asm.py
+-rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/asn1.py
+-rw-r--r--   0        0        0    19815 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/automation.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/bare.py
+-rw-r--r--   0        0        0    27923 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/basic.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/bdd.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/berry.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/bibtex.py
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/blueprint.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/boa.py
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/bqn.py
+-rw-r--r--   0        0        0    28112 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/business.py
+-rw-r--r--   0        0        0    17946 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/c_cpp.py
+-rw-r--r--   0        0        0    29206 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/c_like.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/capnproto.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/carbon.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/cddl.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/chapel.py
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/clean.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/comal.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/compiled.py
+-rw-r--r--   0        0        0    50077 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/configs.py
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/console.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/cplint.py
+-rw-r--r--   0        0        0    15757 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/crystal.py
+-rw-r--r--   0        0        0    16994 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/csound.py
+-rw-r--r--   0        0        0    25322 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/css.py
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/d.py
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/dalvik.py
+-rw-r--r--   0        0        0    27032 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/data.py
+-rw-r--r--   0        0        0     8099 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/dax.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/devicetree.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/diff.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/dns.py
+-rw-r--r--   0        0        0    37623 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/dotnet.py
+-rw-r--r--   0        0        0    36786 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/dsls.py
+-rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/dylan.py
+-rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ecl.py
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/eiffel.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/elm.py
+-rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/elpi.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/email.py
+-rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/erlang.py
+-rw-r--r--   0        0        0    10396 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/esoteric.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ezhil.py
+-rw-r--r--   0        0        0    19531 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/factor.py
+-rw-r--r--   0        0        0    10197 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/fantom.py
+-rw-r--r--   0        0        0     9646 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/felix.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/fift.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/floscript.py
+-rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/forth.py
+-rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/fortran.py
+-rw-r--r--   0        0        0    26212 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/foxpro.py
+-rw-r--r--   0        0        0    26914 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/freefem.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/func.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/functional.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/futhark.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/gcodelexer.py
+-rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/gdscript.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/go.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/grammar_notation.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/graph.py
+-rw-r--r--   0        0        0    39026 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/graphics.py
+-rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/graphql.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/graphviz.py
+-rwxr-xr-x   0        0        0     3991 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/gsql.py
+-rw-r--r--   0        0        0    32898 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/haskell.py
+-rw-r--r--   0        0        0    30976 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/haxe.py
+-rw-r--r--   0        0        0    22520 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/hdl.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/hexdump.py
+-rw-r--r--   0        0        0    20260 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/html.py
+-rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/idl.py
+-rw-r--r--   0        0        0    31658 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/igor.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/inferno.py
+-rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/installers.py
+-rw-r--r--   0        0        0    57119 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/int_fiction.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/iolang.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/j.py
+-rw-r--r--   0        0        0    62859 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/javascript.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/jmespath.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/jslt.py
+-rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/jsonnet.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/jsx.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/julia.py
+-rw-r--r--   0        0        0    72929 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/jvm.py
+-rw-r--r--   0        0        0    11406 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/kuin.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/kusto.py
+-rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ldap.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/lean.py
+-rw-r--r--   0        0        0     9753 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/lilypond.py
+-rw-r--r--   0        0        0   144398 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/lisp.py
+-rw-r--r--   0        0        0    32171 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/macaulay2.py
+-rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/make.py
+-rw-r--r--   0        0        0    60257 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/markup.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/math.py
+-rw-r--r--   0        0        0   132852 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/matlab.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/maxima.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/meson.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/mime.py
+-rw-r--r--   0        0        0    13810 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/minecraft.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/mips.py
+-rw-r--r--   0        0        0    35315 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ml.py
+-rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/modeling.py
+-rw-r--r--   0        0        0    53073 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/modula2.py
+-rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/monte.py
+-rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/mosel.py
+-rw-r--r--   0        0        0    63962 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ncl.py
+-rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/nimrod.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/nit.py
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/nix.py
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/oberon.py
+-rw-r--r--   0        0        0    22961 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/objective.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ooc.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/openscad.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/other.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/parasail.py
+-rw-r--r--   0        0        0    25904 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/parsers.py
+-rw-r--r--   0        0        0    30880 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/pascal.py
+-rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/pawn.py
+-rw-r--r--   0        0        0    39170 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/perl.py
+-rw-r--r--   0        0        0    23252 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/phix.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/php.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/pointless.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/pony.py
+-rw-r--r--   0        0        0    12677 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/praat.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/procfile.py
+-rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/prolog.py
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/promql.py
+-rw-r--r--   0        0        0     8748 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/prql.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ptx.py
+-rw-r--r--   0        0        0    53400 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/python.py
+-rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/q.py
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/qlik.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/qvt.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/r.py
+-rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/rdf.py
+-rw-r--r--   0        0        0    18248 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/rebol.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/resource.py
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ride.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/rita.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/rnc.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/roboconf.py
+-rw-r--r--   0        0        0    18449 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/robotframework.py
+-rw-r--r--   0        0        0    22672 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ruby.py
+-rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/rust.py
+-rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/sas.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/savi.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/scdoc.py
+-rw-r--r--   0        0        0    70014 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/scripting.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/sgf.py
+-rw-r--r--   0        0        0    36466 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/shell.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/sieve.py
+-rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/slash.py
+-rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/smalltalk.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/smithy.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/smv.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/snobol.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/solidity.py
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/sophia.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/special.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/spice.py
+-rw-r--r--   0        0        0    42107 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/sql.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/srcinfo.py
+-rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/stata.py
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/supercollider.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/tal.py
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/tcl.py
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/teal.py
+-rw-r--r--   0        0        0    72610 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/templates.py
+-rw-r--r--   0        0        0     9719 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/teraterm.py
+-rw-r--r--   0        0        0    10767 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/testing.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/text.py
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/textedit.py
+-rw-r--r--   0        0        0    15310 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/textfmts.py
+-rw-r--r--   0        0        0    16659 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/theorem.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/thingsdb.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/tlb.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/tls.py
+-rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/tnt.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/trafficscript.py
+-rw-r--r--   0        0        0     8207 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/typoscript.py
+-rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ul4.py
+-rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/unicon.py
+-rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/urbi.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/usd.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/varnish.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/verification.py
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/verifpal.py
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/vip.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/vyper.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/web.py
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/webassembly.py
+-rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/webidl.py
+-rw-r--r--   0        0        0    40549 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/webmisc.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/wgsl.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/whiley.py
+-rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/wowtoc.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/wren.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/x10.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/xorg.py
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/yang.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/yara.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/zig.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/_mapping.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/abap.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/algol.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/algol_nu.py
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/arduino.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/autumn.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/borland.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/bw.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/colorful.py
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/default.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/dracula.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/emacs.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/friendly.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/friendly_grayscale.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/fruity.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/gh_dark.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/gruvbox.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/igor.py
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/inkpot.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/lightbulb.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/lilypond.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/lovelace.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/manni.py
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/material.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/monokai.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/murphy.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/native.py
+-rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/nord.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/onedark.py
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/paraiso_dark.py
+-rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/paraiso_light.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/pastie.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/perldoc.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/rainbow_dash.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/rrt.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/sas.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/solarized.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/staroffice.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/stata_dark.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/stata_light.py
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/tango.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/trac.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/vim.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/vs.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/xcode.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/zenburn.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/METADATA
+-rw-r--r--   0        0        0    27426 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/REQUESTED
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/WHEEL
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0    10281 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/AUTHORS
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/LICENSE
+-rw-r--r--   0        0        0     8354 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/METADATA
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/REQUESTED
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/zip-safe
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse/VERSION
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse/__init__.py
+-rw-r--r--   0        0        0     6654 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse/timeparse.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse/tests/__init__.py
+-rw-r--r--   0        0        0    16386 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse/tests/testtimeparse.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/DESCRIPTION.rst
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/INSTALLER
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/METADATA
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/REQUESTED
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/WHEEL
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/top_level.txt
+-rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/__init__.py
+-rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/__main__.py
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_export_format.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_extension.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_fileno.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_inspect.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_loop.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_pick.py
+-rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_timer.py
+-rw-r--r--   0        0        0    22784 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_win32_console.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_windows.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_wrap.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/abc.py
+-rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/align.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/ansi.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/bar.py
+-rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/box.py
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/cells.py
+-rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/columns.py
+-rw-r--r--   0        0        0    99101 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/constrain.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/containers.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/control.py
+-rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/default_styles.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/diagnose.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/filesize.py
+-rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/highlighter.py
+-rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/json.py
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/jupyter.py
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/layout.py
+-rw-r--r--   0        0        0    14271 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/live.py
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/live_render.py
+-rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/logging.py
+-rw-r--r--   0        0        0    26167 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/markdown.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/measure.py
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/pager.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/palette.py
+-rw-r--r--   0        0        0    10705 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/panel.py
+-rw-r--r--   0        0        0    35812 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/pretty.py
+-rw-r--r--   0        0        0    59703 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/progress.py
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/progress_bar.py
+-rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/prompt.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/py.typed
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/region.py
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/repr.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/rule.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/scope.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/screen.py
+-rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/segment.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/spinner.py
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/status.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/style.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/styled.py
+-rw-r--r--   0        0        0    35367 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/syntax.py
+-rw-r--r--   0        0        0    39644 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/terminal_theme.py
+-rw-r--r--   0        0        0    47300 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/text.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/themes.py
+-rw-r--r--   0        0        0    29529 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/traceback.py
+-rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/tree.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    18636 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/METADATA
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham/__init__.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham/_core.py
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham/nt.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham/posix/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham/posix/_core.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham/posix/proc.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham/posix/ps.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/INSTALLER
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/LICENSE
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/METADATA
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/REQUESTED
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/WHEEL
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/top_level.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/zip-safe
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/METADATA
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0    15939 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/time_machine/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/time_machine/py.typed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    21388 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/__init__.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/_compat_utils.py
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/_completion_click7.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/_completion_click8.py
+-rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/_completion_shared.py
+-rw-r--r--   0        0        0    19743 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/_typing.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/colors.py
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/completion.py
+-rw-r--r--   0        0        0    26545 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/core.py
+-rw-r--r--   0        0        0    39310 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/main.py
+-rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/models.py
+-rw-r--r--   0        0        0    13401 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/py.typed
+-rw-r--r--   0        0        0    23654 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/rich_utils.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/testing.py
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/utils.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    14615 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/METADATA
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/__init__.py
+-rw-r--r--   0        0        0     9084 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zones
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/CET
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/CST6CDT
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Cuba
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/EET
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/EST
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/EST5EDT
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Egypt
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Eire
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Factory
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GB
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GB-Eire
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GMT
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GMT+0
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GMT-0
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GMT0
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Greenwich
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/HST
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Hongkong
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Iceland
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Iran
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Israel
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Jamaica
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Japan
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Kwajalein
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Libya
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/MET
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/MST
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/MST7MDT
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/NZ
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/NZ-CHAT
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Navajo
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/PRC
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/PST8PDT
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Poland
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Portugal
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/ROC
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/ROK
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Singapore
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Turkey
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/UCT
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/UTC
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Universal
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/W-SU
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/WET
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Zulu
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/__init__.py
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/iso3166.tab
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/leapseconds
+-rw-r--r--   0        0        0   109388 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/tzdata.zi
+-rw-r--r--   0        0        0    18846 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/zone.tab
+-rw-r--r--   0        0        0    17582 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/zone1970.tab
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/zonenow.tab
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Abidjan
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Accra
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Addis_Ababa
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Algiers
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Asmara
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Asmera
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Bamako
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Bangui
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Banjul
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Bissau
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Blantyre
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Brazzaville
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Bujumbura
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Cairo
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Casablanca
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Ceuta
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Conakry
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Dakar
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Dar_es_Salaam
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Djibouti
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Douala
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/El_Aaiun
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Freetown
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Gaborone
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Harare
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Johannesburg
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Juba
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Kampala
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Khartoum
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Kigali
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Kinshasa
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Lagos
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Libreville
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Lome
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Luanda
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Lubumbashi
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Lusaka
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Malabo
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Maputo
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Maseru
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Mbabane
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Mogadishu
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Monrovia
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Nairobi
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Ndjamena
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Niamey
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Nouakchott
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Ouagadougou
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Porto-Novo
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Sao_Tome
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Timbuktu
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Tripoli
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Tunis
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Windhoek
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/__init__.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Adak
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Anchorage
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Anguilla
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Antigua
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Araguaina
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Aruba
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Asuncion
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Atikokan
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Atka
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Bahia
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Bahia_Banderas
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Barbados
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Belem
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Belize
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Blanc-Sablon
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Boa_Vista
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Bogota
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Boise
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Buenos_Aires
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cambridge_Bay
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Campo_Grande
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cancun
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Caracas
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Catamarca
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cayenne
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cayman
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Chicago
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Chihuahua
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Ciudad_Juarez
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Coral_Harbour
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cordoba
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Costa_Rica
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Creston
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cuiaba
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Curacao
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Danmarkshavn
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Dawson
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Dawson_Creek
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Denver
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Detroit
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Dominica
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Edmonton
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Eirunepe
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/El_Salvador
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Ensenada
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Fort_Nelson
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Fort_Wayne
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Fortaleza
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Glace_Bay
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Godthab
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Goose_Bay
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Grand_Turk
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Grenada
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Guadeloupe
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Guatemala
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Guayaquil
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Guyana
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Halifax
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Havana
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Hermosillo
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indianapolis
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Inuvik
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Iqaluit
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Jamaica
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Jujuy
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Juneau
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Knox_IN
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Kralendijk
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/La_Paz
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Lima
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Los_Angeles
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Louisville
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Lower_Princes
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Maceio
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Managua
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Manaus
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Marigot
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Martinique
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Matamoros
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Mazatlan
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Mendoza
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Menominee
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Merida
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Metlakatla
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Mexico_City
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Miquelon
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Moncton
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Monterrey
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Montevideo
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Montreal
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Montserrat
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nassau
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/New_York
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nipigon
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nome
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Noronha
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nuuk
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Ojinaga
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Panama
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Pangnirtung
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Paramaribo
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Phoenix
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Port-au-Prince
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Port_of_Spain
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Porto_Acre
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Porto_Velho
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Puerto_Rico
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Punta_Arenas
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Rainy_River
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Rankin_Inlet
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Recife
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Regina
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Resolute
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Rio_Branco
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Rosario
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Santa_Isabel
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Santarem
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Santiago
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Santo_Domingo
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Sao_Paulo
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Scoresbysund
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Shiprock
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Sitka
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/St_Barthelemy
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/St_Johns
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/St_Kitts
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/St_Lucia
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/St_Thomas
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/St_Vincent
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Swift_Current
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Tegucigalpa
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Thule
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Thunder_Bay
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Tijuana
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Toronto
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Tortola
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Vancouver
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Virgin
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Whitehorse
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Winnipeg
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Yakutat
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Yellowknife
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/__init__.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Buenos_Aires
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Catamarca
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/ComodRivadavia
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Cordoba
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Jujuy
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/La_Rioja
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Mendoza
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Rio_Gallegos
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Salta
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/San_Juan
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/San_Luis
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Tucuman
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Ushuaia
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/__init__.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Indianapolis
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Knox
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Marengo
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Petersburg
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Tell_City
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Vevay
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Vincennes
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Winamac
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/__init__.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Kentucky/Louisville
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Kentucky/Monticello
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Kentucky/__init__.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/North_Dakota/Beulah
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/North_Dakota/Center
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/North_Dakota/New_Salem
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/North_Dakota/__init__.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Casey
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Davis
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/DumontDUrville
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Macquarie
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Mawson
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/McMurdo
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Palmer
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Rothera
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/South_Pole
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Syowa
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Troll
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Vostok
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/__init__.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Arctic/Longyearbyen
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Arctic/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Aden
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Almaty
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Amman
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Anadyr
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Aqtau
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Aqtobe
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ashgabat
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ashkhabad
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Atyrau
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Baghdad
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Bahrain
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Baku
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Bangkok
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Barnaul
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Beirut
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Bishkek
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Brunei
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Calcutta
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Chita
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Choibalsan
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Chongqing
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Chungking
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Colombo
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Dacca
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Damascus
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Dhaka
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Dili
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Dubai
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Dushanbe
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Famagusta
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Gaza
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Harbin
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Hebron
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ho_Chi_Minh
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Hong_Kong
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Hovd
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Irkutsk
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Istanbul
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Jakarta
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Jayapura
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Jerusalem
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kabul
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kamchatka
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Karachi
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kashgar
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kathmandu
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Katmandu
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Khandyga
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kolkata
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Krasnoyarsk
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kuala_Lumpur
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kuching
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kuwait
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Macao
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Macau
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Magadan
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Makassar
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Manila
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Muscat
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Nicosia
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Novokuznetsk
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Novosibirsk
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Omsk
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Oral
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Phnom_Penh
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Pontianak
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Pyongyang
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Qatar
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Qostanay
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Qyzylorda
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Rangoon
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Riyadh
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Saigon
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Sakhalin
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Samarkand
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Seoul
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Shanghai
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Singapore
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Srednekolymsk
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Taipei
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tashkent
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tbilisi
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tehran
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tel_Aviv
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Thimbu
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Thimphu
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tokyo
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tomsk
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ujung_Pandang
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ulaanbaatar
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ulan_Bator
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Urumqi
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ust-Nera
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Vientiane
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Vladivostok
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Yakutsk
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Yangon
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Yekaterinburg
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Yerevan
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/__init__.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Azores
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Bermuda
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Canary
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Cape_Verde
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Faeroe
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Faroe
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Jan_Mayen
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Madeira
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Reykjavik
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/South_Georgia
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/St_Helena
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Stanley
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/__init__.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/ACT
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Adelaide
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Brisbane
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Broken_Hill
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Canberra
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Currie
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Darwin
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Eucla
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Hobart
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/LHI
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Lindeman
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Lord_Howe
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Melbourne
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/NSW
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/North
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Perth
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Queensland
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/South
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Sydney
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Tasmania
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Victoria
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/West
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Yancowinna
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/__init__.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Brazil/Acre
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Brazil/DeNoronha
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Brazil/East
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Brazil/West
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Brazil/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Atlantic
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Central
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Eastern
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Mountain
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Newfoundland
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Pacific
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Saskatchewan
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Yukon
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/__init__.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Chile/Continental
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Chile/EasterIsland
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Chile/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+0
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+1
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+10
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+11
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+12
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+2
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+3
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+4
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+5
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+6
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+7
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+8
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT+9
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-0
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-1
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-10
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-11
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-12
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-13
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-14
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-2
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-3
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-4
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-5
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-6
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-7
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-8
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT-9
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/GMT0
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/Greenwich
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/UCT
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/UTC
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/Universal
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/Zulu
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Etc/__init__.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Amsterdam
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Andorra
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Astrakhan
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Athens
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Belfast
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Belgrade
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Berlin
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Bratislava
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Brussels
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Bucharest
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Budapest
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Busingen
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Chisinau
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Copenhagen
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Dublin
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Gibraltar
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Guernsey
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Helsinki
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Isle_of_Man
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Istanbul
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Jersey
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kaliningrad
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kiev
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kirov
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kyiv
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Lisbon
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Ljubljana
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/London
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Luxembourg
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Madrid
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Malta
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Mariehamn
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Minsk
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Monaco
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Moscow
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Nicosia
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Oslo
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Paris
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Podgorica
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Prague
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Riga
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Rome
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Samara
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/San_Marino
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Sarajevo
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Saratov
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Simferopol
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Skopje
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Sofia
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Stockholm
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Tallinn
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Tirane
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Tiraspol
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Ulyanovsk
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Uzhgorod
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Vaduz
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Vatican
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Vienna
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Vilnius
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Volgograd
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Warsaw
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Zagreb
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Zaporozhye
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Zurich
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Antananarivo
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Chagos
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Christmas
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Cocos
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Comoro
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Kerguelen
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Mahe
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Maldives
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Mauritius
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Mayotte
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/Reunion
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Indian/__init__.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Mexico/BajaNorte
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Mexico/BajaSur
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Mexico/General
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Mexico/__init__.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Apia
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Auckland
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Bougainville
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Chatham
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Chuuk
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Easter
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Efate
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Enderbury
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Fakaofo
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Fiji
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Funafuti
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Galapagos
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Gambier
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Guadalcanal
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Guam
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Honolulu
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Johnston
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Kanton
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Kiritimati
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Kosrae
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Kwajalein
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Majuro
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Marquesas
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Midway
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Nauru
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Niue
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Norfolk
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Noumea
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Pago_Pago
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Palau
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Pitcairn
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Pohnpei
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Ponape
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Port_Moresby
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Rarotonga
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Saipan
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Samoa
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Tahiti
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Tarawa
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Tongatapu
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Truk
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Wake
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Wallis
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Yap
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Alaska
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Aleutian
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Arizona
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Central
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/East-Indiana
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Eastern
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Hawaii
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Indiana-Starke
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Michigan
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Mountain
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Pacific
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Samoa
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/__init__.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/LICENSE_APACHE
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/METADATA
+-rw-r--r--   0        0        0    54836 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 daikanban-0.1.2/daikanban/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 daikanban-0.1.2/daikanban/billboard_art.txt
+-rw-r--r--   0        0        0    48126 2020-02-02 00:00:00.000000 daikanban-0.1.2/daikanban/interface.py
+-rwxr-xr-x   0        0        0     1377 2020-02-02 00:00:00.000000 daikanban-0.1.2/daikanban/main.py
+-rw-r--r--   0        0        0    30784 2020-02-02 00:00:00.000000 daikanban-0.1.2/daikanban/model.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 daikanban-0.1.2/daikanban/prompt.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 daikanban-0.1.2/daikanban/score.py
+-rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 daikanban-0.1.2/daikanban/settings.py
+-rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 daikanban-0.1.2/daikanban/utils.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 daikanban-0.1.2/doc/dkmarkdown.md
+-rw-r--r--   0        0        0   864213 2020-02-02 00:00:00.000000 daikanban-0.1.2/doc/screenshot_v0_1_0.png
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 daikanban-0.1.2/doc/shell.txt
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 daikanban-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0    15461 2020-02-02 00:00:00.000000 daikanban-0.1.2/tests/test_interface.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 daikanban-0.1.2/tests/test_main.py
+-rw-r--r--   0        0        0    25040 2020-02-02 00:00:00.000000 daikanban-0.1.2/tests/test_model.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 daikanban-0.1.2/tests/test_prompt.py
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 daikanban-0.1.2/tests/test_settings.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 daikanban-0.1.2/tests/test_utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 daikanban-0.1.2/.gitignore
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 daikanban-0.1.2/AUTHORS.md
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 daikanban-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 daikanban-0.1.2/README.md
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 daikanban-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 daikanban-0.1.2/PKG-INFO
```

### Comparing `daikanban-0.1.1/.pre-commit-config.yaml` & `daikanban-0.1.2/.pre-commit-config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -12,20 +12,34 @@
     - id: check-case-conflict
     - id: detect-private-key
     - id: check-docstring-first
 - repo: https://github.com/charliermarsh/ruff-pre-commit
   rev: 'v0.3.0'
   hooks:
     - id: ruff
+- repo: https://github.com/netromdk/vermin
+  rev: v1.6.0
+  hooks:
+    - id: vermin-all
+      args: ['-t=3.9-', '--no-tips', '--violations', '.']
 - repo: https://github.com/commitizen-tools/commitizen
-  rev: v3.16.0
+  rev: v3.25.0
   hooks:
     - id: commitizen
       stages: [commit-msg]
-- repo: local
+- repo: https://github.com/jeremander/gadzooks
+  rev: v0.2.6
   hooks:
-    - id: summarize
-      name: summarize
-      entry: summarize.sh
-      language: script
+    - id: loc-summarize
+      args: ['.']
+      pass_filenames: false
+      verbose: true
+    - id: check-version
+      args: ['--dist-dir', 'dist', '--changelog', 'CHANGELOG.md']
       pass_filenames: false
       verbose: true
+      # before pushing, require the git tag match the package version
+    # - id: check-version
+    #   args: ['--check-tag', '--dist-dir', 'dist', '--changelog', 'CHANGELOG.md']
+    #   pass_filenames: false
+    #   verbose: true
+    #   stages: [push]
```

### Comparing `daikanban-0.1.1/TODO.md` & `daikanban-0.1.2/TODO.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # TODO list
 
 ## `v0.2.0`
 
 - Settings customization
+  - Use `fancy_dataclass`
   - Generic pydantic->TOML serialization (rudimentary)
   - Use system default directory for app-specific configs? XDG?
   - Global config file stored in app folder
   - `settings` subcommand of main CLI to interact with settings
     - Also an option within the shell
   - Updates global `Settings` object whenever it is loaded/updated
   - Which items to include when making new tasks (priority/difficulty/duration can be omitted, with default)
   - Priority/difficulty upper bounds?
   - Default size limit, set of statuses to show
   - Show dates as timestamps or human-readable relative times
-  - More flexible datetime parsing
-    - E.g. "tomorrow at 3 PM"
-    - Allow things like "next Tuesday"?
-- Age-off for completed tasks to prevent displaying too many in board
-  - `archived` status? Like `kanban-python`
-  - Or set `limit=none` to view these in `completed` column
+  - `config` subcommand to view configs (at a minimum)
+- More flexible datetime parsing
+  - E.g. "tomorrow at 3 PM", "yesterday 18:00", "1800 yesterday"
+  - Allow things like "next Tuesday"?
+
+## `v0.3.0`
+
+- Set up Github Actions, test coverage
+- Default for dark terminal? (E.g. task IDs are too dark)
 - Use different scorer for completed tasks?
   - E.g. `priority-rate` would use actual duration rather than expected duration
   - Could actually be the same `TaskScorer` object, but it chooses a different field if completed
-  - But then it's less flexible (e.g. might want `completed` board to be chronological
+  - But then it's less flexible (e.g. might want `completed` board to be chronological)
   - Best solution is to allow different scorers, keyed by `TaskStatus`
-  - Short-term: don't display the score by default?
 - Error handling
   - Debug mode: env variable to drop into pdb on unhandled exception
 - Shell features
   - Simple option for JSON output in `project/task show`
   - Don't show `total_time_worked` in table if the task has never been started
   - Scrollable TUI-type thing for editing project/task fields
     - `proj/task edit [ID]`
@@ -67,19 +70,25 @@
 - Migrate from `pydantic` to `fancy_dataclass` for simplicity?
 - [prompt_toolkit](https://python-prompt-toolkit.readthedocs.io) for better prompt auto-completion, etc.
 - Allow custom task status labels?
   - todo/active/paused/complete are still the primary ones; extras would presumably be "sub-statuses" of active
   - What should be the name of this field? "status" would conflict with the existing one. Options:
         1) Use "status", rename the old one to "stage"
         2) Use "active_status", keep the old one the same
-- Github/Gitlab/Jira integration
+- External integrations
   - Query APIs
   - Bidirectional syncing
   - Interface to map between external task metadata and DaiKanban Tasks
   - Need to handle issue assignment (i.e. only pull tasks assigned to you)
+  - Platforms
+    - Github
+    - Gitlab
+    - Jira
+    - ICS calendar
+    - Thunderbird sqlite
 - Write more tests
   - Want high coverage of data model, board manipulations
   - Use `hypothesis` to generate random data?
   - Some UI tests (input command -> terminal output), though these can be brittle if output format changes
 - Better schema documentation
   - Go into more detail about the meaning(s) of priority/difficulty/duration
 - Support task logs
```

### Comparing `daikanban-0.1.1/ruff.toml` & `daikanban-0.1.2/ruff.toml`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/bin/activate` & `daikanban-0.1.2/.venv/bin/activate`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/bin/activate.csh` & `daikanban-0.1.2/.venv/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/bin/activate.fish` & `daikanban-0.1.2/.venv/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/bin/activate.nu` & `daikanban-0.1.2/.venv/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/bin/activate.ps1` & `daikanban-0.1.2/.venv/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/bin/activate_this.py` & `daikanban-0.1.2/.venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/_time_machine.cpython-311-darwin.so` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/_time_machine.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/_virtualenv.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/six.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/six.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typing_extensions.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/annotated_types/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/annotated_types/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/annotated_types/test_cases.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/annotated_types/test_cases.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/licenses/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/annotated_types-0.6.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/_compat.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/_compat.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/_termui_impl.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/_textwrap.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/_winconsole.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/core.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/core.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/decorators.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/decorators.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/exceptions.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/formatting.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/formatting.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/globals.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/globals.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/parser.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/parser.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/shell_completion.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/shell_completion.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/termui.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/termui.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/testing.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/testing.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/types.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/types.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click/utils.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click/utils.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/LICENSE.rst` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/click-8.1.7.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/ansi.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/ansitowin32.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/initialise.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/win32.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/winterm.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/tests/ansi_test.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/tests/ansitowin32_test.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/tests/initialise_test.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/tests/isatty_test.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/tests/utils.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama/tests/winterm_test.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/interface.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/interface.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/main.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/main.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/model.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/model.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/prompt.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/prompt.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/score.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/score.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/settings.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/settings.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban/utils.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban/utils.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/licenses/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/daikanban-0.1.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/_common.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/_common.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/easter.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/easter.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/relativedelta.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/relativedelta.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/rrule.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/rrule.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/utils.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/utils.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/parser/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/parser/_parser.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/parser/_parser.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/parser/isoparser.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/parser/isoparser.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/tz/_common.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/tz/_common.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/tz/_factories.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/tz/_factories.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/tz/tz.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/tz/tz.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/tz/win.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/tz/win.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/zoneinfo/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/zoneinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/zoneinfo/dateutil-zoneinfo.tar.gz` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/zoneinfo/dateutil-zoneinfo.tar.gz`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/dateutil/zoneinfo/rebuild.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/dateutil/zoneinfo/rebuild.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/_punycode.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/_punycode.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/main.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/main.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/parser_block.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/parser_block.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/parser_core.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/parser_core.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/parser_inline.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/parser_inline.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/port.yaml` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/port.yaml`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/renderer.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/renderer.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/ruler.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/ruler.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/token.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/token.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/tree.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/tree.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/utils.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/utils.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/cli/parse.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/cli/parse.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/common/html_blocks.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/common/html_blocks.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/common/html_re.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/common/html_re.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/common/normalize_url.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/common/normalize_url.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/common/utils.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/common/utils.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_destination.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_destination.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_label.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_label.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_title.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_title.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/presets/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/presets/commonmark.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/presets/commonmark.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/presets/default.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/presets/default.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/presets/zero.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/presets/zero.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/blockquote.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/blockquote.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/code.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/code.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/fence.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/fence.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/heading.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/heading.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/hr.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/hr.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/html_block.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/html_block.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/lheading.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/lheading.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/list.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/list.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/paragraph.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/paragraph.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/reference.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/reference.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/state_block.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/state_block.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_block/table.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_block/table.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_core/linkify.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_core/linkify.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_core/replacements.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_core/replacements.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_core/smartquotes.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_core/smartquotes.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_core/state_core.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_core/state_core.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_core/text_join.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_core/text_join.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/autolink.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/autolink.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/backticks.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/backticks.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/balance_pairs.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/balance_pairs.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/emphasis.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/emphasis.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/entity.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/entity.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/escape.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/escape.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/fragments_join.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/fragments_join.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/html_inline.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/html_inline.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/image.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/image.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/link.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/link.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/linkify.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/linkify.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/newline.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/newline.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/state_inline.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/state_inline.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/strikethrough.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/strikethrough.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/text.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it/rules_inline/text.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE.markdown-it` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE.markdown-it`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl/_decode.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl/_decode.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl/_encode.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl/_encode.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl/_format.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl/_format.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl/_parse.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl/_parse.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/_helpers.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/_helpers.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/_pendulum.cpython-311-darwin.so` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/_pendulum.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/_pendulum.pyi` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/_pendulum.pyi`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/constants.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/constants.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/date.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/date.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/datetime.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/datetime.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/duration.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/duration.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/helpers.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/helpers.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/interval.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/interval.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/parser.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/parser.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/time.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/time.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/formatting/difference_formatter.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/formatting/difference_formatter.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/formatting/formatter.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/formatting/formatter.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/cs/custom.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/cs/custom.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/cs/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/cs/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/da/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/da/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/de/custom.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/de/custom.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/de/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/de/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/en/custom.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/en/custom.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/en/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/en/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/en_gb/custom.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/en_gb/custom.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/en_gb/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/en_gb/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/en_us/custom.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/en_us/custom.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/en_us/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/en_us/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/es/custom.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/es/custom.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/es/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/es/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/fa/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/fa/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/fo/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/fo/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/fr/custom.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/fr/custom.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/fr/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/fr/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/he/custom.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/he/custom.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/he/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/he/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/id/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/id/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/it/custom.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/it/custom.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/it/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/it/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/ja/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/ja/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/ko/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/ko/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/lt/custom.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/lt/custom.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/lt/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/lt/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/nb/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/nb/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/nl/custom.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/nl/custom.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/nl/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/nl/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/nn/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/nn/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/pl/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/pl/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/pt_br/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/pt_br/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/ru/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/ru/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/sk/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/sk/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/sv/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/sv/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/tr/custom.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/tr/custom.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/tr/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/tr/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/locales/zh/locale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/locales/zh/locale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/mixins/default.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/mixins/default.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/parsing/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/parsing/iso8601.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/parsing/iso8601.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/testing/traveller.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/testing/traveller.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/tz/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/tz/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/tz/exceptions.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/tz/exceptions.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/tz/local_timezone.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/tz/local_timezone.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/tz/timezone.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/tz/timezone.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/tz/data/windows.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/tz/data/windows.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum/utils/_zoneinfo.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum/utils/_zoneinfo.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/license_files/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pendulum-3.0.0.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_migration.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_migration.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/alias_generators.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/alias_generators.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/aliases.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/aliases.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/annotated_handlers.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/annotated_handlers.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/color.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/color.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/config.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/config.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/dataclasses.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/dataclasses.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/errors.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/errors.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/fields.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/fields.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/functional_serializers.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/functional_serializers.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/functional_validators.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/functional_validators.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/json_schema.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/json_schema.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/main.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/main.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/mypy.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/mypy.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/networks.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/networks.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/root_model.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/root_model.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/type_adapter.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/type_adapter.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/types.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/types.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/validate_call_decorator.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/validate_call_decorator.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/version.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/version.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/warnings.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/warnings.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_config.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_config.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_core_metadata.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_core_metadata.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_core_utils.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_core_utils.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_dataclasses.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_decorators.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_decorators.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_decorators_v1.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_decorators_v1.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_discriminated_union.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_discriminated_union.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_fields.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_fields.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_forward_ref.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_forward_ref.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_generate_schema.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_generate_schema.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_generics.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_generics.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_git.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_git.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_known_annotated_metadata.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_known_annotated_metadata.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_mock_val_ser.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_mock_val_ser.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_model_construction.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_model_construction.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_repr.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_repr.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_schema_generation_shared.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_schema_generation_shared.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_signature.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_signature.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_std_types_schema.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_std_types_schema.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_typing_extra.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_typing_extra.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_utils.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_utils.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_validate_call.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_validate_call.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/_internal/_validators.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/_internal/_validators.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/deprecated/class_validators.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/deprecated/class_validators.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/deprecated/config.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/deprecated/config.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/deprecated/copy_internals.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/deprecated/copy_internals.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/deprecated/decorator.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/deprecated/decorator.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/deprecated/json.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/deprecated/json.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/deprecated/parse.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/deprecated/parse.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/deprecated/tools.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/deprecated/tools.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/plugin/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/plugin/_loader.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/plugin/_loader.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/plugin/_schema_validator.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/plugin/_schema_validator.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/_hypothesis_plugin.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/_hypothesis_plugin.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/annotated_types.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/annotated_types.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/class_validators.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/class_validators.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/color.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/color.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/config.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/config.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/dataclasses.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/dataclasses.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/datetime_parse.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/datetime_parse.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/decorator.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/decorator.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/env_settings.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/env_settings.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/error_wrappers.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/error_wrappers.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/errors.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/errors.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/fields.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/fields.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/generics.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/generics.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/json.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/json.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/main.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/main.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/mypy.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/mypy.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/networks.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/networks.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/parse.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/parse.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/schema.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/schema.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/tools.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/tools.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/types.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/types.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/typing.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/typing.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/utils.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/utils.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/validators.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/validators.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic/v1/version.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic/v1/version.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/licenses/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic-2.6.4.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core/_pydantic_core.cpython-311-darwin.so` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core/_pydantic_core.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core/_pydantic_core.pyi` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core/_pydantic_core.pyi`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core/core_schema.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core/core_schema.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/license_files/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pydantic_core-2.16.3.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/cmdline.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/console.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/console.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/filter.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatter.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexer.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/modeline.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/plugin.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/regexopt.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/scanner.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/sphinxext.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/style.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/style.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/token.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/token.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/unistring.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/util.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/util.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/filters/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/_mapping.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/bbcode.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/groff.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/html.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/img.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/irc.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/latex.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/other.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/pangomarkup.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/rtf.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/svg.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/terminal.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/formatters/terminal256.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_ada_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_ada_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_asy_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_asy_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_cl_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_cl_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_cocoa_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_cocoa_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_csound_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_csound_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_css_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_css_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_julia_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_julia_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_lasso_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_lasso_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_lilypond_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_lilypond_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_lua_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_lua_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_mapping.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_mql_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_mql_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_mysql_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_mysql_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_openedge_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_openedge_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_php_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_php_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_postgres_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_postgres_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_qlik_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_qlik_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_scheme_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_scheme_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_scilab_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_scilab_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_sourcemod_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_sourcemod_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_stan_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_stan_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_stata_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_stata_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_tsql_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_tsql_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_usd_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_usd_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_vbscript_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_vbscript_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/_vim_builtins.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/_vim_builtins.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/actionscript.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/actionscript.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ada.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ada.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/agile.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/agile.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/algebra.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/algebra.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ambient.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ambient.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/amdgpu.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/amdgpu.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ampl.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ampl.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/apdlexer.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/apdlexer.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/apl.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/apl.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/archetype.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/archetype.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/arrow.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/arrow.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/arturo.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/arturo.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/asc.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/asc.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/asm.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/asm.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/asn1.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/asn1.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/automation.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/automation.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/bare.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/bare.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/basic.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/basic.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/bdd.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/bdd.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/berry.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/berry.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/bibtex.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/bibtex.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/blueprint.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/blueprint.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/boa.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/boa.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/bqn.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/bqn.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/business.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/business.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/c_cpp.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/c_cpp.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/c_like.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/c_like.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/capnproto.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/capnproto.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/carbon.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/carbon.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/cddl.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/cddl.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/chapel.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/chapel.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/clean.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/clean.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/comal.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/comal.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/compiled.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/compiled.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/configs.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/configs.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/console.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/console.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/cplint.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/cplint.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/crystal.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/crystal.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/csound.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/csound.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/css.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/css.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/d.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/d.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/dalvik.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/dalvik.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/data.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/data.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/dax.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/dax.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/devicetree.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/devicetree.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/diff.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/diff.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/dns.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/dns.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/dotnet.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/dotnet.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/dsls.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/dsls.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/dylan.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/dylan.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ecl.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ecl.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/eiffel.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/eiffel.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/elm.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/elm.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/elpi.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/elpi.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/email.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/email.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/erlang.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/erlang.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/esoteric.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/esoteric.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ezhil.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ezhil.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/factor.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/factor.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/fantom.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/fantom.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/felix.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/felix.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/fift.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/fift.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/floscript.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/floscript.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/forth.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/forth.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/fortran.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/fortran.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/foxpro.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/foxpro.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/freefem.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/freefem.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/func.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/func.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/functional.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/functional.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/futhark.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/futhark.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/gcodelexer.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/gcodelexer.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/gdscript.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/gdscript.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/go.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/go.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/grammar_notation.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/grammar_notation.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/graph.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/graph.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/graphics.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/graphics.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/graphql.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/graphql.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/graphviz.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/graphviz.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/gsql.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/gsql.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/haskell.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/haskell.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/haxe.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/haxe.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/hdl.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/hdl.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/hexdump.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/hexdump.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/html.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/html.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/idl.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/idl.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/igor.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/igor.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/inferno.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/inferno.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/installers.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/installers.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/int_fiction.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/int_fiction.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/iolang.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/iolang.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/j.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/j.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/javascript.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/javascript.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/jmespath.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/jmespath.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/jslt.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/jslt.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/jsonnet.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/jsonnet.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/jsx.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/jsx.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/julia.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/julia.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/jvm.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/jvm.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/kuin.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/kuin.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/kusto.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/kusto.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ldap.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ldap.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/lean.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/lean.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/lilypond.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/lilypond.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/lisp.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/lisp.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/macaulay2.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/macaulay2.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/make.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/make.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/markup.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/markup.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/math.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/math.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/matlab.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/matlab.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/maxima.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/maxima.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/meson.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/meson.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/mime.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/mime.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/minecraft.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/minecraft.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/mips.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/mips.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ml.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ml.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/modeling.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/modeling.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/modula2.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/modula2.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/monte.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/monte.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/mosel.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/mosel.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ncl.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ncl.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/nimrod.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/nimrod.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/nit.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/nit.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/nix.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/nix.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/oberon.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/oberon.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/objective.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/objective.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ooc.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ooc.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/openscad.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/openscad.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/other.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/other.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/parasail.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/parasail.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/parsers.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/parsers.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/pascal.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/pascal.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/pawn.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/pawn.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/perl.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/perl.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/phix.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/phix.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/php.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/php.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/pointless.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/pointless.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/pony.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/pony.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/praat.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/praat.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/procfile.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/procfile.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/prolog.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/prolog.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/promql.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/promql.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/prql.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/prql.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ptx.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ptx.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/python.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/q.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/q.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/qlik.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/qlik.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/qvt.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/qvt.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/r.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/r.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/rdf.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/rdf.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/rebol.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/rebol.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/resource.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/resource.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ride.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ride.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/rita.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/rita.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/rnc.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/rnc.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/roboconf.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/roboconf.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/robotframework.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/robotframework.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ruby.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ruby.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/rust.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/rust.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/sas.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/sas.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/savi.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/savi.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/scdoc.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/scdoc.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/scripting.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/scripting.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/sgf.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/sgf.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/shell.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/shell.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/sieve.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/sieve.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/slash.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/slash.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/smalltalk.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/smalltalk.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/smithy.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/smithy.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/smv.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/smv.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/snobol.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/snobol.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/solidity.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/solidity.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/sophia.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/sophia.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/special.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/special.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/spice.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/spice.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/sql.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/sql.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/srcinfo.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/srcinfo.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/stata.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/stata.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/supercollider.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/supercollider.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/tal.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/tal.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/tcl.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/tcl.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/teal.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/teal.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/templates.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/templates.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/teraterm.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/teraterm.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/testing.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/testing.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/text.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/text.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/textedit.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/textedit.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/textfmts.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/textfmts.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/theorem.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/theorem.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/thingsdb.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/thingsdb.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/tlb.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/tlb.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/tls.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/tls.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/tnt.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/tnt.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/trafficscript.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/trafficscript.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/typoscript.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/typoscript.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/ul4.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/ul4.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/unicon.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/unicon.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/urbi.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/urbi.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/usd.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/usd.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/varnish.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/varnish.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/verification.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/verification.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/verifpal.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/verifpal.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/vip.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/vip.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/vyper.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/vyper.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/web.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/web.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/webassembly.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/webassembly.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/webidl.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/webidl.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/webmisc.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/webmisc.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/wgsl.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/wgsl.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/whiley.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/whiley.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/wowtoc.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/wowtoc.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/wren.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/wren.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/x10.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/x10.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/xorg.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/xorg.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/yang.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/yang.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/yara.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/yara.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/lexers/zig.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/lexers/zig.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/_mapping.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/_mapping.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/abap.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/abap.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/algol.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/algol.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/algol_nu.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/algol_nu.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/arduino.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/arduino.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/autumn.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/autumn.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/borland.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/borland.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/bw.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/bw.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/colorful.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/colorful.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/default.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/default.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/dracula.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/dracula.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/emacs.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/emacs.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/friendly.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/friendly.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/friendly_grayscale.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/friendly_grayscale.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/fruity.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/fruity.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/gh_dark.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/gh_dark.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/gruvbox.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/gruvbox.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/igor.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/igor.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/inkpot.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/inkpot.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/lightbulb.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/lightbulb.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/lilypond.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/lilypond.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/lovelace.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/lovelace.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/manni.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/manni.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/material.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/material.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/monokai.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/monokai.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/murphy.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/murphy.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/native.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/native.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/nord.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/nord.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/onedark.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/onedark.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/paraiso_dark.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/paraiso_dark.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/paraiso_light.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/paraiso_light.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/pastie.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/pastie.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/perldoc.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/perldoc.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/rainbow_dash.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/rainbow_dash.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/rrt.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/rrt.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/sas.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/sas.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/solarized.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/solarized.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/staroffice.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/staroffice.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/stata_dark.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/stata_dark.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/stata_light.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/stata_light.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/tango.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/tango.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/trac.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/trac.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/vim.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/vim.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/vs.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/vs.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/xcode.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/xcode.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments/styles/zenburn.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments/styles/zenburn.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/AUTHORS` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/AUTHORS`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/python_dateutil-2.9.0.post0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse/timeparse.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse/timeparse.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse/tests/testtimeparse.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse/tests/testtimeparse.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/DESCRIPTION.rst` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/pytimeparse-1.1.8.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/__main__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_cell_widths.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_emoji_codes.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_emoji_replace.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_export_format.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_fileno.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_inspect.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_log_render.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_loop.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_null_file.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_palettes.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_ratio.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_spinners.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_win32_console.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_windows.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_windows_renderer.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/_wrap.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/abc.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/abc.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/align.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/align.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/ansi.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/bar.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/bar.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/box.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/box.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/cells.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/cells.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/color.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/color.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/color_triplet.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/columns.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/columns.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/console.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/console.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/constrain.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/containers.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/containers.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/control.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/control.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/default_styles.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/diagnose.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/emoji.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/errors.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/errors.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/file_proxy.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/filesize.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/highlighter.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/json.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/json.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/jupyter.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/layout.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/layout.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/live.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/live.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/live_render.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/logging.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/logging.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/markdown.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/markdown.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/markup.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/markup.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/measure.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/measure.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/padding.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/padding.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/pager.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/pager.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/palette.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/palette.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/panel.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/panel.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/pretty.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/progress.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/progress.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/progress_bar.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/prompt.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/protocol.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/repr.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/repr.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/rule.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/rule.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/scope.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/scope.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/screen.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/screen.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/segment.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/segment.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/spinner.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/status.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/status.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/style.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/style.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/styled.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/styled.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/syntax.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/table.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/table.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/terminal_theme.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/text.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/text.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/theme.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/theme.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/traceback.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich/tree.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich/tree.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/rich-13.7.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham/nt.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham/nt.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham/posix/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham/posix/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham/posix/proc.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham/posix/proc.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham/posix/ps.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham/posix/ps.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/shellingham-1.5.4.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/six-1.16.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/time_machine/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/time_machine/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/time_machine-2.14.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/__init__.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/__init__.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/_completion_click7.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/_completion_click7.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/_completion_click8.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/_completion_click8.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/_completion_shared.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/_completion_shared.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/_typing.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/_typing.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/completion.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/completion.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/core.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/core.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/main.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/main.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/models.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/models.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/params.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/params.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/rich_utils.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/rich_utils.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/testing.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/testing.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer/utils.py` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer/utils.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typer-0.9.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zones` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zones`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/CET` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/CET`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/CST6CDT` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/CST6CDT`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Cuba` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Cuba`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/EST5EDT` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/EST5EDT`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Egypt` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Egypt`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Eire` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Eire`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GB` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GB`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GB-Eire` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/GB-Eire`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Hongkong` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Hongkong`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Iran` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Iran`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Israel` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Israel`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/MET` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/MET`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/MST7MDT` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/MST7MDT`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/NZ` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/NZ`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/NZ-CHAT` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/NZ-CHAT`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Navajo` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Navajo`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/PST8PDT` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/PST8PDT`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Poland` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Poland`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Portugal` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Portugal`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Turkey` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Turkey`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/W-SU` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/W-SU`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/iso3166.tab` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/iso3166.tab`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/leapseconds` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/leapseconds`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/tzdata.zi` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/tzdata.zi`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/zone.tab` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/zone.tab`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/zone1970.tab` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/zone1970.tab`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/zonenow.tab` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/zonenow.tab`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Cairo` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Cairo`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Casablanca` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Casablanca`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Ceuta` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Ceuta`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/El_Aaiun` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/El_Aaiun`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Windhoek` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Africa/Windhoek`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Adak` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Adak`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Anchorage` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Anchorage`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Araguaina` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Araguaina`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Asuncion` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Asuncion`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Atka` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Atka`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Bahia` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Bahia`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Bahia_Banderas` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Bahia_Banderas`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Belize` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Belize`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Boise` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Boise`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Buenos_Aires` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Buenos_Aires`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cambridge_Bay` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cambridge_Bay`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Campo_Grande` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Campo_Grande`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cancun` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cancun`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Catamarca` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Catamarca`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Chicago` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Chicago`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Chihuahua` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Chihuahua`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Ciudad_Juarez` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Ciudad_Juarez`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cordoba` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cordoba`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cuiaba` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Cuiaba`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Dawson` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Dawson`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Dawson_Creek` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Dawson_Creek`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Denver` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Denver`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Detroit` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Detroit`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Edmonton` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Edmonton`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Ensenada` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Ensenada`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Fort_Nelson` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Fort_Nelson`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Fort_Wayne` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Fort_Wayne`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Glace_Bay` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Glace_Bay`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Godthab` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Godthab`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Goose_Bay` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Goose_Bay`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Grand_Turk` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Grand_Turk`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Halifax` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Halifax`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Havana` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Havana`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indianapolis` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indianapolis`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Inuvik` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Inuvik`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Iqaluit` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Iqaluit`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Jujuy` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Jujuy`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Juneau` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Juneau`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Knox_IN` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Knox_IN`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Los_Angeles` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Los_Angeles`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Louisville` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Louisville`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Mazatlan` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Mazatlan`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Mendoza` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Mendoza`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Menominee` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Menominee`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Merida` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Merida`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Metlakatla` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Metlakatla`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Mexico_City` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Mexico_City`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Miquelon` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Miquelon`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Moncton` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Moncton`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Monterrey` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Monterrey`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Montevideo` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Montevideo`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Montreal` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Montreal`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nassau` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nassau`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/New_York` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/New_York`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nipigon` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nipigon`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nome` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nome`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nuuk` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Nuuk`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Ojinaga` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Ojinaga`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Pangnirtung` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Pangnirtung`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Port-au-Prince` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Port-au-Prince`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Punta_Arenas` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Punta_Arenas`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Rainy_River` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Rainy_River`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Rankin_Inlet` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Rankin_Inlet`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Regina` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Regina`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Resolute` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Resolute`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Rosario` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Rosario`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Santa_Isabel` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Santa_Isabel`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Santiago` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Santiago`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Sao_Paulo` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Sao_Paulo`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Scoresbysund` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Scoresbysund`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Shiprock` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Shiprock`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Sitka` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Sitka`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/St_Johns` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/St_Johns`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Thunder_Bay` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Thunder_Bay`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Tijuana` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Tijuana`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Toronto` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Toronto`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Vancouver` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Vancouver`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Whitehorse` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Whitehorse`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Winnipeg` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Winnipeg`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Yakutat` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Yakutat`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Yellowknife` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Yellowknife`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Buenos_Aires` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Buenos_Aires`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Catamarca` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Catamarca`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/ComodRivadavia` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/ComodRivadavia`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Cordoba` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Cordoba`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Jujuy` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Jujuy`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/La_Rioja` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/La_Rioja`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Mendoza` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Mendoza`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Rio_Gallegos` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Rio_Gallegos`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Salta` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Salta`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/San_Juan` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/San_Juan`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/San_Luis` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/San_Luis`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Tucuman` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Tucuman`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Ushuaia` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Argentina/Ushuaia`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Indianapolis` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Indianapolis`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Knox` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Knox`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Marengo` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Marengo`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Petersburg` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Petersburg`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Tell_City` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Tell_City`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Vincennes` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Vincennes`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Winamac` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Indiana/Winamac`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Kentucky/Louisville` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Kentucky/Louisville`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Kentucky/Monticello` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/Kentucky/Monticello`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/North_Dakota/Beulah` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/North_Dakota/Beulah`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/North_Dakota/Center` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/North_Dakota/Center`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/North_Dakota/New_Salem` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/America/North_Dakota/New_Salem`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Macquarie` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Macquarie`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/McMurdo` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/McMurdo`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Palmer` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/Palmer`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/South_Pole` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Antarctica/South_Pole`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Arctic/Longyearbyen` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Arctic/Longyearbyen`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Almaty` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Almaty`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Amman` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Amman`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Anadyr` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Anadyr`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Aqtau` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Aqtau`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Aqtobe` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Aqtobe`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Atyrau` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Atyrau`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Baghdad` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Baghdad`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Baku` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Baku`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Barnaul` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Barnaul`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Beirut` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Beirut`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Bishkek` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Bishkek`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Chita` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Chita`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Choibalsan` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Choibalsan`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Damascus` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Damascus`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Famagusta` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Famagusta`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Gaza` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Gaza`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Hebron` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Hebron`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Hong_Kong` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Hong_Kong`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Hovd` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Hovd`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Irkutsk` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Irkutsk`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Istanbul` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Istanbul`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Jerusalem` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Jerusalem`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kamchatka` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Kamchatka`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Khandyga` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Khandyga`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Krasnoyarsk` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Krasnoyarsk`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Macao` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Macao`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Macau` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Macau`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Magadan` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Magadan`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Nicosia` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Nicosia`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Novokuznetsk` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Novokuznetsk`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Novosibirsk` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Novosibirsk`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Omsk` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Omsk`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Oral` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Oral`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Qostanay` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Qostanay`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Qyzylorda` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Qyzylorda`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Sakhalin` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Sakhalin`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Srednekolymsk` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Srednekolymsk`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tbilisi` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tbilisi`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tehran` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tehran`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tel_Aviv` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tel_Aviv`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tomsk` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Tomsk`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ulaanbaatar` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ulaanbaatar`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ulan_Bator` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ulan_Bator`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ust-Nera` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Ust-Nera`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Vladivostok` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Vladivostok`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Yakutsk` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Yakutsk`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Yekaterinburg` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Yekaterinburg`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Yerevan` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Asia/Yerevan`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Azores` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Azores`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Bermuda` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Bermuda`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Jan_Mayen` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Jan_Mayen`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Madeira` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Madeira`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Stanley` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Atlantic/Stanley`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/ACT` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/ACT`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Adelaide` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Adelaide`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Broken_Hill` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Broken_Hill`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Canberra` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Canberra`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Currie` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Currie`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Hobart` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Hobart`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/LHI` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/LHI`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Lord_Howe` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Lord_Howe`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Melbourne` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Melbourne`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/NSW` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/NSW`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/South` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/South`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Sydney` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Sydney`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Tasmania` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Tasmania`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Victoria` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Victoria`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Yancowinna` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Australia/Yancowinna`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Brazil/East` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Brazil/East`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Atlantic` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Atlantic`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Central` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Central`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Eastern` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Eastern`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Mountain` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Mountain`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Newfoundland` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Newfoundland`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Pacific` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Pacific`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Saskatchewan` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Saskatchewan`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Yukon` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Canada/Yukon`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Chile/Continental` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Chile/Continental`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Chile/EasterIsland` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Chile/EasterIsland`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Amsterdam` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Amsterdam`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Astrakhan` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Astrakhan`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Athens` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Athens`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Belfast` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Belfast`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Berlin` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Berlin`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Bratislava` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Bratislava`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Brussels` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Brussels`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Bucharest` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Bucharest`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Budapest` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Budapest`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Chisinau` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Chisinau`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Copenhagen` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Copenhagen`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Dublin` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Dublin`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Gibraltar` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Gibraltar`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Guernsey` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Guernsey`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Isle_of_Man` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Isle_of_Man`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Istanbul` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Istanbul`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Jersey` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Jersey`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kaliningrad` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kaliningrad`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kiev` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kiev`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kirov` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kirov`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kyiv` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Kyiv`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Lisbon` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Lisbon`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/London` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/London`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Luxembourg` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Luxembourg`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Madrid` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Madrid`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Malta` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Malta`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Minsk` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Minsk`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Monaco` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Monaco`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Moscow` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Moscow`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Nicosia` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Nicosia`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Oslo` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Oslo`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Paris` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Paris`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Prague` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Prague`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Riga` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Riga`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Rome` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Rome`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Samara` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Samara`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/San_Marino` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/San_Marino`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Saratov` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Saratov`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Simferopol` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Simferopol`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Sofia` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Sofia`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Stockholm` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Stockholm`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Tallinn` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Tallinn`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Tirane` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Tirane`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Tiraspol` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Tiraspol`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Ulyanovsk` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Ulyanovsk`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Uzhgorod` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Uzhgorod`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Vatican` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Vatican`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Vienna` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Vienna`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Vilnius` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Vilnius`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Volgograd` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Volgograd`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Warsaw` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Warsaw`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Zaporozhye` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Europe/Zaporozhye`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Mexico/BajaNorte` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Mexico/BajaNorte`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Mexico/BajaSur` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Mexico/BajaSur`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Mexico/General` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Mexico/General`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Auckland` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Auckland`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Chatham` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Chatham`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Easter` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/Pacific/Easter`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Alaska` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Alaska`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Aleutian` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Aleutian`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Central` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Central`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/East-Indiana` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/East-Indiana`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Eastern` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Eastern`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Indiana-Starke` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Indiana-Starke`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Michigan` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Michigan`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Mountain` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Mountain`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Pacific` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata/zoneinfo/US/Pacific`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/LICENSE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/LICENSE_APACHE` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/LICENSE_APACHE`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/METADATA` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/RECORD` & `daikanban-0.1.2/.venv/lib/python3.11/site-packages/tzdata-2024.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/daikanban/interface.py` & `daikanban-0.1.2/daikanban/interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 from collections import defaultdict
-import csv
-from datetime import datetime
+from dataclasses import dataclass
+from datetime import datetime, timedelta
 from functools import cache, wraps
 import json
 from operator import attrgetter
 from pathlib import Path
 import readline  # improves shell interactivity  # noqa: F401
 import shlex
 import sys
-from typing import Any, Callable, Iterable, Optional, TypeVar, cast
+from typing import Any, Callable, Generic, Iterable, Optional, TypeVar, cast
 
 import pendulum
 import pendulum.parsing
 from pydantic import BaseModel, Field, ValidationError, create_model
 from rich import print
+from rich.console import Console
 from rich.markup import escape
 from rich.prompt import Confirm
 from rich.table import Table
+from typing_extensions import Concatenate, ParamSpec
 
-from daikanban.model import Board, Id, KanbanError, Model, Project, Task, TaskStatus, TaskStatusAction
+from daikanban.model import Board, Id, KanbanError, Model, Project, Task, TaskStatus, TaskStatusAction, TaskStatusError
 from daikanban.prompt import FieldPrompter, Prompter, model_from_prompt, simple_input
 from daikanban.settings import Settings
-from daikanban.utils import StrEnum, UserInputError, err_style, fuzzy_match, get_current_time, handle_error, prefix_match, style_str, to_snake_case
+from daikanban.utils import NotGiven, NotGivenType, StrEnum, UserInputError, err_style, fuzzy_match, get_current_time, get_duration_between, handle_error, human_readable_duration, parse_string_set, prefix_match, style_str, to_snake_case
 
 
 M = TypeVar('M', bound=BaseModel)
 T = TypeVar('T')
+BI = TypeVar('BI', bound='BoardInterface')
+P = ParamSpec('P')
 
 PKG_DIR = Path(__file__).parent
 BILLBOARD_ART_PATH = PKG_DIR / 'billboard_art.txt'
 
 
 ##########
 # ERRORS #
@@ -68,16 +72,19 @@
         raise err
     return tup  # type: ignore[return-value]
 
 def split_comma_list(s: str) -> list[str]:
     """Given a comma-separated list, splits it into a list of strings."""
     return [token for token in s.split(',') if token]
 
-def parse_task_limit(s: str) -> int:
-    """Parses an integer task limit, raising a UserInputError if invalid."""
+def parse_task_limit(s: str) -> Optional[int]:
+    """Parses an integer task limit, raising a UserInputError if invalid.
+    If the input string is 'none', returns None."""
+    if s.strip().lower() == 'none':
+        return None
     try:
         return int(s)
     except ValueError:
         raise UserInputError('Must select a positive whole number for task limit') from None
 
 
 ##########
@@ -119,20 +126,14 @@
 # PARSING #
 ###########
 
 def empty_is_none(s: str) -> Optional[str]:
     """Identity function on strings, except if the string is empty, returns None."""
     return s or None
 
-def parse_string_set(s: str) -> Optional[set[str]]:
-    """Parses a comma-separated string into a set of strings.
-    Allows for quote delimiting so that commas can be escaped."""
-    strings = set(list(csv.reader([s]))[0])
-    return strings or None
-
 def parse_date_as_string(s: str) -> Optional[str]:
     """Parses a string into a timestamp string.
     The input string can either specify a datetime directly, or a time duration from the present moment."""
     if not s.strip():
         return None
     settings = Settings.global_settings().time
     return settings.render_datetime(settings.parse_datetime(s))
@@ -188,40 +189,59 @@
 
 def simple_task_row_type(*fields: str) -> type[BaseModel]:
     """Given a list of fields associated with a task, creates a BaseModel subclass that will be used to display a simplified row for each task.
     These rows are presented in the DaiKanban board view."""
     kwargs: dict[str, Any] = {}
     for field in fields:
         if field == 'id':
-            val: tuple[type, Any] = (str, Field(json_schema_extra={'justify': 'right'}))  # type: ignore[call-arg]
+            val: tuple[Any, Any] = (str, Field(json_schema_extra={'justify': 'right'}))
         elif field == 'name':
             val = (str, ...)
         elif field == 'project':
-            val = (Optional[str], ...)  # type: ignore[assignment]
+            val = (Optional[str], ...)
         elif field == 'priority':
-            val = (Optional[float], Field(title="pri…ty"))  # type: ignore[assignment]
+            val = (Optional[float], Field(title="pri…ty"))
         elif field == 'difficulty':
-            val = (Optional[float], Field(title="diff…ty"))  # type: ignore[assignment]
+            val = (Optional[float], Field(title="diff…ty"))
+        elif field == 'completed_time':
+            val = (Optional[datetime], Field(title='completed'))
         elif field == 'score':
-            val = (float, Field(json_schema_extra={'justify': 'right'}))  # type: ignore[call-arg]
+            val = (float, Field(json_schema_extra={'justify': 'right'}))
         # TODO: add more fields
         else:
             raise ValueError(f'Unrecognized Task field {field}')
         kwargs[field] = val
     return create_model('SimpleTaskRow', **kwargs)
 
 
+@dataclass
+class TaskGroupSettings(Generic[M]):
+    """Class responsible for simplifying task info for displaying it in a DaiKanban board subtable."""
+    task_row_type: type[M]  # type of task row to display
+    sort_key: str  # attribute by which to sort the tasks
+    get_task_info: Callable[[Id, Task], dict[str, Any]]  # given ID and task, returns data for task row
+    get_group_header: Callable[[int], str]  # given task count, returns column header for the group
+
+    def get_task_row(self, id_: Id, task: Task) -> M:
+        """Given a task ID and Task, returns a simplified task row object."""
+        return self.task_row_type(**self.get_task_info(id_, task))
+
+    def sort_task_rows(self, task_rows: list[M]) -> None:
+        """Sorts, in-place, a list of task rows."""
+        task_rows.sort(key=attrgetter(self.sort_key), reverse=True)
+
+
 ###################
 # BOARD INTERFACE #
 ###################
 
-def require_board(func):  # noqa
+def require_board(func: Callable[Concatenate[BI, P], None]) -> Callable[Concatenate[BI, P], None]:
     """Decorator for a method which makes it raise a BoardNotLoadedError if a board path is not set."""
     @wraps(func)
-    def wrapped(self, *args, **kwargs):  # noqa
+    def wrapped(self: BI, *args: P.args, **kwargs: P.kwargs) -> None:
         if self.board is None:
             raise BoardNotLoadedError("No board has been loaded.\nRun 'board load' to load a board.")
         func(self, *args, **kwargs)
     return wrapped
 
 
 class BoardInterface(BaseModel):
@@ -312,20 +332,26 @@
         grid.add_column(style='bold')
         grid.add_column(style='bold')
         grid.add_column()
         return grid
 
     def add_board_help(self, grid: Table) -> None:
         """Adds entries to help menu related to boards."""
+        statuses = ', '.join(TaskStatus)
         grid.add_row('\[b]oard', '\[d]elete', 'delete current board')
         grid.add_row('', '\[n]ew', 'create new board')
         grid.add_row('', '\[l]oad [not bold]\[FILENAME][/]', 'load board from file')
         grid.add_row('', 'schema', 'show board JSON schema')
         grid.add_row('', '\[s]how', 'show current board, can provide extra filters like:')
-        grid.add_row('', '', '  status=\[STATUSES] project=\[PROJECT_IDS] tag=\[TAGS] limit=\[SIZE]')
+        # grid.add_row('', '', '  status=\[STATUSES] project=\[PROJECT_IDS] tag=\[TAGS] limit=\[SIZE] since=\[WHEN]')
+        grid.add_row('', '', f'  status=\[STATUSES]  | list of statuses ({statuses})')
+        grid.add_row('', '', '  project=\[PROJECTS] | list of project names or IDs')
+        grid.add_row('', '', '  tag=\[TAGS]         | list of tags')
+        grid.add_row('', '', '  limit=\[SIZE]       | max number of tasks to show per column (a number, or "none" for no limit)')
+        grid.add_row('', '', '  since=\[WHEN]       | date/time expression (or "anytime" for no time limit), used to limit completed tasks only')
 
     def add_project_help(self, grid: Table) -> None:
         """Adds entries to help menu related to projects."""
         id_str = '[not bold]\[ID/NAME][/]'
         grid.add_row('\[p]roject', f'\[d]elete {id_str}', 'delete a project')
         grid.add_row('', '\[n]ew', 'create new project')
         grid.add_row('', '\[s]how', 'show project list')
@@ -381,15 +407,15 @@
 
     @staticmethod
     def show_schema(cls: type[BaseModel], indent: int = 2) -> None:
         """Prints out the JSON schema of the given type."""
         print(json.dumps(cls.model_json_schema(mode='serialization'), indent=indent))
 
     @require_board
-    def _update_project_or_task(self, id_or_name: str, field: str, value: str, is_task: bool) -> None:
+    def _update_project_or_task(self, id_or_name: str, field: str, value: Optional[str], is_task: bool) -> None:
         """Updates an attribute of a project or task."""
         assert self.board is not None
         cls = Task if is_task else Project
         if field in cls.model_computed_fields:  # type: ignore[attr-defined]
             raise UserInputError(f'Field {field!r} cannot be updated')
         name = cls.__name__.lower()
         id_ = getattr(self, f'_parse_{name}')(id_or_name)
@@ -419,15 +445,15 @@
         assert id_ is not None
         proj = self.board.get_project(id_)
         self.board.delete_project(id_)
         self.save_board()
         print(f'Deleted project {name_style(proj.name)} with ID {proj_id_style(id_)}')
 
     @require_board
-    def new_project(self) -> None:
+    def new_project(self, name: Optional[str] = None) -> None:
         """Creates a new project."""
         assert self.board is not None
         def _parse_name(name: Any) -> str:
             if isinstance(name, str):
                 # catch duplicate project name early
                 self.board._check_duplicate_project_name(name)  # type: ignore[union-attr]
             return name
@@ -441,16 +467,22 @@
             },
             'links': {
                 'prompt': 'Links [not bold]\[optional, comma-separated][/]',
                 'parse': parse_string_set
             }
         }
         prompters: dict[str, FieldPrompter] = {field: FieldPrompter(Project, field, **kwargs) for (field, kwargs) in params.items()}
+        if name is None:
+            defaults = {}
+        else:
+            self.board._check_duplicate_project_name(name)
+            del prompters['name']
+            defaults = {'name': name}
         try:
-            proj = model_from_prompt(Project, prompters)
+            proj = model_from_prompt(Project, prompters, defaults=defaults)
         except KeyboardInterrupt:  # go back to main REPL
             print()
             return
         id_ = self.board.create_project(proj)
         self.save_board()
         print(f'Created new project {name_style(proj.name)} with ID {proj_id_style(id_)}')
 
@@ -471,65 +503,83 @@
         """Shows project info."""
         assert self.board is not None
         id_ = self._parse_project(id_or_name)
         assert id_ is not None
         proj = self.board.get_project(id_)
         print(self._model_pretty(proj, id_=id_))
 
-    def update_project(self, id_or_name: str, field: str, value: str) -> None:
+    def update_project(self, id_or_name: str, field: str, value: Optional[str] = None) -> None:
         """Updates an attribute of a project."""
         return self._update_project_or_task(id_or_name, field, value, is_task=False)
 
     # TASK
 
     @require_board
     def change_task_status(self, action: TaskStatusAction, id_or_name: Optional[str] = None) -> None:
         """Changes a task to a new stage."""
         assert self.board is not None
+        board: Board = self.board
         id_ = self._prompt_and_parse_task(id_or_name)
-        task = self.board.get_task(id_)
+        task = board.get_task(id_)
         # fail early if the action is invalid for the status
         _ = task.apply_status_action(action)
-        _parse_datetime = Settings.global_settings().time.parse_datetime
+        def parse_datetime(s: str) -> datetime:
+            task = board.get_task(id_)
+            settings = Settings.global_settings()
+            dt = settings.time.parse_datetime(s)
+            if dt < task.created_time:
+                created_str = settings.time.render_datetime(task.created_time)
+                dt_str = settings.time.render_datetime(dt)
+                Console().print(f'Time is earlier than task creation time ({created_str}).', highlight=False)
+                overwrite = Confirm.ask(f'Set creation time to {dt_str}?')
+                if overwrite:
+                    board.update_task(id_, created_time=dt)
+                else:
+                    raise TaskStatusError(f'cannot start a task before its creation time ({created_str})')
+            return dt
         # if valid, prompt the user for when the action took place
         # ask for time of intermediate status change, which occurs if:
         #   todo -> active -> complete
         #   todo -> active -> paused
         #   paused -> active -> complete
         intermediate_action_map = {
             (TaskStatus.todo, TaskStatusAction.complete): TaskStatusAction.start,
             (TaskStatus.todo, TaskStatusAction.pause): TaskStatusAction.start,
             (TaskStatus.paused, TaskStatusAction.complete): TaskStatusAction.resume
         }
         if (intermediate := intermediate_action_map.get((task.status, action))):
             prompt = f'When was the task {intermediate.past_tense()}? [not bold]\[now][/] '
-            prompter = Prompter(prompt, _parse_datetime, validate=None, default=get_current_time)
+            prompter = Prompter(prompt, parse_datetime, validate=None, default=get_current_time)
             first_dt = prompter.loop_prompt(use_prompt_suffix=False, show_default=False)
         else:
             first_dt = None
         # prompt user for time of latest status change
         prompt = f'When was the task {action.past_tense()}? [not bold]\[now][/] '
-        prompter = Prompter(prompt, _parse_datetime, validate=None, default=get_current_time)
-        dt = prompter.loop_prompt(use_prompt_suffix=False, show_default=False)
-        task = self.board.apply_status_action(id_, action, dt=dt, first_dt=first_dt)
+        prompter = Prompter(prompt, parse_datetime, validate=None, default=get_current_time)
+        try:
+            dt = prompter.loop_prompt(use_prompt_suffix=False, show_default=False)
+        except KeyboardInterrupt:  # go back to main REPL
+            print()
+            return
+        task = board.apply_status_action(id_, action, dt=dt, first_dt=first_dt)
         self.save_board()
         print(f'Changed task {name_style(task.name)} [not bold]\[{task_id_style(id_)}][/] to {status_style(task.status)} state')
 
     @require_board
     def delete_task(self, id_or_name: Optional[str] = None) -> None:
         """Deletes a task with the given ID or name."""
         assert self.board is not None
         id_ = self._prompt_and_parse_task(id_or_name)
         task = self.board.get_task(id_)
         self.board.delete_task(id_)
         self.save_board()
         print(f'Deleted task {name_style(task.name)} with ID {task_id_style(id_)}')
 
     @require_board
-    def new_task(self) -> None:
+    def new_task(self, name: Optional[str] = None) -> None:
         """Creates a new task."""
         assert self.board is not None
         def _parse_name(name: Any) -> str:
             if isinstance(name, str):
                 # catch duplicate task name early
                 self.board._check_duplicate_task_name(name)  # type: ignore[union-attr]
             return name
@@ -568,17 +618,23 @@
             'links': {
                 'prompt': 'Links [not bold]\[optional, comma-separated][/]',
                 'parse': parse_string_set
             }
         }
         # only prompt for the fields specified in the settings
         task_fields = set(self.settings.task.new_task_fields)
+        if name is None:
+            defaults = {}
+        else:
+            self.board._check_duplicate_task_name(name)
+            task_fields.discard('name')
+            defaults = {'name': name}
         prompters: dict[str, FieldPrompter] = {field: FieldPrompter(Task, field, **kwargs) for (field, kwargs) in params.items() if field in task_fields}
         try:
-            task = model_from_prompt(Task, prompters)
+            task = model_from_prompt(Task, prompters, defaults=defaults)
         except KeyboardInterrupt:  # go back to main REPL
             print()
             return
         id_ = self.board.create_task(task)
         self.save_board()
         print(f'Created new task {name_style(task.name)} with ID {task_id_style(id_)}')
 
@@ -626,17 +682,19 @@
         assert self.board is not None
         id_ = self._parse_task(id_or_name)
         if id_ is None:
             raise UserInputError('Invalid task')
         task = self.board.get_task(id_)
         print(self._model_pretty(task, id_=id_))
 
-    def update_task(self, id_or_name: str, field: str, value: str) -> None:
+    def update_task(self, id_or_name: str, field: str, value: Optional[str] = None) -> None:
         """Updates an attribute of a task."""
         if field == 'project':  # allow a name or ID
+            if value is None:
+                raise UserInputError('Must provide a valid project name or ID')
             id_ = self._parse_project(value)
             if id_ is None:
                 raise UserInputError('Invalid project')
             return self.update_task(id_or_name, 'project_id', str(id_))
         return self._update_project_or_task(id_or_name, field, value, is_task=True)
 
     @require_board
@@ -742,60 +800,118 @@
             # show task if any tag matches one in the list
             filters.append(lambda task: task.tags and task.tags.intersection(tag_set))
         if filters:
             return lambda task: any(flt(task) for flt in filters)
         # no filters, so permit any task
         return lambda _: True
 
+    def _get_task_limit(self, limit: int | None | NotGivenType) -> Optional[int]:
+        if limit is NotGiven:
+            limit = self.settings.display.max_tasks
+        if (limit is not None) and (limit <= 0):
+            raise UserInputError('Must select a positive number for task limit')
+        return limit
+
+    def _get_completed_since(self, since: datetime | None | NotGivenType) -> Optional[datetime]:
+        now = get_current_time()
+        if since is NotGiven:
+            if isinstance(self.settings.display.completed_age_off, timedelta):
+                since = now - self.settings.display.completed_age_off
+            else:
+                return None
+        if since and (since > now):
+            raise UserInputError('Must provide a time in the past')
+        return since
+
+    def _get_task_group_settings(self, group: str, color: str, since: Optional[datetime]) -> TaskGroupSettings:
+        # TODO: customize based on settings
+        def _get_task_kwargs(id_: Id, task: Task) -> dict[str, Any]:
+            proj_str = None if (task.project_id is None) else self._project_str_from_id(task.project_id)
+            icons = task.status_icons
+            name = task.name + (f' {icons}' if icons else '')
+            return {'id': task_id_style(id_, bold=True), 'name': name, 'project': proj_str}
+        def _get_group_header(task_count: int) -> str:
+            return style_str(group, color, bold=True) + style_str(f' ({task_count})', 'bright_black')
+        if group == 'complete':
+            fields = ('id', 'name', 'project', 'completed_time')
+            sort_key = 'completed_time'
+            def get_task_info(id_: Id, task: Task) -> dict[str, Any]:
+                return {'completed_time': task.completed_time, **_get_task_kwargs(id_, task)}
+            def get_group_header(task_count: int) -> str:
+                header = _get_group_header(task_count)
+                if since:
+                    dur = get_duration_between(since, get_current_time())
+                    since_str = human_readable_duration(dur, prefer_days=True)
+                    header += style_str(f'\nlast {since_str}', 'bright_black', italic=True)
+                return header
+        else:
+            fields = ('id', 'name', 'project', 'score')
+            sort_key = 'score'
+            def get_task_info(id_: Id, task: Task) -> dict[str, Any]:
+                return {'score': self.settings.task.scorer(task), **_get_task_kwargs(id_, task)}
+            def get_group_header(task_count: int) -> str:
+                header = _get_group_header(task_count)
+                return (header + '\n') if since else header
+        # create BaseModel corresponding to a table row summarizing each Task
+        task_row_type = simple_task_row_type(*fields)
+        return TaskGroupSettings(task_row_type, sort_key, get_task_info, get_group_header)
+
     def show_board(self,  # noqa: C901
         statuses: Optional[list[str]] = None,
         projects: Optional[list[str]] = None,
         tags: Optional[list[str]] = None,
-        limit: Optional[int] = None
+        limit: int | None | NotGivenType = NotGiven,
+        since: datetime | None | NotGivenType = NotGiven,
     ) -> None:
         """Displays the board to the screen using the current configurations."""
         if self.board is None:
             raise BoardNotLoadedError("No board has been loaded.\nRun 'board new' to create a new board or 'board load' to load an existing one.")
         task_filter = self._filter_task_by_project_or_tag(projects=projects, tags=tags)
-        if limit is None:
-            limit = self.settings.display.limit
-        if (limit is not None) and (limit <= 0):
-            raise UserInputError('Must select a positive number for task limit')
+        limit = self._get_task_limit(limit)
+        since = self._get_completed_since(since)
         (group_by_status, group_colors) = self._status_group_info(statuses)
-        # create BaseModel corresponding to a table row summarizing a Task
-        # TODO: this class may be customized based on settings
-        TaskInfo = simple_task_row_type('id', 'name', 'project', 'score')
+        group_settings_by_group = {group: self._get_task_group_settings(group, group_colors[group], since) for group in group_by_status.values()}
         scorer = self.settings.task.scorer
-        grouped_task_info: dict[str, list[BaseModel]] = defaultdict(list)
+        grouped_task_rows: dict[str, list[BaseModel]] = defaultdict(list)
         for (id_, task) in self.board.tasks.items():
             if not task_filter(task):
                 continue
-            proj_str = None if (task.project_id is None) else self._project_str_from_id(task.project_id)
-            icons = task.status_icons
-            name = task.name + (f' {icons}' if icons else '')
-            task_info = TaskInfo(id=task_id_style(id_, bold=True), name=name, project=proj_str, score=scorer(task))
+            if since and (task.status == TaskStatus.complete) and (cast(datetime, task.completed_time) < since):
+                continue
             if (group := group_by_status.get(task.status)):
-                grouped_task_info[group].append(task_info)
-        # sort by the scoring criterion, in reverse score order
-        for task_infos in grouped_task_info.values():
-            task_infos.sort(key=attrgetter('score'), reverse=True)
+                group_settings = group_settings_by_group[group]
+                task_row = group_settings.get_task_row(id_, task)
+                grouped_task_rows[group].append(task_row)
+        # sort by the group's criterion, in reverse score order
+        for (group, task_rows) in grouped_task_rows.items():
+            group_settings = group_settings_by_group[group]
+            group_settings.sort_task_rows(task_rows)
+        # count tasks in each group prior to limiting
+        task_counts = {group: len(task_rows) for (group, task_rows) in grouped_task_rows.items()}
         if limit is not None:  # limit the number of tasks in each group
-            grouped_task_info = {group: task_infos[:limit] for (group, task_infos) in grouped_task_info.items()}
+            grouped_task_rows = {group: task_rows[:limit] for (group, task_rows) in grouped_task_rows.items()}
         # build table
-        caption = f'[not italic]Score[/]: {scorer.name}'
-        if scorer.description:
-            caption += f' ({scorer.description})'
+        if {'todo', 'active'} & set(grouped_task_rows):  # only show scorer name if showing scores
+            caption = f'[not italic]Score[/]: {scorer.name}'
+            if scorer.description:
+                caption += f' ({scorer.description})'
+        else:
+            caption = None
         table = Table(title=self.board.name, title_style='bold italic blue', caption=caption)
+        # make a subtable for each status group
         subtables = []
-        for (group, color) in group_colors.items():
-            if group in grouped_task_info:
+        for group in group_colors:
+            if group in grouped_task_rows:
+                group_settings = group_settings_by_group[group]
+                task_count = task_counts[group]
+                header = group_settings.get_group_header(task_count)
                 # each status group is a main table column
-                table.add_column(group, header_style=color, justify='center')
-                task_infos = grouped_task_info[group]
-                subtable: Table | str = make_table(TaskInfo, task_infos) if task_infos else ''
+                table.add_column(header, justify='center')
+                task_rows = grouped_task_rows[group]
+                subtable: Table | str = make_table(group_settings.task_row_type, task_rows) if task_rows else ''
                 subtables.append(subtable)
         if subtables:
             table.add_row(*subtables)
             print(table)
         else:
             msg = 'No tasks'
             if (statuses is not None) or (projects is not None) or (tags is not None) or (limit is not None):
@@ -825,65 +941,70 @@
                 return self.new_board()
             if prefix_match(tok1, 'show'):
                 # parse colon-separated arguments
                 d = dict([parse_option_value_pair(tok) for tok in tokens[2:]])
                 kwargs: dict[str, Any] = {}
                 _keys = set()
                 for (singular, plural) in [('status', 'statuses'), ('project', 'projects'), ('tag', 'tags')]:
-                    for key in d:
+                    for (key, val) in d.items():
                         key_lower = key.lower()
                         if prefix_match(key_lower, singular, minlen=3) or prefix_match(key_lower, plural, minlen=3):
-                            values = split_comma_list(d[key])
-                            _keys.add(key)
+                            values = split_comma_list(val)
                             if not values:
                                 raise UserInputError(f'Must provide at least one {singular}')
                             kwargs[plural] = values
                         elif prefix_match(key_lower, 'limit', minlen=3):
-                            kwargs['limit'] = parse_task_limit(d[key])
-                            _keys.add(key)
+                            kwargs['limit'] = parse_task_limit(val)
+                        elif key_lower == 'since':
+                            none_vals = ['all', 'always', 'any', 'anytime']
+                            since = None if (val.strip().lower() in none_vals) else self.settings.time.parse_datetime(val)
+                            kwargs['since'] = since
+                        else:
+                            continue
+                        _keys.add(key)
                 for key in d:
                     if key not in _keys:  # reject unknown keys
                         raise UserInputError(f'Invalid option: {key}')
                 return self.show_board(**kwargs)
             if prefix_match(tok1, 'schema', minlen=2):
                 return self.show_schema(Board)
         elif prefix_match(tok0, 'help') or (tok0 == 'info'):
             return self.show_help()
         elif prefix_match(tok0, 'project'):
             if (ntokens == 1) or prefix_match(tokens[1], 'help'):
                 return self.show_project_help()
             tok1 = tokens[1]
             if prefix_match(tok1, 'new'):
-                return self.new_project()
+                return self.new_project(None if (ntokens == 2) else tokens[2])
             if prefix_match(tok1, 'delete'):
                 return self.delete_project(None if (ntokens == 2) else tokens[2])
             if prefix_match(tok1, 'show'):
                 if ntokens == 2:
                     return self.show_projects()
                 return self.show_project(tokens[2])
             if tok1 == 'set':
-                if len(tokens) < 5:
+                if len(tokens) < 4:
                     raise UserInputError('Must provide [ID/NAME] [FIELD] [VALUE]')
                 return self.update_project(*tokens[2:5])
         elif prefix_match(tok0, 'quit') or (tok0 == 'exit'):
             return self.quit_shell()
         elif prefix_match(tok0, 'task'):
             if (ntokens == 1) or prefix_match(tokens[1], 'help'):
                 return self.show_task_help()
             tok1 = tokens[1]
             if prefix_match(tok1, 'new'):
-                return self.new_task()
+                return self.new_task(None if (ntokens == 2) else tokens[2])
             if prefix_match(tok1, 'delete'):
                 return self.delete_task(None if (ntokens == 2) else tokens[2])
             if prefix_match(tok1, 'show'):
                 if ntokens == 2:
                     return self.show_tasks()
                 return self.show_task(tokens[2])
             if tok1 == 'set':
-                if len(tokens) < 5:
+                if len(tokens) < 4:
                     raise UserInputError('Must provide [ID/NAME] [FIELD] [VALUE]')
                 return self.update_task(*tokens[2:5])
             action: Optional[TaskStatusAction] = None
             if prefix_match(tok1, 'begin'):
                 # for convenience, use 'begin' instead of 'start' to avoid prefix collision with 'show'
                 action = TaskStatusAction.start
             else:
```

### Comparing `daikanban-0.1.1/daikanban/main.py` & `daikanban-0.1.2/daikanban/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python3
 
 from pathlib import Path
 from typing import Annotated, Optional
 
 import typer
 
+from daikanban import __version__
 from daikanban.interface import BoardInterface
 from daikanban.model import Board
 
 
 APP = typer.Typer(
     add_completion=False,
-    no_args_is_help=True,
     context_settings={'help_option_names': ['-h', '--help']}
 )
 
 
 @APP.command(short_help='create new board')
 def new() -> None:
     """Create a new DaiKanban board."""
@@ -31,10 +31,22 @@
 @APP.command(short_help='enter interactive shell')
 def shell(
     board: Annotated[Optional[Path], typer.Option('--board', '-b', help='DaiKanban board JSON file')] = None
 ) -> None:
     """Launch the DaiKanban shell."""
     BoardInterface().launch_shell(board_path=board)
 
+@APP.callback(invoke_without_command=True)
+def main(
+    ctx: typer.Context,
+    version: Annotated[bool, typer.Option('--version', help='show version number')] = False
+) -> None:
+    """A kanban-style project task queue."""
+    if ctx.invoked_subcommand is None:
+        if version:
+            print(__version__)
+        else:
+            ctx.get_help()
+
 
 if __name__ == '__main__':
     APP()
```

### Comparing `daikanban-0.1.1/daikanban/model.py` & `daikanban-0.1.2/daikanban/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Annotated, Any, ClassVar, Counter, Iterator, Literal, Optional, TypeVar, cast
 from urllib.parse import urlparse
 
 from pydantic import AfterValidator, AnyUrl, BaseModel, BeforeValidator, Field, PlainSerializer, computed_field, model_validator
 from typing_extensions import Self, TypeAlias
 
 from daikanban.settings import Settings, TaskStatus
-from daikanban.utils import KanbanError, NameMatcher, StrEnum, exact_match, first_name_match, get_current_time, get_duration_between, human_readable_duration
+from daikanban.utils import KanbanError, NameMatcher, StrEnum, exact_match, first_name_match, get_current_time, get_duration_between, human_readable_duration, parse_string_set
 
 
 T = TypeVar('T')
 M = TypeVar('M', bound=BaseModel)
 
 NEARLY_DUE_THRESH = timedelta(days=1)
 
@@ -45,14 +45,24 @@
     return Settings.global_settings().time.parse_duration(obj) if isinstance(obj, str) else obj
 
 def _parse_optional(obj: Any) -> Any:
     if (obj is None) or (isinstance(obj, str) and (not obj)):
         return None
     return obj
 
+def _parse_str_set(obj: str | set[str]) -> set[str]:
+    return (parse_string_set(obj) or set()) if isinstance(obj, str) else obj
+
+def _parse_url_set(obj: str | set[str]) -> set[AnyUrl]:
+    if obj == '':
+        return set()
+    strings = parse_string_set(obj) if isinstance(obj, str) else obj
+    return set(map(_check_url, strings))  # type: ignore[arg-type]
+
+
 Name: TypeAlias = Annotated[str, AfterValidator(_check_name)]
 
 Url: TypeAlias = Annotated[AnyUrl, BeforeValidator(_check_url)]
 
 Datetime: TypeAlias = Annotated[
     datetime,
     BeforeValidator(_parse_datetime),
@@ -69,14 +79,18 @@
 
 OptionalDuration: TypeAlias = Annotated[Optional[Duration], BeforeValidator(_parse_optional)]
 
 Score: TypeAlias = Annotated[float, Field(description='A score (positive number)', ge=0.0)]
 
 OptionalScore: TypeAlias = Annotated[Optional[Score], BeforeValidator(_parse_optional)]
 
+StrSet: TypeAlias = Annotated[set[str], BeforeValidator(_parse_str_set)]
+
+UrlSet: TypeAlias = Annotated[set[Url], BeforeValidator(_parse_url_set)]
+
 
 ##################
 # ERROR HANDLING #
 ##################
 
 class InconsistentTimestampError(KanbanError):
     """Error that occurs if a timestamp is inconsistent."""
@@ -118,16 +132,15 @@
 
 #########
 # MODEL #
 #########
 
 class Model(BaseModel):
     """Base class setting up pydantic configs."""
-    class Config:  # noqa: D106
-        frozen = True
+    model_config = {'frozen': True}
 
     def _replace(self, **kwargs: Any) -> Self:
         """Creates a new copy of the object with the given kwargs replaced.
         Validation will be performed."""
         d = dict(self)
         for (key, val) in kwargs.items():
             if key not in d:  # do not allow extra fields
@@ -179,15 +192,15 @@
         default=None,
         description='Project description'
     )
     created_time: Datetime = Field(
         default_factory=get_current_time,
         description='Time the project was created'
     )
-    links: Optional[set[Url]] = Field(
+    links: Optional[UrlSet] = Field(
         default=None,
         description='Links associated with the project'
     )
 
 
 class Log(Model):
     """A piece of information associated with a task at a particular time."""
@@ -230,19 +243,19 @@
         default=None,
         description='Date the task is due'
     )
     project_id: Optional[Id] = Field(
         default=None,
         description='Project ID'
     )
-    tags: Optional[set[str]] = Field(
+    tags: Optional[StrSet] = Field(
         default=None,
         description='Tags associated with the task'
     )
-    links: Optional[set[Url]] = Field(
+    links: Optional[UrlSet] = Field(
         default=None,
         description='Links associated with the project'
     )
     created_time: Datetime = Field(
         default_factory=get_current_time,
         description='Time the task was created'
     )
@@ -287,17 +300,14 @@
         for field in self.DURATION_FIELDS:
             # make durations human-readable
             if field in d:
                 val = getattr(self, field)
                 if (val is not None):
                     assert isinstance(val, float)
                     d[field] = '-' if (val == 0) else human_readable_duration(val)
-            if ('cycle_time' in d) and ('total_time_worked' in d) and (d['cycle_time'] == d['total_time_worked']):
-                # remove redundant field since they are equivalent here
-                del d['cycle_time']
         if self.project_id is None:
             d['project_id'] = '-'
         return d
 
     @computed_field  # type: ignore[misc]
     @property
     def status(self) -> TaskStatus:
@@ -414,15 +424,16 @@
 
     def started(self, dt: Optional[Datetime] = None) -> 'Task':
         """Returns a new started version of the task, if its status is todo.
         Otherwise raises a TaskStatusError."""
         if self.status == TaskStatus.todo:
             dt = dt or get_current_time()
             if dt < self.created_time:
-                raise TaskStatusError('cannot start a task before its creation time')
+                dt_str = Settings.global_settings().time.render_datetime(self.created_time)
+                raise TaskStatusError(f'cannot start a task before its creation time ({dt_str})')
             return self.model_copy(update={'first_started_time': dt})
         raise TaskStatusError(f"cannot start task with status '{self.status}'")
 
     def completed(self, dt: Optional[datetime] = None) -> 'Task':
         """Returns a new completed version of the task, if its status is active.
         Otherwise raises a TaskStatusError."""
         if self.status == TaskStatus.active:
```

### Comparing `daikanban-0.1.1/daikanban/prompt.py` & `daikanban-0.1.2/daikanban/prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class Console(rich.console.Console):
     """Subclass of rich's Console that fixes a terminal bug.
     See:
         - https://github.com/Textualize/rich/issues/2293
         - https://github.com/Textualize/rich/commit/568b9517b63282ac781a907d82b0c2965242be54"""
 
-    def input(self, prompt: TextType = '', password: bool = False, stream: Optional[TextIO] = None) -> str:  # type: ignore  # noqa
+    def input(self, prompt: TextType = '', password: bool = False, stream: Optional[TextIO] = None) -> str:  # type: ignore  # noqa: D102
         prompt_str = ''
         if prompt:
             with self.capture() as capture:
                 self.print(prompt, markup=True, emoji=True, end='')
             prompt_str = capture.get()
         return input(prompt_str)
 
@@ -40,32 +40,34 @@
     regex = re.compile(match)
     while True:
         result = Prompt.ask(f'[bold]{prompt}[/]', default=default, console=Console()) or ''
         if regex.fullmatch(result):
             break
     return result
 
-def validated_input(prompt: str, validator: Callable[[str], T], default: Any = None, use_prompt_suffix: bool = True, **kwargs: Any) -> T:
+def validated_input(prompt: str, validator: Callable[[str], T], default: Any = None, use_prompt_suffix: bool = True, print_error: bool = True, **kwargs: Any) -> T:
     """Prompts the user with the given string until the user's response passes a validator function with no error.
         prompt: prompt string
         validator: function to parse and validate the input
         default: default value
-        use_prompt_suffix: display the default prompt suffix (colon) after the prompt and default
+        use_prompt_suffix: displays the default prompt suffix (colon) after the prompt and default
+        print_error: if True, displays an error message upon each failed iteration of input
         kwargs: passed to the rich prompt"""
     if default not in (None, PydanticUndefined):
         if isinstance(default, float) and (int(default) == default):
             default = int(default)
         default = str(default)
     prompt_cls = Prompt if use_prompt_suffix else PromptNoSuffix
     while True:
         result = prompt_cls.ask(f'[bold]{prompt}[/]', default=default, console=Console(), **kwargs) or ''
         try:
             return validator(result)
         except Exception as e:
-            rich.print(err_style(e))
+            if print_error:
+                rich.print(err_style(e))
 
 
 @dataclass
 class Prompter(Generic[T]):
     """Class which prompts a user for input, then parses and validates the response."""
     prompt: str  # prompt string
     parse: Optional[Callable[[str], T]] = None  # function to parse input
@@ -113,13 +115,14 @@
             raise UserInputError(msg) from None
 
     def prompt_field(self) -> T:
         """Prompts the user for the field until a valid one is entered."""
         return self.prompter.loop_prompt()
 
 
-def model_from_prompt(model_type: type[M], prompters: dict[str, FieldPrompter] = {}) -> M:  # noqa: B006
-    """Given a BaseModel type and collection of FieldPrompters, constructs an instance of the type from a sequence of user prompts."""
-    kwargs: dict[str, Any] = {}
+def model_from_prompt(model_type: type[M], prompters: dict[str, FieldPrompter] = {}, defaults: dict[str, Any] = {}) -> M:  # noqa: B006
+    """Given a BaseModel type and collection of FieldPrompters, constructs an instance of the type from a sequence of user prompts.
+    A collection of defaults may also be provided for any fields which are missing a prompter."""
+    kwargs: dict[str, Any] = dict(defaults)
     for (field, prompter) in prompters.items():
         kwargs[field] = prompter.prompt_field()
     return model_type(**kwargs)
```

### Comparing `daikanban-0.1.1/daikanban/score.py` & `daikanban-0.1.2/daikanban/score.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/daikanban/settings.py` & `daikanban-0.1.2/daikanban/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,19 +193,23 @@
     def scorer(self) -> TaskScorer:
         """Gets the TaskScorer object used to score tasks."""
         return TASK_SCORERS[self.scorer_name]
 
 
 class DisplaySettings(BaseModel):
     """Display settings."""
-    limit: Optional[int] = Field(
+    max_tasks: Optional[int] = Field(
         default=None,
-        description='max number of tasks to display',
+        description='max number of tasks to display per column',
         ge=0
     )
+    completed_age_off: Optional[timedelta] = Field(
+        default=timedelta(days=30),
+        description='length of time after which to stop displaying completed tasks'
+    )
     status_groups: dict[str, list[str]] = Field(
         default=DEFAULT_STATUS_GROUPS,
         description='map from board columns (groups) to task statuses'
     )
 
 
 class Settings(BaseModel):
```

### Comparing `daikanban-0.1.1/daikanban/utils.py` & `daikanban-0.1.2/daikanban/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from contextlib import contextmanager
+import csv
 from datetime import datetime, timezone
 from enum import Enum
 import operator
 import re
 import sys
 from typing import Any, Callable, Iterable, Iterator, Optional
 
@@ -13,22 +14,34 @@
 
 SECS_PER_HOUR = 3600
 HOURS_PER_DAY = 24
 DAYS_PER_WEEK = 7
 SECS_PER_DAY = SECS_PER_HOUR * HOURS_PER_DAY
 
 
+#########
+# ENUMS #
+#########
+
 class StrEnum(str, Enum):
     """Enum class whose __str__ representation is just a plain string value.
     NOTE: this class exists in the standard library in Python >= 3.11."""
 
     def __str__(self) -> str:
         return self.value
 
 
+class NotGivenType(Enum):
+    """Sentinel class for a value of "not given," when needed to distinguish it from None."""
+    NotGiven = 'NotGiven'
+
+
+NotGiven = NotGivenType.NotGiven
+
+
 ###################
 # STRING HANDLING #
 ###################
 
 def to_snake_case(name: str) -> str:
     """Converts an arbitrary string to snake case."""
     name = name.replace('"', '').replace("'", '')
@@ -75,45 +88,55 @@
     s2 = name2.strip().casefold()
     return (s1 == s2) or ((len(s1) >= 3) and s2.startswith(s1))
 
 def first_name_match(matcher: NameMatcher, name1: str, names2: Iterable[str]) -> Optional[str]:
     """Given a NameMatcher, query name, and an iterable of names to compare against, returns the first name that matches (if there is one), otherwise None."""
     return next((name2 for name2 in names2 if matcher(name1, name2)), None)
 
+def parse_string_set(s: str) -> Optional[set[str]]:
+    """Parses a comma-separated string into a set of strings.
+    Allows for quote delimiting so that commas can be escaped.
+    Strips any leading or trailing whitespace from each string."""
+    return {string.strip() for string in list(csv.reader([s]))[0]} or None
+
 
 ############
 # DATETIME #
 ############
 
 def get_current_time() -> datetime:
     """Gets the current time (timezone-aware)."""
     return datetime.now(timezone.utc).astimezone()
 
 def get_duration_between(dt1: datetime, dt2: datetime) -> float:
     """Gets the duration (in days) between two datetimes."""
     return (dt2 - dt1).total_seconds() / SECS_PER_DAY
 
-def human_readable_duration(days: float) -> str:
+def human_readable_duration(days: float, prefer_days: bool = False) -> str:
     """Given a duration (in days), converts it to a human-readable string.
-    This goes out to minute precision only."""
+    This goes out to minute precision only.
+    If prefer_days=True, show days and not weeks."""
     if days == 0:
         return '0 seconds'
-    s = pendulum.Duration(days=days).in_words()
+    dur = pendulum.Duration(days=days)
+    s = dur.in_words()
+    if prefer_days and ('week' in s):
+        s = re.sub(r'\d+ weeks?( \d+ days?)?', f'{dur.days} days', s)
     # hacky way to truncate the seconds
     return re.sub(r'\s+\d+ seconds?', '', s)
 
 
 #########
 # STYLE #
 #########
 
-def style_str(val: Any, color: str, bold: bool = False) -> str:
-    """Renders a value as a rich-formatted string with a given color.
-    If bold=True, make it bold."""
-    tag = ('' if bold else 'not ') + f'bold {color}'
+def style_str(val: Any, color: str, bold: bool = False, italic: bool = False) -> str:
+    """Renders a value as a rich-formatted string with a given color, bold, and italic settings."""
+    tags = [('' if bold else 'not ') + 'bold', ('' if italic else 'not ') + 'italic', color]
+    tag = ' '.join(tags)
     return f'[{tag}]{val}[/]'
 
 def err_style(obj: object) -> str:
     """Renders an error as a rich-styled string."""
     s = str(obj)
     if s:
         s = s[0].upper() + s[1:]
```

### Comparing `daikanban-0.1.1/doc/dkmarkdown.md` & `daikanban-0.1.2/doc/dkmarkdown.md`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/doc/screenshot_v0_1_0.png` & `daikanban-0.1.2/doc/screenshot_v0_1_0.png`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/tests/test_model.py` & `daikanban-0.1.2/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 
 class TestProject:
 
     def test_links(self):
         proj = Project(name='proj')
         assert proj.links is None
-        with pytest.raises(ValidationError, match='Input should be a valid set'):
-            proj = Project(name='proj', links='')
+        proj = Project(name='proj', links='')
+        assert proj.links == set()
         proj = Project(name='proj', links=set())
         assert proj.links == set()
         with pytest.raises(ValidationError, match='Invalid URL'):
             proj = Project(name='proj', links={''})
         with pytest.raises(ValidationError, match='Invalid URL'):
             proj = Project(name='proj', links={'example'})
         proj = Project(name='proj', links={'example.com'})
@@ -32,14 +32,18 @@
         assert proj.links == {Url('https://www.example.com/')}
         proj = Project(name='proj', links={'http://example.com'})
         assert proj.links == {Url('http://example.com/')}
         proj = Project(name='proj', links={'fake://example.com'})
         assert proj.links == {Url('fake://example.com')}
         proj = Project(name='proj', links={'scheme://netloc/path;parameters?query#fragment'})
         assert proj.links == {Url('scheme://netloc/path;parameters?query#fragment')}
+        proj = Project(name='proj', links='link1.com')
+        assert proj.links == {Url('https://link1.com')}
+        proj = Project(name='proj', links='link1.com, link2.org')
+        assert proj.links == {Url('https://link1.com'), Url('https://link2.org')}
 
 
 class TestTask:
 
     def test_priority(self):
         assert Task(name='task', priority=1).priority == 1
         assert Task(name='task', priority=0).priority == 0
@@ -70,14 +74,23 @@
         dt = Settings.global_settings().time.parse_datetime('2024-01-01')
         assert Task(name='task').due_date is None
         assert Task(name='task', due_date=None).due_date is None
         assert Task(name='task', due_date='').due_date is None
         assert Task(name='task', due_date=dt).due_date == dt
         assert Task(name='task', due_date=dt.strftime(DEFAULT_DATETIME_FORMAT)).due_date == dt
 
+    def test_tags(self):
+        assert Task(name='task').tags is None
+        assert Task(name='task', tags=None).tags is None
+        assert Task(name='task', tags={'a', 'b'}).tags == {'a', 'b'}
+        assert Task(name='task', tags='').tags == set()
+        assert Task(name='task', tags='a').tags == {'a'}
+        assert Task(name='task', tags='a,b').tags == {'a', 'b'}
+        assert Task(name='task', tags=' a,  b').tags == {'a', 'b'}
+
     def test_replace(self):
         now = get_current_time()
         task = Task(name='task', created_time=now)
         assert task._replace(name='new').name == 'new'
         assert task._replace(name='new')._replace(name='task') == task
         assert task == Task(name='task', created_time=now)
         with pytest.raises(TypeError, match="Unknown field 'fake'"):
```

### Comparing `daikanban-0.1.1/tests/test_settings.py` & `daikanban-0.1.2/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/LICENSE` & `daikanban-0.1.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
```

### Comparing `daikanban-0.1.1/README.md` & `daikanban-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # DaiKanban <br/> 大看板
 
+[![PyPI - Version](https://img.shields.io/pypi/v/daikanban)](https://pypi.org/project/daikanban)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://raw.githubusercontent.com/jeremander/daikanban/main/LICENSE)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+
 A command-line Kanban board that helps you prioritize and organize your projects.
 
 ## Screenshot
 
 ![Screenshot](doc/screenshot_v0_1_0.png)
 
 (*[screenshot](https://github.com/jeremander/daikanban/blob/main/doc/screenshot_v0_1_0.png) from `v0.1.0`*)
@@ -56,14 +60,15 @@
 | `quit` | `q` | Quit |
 | `board load` | `b l` | Load a board |
 | `board show` | `b s` | Show current board |
 | `project new` | `p n` | Create new project |
 | `project show [PROJECT]` | `p s [PROJECT]` | Show project info |
 | `task new` | `t n` | Create new task |
 | `task show [TASK]` | `t s [TASK]` | Show task info |
+| `task set [FIELD] [VALUE]` | `t set [FIELD] [VALUE]` | Update task info (if `VALUE` is omitted, set it to null) |
 
 Projects and tasks can be referred to either by their ID (a unique number assigned at creation) or their name. For ease of use, it is recommended to avoid whitespace characters in names:
 
 - ❌ `Do the thing`
 - ✅ `do-the-thing`
 
 ### Shell commands to advance tasks
```

### Comparing `daikanban-0.1.1/pyproject.toml` & `daikanban-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `daikanban-0.1.1/PKG-INFO` & `daikanban-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daikanban
-Version: 0.1.1
+Version: 0.1.2
 Summary: A kanban-style project task queue.
 Project-URL: Documentation, https://github.com/jeremander/daikanban#readme
 Project-URL: Issues, https://github.com/jeremander/daikanban/issues
 Project-URL: Source, https://github.com/jeremander/daikanban
 Author-email: Jeremy Silver <jeremys@nessiness.com>
 License-Expression: MIT
 License-File: AUTHORS.md
@@ -17,14 +17,18 @@
 Requires-Dist: pytimeparse>=1.1
 Requires-Dist: typer[all]>=0.9
 Requires-Dist: typing-extensions>=4.10
 Description-Content-Type: text/markdown
 
 # DaiKanban <br/> 大看板
 
+[![PyPI - Version](https://img.shields.io/pypi/v/daikanban)](https://pypi.org/project/daikanban)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://raw.githubusercontent.com/jeremander/daikanban/main/LICENSE)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+
 A command-line Kanban board that helps you prioritize and organize your projects.
 
 ## Screenshot
 
 ![Screenshot](doc/screenshot_v0_1_0.png)
 
 (*[screenshot](https://github.com/jeremander/daikanban/blob/main/doc/screenshot_v0_1_0.png) from `v0.1.0`*)
@@ -77,14 +81,15 @@
 | `quit` | `q` | Quit |
 | `board load` | `b l` | Load a board |
 | `board show` | `b s` | Show current board |
 | `project new` | `p n` | Create new project |
 | `project show [PROJECT]` | `p s [PROJECT]` | Show project info |
 | `task new` | `t n` | Create new task |
 | `task show [TASK]` | `t s [TASK]` | Show task info |
+| `task set [FIELD] [VALUE]` | `t set [FIELD] [VALUE]` | Update task info (if `VALUE` is omitted, set it to null) |
 
 Projects and tasks can be referred to either by their ID (a unique number assigned at creation) or their name. For ease of use, it is recommended to avoid whitespace characters in names:
 
 - ❌ `Do the thing`
 - ✅ `do-the-thing`
 
 ### Shell commands to advance tasks
```

