# Comparing `tmp/matplotlibapi-3.1.0.tar.gz` & `tmp/matplotlibapi-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlibapi-3.1.0.tar", last modified: Fri May 31 13:36:33 2024, max compression
+gzip compressed data, was "matplotlibapi-3.1.1.tar", last modified: Mon Jun  3 09:48:39 2024, max compression
```

## Comparing `matplotlibapi-3.1.0.tar` & `matplotlibapi-3.1.1.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:36:33.474310 matplotlibapi-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-31 13:36:26.000000 matplotlibapi-3.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:36:33.474310 matplotlibapi-3.1.0/MatplotLibAPI/
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-31 13:36:26.000000 matplotlibapi-3.1.0/MatplotLibAPI/Bubble.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-31 13:36:26.000000 matplotlibapi-3.1.0/MatplotLibAPI/Composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-31 13:36:26.000000 matplotlibapi-3.1.0/MatplotLibAPI/Network.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-31 13:36:26.000000 matplotlibapi-3.1.0/MatplotLibAPI/Pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-31 13:36:26.000000 matplotlibapi-3.1.0/MatplotLibAPI/Style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-31 13:36:26.000000 matplotlibapi-3.1.0/MatplotLibAPI/Table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-31 13:36:26.000000 matplotlibapi-3.1.0/MatplotLibAPI/Timeserie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-31 13:36:26.000000 matplotlibapi-3.1.0/MatplotLibAPI/Treemap.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-31 13:36:26.000000 matplotlibapi-3.1.0/MatplotLibAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-05-31 13:36:26.000000 matplotlibapi-3.1.0/MatplotLibAPI/pdAccessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:36:33.474310 matplotlibapi-3.1.0/MatplotLibAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-31 13:36:33.000000 matplotlibapi-3.1.0/MatplotLibAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-31 13:36:33.000000 matplotlibapi-3.1.0/MatplotLibAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:36:33.000000 matplotlibapi-3.1.0/MatplotLibAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-31 13:36:33.000000 matplotlibapi-3.1.0/MatplotLibAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-31 13:36:33.000000 matplotlibapi-3.1.0/MatplotLibAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-31 13:36:33.474310 matplotlibapi-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-31 13:36:26.000000 matplotlibapi-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-31 13:36:26.000000 matplotlibapi-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:36:33.474310 matplotlibapi-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:48:39.352977 matplotlibapi-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:48:39.352977 matplotlibapi-3.1.1/MatplotLibAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/Bubble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/Composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14851 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/Network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/Pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/Table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/Timeserie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/Treemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/MatplotLibAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:48:39.352977 matplotlibapi-3.1.1/MatplotLibAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-06-03 09:48:39.000000 matplotlibapi-3.1.1/MatplotLibAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-03 09:48:39.000000 matplotlibapi-3.1.1/MatplotLibAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:48:39.000000 matplotlibapi-3.1.1/MatplotLibAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-03 09:48:39.000000 matplotlibapi-3.1.1/MatplotLibAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-03 09:48:39.000000 matplotlibapi-3.1.1/MatplotLibAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-06-03 09:48:39.352977 matplotlibapi-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-03 09:48:31.000000 matplotlibapi-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:48:39.352977 matplotlibapi-3.1.1/setup.cfg
```

### Comparing `matplotlibapi-3.1.0/LICENSE` & `matplotlibapi-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlibapi-3.1.0/MatplotLibAPI/Bubble.py` & `matplotlibapi-3.1.1/MatplotLibAPI/Bubble.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Hint for Visual Code Python Interactive window
 # %%
-
+from typing import Optional
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
 import seaborn as sns
-from typing import Optional
-from .Style import DynamicFuncFormatter, StyleTemplate, generate_ticks, _validate_panda, string_formatter, bmk_formatter, percent_formatter, format_func
 
