# Comparing `tmp/LearningNashQLearning-0.4.tar.gz` & `tmp/LearningNashQLearning-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LearningNashQLearning-0.4.tar", last modified: Fri May 31 11:51:11 2024, max compression
+gzip compressed data, was "LearningNashQLearning-0.5.tar", last modified: Mon Jun  3 09:23:48 2024, max compression
```

## Comparing `LearningNashQLearning-0.4.tar` & `LearningNashQLearning-0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 11:51:11.663005 LearningNashQLearning-0.4/
-drwxrwxrwx   0        0        0        0 2024-05-31 11:51:11.527145 LearningNashQLearning-0.4/LearningNashQLearning/
-drwxrwxrwx   0        0        0        0 2024-05-31 11:51:11.597004 LearningNashQLearning-0.4/LearningNashQLearning/Model/
--rw-rw-rw-   0        0        0      888 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/Model/Agent.py
--rw-rw-rw-   0        0        0    11859 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/Model/Environment.py
--rw-rw-rw-   0        0        0     1232 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/Model/History.py
--rw-rw-rw-   0        0        0    26997 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/Model/NashQLearning.py
--rw-rw-rw-   0        0        0        0 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/Model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 11:51:11.663005 LearningNashQLearning-0.4/LearningNashQLearning/View/
--rw-rw-rw-   0        0        0     3964 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/View/EnvGraphDisplay.py
--rw-rw-rw-   0        0        0    18664 2024-05-31 11:50:27.000000 LearningNashQLearning-0.4/LearningNashQLearning/View/FinalDisplay.py
--rw-rw-rw-   0        0        0    14709 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/View/GameEditor.py
--rw-rw-rw-   0        0        0     3437 2024-05-31 11:50:16.000000 LearningNashQLearning-0.4/LearningNashQLearning/View/GraphClass.py
--rw-rw-rw-   0        0        0    11881 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/View/PresetGames.py
--rw-rw-rw-   0        0        0        0 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/View/__init__.py
--rw-rw-rw-   0        0        0       43 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/LearningNashQLearning/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 11:51:11.578997 LearningNashQLearning-0.4/LearningNashQLearning.egg-info/
--rw-rw-rw-   0        0        0      423 2024-05-31 11:51:11.000000 LearningNashQLearning-0.4/LearningNashQLearning.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      747 2024-05-31 11:51:11.000000 LearningNashQLearning-0.4/LearningNashQLearning.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 11:51:11.000000 LearningNashQLearning-0.4/LearningNashQLearning.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-31 11:51:11.000000 LearningNashQLearning-0.4/LearningNashQLearning.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-31 11:51:11.000000 LearningNashQLearning-0.4/LearningNashQLearning.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      423 2024-05-31 11:51:11.663005 LearningNashQLearning-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       23 2024-05-30 08:19:52.000000 LearningNashQLearning-0.4/README.md
--rw-rw-rw-   0        0        0      698 2024-05-31 11:50:37.000000 LearningNashQLearning-0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-31 11:51:11.663005 LearningNashQLearning-0.4/setup.cfg
--rw-rw-rw-   0        0        0      380 2024-05-31 11:50:55.000000 LearningNashQLearning-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:23:48.805022 LearningNashQLearning-0.5/
+drwxrwxrwx   0        0        0        0 2024-06-03 09:23:48.764031 LearningNashQLearning-0.5/LearningNashQLearning/
+drwxrwxrwx   0        0        0        0 2024-06-03 09:23:48.797516 LearningNashQLearning-0.5/LearningNashQLearning/Model/
+-rw-rw-rw-   0        0        0      888 2024-05-30 08:19:52.000000 LearningNashQLearning-0.5/LearningNashQLearning/Model/Agent.py
+-rw-rw-rw-   0        0        0    11859 2024-05-30 08:19:52.000000 LearningNashQLearning-0.5/LearningNashQLearning/Model/Environment.py
+-rw-rw-rw-   0        0        0     1232 2024-05-30 08:19:52.000000 LearningNashQLearning-0.5/LearningNashQLearning/Model/History.py
+-rw-rw-rw-   0        0        0    26997 2024-05-30 08:19:52.000000 LearningNashQLearning-0.5/LearningNashQLearning/Model/NashQLearning.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 08:19:52.000000 LearningNashQLearning-0.5/LearningNashQLearning/Model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:23:48.803517 LearningNashQLearning-0.5/LearningNashQLearning/View/
+-rw-rw-rw-   0        0        0     4006 2024-06-03 09:10:17.000000 LearningNashQLearning-0.5/LearningNashQLearning/View/EnvGraphDisplay.py
+-rw-rw-rw-   0        0        0    18699 2024-06-03 09:21:28.000000 LearningNashQLearning-0.5/LearningNashQLearning/View/FinalDisplay.py
+-rw-rw-rw-   0        0        0    14709 2024-05-30 08:19:52.000000 LearningNashQLearning-0.5/LearningNashQLearning/View/GameEditor.py
+-rw-rw-rw-   0        0        0     3518 2024-06-03 09:21:32.000000 LearningNashQLearning-0.5/LearningNashQLearning/View/GraphClass.py
+-rw-rw-rw-   0        0        0    11881 2024-05-30 08:19:52.000000 LearningNashQLearning-0.5/LearningNashQLearning/View/PresetGames.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 08:19:52.000000 LearningNashQLearning-0.5/LearningNashQLearning/View/__init__.py
+-rw-rw-rw-   0        0        0       43 2024-05-30 08:19:52.000000 LearningNashQLearning-0.5/LearningNashQLearning/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:23:48.788074 LearningNashQLearning-0.5/LearningNashQLearning.egg-info/
+-rw-rw-rw-   0        0        0      423 2024-06-03 09:23:48.000000 LearningNashQLearning-0.5/LearningNashQLearning.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      747 2024-06-03 09:23:48.000000 LearningNashQLearning-0.5/LearningNashQLearning.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 09:23:48.000000 LearningNashQLearning-0.5/LearningNashQLearning.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-06-03 09:23:48.000000 LearningNashQLearning-0.5/LearningNashQLearning.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-06-03 09:23:48.000000 LearningNashQLearning-0.5/LearningNashQLearning.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      423 2024-06-03 09:23:48.805022 LearningNashQLearning-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2024-05-30 08:19:52.000000 LearningNashQLearning-0.5/README.md
+-rw-rw-rw-   0        0        0      698 2024-06-03 09:23:41.000000 LearningNashQLearning-0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 09:23:48.805022 LearningNashQLearning-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      380 2024-06-03 09:23:29.000000 LearningNashQLearning-0.5/setup.py
```

### Comparing `LearningNashQLearning-0.4/LearningNashQLearning/Model/Agent.py` & `LearningNashQLearning-0.5/LearningNashQLearning/Model/Agent.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.4/LearningNashQLearning/Model/Environment.py` & `LearningNashQLearning-0.5/LearningNashQLearning/Model/Environment.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.4/LearningNashQLearning/Model/History.py` & `LearningNashQLearning-0.5/LearningNashQLearning/Model/History.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.4/LearningNashQLearning/Model/NashQLearning.py` & `LearningNashQLearning-0.5/LearningNashQLearning/Model/NashQLearning.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.4/LearningNashQLearning/View/EnvGraphDisplay.py` & `LearningNashQLearning-0.5/LearningNashQLearning/View/EnvGraphDisplay.py`

 * *Files 16% similar despite different names*

```diff
@@ -50,21 +50,22 @@
             description='Labels:',
             disabled=False,
         )
 
         self.labelOptionsDropdown.observe(
             lambda x: self.updateEnv(self.env), names='value')
 
