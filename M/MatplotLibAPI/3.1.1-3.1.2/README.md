# Comparing `tmp/matplotlibapi-3.1.1.tar.gz` & `tmp/matplotlibapi-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlibapi-3.1.1.tar", last modified: Mon Jun  3 09:48:39 2024, max compression
+gzip compressed data, was "matplotlibapi-3.1.2.tar", last modified: Mon Jun  3 11:09:47 2024, max compression
```

## Comparing `matplotlibapi-3.1.1.tar` & `matplotlibapi-3.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:48:39.352977 matplotlibapi-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:48:39.352977 matplotlibapi-3.1.1/MatplotLibAPI/
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/Bubble.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/Composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    14851 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/Network.py
--rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/Pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/Table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/Timeserie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/Treemap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:48:39.352977 matplotlibapi-3.1.1/MatplotLibAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-06-03 09:48:39.000000 matplotlibapi-3.1.1/MatplotLibAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-03 09:48:39.000000 matplotlibapi-3.1.1/MatplotLibAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:48:39.000000 matplotlibapi-3.1.1/MatplotLibAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-03 09:48:39.000000 matplotlibapi-3.1.1/MatplotLibAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-03 09:48:39.000000 matplotlibapi-3.1.1/MatplotLibAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-06-03 09:48:39.352977 matplotlibapi-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:48:39.352977 matplotlibapi-3.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:09:47.388282 matplotlibapi-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-03 11:09:43.000000 matplotlibapi-3.1.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:09:47.388282 matplotlibapi-3.1.2/MatplotLibAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-06-03 11:09:43.000000 matplotlibapi-3.1.2/MatplotLibAPI/Bubble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-06-03 11:09:43.000000 matplotlibapi-3.1.2/MatplotLibAPI/Composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14836 2024-06-03 11:09:43.000000 matplotlibapi-3.1.2/MatplotLibAPI/Network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-06-03 11:09:43.000000 matplotlibapi-3.1.2/MatplotLibAPI/Pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-06-03 11:09:43.000000 matplotlibapi-3.1.2/MatplotLibAPI/Table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-06-03 11:09:43.000000 matplotlibapi-3.1.2/MatplotLibAPI/Timeserie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-06-03 11:09:43.000000 matplotlibapi-3.1.2/MatplotLibAPI/Treemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-06-03 11:09:43.000000 matplotlibapi-3.1.2/MatplotLibAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:09:47.388282 matplotlibapi-3.1.2/MatplotLibAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-06-03 11:09:47.000000 matplotlibapi-3.1.2/MatplotLibAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-03 11:09:47.000000 matplotlibapi-3.1.2/MatplotLibAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:09:47.000000 matplotlibapi-3.1.2/MatplotLibAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-03 11:09:47.000000 matplotlibapi-3.1.2/MatplotLibAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-03 11:09:47.000000 matplotlibapi-3.1.2/MatplotLibAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-06-03 11:09:47.388282 matplotlibapi-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-03 11:09:43.000000 matplotlibapi-3.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-03 11:09:43.000000 matplotlibapi-3.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 11:09:47.388282 matplotlibapi-3.1.2/setup.cfg
```

### Comparing `matplotlibapi-3.1.1/LICENSE` & `matplotlibapi-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlibapi-3.1.1/MatplotLibAPI/Bubble.py` & `matplotlibapi-3.1.2/MatplotLibAPI/Bubble.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 # %%
 from typing import Optional
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
 import seaborn as sns
 