+from . import DynamicFuncFormatter, StyleTemplate, generate_ticks, string_formatter, bmk_formatter, percent_formatter, format_func
+from .. import validate_dataframe
 
 BUBBLE_STYLE_TEMPLATE = StyleTemplate(
     format_funcs={"label": string_formatter,
                   "x": bmk_formatter,
                   "y": percent_formatter,
                   "label": string_formatter,
                   "z": bmk_formatter},
@@ -29,15 +29,15 @@
         style: StyleTemplate = BUBBLE_STYLE_TEMPLATE,
         max_values: int = BUBBLE_STYLE_TEMPLATE,
         center_to_mean: bool = False,
         sort_by: Optional[str] = None,
         ascending: bool = False,
         ax: Optional[Axes] = None):
 
-    _validate_panda(pd_df, cols=[label, x, y, z], sort_by=sort_by)
+    validate_dataframe(pd_df, cols=[label, x, y, z], sort_by=sort_by)
     style.format_funcs = format_func(
         style.format_funcs, label=label, x=x, y=y, z=z)
     if not sort_by:
         sort_by = z
 
     plot_df = pd_df[[label, x, y, z]].sort_values(
         by=sort_by, ascending=ascending).head(max_values)
```

### Comparing `matplotlibapi-3.1.0/MatplotLibAPI/Composite.py` & `matplotlibapi-3.1.1/MatplotLibAPI/Composite.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # Hint for Visual Code Python Interactive window
 # %%
+from typing import Optional, Tuple
+import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.figure import Figure
-import pandas as pd
+
+from .Network import plot_network, plot_network_components, DEFAULT
 from .Bubble import plot_bubble, BUBBLE_STYLE_TEMPLATE
 from .Table import plot_table
-from typing import Optional, Tuple
-from .Style import StyleTemplate, _validate_panda, format_func
+from . import StyleTemplate, format_func
+from .. import validate_dataframe
 
 
 def plot_composite_bubble(
         pd_df: pd.DataFrame,
         label: str,
         x: str,
         y: str,
         z: str,
         title: Optional[str] = "Test",
         style: StyleTemplate = BUBBLE_STYLE_TEMPLATE,
         max_values: int = 50,
         center_to_mean: bool = False,
-        filter_by:Optional[str] = None,
+        filter_by: Optional[str] = None,
         sort_by: Optional[str] = None,
         ascending: bool = False,
         table_rows: int = 10,
         figsize: Tuple[float, float] = (19.2, 10.8)) -> Figure:
 
-    _validate_panda(pd_df, cols=[label, x, y, z], sort_by=sort_by)
+    validate_dataframe(pd_df, cols=[label, x, y, z], sort_by=sort_by)
 
     if not sort_by:
         sort_by = z
     if not filter_by:
         filter_by = z
     plot_df = pd_df.sort_values(by=filter_by,
                                 ascending=ascending)[[label, x, y, z]].head(max_values)
```

### Comparing `matplotlibapi-3.1.0/MatplotLibAPI/Network.py` & `matplotlibapi-3.1.1/MatplotLibAPI/Network.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import networkx as nx
 import numpy as np
 import pandas as pd
 from networkx import Graph
 from networkx.classes.graph import Graph
 
 