-        self.out = widgets.Output()
-        self.box = widgets.VBox([self.labelOptionsDropdown, self.out])
+        with plt.ioff():
+            self.fig, self.ax = plt.subplots(figsize=(6, 6))
+            self.fig.canvas.layout.min_height = '400px'
+            self.fig.tight_layout()
+            self.ax.set_aspect('equal')
+            self.ax.axis('off')
 
-        with self.out:
-            fig, self.ax = plt.subplots()
-            self.ax.get_xaxis().set_visible(False)
-            self.ax.get_yaxis().set_visible(False)
+        self.box = widgets.VBox([self.labelOptionsDropdown, self.fig.canvas])
 
         self.updateEnv(env)
         self.update_graph()
 
     def resetTimer(self):
         self.timer = self.timeBuffer
 
@@ -106,12 +107,11 @@
             sleep(2)
             self.__execute_tasks()
 
     def update_graph(self):
         self.graph = GraphClass()
         self.graph.create_graph(self.env)
         self.labelOptions[self.labelOptionsDropdown.value]()
-        self.ax.cla()
-        self.graph.plotGraph(self.ax)
+        self.graph.plotGraph(self.ax, self.fig)
 
     def get_widget(self):
         return self.box
```

### Comparing `LearningNashQLearning-0.4/LearningNashQLearning/View/FinalDisplay.py` & `LearningNashQLearning-0.5/LearningNashQLearning/View/FinalDisplay.py`

 * *Files 7% similar despite different names*

```diff
@@ -146,41 +146,40 @@
 
         self.targetPlayerOptions.observe(
             lambda x: self.__updateLabelsAndPlot(), names='value')
 
         self.graphSettings = widgets.HBox(
             [self.targetPlayerOptions, self.graphLabelsOptions])
 
-        # Create the VBox containing all the widgets
-        self.box = widgets.VBox(
-            [self.title, self.subTitle1,  self.window_slider, self.plotOut, self.sliderBox, self.graphSettings, self.graphOut, self.currentGame, self.actionProfileBox, self.payoffBox, self.currentPolicyBox, self.qTableBox])
-
         self.graph = GraphClass()
         self.graph.create_graph(env)
         self.graph.current_state_set(0)
 
         # create figure and axes