-from . import DynamicFuncFormatter, StyleTemplate, generate_ticks, string_formatter, bmk_formatter, percent_formatter, format_func
-from .. import validate_dataframe
+from . import DynamicFuncFormatter, StyleTemplate, generate_ticks, string_formatter, bmk_formatter, percent_formatter, format_func,validate_dataframe
 
 BUBBLE_STYLE_TEMPLATE = StyleTemplate(
     format_funcs={"label": string_formatter,
                   "x": bmk_formatter,
                   "y": percent_formatter,
                   "label": string_formatter,
                   "z": bmk_formatter},
```

### Comparing `matplotlibapi-3.1.1/MatplotLibAPI/Composite.py` & `matplotlibapi-3.1.2/MatplotLibAPI/Composite.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.figure import Figure
 
 from .Network import plot_network, plot_network_components, DEFAULT
 from .Bubble import plot_bubble, BUBBLE_STYLE_TEMPLATE
 from .Table import plot_table
-from . import StyleTemplate, format_func
-from .. import validate_dataframe
+from . import StyleTemplate, format_func, validate_dataframe
 
 
 def plot_composite_bubble(
         pd_df: pd.DataFrame,
         label: str,
         x: str,
         y: str,
```

### Comparing `matplotlibapi-3.1.1/MatplotLibAPI/Network.py` & `matplotlibapi-3.1.2/MatplotLibAPI/Network.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 import networkx as nx
 import numpy as np
 import pandas as pd
 from networkx import Graph
 from networkx.classes.graph import Graph
 
 
-from . import StyleTemplate, string_formatter, format_func
-from .. import validate_dataframe
+from . import StyleTemplate, string_formatter, format_func,validate_dataframe
 
 NETWORK_STYLE_TEMPLATE = StyleTemplate(
 )
 
 DEFAULT = {"MAX_EDGES": 100,
            "MAX_NODES": 30,
            "MIN_NODE_SIZE": 100,
```

### Comparing `matplotlibapi-3.1.1/MatplotLibAPI/Pivot.py` & `matplotlibapi-3.1.2/MatplotLibAPI/Pivot.py`

 * *Files identical despite different names*

### Comparing `matplotlibapi-3.1.1/MatplotLibAPI/Table.py` & `matplotlibapi-3.1.2/MatplotLibAPI/Table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import List, Optional
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
 
-from . import StyleTemplate,  string_formatter
-from .. import validate_dataframe
+from . import StyleTemplate,  string_formatter,validate_dataframe
 
 TABLE_STYLE_TEMPLATE = StyleTemplate(
     background_color='black',
     fig_border='darkgrey',
     font_color='white',
     palette='magma'
 )
```

### Comparing `matplotlibapi-3.1.1/MatplotLibAPI/Timeserie.py` & `matplotlibapi-3.1.2/MatplotLibAPI/Timeserie.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 # %%
 from typing import Optional
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
 import seaborn as sns
 
-from . import DynamicFuncFormatter, StyleTemplate, string_formatter, bmk_formatter, format_func
-from .. import validate_dataframe
+from . import DynamicFuncFormatter, StyleTemplate, string_formatter, bmk_formatter, format_func,validate_dataframe
 
 
 TIMESERIE_STYLE_TEMPLATE = StyleTemplate(
     palette='rocket',
     format_funcs={"y": bmk_formatter, "label": string_formatter}
 )
```

### Comparing `matplotlibapi-3.1.1/MatplotLibAPI/Treemap.py` & `matplotlibapi-3.1.2/MatplotLibAPI/Treemap.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Hint for Visual Code Python Interactive window
 # %%
 from typing import Optional
 import pandas as pd
+from pandas import CategoricalDtype,BooleanDtype
 import plotly.graph_objects as go
 
-from . import StyleTemplate, string_formatter, percent_formatter
-from .. import validate_dataframe
+from . import StyleTemplate, string_formatter, percent_formatter,validate_dataframe
+
 
 
 TREEMAP_STYLE_TEMPLATE = StyleTemplate(
     background_color='black',
     fig_border='darkgrey',
     font_color='white',
     palette='magma',
@@ -45,17 +46,17 @@
                 {"family": style.font_name,
                  "size": style.font_size,
                  "color": style.font_color}
             }
 
     if color and color in pd_df.columns:
         color_data = pd_df[color]
-        if pd.api.types.is_categorical_dtype(color_data) or pd.api.types.is_object_dtype(color_data):
+        if isinstance(color_data, CategoricalDtype) or pd.api.types.is_object_dtype(color_data):
             color_data = color_data.astype('category').cat.codes
-        elif pd.api.types.is_bool_dtype(color_data):
+        elif isinstance(color_data, BooleanDtype):
             color_data = color_data.astype(int)
         data['marker'] = dict(colorscale="Viridis",
                               colors=color_data.to_list())
 
     g = go.Treemap(data)
 
     if not fig:
```

### Comparing `matplotlibapi-3.1.1/MatplotLibAPI/__init__.py` & `matplotlibapi-3.1.2/MatplotLibAPI/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 
+from .Treemap import plot_treemap, TREEMAP_STYLE_TEMPLATE
+from .Network import Graph
+from .Table import plot_table, TABLE_STYLE_TEMPLATE
+from .Timeserie import plot_timeserie, TIMESERIE_STYLE_TEMPLATE
+from .Composite import plot_composite_bubble
+from .Bubble import plot_bubble, BUBBLE_STYLE_TEMPLATE
 from typing import List, Optional, Dict, Callable, Union
 from dataclasses import dataclass
 import pandas as pd
 from pandas.api.extensions import register_dataframe_accessor
 import numpy as np
 
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib.dates import num2date
 from matplotlib.ticker import FuncFormatter
 import plotly.graph_objects as go
 
-from . import StyleTemplate
-from .Bubble import plot_bubble, BUBBLE_STYLE_TEMPLATE
-from .Composite import plot_composite_bubble
-from .Timeserie import plot_timeserie, TIMESERIE_STYLE_TEMPLATE
-from .Table import plot_table, TABLE_STYLE_TEMPLATE
-from .Network import Graph
-from .Treemap import plot_treemap, TREEMAP_STYLE_TEMPLATE
 
 # region Utils
 
+def validate_dataframe(pd_df: pd.DataFrame,
+                       cols: List[str],
+                       sort_by: Optional[str] = None):
+    _columns = cols.copy()
+    if sort_by and sort_by not in _columns:
+        _columns.append(sort_by)
+    for col in _columns:
+        if col not in pd_df.columns:
+            raise AttributeError(f"{col} is not a DataFrame's column")
+
 
 def format_func(
         format_funcs: Optional[Dict[str, Optional[Callable[[Union[int, float, str]], str]]]],
         label: Optional[str] = None,
         x: Optional[str] = None,
         y: Optional[str] = None,
         z: Optional[str] = None):
```