-from .Style import StyleTemplate, string_formatter, _validate_panda,format_func
+from . import StyleTemplate, string_formatter, format_func
+from .. import validate_dataframe
 
 NETWORK_STYLE_TEMPLATE = StyleTemplate(
 )
 
 DEFAULT = {"MAX_EDGES": 100,
            "MAX_NODES": 30,
            "MIN_NODE_SIZE": 100,
@@ -161,31 +162,30 @@
         fonts_size = defaultdict(list)
         for node, width in node_size_dict.items():
             fonts_size[int(width)].append(node)
         fonts_size = dict(fonts_size)
 
         return node_size, edges_width, fonts_size
 
-    def subgraphX(self, node_list=None, max_edges: int = DEFAULT["MAX_EDGES"]):
+    def subgraph(self, node_list=None, max_edges: int = DEFAULT["MAX_EDGES"]) -> Graph:
         if node_list is None:
             node_list = self.nodes.sort("weight")[:DEFAULT["MAX_NODES"]]
         connected_subgraph_nodes = list(self.find_connected_subgraph())
         node_list = [
             node for node in node_list if node in connected_subgraph_nodes]
 
-        subgraph = nx.subgraph(
-            self, nbunch=node_list)
+        subgraph = nx.subgraph(self, nbunch=node_list)
         edges = subgraph.top_k_edges(attribute="weight", k=5).keys()
         subgraph = subgraph.edge_subgraph(list(edges)[:max_edges])
-        return subgraph
+        return Graph(subgraph)
 
-    def plotX(self,
-              title: str = "Test",
-              style: StyleTemplate = NETWORK_STYLE_TEMPLATE,
-              ax: Optional[Axes] = None) -> Axes:
+    def plot_network(self,
+                   title: str = "Test",
+                   style: StyleTemplate = NETWORK_STYLE_TEMPLATE,
+                   ax: Optional[Axes] = None) -> Axes:
         """
         Plots the degree distribution of the graph, including a degree rank plot and a degree histogram.
         """
         degree_sequence = sorted([d for n, d in self.degree()], reverse=True)
         dmax = max(degree_sequence)
         sns.set_palette(style.palette)
         if ax is None:
@@ -223,29 +223,32 @@
                 labels={n: string_formatter(n) for n in nodes})
         ax.set_facecolor(style.background_color)
         ax.set_title(title, color=style.font_color, fontsize=style.font_size*2)
         ax.set_axis_off()
 
         return ax
 
-    def analysis(self, node_list: Optional[List] = None,
+    def plot_network_components(self, node_list: Optional[List] = None,
                  scale: int = DEFAULT["GRAPH_SCALE"],
                  node_scale: int = DEFAULT["MAX_NODE_SIZE"],
                  edge_scale: float = DEFAULT["MAX_EDGE_WIDTH"],
                  max_nodes: int = DEFAULT["MAX_NODES"],
                  max_edges: int = DEFAULT["MAX_EDGES"],
                  plt_title: Optional[str] = "Top keywords"):
         # node_list=self.nodes_circuits(node_list)
-        g = self.subgraphX(max_edges=max_edges, node_list=node_list)
+        g = self.subgraph(max_edges=max_edges, node_list=node_list)
         connected_components = nx.connected_components(g)
+        axes=[]
         for connected_component in connected_components:
             if len(connected_component) > 5:
-                connected_component_graph = self.subgraphX(max_edges=max_edges,
-                                                           node_list=connected_component)
-                connected_component_graph.plotX()
+                connected_component_graph = self.subgraph(max_edges=max_edges,
+                                                          node_list=connected_component)
+                ax=connected_component_graph.plot_network()
+                axes.append(ax)
+        return axes
 
     def find_connected_subgraph(self):
         logging.info(f'find_connected_subgraph')
         # Copy the original graph to avoid modifying it
         H = self.copy()
 
         # Flag to keep track of whether any node with degree < 2 was removed
@@ -291,25 +294,24 @@
                 top_list[edge_key] = data[attribute]
         return top_list
 
     @staticmethod
     def from_pandas_edgelist(df: pd.DataFrame,
                              source: str = "source",
                              target: str = "target",
-                             weight: str = "weight"):
+                             weight: str = "weight") -> Graph:
         """
         Initialize netX instance with a simple dataframe
 
         :param df_source: DataFrame containing network data.
         :param source: Name of source nodes column in df_source.
         :param target: Name of target nodes column in df_source.
         :param weight: Name of edges weight column in df_source.
 
         """