-        with self.graphOut:
+        with plt.ioff():
             self.graphFig, self.graphAx = plt.subplots(figsize=(8, 8))
             self.graphFig.canvas.header_visible = False
             self.graphAx.set_title('')
             self.graphAx.get_xaxis().set_visible(False)
             self.graphAx.get_yaxis().set_visible(False)
-            self.graph.plotGraph(self.graphAx)
-            plt.tight_layout()
-            plt.show()
+            self.graph.plotGraph(self.graphAx, self.graphFig)
+            # plt.tight_layout()
 
-        with self.plotOut:
+        with plt.ioff():
             sns.set_theme()
             self.plotFig, self.plotAx = plt.subplots(figsize=(6, 3))
             self.plotFig.canvas.header_visible = False
             self.plotAx.set_title('Rewards during the training episodes')
             self.plotAx.set_xlim(0, 1000)
-            plt.tight_layout()
-            plt.show()
+            # plt.tight_layout()
+            # plt.show()
+
+        # Create the VBox containing all the widgets
+        self.box = widgets.VBox(
+            [self.title, self.subTitle1,  self.window_slider, self.plotFig.canvas, self.sliderBox, self.graphSettings, self.graphFig.canvas, self.currentGame, self.actionProfileBox, self.payoffBox, self.currentPolicyBox, self.qTableBox])
 
         nashQ.attach(self)
 
     def next(self):
         self.slider.set_trait(name='value', value=self.slider.value + 1)
 
     def update(self, gamesHistory: History, rewards):
@@ -306,14 +305,16 @@
         self.plotAx.set_ylabel('Reward')
         self.plotAx.legend()
 
         # plot the vertical line
         self.line = self.plotAx.axvline(
             x=self.gameNum, color='r', linestyle='--', label='Current Game')
 
+        self.plotAx.figure.canvas.draw()
+
     def __smooth_rewards(self, rewards, window=100):
         if window == 0:
             return rewards, np.sum(rewards, axis=0)
 
         rewardsPlayersSmooth = []
         for i in range(rewards.shape[0]):
             cumsum = np.cumsum(rewards[i, :])
@@ -326,23 +327,22 @@
 
             rewardsPlayersSmooth.append(cumsum)
 
         rewardsPlayersSmooth = np.array(rewardsPlayersSmooth)
         return rewardsPlayersSmooth, np.sum(rewardsPlayersSmooth, axis=0)
 
     def __plot_graph(self):
-        self.graphAx.clear()
         current_state = self.history.get(self.gameNum).get('current_state')
         self.graph.current_state_set(current_state)
 
         if self.gameNum < len(self.history.getHistory()) - 1:
             next_state = self.history.get(self.gameNum+1).get('current_state')
             self.graph.setCurrentActionProfile(current_state, next_state)
 
-        self.graph.plotGraph(self.graphAx)
+        self.graph.plotGraph(self.graphAx, self.graphFig)
 
     def __getQTables(self):
         qTables = []
         for i in range(self.env.NPlayers):
             qTables.append(self.history.get(self.gameNum).get('Q' + str(i)))
         return qTables
```

### Comparing `LearningNashQLearning-0.4/LearningNashQLearning/View/GameEditor.py` & `LearningNashQLearning-0.5/LearningNashQLearning/View/GameEditor.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.4/LearningNashQLearning/View/GraphClass.py` & `LearningNashQLearning-0.5/LearningNashQLearning/View/GraphClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,21 @@
             self.node_colors.update({node: 'blue'})
 
         for edge in list(self.graph.edges):
             self.edge_colors.update({edge: 'black'})
 
         return self
 
-    def plotGraph(self, ax: plt.Axes):
-        ax.cla()
+    def plotGraph(self, ax: plt.Axes, fig: plt.Figure):
+        ax.clear()
         self.updateLabelsFromActionLabels()
         Graph(self.graph, node_labels=True, node_layout='circular', edge_labels=self.edge_labels, edge_label_fontdict=dict(size=8), edge_layout='arc', node_size=10,
               edge_width=0.5, arrows=True, ax=ax, node_edge_color=self.node_colors, node_label_fontdict=dict(size=10), edge_label_position=0.3, edge_labels_rotate=False, edge_color=self.edge_colors)
+        fig.canvas.draw()
+        fig.canvas.flush_events()
 
     def current_state_set(self, state):
         for node in list(self.graph.nodes):
             if node == state:
                 self.node_colors.update({node: 'red'})
             else:
                 self.node_colors.update({node: 'blue'})
```

### Comparing `LearningNashQLearning-0.4/LearningNashQLearning/View/PresetGames.py` & `LearningNashQLearning-0.5/LearningNashQLearning/View/PresetGames.py`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.4/LearningNashQLearning.egg-info/SOURCES.txt` & `LearningNashQLearning-0.5/LearningNashQLearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LearningNashQLearning-0.4/pyproject.toml` & `LearningNashQLearning-0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LearningNashQLearning"
-version = "0.4"
+version = "0.5"
 description = "A simple NashQ-learning implementation in Python"
 readme = "README.md"
 authors = [{ name = "Paolo Ginefra" }, { name = "Federico Rocca"}, { name = "Andrea Tarabotto" }]
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

