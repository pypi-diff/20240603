# Comparing `tmp/chasta-0.1.4.tar.gz` & `tmp/chasta-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chasta-0.1.4.tar", max compression
+gzip compressed data, was "chasta-0.1.5.tar", max compression
```

## Comparing `chasta-0.1.4.tar` & `chasta-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      663 2024-03-10 22:17:25.729493 chasta-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-07-16 02:58:42.192702 chasta-0.1.4/chasta/__init__.py
--rw-r--r--   0        0        0     7554 2024-06-03 01:46:47.690911 chasta-0.1.4/chasta/chasta.py
--rw-r--r--   0        0        0      447 2024-06-03 02:31:27.705292 chasta-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 chasta-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      663 2024-03-10 22:17:25.729493 chasta-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-07-16 02:58:42.192702 chasta-0.1.5/chasta/__init__.py
+-rw-r--r--   0        0        0     7849 2024-06-03 03:10:36.035522 chasta-0.1.5/chasta/chasta.py
+-rw-r--r--   0        0        0      447 2024-06-03 03:14:18.995544 chasta-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 chasta-0.1.5/PKG-INFO
```

### Comparing `chasta-0.1.4/README.md` & `chasta-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `chasta-0.1.4/chasta/chasta.py` & `chasta-0.1.5/chasta/chasta.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,28 +116,29 @@
         col_decimals = determine_decimals(stats[column])
         if col_decimals > decimals:
             decimals = col_decimals
     formatted_stats = stats.applymap(lambda x: f"{x:,.{decimals}f}")
 
     return formatted_stats
 
-def get_stats_from_df(df_to_stats: pd.DataFrame, do_instance_count: bool) -> Union[Series, DataFrame]:
+def get_stats_from_df(df_to_stats: pd.DataFrame, do_instance_count: bool, smart_stat_formatting:bool) -> Union[Series, DataFrame]:
     if do_instance_count:
         stats = df_to_stats.value_counts()
     else:
         stats = df_to_stats.describe(percentiles=[.25, .50, .75, .90, .95, .99, .999], include='all')
         if '50%' in stats.index:
             stats.loc['median'] = stats.loc['50%']
-            stats = format_stats(stats)
+            if smart_stat_formatting:
+                stats = format_stats(stats)
 
     return stats
 
 
 def analyze_file(file_path: str, do_instance_count: bool = False, chart: Union[None, str] = None, delimiter: str = ',',
-                 columns_str: str = '0') -> Tuple[Union[None, pd.DataFrame], Union[pd.DataFrame, pd.Series, None]]:
+                 columns_str: str = '0',smart_stat_formatting:bool=False) -> Tuple[Union[None, pd.DataFrame], Union[pd.DataFrame, pd.Series, None]]:
     try:
         delimiter = guess_delimiter(file_path, delimiter)
         col_names, has_header = determine_col_names(file_path, delimiter)
         if has_header:
             df = pd.read_csv(file_path, sep=delimiter, names=col_names, skiprows=1)
         else:
             df = pd.read_csv(file_path, sep=delimiter, header=None)
@@ -147,15 +148,15 @@
         return None, None
 
     if Debug:
         print(df)
 
     selected_column_names = get_column_names(columns_str, col_names)
     df_to_stats, df_to_chart = get_stats_and_chart_dfs(df, chart, selected_column_names)
-    stats = get_stats_from_df(df_to_stats, do_instance_count)
+    stats = get_stats_from_df(df_to_stats, do_instance_count, smart_stat_formatting)
 
     return stats, df_to_chart
 
 
 def print_stats(stats: Union[None, pd.DataFrame, pd.Series]) -> None:
     if stats is not None:
         if isinstance(stats, pd.DataFrame):
@@ -196,14 +197,15 @@
     parser = argparse.ArgumentParser(description="Analyze a CSV file")
     parser.add_argument("-d", "--delimiter", type=str, default=DEFAULT_DELIMITER,
                         help=f"column delimiter (default: {DEFAULT_DELIMITER})")
     parser.add_argument("-c", "--columns", type=str, default="0",
                         help="CSV list of column number(s) or name(s) to analyze (default: 0)")
     parser.add_argument("-C", "--chart", nargs='?', const='', default=None,
                         help="Chart column(s) optionally specifying the column number/name for the x-axis")
+    parser.add_argument("-F", "--no_smart_stat_formatting", action='store_true', help="Don't try to format the stats decimal places")
     parser.add_argument("-i", "--instance_count", action='store_true', help="Instance count")
     parser.add_argument("-n", "--num_only", action='store_true', help="Only consider numeric values")
     #    parser.add_argument("-u", "--use_header", action='store_true', help="Use provided headers")
 
     parser.add_argument("file", type=str, nargs='?', help="path to the CSV file or none for STDIN")
 
     return parser.parse_args()
@@ -212,15 +214,15 @@
 def main():
     args = parse_args()
     if args.file:
         file_path = args.file
     else:
         file_path = create_tmp_file_with_stdin()
 
-    stats_obj, chart_df = analyze_file(file_path, args.instance_count, args.chart, args.delimiter, args.columns)
+    stats_obj, chart_df = analyze_file(file_path, args.instance_count, args.chart, args.delimiter, args.columns, not args.no_smart_stat_formatting)
 
     print_stats(stats_obj)
 
     if args.chart is not None:
         chart(chart_df, args.chart)
 
     if file_path != args.file:
```

### Comparing `chasta-0.1.4/PKG-INFO` & `chasta-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chasta
-Version: 0.1.4
+Version: 0.1.5
 Summary: CHArt and run STAtitics on CSV data
 Author: Jerome Provensal
 Author-email: jeromegit@provensal.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