-        G = Graph()
         G = nx.from_pandas_edgelist(
             df, source=source, target=target, edge_attr=weight, create_using=G)
         G = G.find_connected_subgraph()
 
         edge_aggregates = G.top_k_edges(attribute=weight, k=10)
         node_aggregates = {}
         for (u, v), weight_value in edge_aggregates.items():
@@ -319,29 +321,63 @@
                 node_aggregates[v] = 0
             node_aggregates[u] += weight_value
             node_aggregates[v] += weight_value
 
         nx.set_node_attributes(G, node_aggregates, name=weight)
 
         G = G.edge_subgraph(edges=G.top_k_edges(attribute=weight))
-        return G
+        return Graph(G)
 
 
 def plot_network(pd_df: pd.DataFrame,
                  source: str = "source",
                  target: str = "target",
                  weight: str = "weight",
                  title: str = "Test",
                  style: StyleTemplate = NETWORK_STYLE_TEMPLATE,
                  sort_by: Optional[str] = None,
-                 ascending: bool = False,
+                 ascending: bool = False, 
+                 node_list: Optional[List] = None,
                  ax: Optional[Axes] = None) -> Axes:
+    if node_list:
+        df = pd_df[(pd_df["source"].isin(node_list)) | (pd_df["target"].isin(node_list))]
+    else:
+        df = pd_df
+    validate_dataframe(df, cols=[source, target, weight], sort_by=sort_by)
 
-    _validate_panda(pd_df, cols=[source, target, weight], sort_by=sort_by)
-    
-    graph = Graph.from_pandas_edgelist(pd_df,
+    graph = Graph.from_pandas_edgelist(df,
                                        source=source,
                                        target=target,
                                        weight=weight)
-    return graph.plotX(title=title,
+    return graph.plot_network(title=title,
                        style=style,
                        ax=ax)
+
+def plot_network_components(pd_df: pd.DataFrame,
+                 source: str = "source",
+                 target: str = "target",
+                 weight: str = "weight",
+                 title: str = "Test",
+                 style: StyleTemplate = NETWORK_STYLE_TEMPLATE,
+                 sort_by: Optional[str] = None,
+                 node_list: Optional[List] = None,
+                 ascending: bool = False,
+                 ax: Optional[List[Axes]] = None) -> List[Axes]:
+    if node_list:
+        df = pd_df[(pd_df["source"].isin(node_list)) | (pd_df["target"].isin(node_list))]
+    else:
+        df = pd_df
+    validate_dataframe(df, cols=[source, target, weight], sort_by=sort_by)
+
+    graph = Graph.from_pandas_edgelist(df,
+                                       source=source,
+                                       target=target,
+                                       weight=weight)
+    connected_components = nx.connected_components(graph)
+    axes=[]
+    for connected_component in connected_components:
+        if len(connected_component) > 5:
+            connected_component_graph = graph.subgraph(node_list=connected_component)
+            ax=connected_component_graph.plot_network()
+            axes.append(ax)
+    return axes
+
```

### Comparing `matplotlibapi-3.1.0/MatplotLibAPI/Pivot.py` & `matplotlibapi-3.1.1/MatplotLibAPI/Pivot.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,45 +6,46 @@
 
 import matplotlib.dates as mdates
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
 from matplotlib.dates import DateFormatter, MonthLocator
 
 
-
-from .Style import DynamicFuncFormatter, StyleTemplate, generate_ticks, string_formatter, _validate_panda, percent_formatter,format_func
+from . import DynamicFuncFormatter, StyleTemplate, generate_ticks, string_formatter,  percent_formatter, format_func
+from .. import validate_dataframe
 
 PIVOTBARS_STYLE_TEMPLATE = StyleTemplate(
     background_color='black',
     fig_border='darkgrey',
     font_color='white',
     palette='magma',
-    format_funcs={"y": percent_formatter, 
+    format_funcs={"y": percent_formatter,
                   "label": string_formatter}
 )
 PIVOTLINES_STYLE_TEMPLATE = StyleTemplate(
     background_color='white',
     fig_border='lightgrey',
     palette='viridis',
     format_funcs={"y": percent_formatter, "label": string_formatter}
 )
 
+
 def plot_pivotbar(pd_df: pd.DataFrame,
                   label: str,
                   x: str,
                   y: str,
                   agg: str = "sum",
                   style: StyleTemplate = PIVOTBARS_STYLE_TEMPLATE,
                   title: Optional[str] = None,
                   sort_by: Optional[str] = None,
                   ascending: bool = False,
                   ax: Optional[Axes] = None):
 
-    _validate_panda(pd_df, cols=[label, x, y], sort_by=sort_by)
-    style.format_funcs=format_func(style.format_funcs,label=label,x=x,y=y)
+    validate_dataframe(pd_df, cols=[label, x, y], sort_by=sort_by)
+    style.format_funcs = format_func(style.format_funcs, label=label, x=x, y=y)
     pivot_df = pd.pivot_table(pd_df, values=y, index=[
                               x], columns=[label], aggfunc=agg)
     # Reset index to make x a column again
     pivot_df = pivot_df.reset_index()
 
     if not ax:
         ax = plt.gca()
```

### Comparing `matplotlibapi-3.1.0/MatplotLibAPI/Table.py` & `matplotlibapi-3.1.1/MatplotLibAPI/Table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import List, Optional
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
-from .Style import StyleTemplate, _validate_panda, string_formatter
+
+from . import StyleTemplate,  string_formatter
+from .. import validate_dataframe
 
 TABLE_STYLE_TEMPLATE = StyleTemplate(
     background_color='black',
     fig_border='darkgrey',
     font_color='white',
     palette='magma'
 )
@@ -17,15 +19,15 @@
                title: Optional[str] = None,
                style: StyleTemplate = TABLE_STYLE_TEMPLATE,
                max_values: int = 20,
                sort_by: Optional[str] = None,
                ascending: bool = False,
                ax: Optional[Axes] = None
                ) -> Axes:
-    _validate_panda(pd_df, cols=cols, sort_by=sort_by)
+    validate_dataframe(pd_df, cols=cols, sort_by=sort_by)
     
     if not sort_by:
         sort_by = cols[0]
 
     plot_df = pd_df[cols].sort_values(
         by=sort_by, ascending=ascending).head(max_values)
```

### Comparing `matplotlibapi-3.1.0/MatplotLibAPI/Timeserie.py` & `matplotlibapi-3.1.1/MatplotLibAPI/Timeserie.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Hint for Visual Code Python Interactive window
 # %%
+from typing import Optional
 import pandas as pd
-
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
 import seaborn as sns
-from .Style import DynamicFuncFormatter, StyleTemplate, string_formatter, _validate_panda, bmk_formatter, format_func
-from typing import Optional
+
+from . import DynamicFuncFormatter, StyleTemplate, string_formatter, bmk_formatter, format_func
+from .. import validate_dataframe
+
 
 TIMESERIE_STYLE_TEMPLATE = StyleTemplate(
     palette='rocket',
     format_funcs={"y": bmk_formatter, "label": string_formatter}
 )
 
 # region Line
@@ -22,15 +24,15 @@
                    title: Optional[str] = None,
                    style: StyleTemplate = TIMESERIE_STYLE_TEMPLATE,
                    max_values: int = 100,
                    sort_by: Optional[str] = None,
                    ascending: bool = False,
                    ax: Optional[Axes] = None) -> Axes:
 
-    _validate_panda(pd_df, cols=[label, x, y], sort_by=sort_by)
+    validate_dataframe(pd_df, cols=[label, x, y], sort_by=sort_by)
     style.format_funcs = format_func(style.format_funcs, label=label, x=x, y=y)
 
     df = pd_df[[label, x, y]].sort_values(by=[label, x])
     df[x] = pd.to_datetime(df[x])
     df.set_index(x, inplace=True)
 
     sns.set_palette(style.palette)
```

