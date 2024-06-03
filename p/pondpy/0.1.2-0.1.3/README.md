# Comparing `tmp/pondpy-0.1.2.tar.gz` & `tmp/pondpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pondpy-0.1.2.tar", max compression
+gzip compressed data, was "pondpy-0.1.3.tar", max compression
```

## Comparing `pondpy-0.1.2.tar` & `pondpy-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1092 2024-05-24 22:17:18.743268 pondpy-0.1.2/LICENSE
--rw-r--r--   0        0        0      466 2024-05-26 23:17:09.445725 pondpy-0.1.2/pondpy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 13:18:41.574068 pondpy-0.1.2/pondpy/analysis/__init__.py
--rw-r--r--   0        0        0    31007 2024-05-26 23:17:09.445725 pondpy-0.1.2/pondpy/analysis/fem_analysis.py
--rw-r--r--   0        0        0    19704 2024-05-29 20:50:24.129982 pondpy-0.1.2/pondpy/analysis/pond_analysis.py
--rw-r--r--   0        0        0        0 2024-05-26 23:17:09.445725 pondpy-0.1.2/pondpy/design/__init__.py
--rw-r--r--   0        0        0       70 2024-05-26 23:17:09.445725 pondpy-0.1.2/pondpy/design/steel_beam_design.py
--rw-r--r--   0        0        0       72 2024-05-26 23:17:09.445725 pondpy-0.1.2/pondpy/design/steel_joist_design.py
--rw-r--r--   0        0        0    11405 2024-05-29 20:55:57.137409 pondpy-0.1.2/pondpy/pondpy.py
--rw-r--r--   0        0        0      584 2024-05-29 20:57:47.729009 pondpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5529 2024-05-26 23:17:09.445725 pondpy-0.1.2/README.md
--rw-r--r--   0        0        0     6006 1970-01-01 00:00:00.000000 pondpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-05-24 22:17:18.743268 pondpy-0.1.3/LICENSE
+-rw-r--r--   0        0        0      486 2024-06-02 22:15:23.052548 pondpy-0.1.3/pondpy/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 02:08:16.340245 pondpy-0.1.3/pondpy/analysis/__init__.py
+-rw-r--r--   0        0        0    40510 2024-06-02 22:15:23.052548 pondpy-0.1.3/pondpy/analysis/fem_analysis.py
+-rw-r--r--   0        0        0    23988 2024-06-02 22:15:23.052548 pondpy-0.1.3/pondpy/analysis/pond_analysis.py
+-rw-r--r--   0        0        0        0 2024-05-31 18:00:29.269189 pondpy-0.1.3/pondpy/design/__init__.py
+-rw-r--r--   0        0        0       70 2024-05-31 18:00:29.270807 pondpy-0.1.3/pondpy/design/steel_beam_design.py
+-rw-r--r--   0        0        0       72 2024-05-31 18:00:29.271848 pondpy-0.1.3/pondpy/design/steel_joist_design.py
+-rw-r--r--   0        0        0    12571 2024-06-02 22:15:23.052548 pondpy-0.1.3/pondpy/pondpy.py
+-rw-r--r--   0        0        0      584 2024-06-03 04:42:04.942580 pondpy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6910 2024-06-03 04:41:39.659293 pondpy-0.1.3/README.md
+-rw-r--r--   0        0        0     7364 1970-01-01 00:00:00.000000 pondpy-0.1.3/PKG-INFO
```

### Comparing `pondpy-0.1.2/LICENSE` & `pondpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pondpy-0.1.2/pondpy/analysis/fem_analysis.py` & `pondpy-0.1.3/pondpy/analysis/fem_analysis.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,18 @@
+import joistpy
 import math
 import matplotlib.pyplot as plt
 import numpy as np
+import steelpy
+
+beam_section_types = ['AISC']
+joist_section_types = ['SJI']
+
+class AnalysisError(Exception):
+    pass
 
 class SteelBeamSize:
     '''
     A class representing a steel beam size.
 
     ...
 
@@ -30,14 +38,23 @@
         name : str
             name of the steel beam size
         properties : steelpy object
             steelpy object containing properties for the specified steel beam size
         section_type : str, optional
             string indicating the section type of the steel shape
         '''
+        if not isinstance(name, str):
+            raise TypeError('name must be a string.')
+        if not isinstance(properties, steelpy.steelpy.Section):
+            raise TypeError('properties must be a valid steelpy Section object.')
+        if not isinstance(e_mod, (int, float)):
+            raise TypeError('e_mod must be int or float.')
+        if not isinstance(section_type, str) or section_type not in beam_section_types:
+            raise TypeError(f'section_type must be a string. Options are: AISC.')
+        
         self.name = name
         self.properties = properties
         self.e_mod = e_mod
         self.section_type = section_type
 
     def __str__(self):
         '''
@@ -73,14 +90,23 @@
         name : str
             name of the steel joist size
         properties : joistpy object
             joistpy object containing properties for the specified steel joist size
         section_type : str, optional
             string indicating the section type of the steel shape
         '''
+        if not isinstance(name, str):
+            raise TypeError('name must be a string.')
+        if not isinstance(properties, joistpy.joistpy.Designation):
+            raise TypeError('properties must be a valid joistpy Designation object.')
+        if not isinstance(e_mod, (int, float)):
+            raise TypeError('e_mod must be int or float.')
+        if not isinstance(section_type, str) or section_type not in joist_section_types:
+            raise TypeError(f'section_type must be a string. Options are: SJI.')
+        
         self.name = name
         self.properties = properties
         self.e_mod = e_mod
         self.section_type = section_type
 
     def __str__(self):
         '''
@@ -120,14 +146,28 @@
         size : steel beam size object
             steel beam size object for the beam
         supports : list
             list of tuples indicating location and type of beam supports
         ploads : list, optional
             list of point load objects
         '''
+        if not isinstance(length, (int, float)):
+            raise TypeError('length must be int or float.')
+        if not isinstance(size, (SteelBeamSize, SteelJoistSize)):
+            raise TypeError('size must be a valid SteelBeamSize or SteelJoistSize object.')
+        if not isinstance(ploads, list):
+            raise TypeError('ploads must be a list of DistLoad objects or empty list.')
+        if not isinstance(dloads, list):
+            raise TypeError('dloads must be a list of PointLoad objects or empty list.')
+        if not isinstance(supports, list):
+            raise TypeError('supports must be a list of tuples of tuples indicating location and type of support.')
+        
+        if size.section_type == 'SJI' and size.properties.get_wl360(span=length/12) == 0.0:
+            raise ValueError(f'Joist span exceeds allowable span for {size.name}.')
+        
         self.length = length
         self.size = size
         self.ploads = ploads
         self.dloads = dloads
         self.supports = supports
 
         self.e_mod = size.e_mod
@@ -140,16 +180,20 @@
 
 class BeamModel:
     '''
     A class representing the analytical model of an idealized beam
 
     ...
 
-    Parameters
+    Attributes
     ----------
+    analysis_complete : bool
+        bool indicating whether the analysis has been performed and is complete
+    analysis_ready : bool
+        bool indicating whether the analysis has been initialized and is ready to be performed
     beam : beam object
         beam object to be analyzed
     dof_num : list
         list of lists representing the degrees of freedom for each node in the model
     elem_dload : list
         list of lists representing the distributed load acting on each element in the model
     elem_loads : list
@@ -214,24 +258,55 @@
 
         Parameters
         ----------
         beam : beam object
             beam object to be analyzed
         ini_analysis : bool, optional
             indicates whether or not to initialize analysis upon instantiation
-        max_node_spacing : float, optional
+        max_node_spacing : int or float, optional
             maximum node spacing along the length of the beam model
         '''
+        if not isinstance(beam, Beam):
+            raise TypeError('beam must be a valid Beam object.')
+        if not isinstance(ini_analysis, bool):
+            raise TypeError('ini_analysis must be either True or False')
+        if not isinstance(max_node_spacing, (int, float)):
+            raise TypeError('max_node_spacing must be int or float')
+
         self.beam = beam
+        self.ini_analysis = ini_analysis
         self.max_node_spacing = max_node_spacing
 
-        if ini_analysis:
+        if self.ini_analysis:
             self.initialize_analysis()
+            self.global_displacement = np.zeros((self.n_dof, 1))
+            self.global_stiffness_matrix = np.zeros((self.n_dof, self.n_dof))
             self.element_forces = np.zeros((len(self.elem_nodes), 6))
             self.support_reactions = np.zeros((len(self.model_nodes), 3))
+        else:
+            self.analysis_complete = False
+            self.analysis_ready = False
+            self.dof_num = []
+            self.elem_dload = []
+            self.elem_loads = []
+            self.elem_nodes = []
+            self.element_forces = np.empty([0, 0])
+            self.fef_load_vector = np.empty([0, 0])
+            self.global_displacement = np.empty([0, 0])
+            self.global_stiffness_matrix = np.empty([0, 0])
+            self.local_stiffness_matrices = []
+            self.model_nodes = []
+            self.n_dof = 0
+            self.nodal_load_vector = np.empty([0, 0])
+            self.node_elem_fef = []
+            self.node_pload = []
+            self.node_support = []
+            self.points_of_interest = []
+            self.support_nodes = []
+            self.support_reactions = np.empty([0, 0])
 
     def _assemble_global_stiffness(self):
         '''
         Assembles the global stiffness matrix for the model.
 
         Parameters
         ----------
@@ -246,15 +321,15 @@
         S = np.zeros((self.n_dof, self.n_dof))
 
         # Loop over all model elements
         for i_elem in range(len(self.elem_nodes)):
             # Get the local element stiffness matrix, K
             node_i = self.elem_nodes[i_elem][0]
             node_j = self.elem_nodes[i_elem][1]
-            L = self.model_nodes[node_i] - self.model_nodes[node_j]
+            L = self.model_nodes[node_j] - self.model_nodes[node_i]
             E = self.beam.e_mod
             A = self.beam.area
             I = self.beam.mom_inertia
 
             K = np.zeros((6, 6))
             K[0][0] = (E*A)/L
             K[0][3] = -K[1][1]
@@ -266,17 +341,16 @@
             K[2][4] = -K[1][2]
             K[2][5] = 0.5*K[2][2]
             K[3][3] = K[0][0]
             K[4][4] = K[1][1]
             K[4][5] = -K[1][2]
             K[5][5] = K[2][2]
 
-            for i_row in range(6):
-                for i_col in range(i_row+1, 6):
-                    K[i_col][i_row] = K[i_row][i_col]
+            # Fill in symmetric terms of K
+            K = K + K.T - np.diag(K.diagonal())
 
             local_stiffness_matrices.append(K)
 
             l_dof1 = -1
             #Fill in the upper triangle terms of [K] into [S]
             for i_node1 in range(2):
                 # Get end node number for element #i_elem
@@ -292,18 +366,16 @@
                             B_dof2 = i_dof1
                         for i_dof2 in range(B_dof2, 3):
                             l_dof2 += 1
                             G_dof2 = self.dof_num[node_num2][i_dof2]
                             if G_dof1 != 0 and G_dof2 != 0:
                                 S[G_dof1-1][G_dof2-1] += K[l_dof1][l_dof2]
 
-            # Fill in symmetric terms
-            for i_row in range(self.n_dof):
-                for i_col in range(i_row+1, self.n_dof):
-                    S[i_col][i_row] = S[i_row][i_col]
+        # Fill in symmetric terms of S
+        S = S + S.T - np.diag(S.diagonal())
 
         self.global_stiffness = S
         self.local_stiffness_matrices = local_stiffness_matrices
 
     def _create_model_nodes_and_elems(self):
         '''
         Defines the model nodes based on the points of interest
@@ -439,23 +511,23 @@
                 # Calculate fixed end forces if w1 <= w2
                 elif abs(w2) >= abs(w1):
                     v_react_i = (w1*L)/2 + (3*(w2-w1)*L)/20
                     v_react_j = (w1*L)/2 + (7*(w2-w1)*L)/20
                     m_react_i = (w1*L**2)/12 + ((w2-w1)*L**2)/30
                     m_react_j = -(w1*L**2)/12 - ((w2-w1)*L**2)/20
                 # Place the fixed end forces in the proper location
-                node_elem_fef[elem[0]][1] += v_react_i
-                node_elem_fef[elem[0]][2] += m_react_i
-                node_elem_fef[elem[1]][1] += v_react_j
-                node_elem_fef[elem[1]][2] += m_react_j
-
-                elem_loads[i_elem][1] += v_react_i
-                elem_loads[i_elem][2] += m_react_i
-                elem_loads[i_elem][4] += v_react_j
-                elem_loads[i_elem][5] += m_react_j
+                node_elem_fef[elem[0]][1] += -v_react_i
+                node_elem_fef[elem[0]][2] += -m_react_i
+                node_elem_fef[elem[1]][1] += -v_react_j
+                node_elem_fef[elem[1]][2] += -m_react_j
+
+                elem_loads[i_elem][1] += -v_react_i
+                elem_loads[i_elem][2] += -m_react_i
+                elem_loads[i_elem][4] += -v_react_j
+                elem_loads[i_elem][5] += -m_react_j
 
         self.node_elem_fef = node_elem_fef
         self.elem_loads = elem_loads
 
     def _get_points_of_interest(self):
         '''
         Defines points of interest along the length of the beam model,
@@ -558,14 +630,34 @@
                 if support[0] == node:
                     node_support[i_node] = support[1]
                     support_nodes.append(i_node)
 
         self.node_support = node_support
         self.support_nodes = support_nodes
 
+    
+    def _valid_add_type(self, add_type):
+        '''
+        Checks if the add_type parameter passed to the add_beam_dload or add_beam_pload methods if valid.
+
+        Parameters
+        ----------
+        add_type : str
+            indicates whether to add the dload to the existing loads or replace the existing loads
+
+        Returns
+        -------
+        bool : bool
+            bool indicating whether the add_type parameter is valid
+        '''
+        if not isinstance(add_type, str) or add_type not in ['add', 'replace']:
+            return False
+        else:
+            return True
+
     def add_beam_dload(self, dload, add_type='add'):
         '''
         Adds a distributed load to the Beam object referenced by the BeamModel object.
 
         Parameters
         ----------
         add_type : str, optional
@@ -573,14 +665,19 @@
         dload : list
             list of dist load objects representing the distributed load(s) to be added to the beam referenced by the beam model
 
         Returns
         -------
         None
         '''
+        if not isinstance(dload, list) or not all(isinstance(item, DistLoad) for item in dload):
+            raise TypeError('dload must be list of valid DistLoad objects')
+        if not self._valid_add_type(add_type):
+            raise TypeError('add_type must be a string containing "add" or "replace"')
+
         # Add the distributed load
         if add_type == 'replace':
             self.beam.dloads = dload
         elif add_type == 'add':
             self.beam.dloads.extend(dload)
 
         # Re-initialize the analysis
@@ -597,14 +694,19 @@
         pload : list
             list of point load objects representing the point load(s) to be added to the beam referenced by the beam model
 
         Returns
         -------
         None
         '''
+        if not isinstance(pload, list) or not all(isinstance(item, PointLoad) for item in pload):
+            raise TypeError('pload must be list of valid PointLoad objects')
+        if not self._valid_add_type(add_type):
+            raise TypeError('add_type must be a string containing "add" or "replace"')
+        
         # Add the point load
         if add_type == 'replace':
             self.beam.ploads = pload
         elif add_type == 'add':
             self.beam.ploads.extend(pload)
 
         # Re-initialize the analysis
@@ -627,97 +729,107 @@
         self._set_support_nodes()
         self._set_pload_nodes()
         self._set_dload_elems()
         self._get_node_elem_fef()
         self._fill_global_dof()
         self._assemble_global_stiffness()
         self._get_load_vector()
+        self.analysis_complete = False
+        self.analysis_ready = True
 
     def perform_analysis(self):
         '''
         Computes the displacement vector, element force matrix, and support reaction vector.
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
         '''
-        # Calculate the global displacement vector
-        load_vector = self.nodal_load_vector - self.fef_load_vector
-        self.global_displacement = np.matmul(
-                np.linalg.inv(self.global_stiffness), load_vector
-                )
-
-        # Calculate element forces
-        elemxyM = np.zeros((len(self.elem_nodes), 6))
-
-        # Loop over all elements
-        for i_elem in range(len(self.elem_nodes)):
-            local_delta = np.zeros((6, 1))
-            local_Pf = np.zeros((6, 1))
-
-            # Get local element stiffness matrix
-            K = self.local_stiffness_matrices[i_elem]
-
-            l_dof = -1
-            # Extract local data first
-            for i_node in range(2):
-                # Get end node number for element # i_elem
-                node_num = self.elem_nodes[i_elem][i_node]
-                for i_dof in range(3):
-                    l_dof += 1
-                    # Extract local element loads
-                    local_Pf[l_dof] = self.elem_loads[i_elem][l_dof]
-
-                    # Extract local deformations
-                    G_dof = self.dof_num[node_num][i_dof]
-                    if G_dof != 0:
-                        local_delta[l_dof] = self.global_displacement[G_dof-1]
 
+        if not self.analysis_ready:
+            raise AnalysisError('Analysis must first be initialized by calling the initialize_analysis() method.')
+        elif self.analysis_ready:
+            # Calculate the global displacement vector
+            load_vector = self.nodal_load_vector - self.fef_load_vector
+            self.global_displacement = np.linalg.solve(
+                self.global_stiffness, load_vector
+            )
+            
             # Calculate element forces
-            local_element_forces = np.matmul(K, local_delta) + local_Pf
-
-            # Store element forces
-            elemxyM[i_elem] = local_element_forces.transpose()
-
-        # Calculate support reactions
-        support_reactions = np.zeros((len(self.model_nodes), 3))
-
-        # Loop over all elements
-        for i_elem in range(len(self.elem_nodes)):
-            l_dof = -1
-
-            # Loop over each node in the element
-            for i_node in range(2):
-                node_num = self.elem_nodes[i_elem][i_node]
-                # Loop over each dof
-                for i_dof in range(3):
-                    l_dof += 1
-                    if self.dof_num[node_num][i_dof] == 0:
-                        support_reactions[node_num][i_dof] += elemxyM[i_elem][l_dof]
-
-        self.element_forces = elemxyM
-        self.support_reactions = support_reactions
+            elemxyM = np.zeros((len(self.elem_nodes), 6))
+    
+            # Loop over all elements
+            for i_elem in range(len(self.elem_nodes)):
+                local_delta = np.zeros((6, 1))
+                local_Pf = np.zeros((6, 1))
+    
+                # Get local element stiffness matrix
+                K = self.local_stiffness_matrices[i_elem]
+    
+                l_dof = -1
+                # Extract local data first
+                for i_node in range(2):
+                    # Get end node number for element # i_elem
+                    node_num = self.elem_nodes[i_elem][i_node]
+                    for i_dof in range(3):
+                        l_dof += 1
+                        # Extract local element loads
+                        local_Pf[l_dof] = self.elem_loads[i_elem][l_dof]
+    
+                        # Extract local deformations
+                        G_dof = self.dof_num[node_num][i_dof]
+                        if G_dof != 0:
+                            local_delta[l_dof] = self.global_displacement[G_dof-1]
+    
+                # Calculate element forces
+                local_element_forces = np.matmul(K, local_delta) + local_Pf
+    
+                # Store element forces
+                elemxyM[i_elem] = local_element_forces.transpose()
+    
+            # Calculate support reactions
+            support_reactions = np.zeros((len(self.model_nodes), 3))
+    
+            # Loop over all elements
+            for i_elem in range(len(self.elem_nodes)):
+                l_dof = -1
+    
+                # Loop over each node in the element
+                for i_node in range(2):
+                    node_num = self.elem_nodes[i_elem][i_node]
+                    # Loop over each dof
+                    for i_dof in range(3):
+                        l_dof += 1
+                        if self.dof_num[node_num][i_dof] == 0:
+                            support_reactions[node_num][i_dof] += elemxyM[i_elem][l_dof]
+    
+            self.analysis_complete = True
+            self.element_forces = elemxyM
+            self.support_reactions = support_reactions
 
     def plot_bmd(self):
         '''
         Plots the bending moment diagram of the analyzed beam.
 
         Parameters
         ----------
         None
 
         Returns
         -------
-        plt : pyplot object
-            pyplot object representing the bending moment diagram for the analyzed model
+        fig : matplotlib.figure.Figure object
+            figure object representing the bending moment diagram for the analyzed model
         '''
+        if not self.analysis_complete:
+            raise AnalysisError('Analysis must be performed prior to generating plots.')
+
         left_moment = []
         right_moment = []
         for elem_f in self.element_forces:
             left_moment.append(elem_f[2]/12)
             right_moment.append(elem_f[5]/12)
         
         mom_count1 = 0
@@ -739,105 +851,107 @@
         lval_bmd = np.zeros(2*(len(self.model_nodes)))
         lval_bmd_count = 0
         for i_lval_bmd in range(len(self.model_nodes)):
             lval_bmd[i_lval_bmd+lval_bmd_count] = self.model_nodes[i_lval_bmd]/12
             lval_bmd[i_lval_bmd+lval_bmd_count+1] = self.model_nodes[i_lval_bmd]/12
             lval_bmd_count += 1
         
-        plt.figure()
-        plt.plot(lval_bmd.tolist(), bmd_val.tolist(),'b-')
+        fig, ax = plt.subplots()
+        ax.plot(lval_bmd.tolist(), bmd_val.tolist(), 'b-')
 
-        plt.xlabel('Length (ft)')
-        plt.ylabel(f'Bending Moment (k-ft)')
+        ax.set_xlabel('Length (ft)')
+        ax.set_ylabel('Bending Moment (k-ft)')
+        ax.grid()
 
-        plt.grid()
-
-        return plt
+        return fig
 
     def plot_deflected_shape(self, scale=1):
         '''
         Plots the deflected shape of the analyzed beam.
 
         Parameters
         ----------
         scale : int, optional
             scale to be applied to the deflected shape
 
         Returns
         -------
-        plt : pyplot object
-            pyplot object representing the deflected shape of the analyzed beam
+        fig : matplotlib.figure.Figure object
+            figure object representing the deflected shape of the analyzed beam
         '''
+        if not self.analysis_complete:
+            raise AnalysisError('Analysis must be performed prior to generating plots.')
+
         y_disp = []
         for i_node in range(len(self.model_nodes)):
             G_dof = self.dof_num[i_node][1]
             if G_dof != 0:
                 y_disp.append(self.global_displacement[G_dof-1][0]*scale)
             else:
                 y_disp.append(0.0)
         
-        plt.figure()
-        plt.plot([x/12 for x in self.model_nodes], y_disp, 'b-')
-
-        plt.xlabel('Length (ft)')
-        plt.ylabel(f'Deflection (in) - Scale={scale}:1')
+        fig, ax = plt.subplots()
+        ax.plot([x/12 for x in self.model_nodes], y_disp, 'b-')
 
-        plt.grid()
+        ax.set_xlabel('Length (ft)')
+        ax.set_ylabel(f'Deflection (in) - Scale={scale}:1')
+        ax.grid()
 
-        return plt
+        return fig
 
     def plot_sfd(self):
         '''
         Plots the shear force diagram of the analyzed beam.
 
         Parameters
         ----------
         None
 
         Returns
         -------
-        plt : pyplot object
-            pyplot object representing the shear force diagram for the analyzed model
+        fig : matplotlib.figure.Figure object
+            figure object representing the shear force diagram for the analyzed model
         '''
+        if not self.analysis_complete:
+            raise AnalysisError('Analysis must be performed prior to generating plots.')
+        
         left_shear = []
         right_shear = []
         for elem_f in self.element_forces:
             left_shear.append(elem_f[1])
             right_shear.append(elem_f[4])
 
         shear_count1 = 0
         shear_count2 = 0
 
         sfd_val = np.zeros(2*len(self.model_nodes))
         for i_sfd in range(1, len(self.model_nodes)):
             if i_sfd < 2*len(self.model_nodes)-1:
-                #print(shear_count1, shear_count2)
-                sfd_val[i_sfd+shear_count2] = -left_shear[shear_count1]
-                sfd_val[i_sfd+shear_count2+1] = right_shear[shear_count1]
+                sfd_val[i_sfd+shear_count2] = left_shear[shear_count1]
+                sfd_val[i_sfd+shear_count2+1] = -right_shear[shear_count1]
                 shear_count1 += 1
                 shear_count2 += 1
             elif i_sfd == 2*len(self.model_nodes)-1:
                 sfd_val[i_sfd] = 0
 
         lval_sfd = np.zeros(2*(len(self.model_nodes)))
         lval_sfd_count = 0
         for i_lval_sfd in range(len(self.model_nodes)):
             lval_sfd[i_lval_sfd+lval_sfd_count] = self.model_nodes[i_lval_sfd]/12
             lval_sfd[i_lval_sfd+lval_sfd_count+1] = self.model_nodes[i_lval_sfd]/12
             lval_sfd_count += 1
+        
+        fig, ax = plt.subplots()
+        ax.plot(lval_sfd.tolist(), sfd_val.tolist(), 'b-')
 
-        plt.figure()
-        plt.plot(lval_sfd.tolist(), sfd_val.tolist(), 'b-')
-
-        plt.xlabel('Length (ft)')
-        plt.ylabel(f'Shear Force (k)')
-
-        plt.grid()
+        ax.set_xlabel('Length (ft)')
+        ax.set_ylabel('Shear Force (k)')
+        ax.grid()
 
-        return plt
+        return fig
 
 class DistLoad:
     '''
     A class representing a distributed load.
 
     Attributes
     ----------
@@ -853,35 +967,138 @@
         Parameters
         ----------
         location : tuple
             tuple representing the start and end locations of the distributed load along the beam
         magntidue : tuple
             tuple of tuples representing the magnitude of the distributed load at its start and end locations
         '''
+        if not self._valid_dload_location(location):
+            raise TypeError('location must be a tuple of length 2 containing int or float.')
+        if not self._valid_dload_magnitude(magnitude):
+            raise TypeError('magnitude must be a tuple of 3 tuples each with length 2 containing int or float.')
+        
         self.location = location
         self.magnitude = magnitude
+        
+    def _valid_dload_location(self, location):
+        '''
+        Checks that the location parameter passed to the __init__ method is valid.
+        
+        Parameters
+        __________
+        location : tuple
+            tuple representing the start and end locations of the distributed load along the beam
+            
+        Returns
+        -------
+        bool : bool
+            bool indicating whether the location is valid input
+        '''
+        if not isinstance(location, tuple):
+            return False
+        elif len(location) != 2:
+            return False
+        elif not all(isinstance(item, (int, float)) for item in location):
+            return False
+        else:
+            return True
+    
+    def _valid_dload_magnitude(self, magnitude):
+        '''
+        Checks that the magnitude parameter passed to the __init__ method is valid.
+        
+        Parameters
+        __________
+        magntidue : tuple
+            tuple of tuples representing the magnitude of the distributed load at its start and end locations
+            
+        Returns
+        -------
+        bool : bool
+            bool indicating whether the magnitude is valid input
+        '''
+        if not isinstance(magnitude, tuple):
+            return False
+        elif len(magnitude) != 3:
+            return False
+        elif not all(isinstance(item, tuple) for item in magnitude):
+            return False
+        else:
+            for item in magnitude:
+                if len(item) != 2:
+                    return False
+                for mag in item:
+                    if not isinstance(mag, (int, float)):
+                        return False
+            return True
 
 class PointLoad:
     '''
     A class representing a concentrated load.
 
     Attributes
     ----------
-    location : tuple
-        tuple representing the locations of the concentrated load along the beam
+    location : int or float
+        int or float representing the location of the concentrated load along the beam
     magntidue : tuple
         tuple representing the magnitude of the concentrated load
     '''
     def __init__(self, location, magnitude):
         '''
         Constructs all the necessary attributes for the point load object.
 
         Parameters
             ----------
-        location : tuple
-            tuple representing the locations of the concentrated load along the beam
+        location : int or float
+            int or float representing the location of the concentrated load along the beam
         magntidue : tuple
             tuple representing the magnitude of the concentrated load
         '''
-    def __init__(self, location, magnitude):
+        if not self._valid_pload_location(location):
+            raise TypeError('location must be int or float.')
+        if not self._valid_pload_magnitude(magnitude):
+            raise TypeError('magnitude must be a tuple of length 3 containing int or float.')
+            
         self.location = location
         self.magnitude = magnitude
+        
+    def _valid_pload_location(self, location):
+        '''
+        Checks that the location parameter passed to the __init__ method is valid.
+        
+        Parameters
+        __________
+        location : int or float
+            int or float representing the location of the concentrated load along the beam
+            
+        Returns
+        -------
+        bool : bool
+            bool indicating whether the location is valid input
+        '''
+        if not isinstance(location, (int, float)):
+            return False
+        else:
+            return True
+    
+    def _valid_pload_magnitude(self, magnitude):
+        '''
+        Checks that the magnitude parameter passed to the __init__ method is valid.
+        
+        Parameters
+        __________
+        magntidue : tuple
+            tuple representing the magnitude of the concentrated load
+            
+        Returns
+        -------
+        bool : bool
+            bool indicating whether the magnitude is valid input
+        '''
+        if not isinstance(magnitude, tuple):
+            return False
+        elif len(magnitude) != 3:
+            return False
+        elif not all(isinstance(item, (int, float)) for item in magnitude):
+            return False
+        else:
+            return True
```

### Comparing `pondpy-0.1.2/pondpy/analysis/pond_analysis.py` & `pondpy-0.1.3/pondpy/analysis/pond_analysis.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .fem_analysis import (
+from pondpy import (
+    AnalysisError,
     Beam,
     BeamModel,
     DistLoad,
     PointLoad,
 )
 
 CONV_D_TO_Q = 62.4/(12**3)/1000 # Constant to convert water depth in inches to rain load in k/in^2
@@ -31,14 +32,21 @@
         dead_load : float
             magnitude of the dead load on the roof in k/in^2
         rain_load : float
             magnitude of the rain load on the roof in k/in^2
         include_sw : bool, optional
             indicates whether to conside member self-weight in the analysis
         '''
+        if not isinstance(dead_load, (int, float)):
+            raise TypeError('dead_load must be either int or float')
+        if not isinstance(rain_load, (int, float)):
+            raise TypeError('rain_load must be either int or float')
+        if not isinstance(include_sw, bool):
+            raise TypeError('include_sw must be either True or False')
+        
         self.dead_load = dead_load # Units: k/in^2
         self.rain_load = rain_load # Units: k/in^2
         self.include_sw = include_sw
 
 class PrimaryMember(Beam):
     '''
     A class representing a primary member in the roof bay.
@@ -74,14 +82,17 @@
         Constructs all the necessary attributes for the primary framing object.
 
         Parameters
         ----------
         primary_members : list
             list of all primary members in the primary framing system
         '''
+        if not isinstance(primary_members, list) or not all(isinstance(item, (PrimaryMember)) for item in primary_members):
+            raise TypeError('primary_members must be a list of valid PrimaryMember objects')
+        
         self.primary_members = primary_members
 
     def __str__(self):
         '''
         Prints the size of each primary framing member in the framing system.
         '''
         return f'Primary framing members: {[member.size.name for member in self.primary_members]}'
@@ -126,14 +137,25 @@
         mirrored_right : bool, optional
             indicates whether the roof bay is mirrored on the right
         primary_framing : primary framing
             primary framing object for the roof bay
         secondary_framing : secondary framing
             secondary framing object for the roof bay
         '''
+        if not isinstance(loading, Loading):
+            raise TypeError('loading must be a valid Loading object')
+        if not isinstance(primary_framing, PrimaryFraming):
+            raise TypeError('primary_framing must be a valid PrimaryFraming object')
+        if not isinstance(secondary_framing, SecondaryFraming):
+            raise TypeError('secondary_framing must be a valid SecondaryFraming object')
+        if not isinstance(mirrored_left, bool):
+            raise TypeError('mirrored_left must be either True or False')
+        if not isinstance(mirrored_right, bool):
+            raise TypeError('mirrored_right must be either True or False')
+
         self.primary_framing = primary_framing
         self.secondary_framing = secondary_framing
         self.loading = loading
         self.mirrored_left = mirrored_left
         self.mirrored_right = mirrored_right
 
         self._get_secondary_spacing()
@@ -242,14 +264,18 @@
     '''
     A class representing the roof bay model object.
 
     ...
 
     Attributes
     ----------
+    analysis_complete : bool
+        bool indicating whether the analysis has been successfully performed
+    analysis_ready : bool
+        bool indicating whether the analysis has been initialized and is ready to be performed
     initial_impounded_depth : dict
         dictionary containing initial impounded water depth in inches for each primary and secondary member
     max_node_spacing : int or float
         maximum node spacing along length of beam model objects in inches
     primary_models : list
         list of beam model objects for the primary framing members
     roof_bay : roof bay
@@ -257,29 +283,38 @@
     secondary_models : list
         list of beam model objects for the secondary framing members
 
     Methods
     -------
     analyze_roof_bay(rain_load):
         Analyzes the roof bay for the dead load and the input rain loads.
+    generate_plots():
+        Generates the deflected shape, shear force diagram, and bending moment diagram plots for each primary and secondary member.
     initialize_analysis():
         Prepares the model for analysis. To be called at instantiation and when the user specifies.
     '''
 
     def __init__(self, roof_bay, max_node_spacing = 6):
         '''
         Constructs all the necessary attributes for the roof bay object.
 
         Parameters
         ----------
-        max_node_spacing : int or float
+        max_node_spacing : int or float, optional
             maximum node spacing along length of beam model objects in inches
         roof_bay : roof bay
             roof bay object
         '''
+        if not isinstance(roof_bay, RoofBay):
+            raise TypeError('roof_bay must be a valid RoofBay object')
+        if not isinstance(max_node_spacing, (int, float)):
+            raise TypeError('max_node_spacing must be int or float')
+
+        self.analysis_complete = False
+        self.analysis_ready = False
         self.roof_bay = roof_bay
         self.max_node_spacing = max_node_spacing
 
         self.initialize_analysis()
 
     def _apply_primary_loads(self):
         '''
@@ -498,14 +533,73 @@
         # Apply the secondary member reactions as point loads to the primary members
         self._apply_primary_loads()
 
         # Perform the primary member analysis
         for p_model in self.primary_models:
             p_model.perform_analysis()
 
+        self.analysis_complete = True
+
+    def generate_plots(self):
+        '''
+        Generates the deflected shape, shear force diagram, and bending moment
+        diagram plots for each primary and secondary member.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        plots : dict
+            dictionary of dictionaries of lists containing the deflected shape,
+            shear force diagram, and bending moment diagram plots for each
+            primary and secondary member
+        '''
+        if not self.analysis_complete:
+            raise AnalysisError('Analysis must be performed prior to generating plots.')
+        
+        plots = {
+            'bmd':{
+                'Primary': [],
+                'Secondary': [],
+            },
+            'sfd':{
+                'Primary': [],
+                'Secondary': [],
+            },
+            'defl':{
+                'Primary': [],
+                'Secondary': [],
+            },
+        }
+
+        # First loop over the primary models
+        for p_model in self.primary_models:
+            cur_bmd = p_model.plot_bmd()
+            cur_sfd = p_model.plot_sfd()
+            cur_defl = p_model.plot_deflected_shape()
+
+            plots['bmd']['Primary'].append(cur_bmd)
+            plots['sfd']['Primary'].append(cur_sfd)
+            plots['defl']['Primary'].append(cur_defl)
+
+        # Next loop over the secondary models
+        for s_model in self.secondary_models:
+            cur_bmd = s_model.plot_bmd()
+            cur_sfd = s_model.plot_sfd()
+            cur_defl = s_model.plot_deflected_shape()
+
+            plots['bmd']['Secondary'].append(cur_bmd)
+            plots['sfd']['Secondary'].append(cur_sfd)
+            plots['defl']['Secondary'].append(cur_defl)
+
+        # Return the plots dict
+        return plots
+
     def initialize_analysis(self):
         '''
         Prepares the model for analysis. To be called at instantiation and 
         when the user specifies.
 
         Parameters
         ----------
@@ -515,14 +609,15 @@
         -------
         None
         '''
         self._create_primary_models()
         self._create_secondary_models()
         self.initial_impounded_depth = self._initial_impounded_water_depth()
         self.initial_secondary_rl = self._get_secondary_rl(impounded_depth=self.initial_impounded_depth)
+        self.analysis_ready = True
 
 class SecondaryMember(Beam):
     '''
     A class representing a secondary member in the roof bay.
 
     Attributes
     ----------
@@ -556,17 +651,22 @@
         '''
         Constructs all the necessary attributes for the secondary framing object.
 
         Parameters
         ----------
         secondary_members : list
             list of all primary members in the framing system
-        slope : float, optional
+        slope : int or float, optional
             slope of the roof bay in in/ft
         '''
+        if not isinstance(secondary_members, list) or not all(isinstance(item, SecondaryMember) for item in secondary_members):
+            raise TypeError('secondary_members must be a list of valid SecondaryFraming objects')
+        if not isinstance(slope, (int, float)):
+            raise TypeError('slope must be int or float')
+
         self.secondary_members = secondary_members
         self.slope = slope
 
     def __str__(self):
         '''
         Prints the size of each primary framing member in the framing system.
         '''
```

### Comparing `pondpy-0.1.2/pondpy/pondpy.py` & `pondpy-0.1.3/pondpy/pondpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from scipy import integrate
 import time
 
 from pondpy import (
+    Loading,
+    PrimaryFraming,
+    PrimaryMember,
     RoofBay,
     RoofBayModel,
+    SecondaryFraming,
+    SecondaryMember,
 )
 
 class PondPyModel:
     '''
     A class to represent a pondpy analysis object.
 
     ...
@@ -38,15 +43,15 @@
         criterion to stop the iterative analysis
 
     Methods
     -------
     perform_analysis():
         Performs the iterative analysis of the PondPy object.
     '''
-    def __init__(self, primary_framing, secondary_framing, loading, mirrored_left=False, mirrored_right=False, stop_criterion=0.0001, max_iter=50, show_results=True):
+    def __init__(self, primary_framing, secondary_framing, loading, mirrored_left=False, mirrored_right=False, stop_criterion=0.001, max_iter=50, show_results=True):
         '''
         Constructs the required input attributes for the PondPy object.
 
         Parameters
         ----------
         loading : loading
             Loading object representing the loading criteria for the roof bay
@@ -65,14 +70,31 @@
         secondary_framing : list
             list of SecondaryFraming objects representing the secondary framing for the roof bay
         show_results : bool, optional
             indicates whether or not to print the results to the console
         stop_criterion : float, optional
             criterion to stop the iterative analysis
         '''
+        if not isinstance(loading, Loading):
+            raise TypeError('loaidng must be a valid Loading object')
+        if not isinstance(max_iter, int) or max_iter <= 0:
+            raise TypeError('max_iter must be a positive integer')
+        if not isinstance(mirrored_left, bool):
+            raise TypeError('mirrored_left must be either True or False')
+        if not isinstance(mirrored_right, bool):
+            raise TypeError('mirrored_right must be either True or False')
+        if not isinstance(primary_framing, PrimaryFraming):
+            raise TypeError('primary_framing must be a valid PrimaryFraming object')
+        if not isinstance(secondary_framing, SecondaryFraming):
+            raise TypeError('secondary_framing must be a valid SecondaryFraming object')
+        if not isinstance(show_results, bool):
+            raise TypeError('show_results must be either True or False')
+        if not isinstance(stop_criterion, float) or stop_criterion <= 0:
+            raise TypeError('stop_criterion must be a positive float')
+
         self.loading = loading
         self.max_iter = max_iter
         self.mirrored_left = mirrored_left
         self.mirrored_right = mirrored_right
         self.primary_framing = primary_framing
         self.secondary_framing = secondary_framing
         self.show_results = show_results
```

### Comparing `pondpy-0.1.2/pyproject.toml` & `pondpy-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pondpy"
-version = "0.1.2"
+version = "0.1.3"
 description = "Package to aid in the design of low-slope roof systems for ponding stability and impounded rain load."
 authors = ["Matthew Upshaw <matthew.upshaw02@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 numpy = "1.26.4"
 scipy = "1.13.1"
-joistpy = "0.1.4"
+joistpy = "1.0.0"
 steelpy = "1.1.1"
 matplotlib = "3.9.0"
 
 [project.urls]
 "Homepage" = "https://github.com/matthew-upshaw/pondpy"
 
 [build-system]
```

### Comparing `pondpy-0.1.2/README.md` & `pondpy-0.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,346 +1,432 @@
-00000000: 2320 506f 6e64 5079 0d0a 506f 6e64 5079  # PondPy..PondPy
-00000010: 2069 7320 6120 7061 636b 6167 6520 6275   is a package bu
-00000020: 696c 7420 746f 2061 6964 2069 6e20 7468  ilt to aid in th
-00000030: 6520 6465 7369 676e 206f 6620 6c6f 772d  e design of low-
-00000040: 736c 6f70 6520 726f 6f66 2062 6179 7320  slope roof bays 
-00000050: 666f 7220 0d0a 706f 6e64 696e 6720 7374  for ..ponding st
-00000060: 6162 696c 6974 7920 616e 6420 696d 706f  ability and impo
-00000070: 756e 6465 6420 7261 696e 206c 6f61 6469  unded rain loadi
-00000080: 6e67 2e20 4974 2075 7469 6c69 7a65 7320  ng. It utilizes 
-00000090: 6120 7365 7269 6573 206f 660d 0a70 7572  a series of..pur
-000000a0: 706f 7365 2d62 7569 6c74 2066 696e 6974  pose-built finit
-000000b0: 6520 656c 656d 656e 7420 616e 6420 706f  e element and po
-000000c0: 6e64 696e 6720 616e 616c 7973 6973 2063  nding analysis c
-000000d0: 6c61 7373 6573 2061 6e64 206d 6574 686f  lasses and metho
-000000e0: 6473 2074 6f20 6265 0d0a 6173 2069 6e74  ds to be..as int
-000000f0: 7569 7469 7665 2061 7320 706f 7373 6962  uitive as possib
-00000100: 6c65 2066 6f72 2074 6865 206d 6f64 6572  le for the moder
-00000110: 6e20 656e 6769 6e65 6572 2e0d 0a0d 0a23  n engineer.....#
-00000120: 2323 2049 6e73 7461 6c6c 6174 696f 6e0d  ## Installation.
-00000130: 0a49 6e73 7461 6c6c 2070 6f6e 6470 7920  .Install pondpy 
-00000140: 7769 7468 2070 6970 3a0d 0a60 6060 6261  with pip:..```ba
-00000150: 7368 0d0a 7069 7020 696e 7374 616c 6c20  sh..pip install 
-00000160: 706f 6e64 7079 0d0a 6060 600d 0a0d 0a23  pondpy..```....#
-00000170: 2323 2055 7361 6765 0d0a 5468 6520 506f  ## Usage..The Po
-00000180: 6e64 5079 4d6f 6465 6c20 636c 6173 7320  ndPyModel class 
-00000190: 6973 2064 6573 6967 6e65 6420 746f 2077  is designed to w
-000001a0: 6f72 6b20 7769 7468 2073 6576 6572 616c  ork with several
-000001b0: 2070 7572 706f 7365 2d62 7569 6c74 2063   purpose-built c
-000001c0: 6c61 7373 6573 0d0a 7468 6174 2068 656c  lasses..that hel
-000001d0: 7020 7468 6520 7573 6572 206f 7267 616e  p the user organ
-000001e0: 697a 6520 7468 6569 7220 696e 7075 7420  ize their input 
-000001f0: 696e 746f 2061 2066 6f72 6d20 7468 6174  into a form that
-00000200: 2061 7265 2072 6561 6469 6c79 2075 7469   are readily uti
-00000210: 6c69 7a65 640d 0a74 6f20 6275 696c 6420  lized..to build 
-00000220: 616e 6420 616e 616c 797a 6520 7468 6520  and analyze the 
-00000230: 6d6f 6465 6c2e 2054 6865 7365 2061 7265  model. These are
-00000240: 2074 6865 2060 6060 5072 696d 6172 7946   the ```PrimaryF
-00000250: 7261 6d69 6e67 6060 602c 0d0a 6060 6053  raming```,..```S
-00000260: 6563 6f6e 6461 7279 4672 616d 696e 6760  econdaryFraming`
-00000270: 6060 2c20 616e 6420 6060 604c 6f61 6469  ``, and ```Loadi
-00000280: 6e67 6060 6020 636c 6173 7365 732e 2049  ng``` classes. I
-00000290: 6e20 6164 6469 7469 6f6e 2c20 7468 6520  n addition, the 
-000002a0: 7061 636b 6167 6520 6973 0d0a 6465 7369  package is..desi
-000002b0: 676e 6564 2074 6f20 776f 726b 2077 6974  gned to work wit
-000002c0: 6820 7468 6520 6060 6073 7465 656c 7079  h the ```steelpy
-000002d0: 6060 6020 616e 6420 6060 606a 6f69 7374  ``` and ```joist
-000002e0: 7079 6060 6020 7061 636b 6167 6573 2c20  py``` packages, 
-000002f0: 7468 6f75 6768 2061 6e79 0d0a 6f62 6a65  though any..obje
-00000300: 6374 2063 6f6e 7461 696e 696e 6720 7468  ct containing th
-00000310: 6520 7265 7175 6972 696e 6720 696e 666f  e requiring info
-00000320: 726d 6174 696f 6e20 6174 7472 6962 7572  rmation attribur
-00000330: 6573 2028 692e 652e 206d 6f6d 656e 7420  es (i.e. moment 
-00000340: 6f66 2069 6e65 7274 6961 2c0d 0a63 726f  of inertia,..cro
-00000350: 7373 2d73 6563 7469 6f6e 616c 2061 7265  ss-sectional are
-00000360: 612c 2065 6c61 7374 6963 206d 6f64 756c  a, elastic modul
-00000370: 7573 2c20 6574 632e 2920 636f 756c 6420  us, etc.) could 
-00000380: 6265 2075 7365 6420 696e 206c 6965 7520  be used in lieu 
-00000390: 6f66 2065 6974 6865 720d 0a70 6163 6b61  of either..packa
-000003a0: 6765 2e0d 0a0d 0a54 6f20 6372 6561 7465  ge.....To create
-000003b0: 2061 6e64 2061 6e61 6c79 7a65 2061 2072   and analyze a r
-000003c0: 6f6f 6620 6261 7920 6d6f 6465 6c2c 2066  oof bay model, f
-000003d0: 6972 7374 2069 6d70 6f72 7420 7468 6520  irst import the 
-000003e0: 7265 7175 6972 6564 2064 6570 656e 6465  required depende
-000003f0: 6e63 6965 730d 0a61 6e64 2063 6c61 7373  ncies..and class
-00000400: 6573 3a0d 0a60 6060 7079 7468 6f6e 0d0a  es:..```python..
-00000410: 6672 6f6d 206a 6f69 7374 7079 2069 6d70  from joistpy imp
-00000420: 6f72 7420 736a 690d 0a66 726f 6d20 7374  ort sji..from st
-00000430: 6565 6c70 7920 696d 706f 7274 2061 6973  eelpy import ais
-00000440: 630d 0a0d 0a66 726f 6d20 706f 6e64 7079  c....from pondpy
-00000450: 2e61 6e61 6c79 7369 732e 6665 6d5f 616e  .analysis.fem_an
-00000460: 616c 7973 6973 2069 6d70 6f72 7420 280d  alysis import (.
-00000470: 0a20 2020 2053 7465 656c 4265 616d 5369  .    SteelBeamSi
-00000480: 7a65 2c0d 0a20 2020 2053 7465 656c 4a6f  ze,..    SteelJo
-00000490: 6973 7453 697a 652c 0d0a 290d 0a0d 0a66  istSize,..)....f
-000004a0: 726f 6d20 706f 6e64 7079 2e61 6e61 6c79  rom pondpy.analy
-000004b0: 7369 732e 706f 6e64 5f61 6e61 6c79 7369  sis.pond_analysi
-000004c0: 7320 696d 706f 7274 2028 0d0a 2020 2020  s import (..    
-000004d0: 5072 696d 6172 794d 656d 6265 722c 0d0a  PrimaryMember,..
-000004e0: 2020 2020 5072 696d 6172 7946 7261 6d69      PrimaryFrami
-000004f0: 6e67 2c0d 0a20 2020 2053 6563 6f6e 6461  ng,..    Seconda
-00000500: 7279 4d65 6d62 6572 2c0d 0a20 2020 2053  ryMember,..    S
-00000510: 6563 6f6e 6461 7279 4672 616d 696e 672c  econdaryFraming,
-00000520: 0d0a 2020 2020 4c6f 6164 696e 670d 0a29  ..    Loading..)
-00000530: 0d0a 0d0a 6672 6f6d 2070 6f6e 6470 792e  ....from pondpy.
-00000540: 706f 6e64 7079 2069 6d70 6f72 7420 506f  pondpy import Po
-00000550: 6e64 5079 4d6f 6465 6c0d 0a60 6060 0d0a  ndPyModel..```..
-00000560: 0d0a 4e65 7874 2c20 6465 6669 6e65 2074  ..Next, define t
-00000570: 6865 2073 7465 656c 2073 6861 7065 7320  he steel shapes 
-00000580: 616e 6420 6a6f 6973 7420 6465 7369 676e  and joist design
-00000590: 6174 696f 6e73 2069 6e20 796f 7572 206d  ations in your m
-000005a0: 6f64 656c 2e0d 0a60 6060 7079 7468 6f6e  odel...```python
-000005b0: 0d0a 7731 3278 3136 203d 2053 7465 656c  ..w12x16 = Steel
-000005c0: 4265 616d 5369 7a65 2827 5731 3258 3136  BeamSize('W12X16
-000005d0: 272c 2061 6973 632e 575f 7368 6170 6573  ', aisc.W_shapes
-000005e0: 2e57 3132 5831 3629 0d0a 7731 3678 3236  .W12X16)..w16x26
-000005f0: 203d 2053 7465 656c 4265 616d 5369 7a65   = SteelBeamSize
-00000600: 2827 5731 3658 3236 272c 2061 6973 632e  ('W16X26', aisc.
-00000610: 575f 7368 6170 6573 2e57 3136 5832 3629  W_shapes.W16X26)
-00000620: 0d0a 6b5f 3134 6b31 203d 2053 7465 656c  ..k_14k1 = Steel
-00000630: 4a6f 6973 7453 697a 6528 2731 344b 3127  JoistSize('14K1'
-00000640: 2c20 736a 692e 4b5f 5365 7269 6573 2e4b  , sji.K_Series.K
-00000650: 5f31 344b 3129 0d0a 6060 600d 0a0d 0a4e  _14K1)..```....N
-00000660: 6578 742c 2064 6566 696e 6520 7468 6520  ext, define the 
-00000670: 7072 696d 6172 7920 616e 6420 7365 636f  primary and seco
-00000680: 6e64 6172 7920 6672 616d 696e 6720 696e  ndary framing in
-00000690: 2074 6865 2072 6f6f 6620 6261 7920 6672   the roof bay fr
-000006a0: 616d 696e 6720 7379 7374 656d 2e20 0d0a  aming system. ..
-000006b0: 4e6f 7465 2074 6861 7420 616c 6c20 696e  Note that all in
-000006c0: 7075 7473 2073 686f 756c 6420 6265 2069  puts should be i
-000006d0: 6e20 6b69 7073 2061 6e64 2069 6e63 6865  n kips and inche
-000006e0: 732e 0d0a 6060 6070 7974 686f 6e0d 0a70  s...```python..p
-000006f0: 5f6c 656e 6774 6820 3d20 3230 2a31 3220  _length = 20*12 
-00000700: 2320 6c65 6e67 7468 206f 6620 7072 696d  # length of prim
-00000710: 6172 7920 6d65 6d62 6572 7320 696e 2069  ary members in i
-00000720: 6e63 6865 730d 0a73 5f6c 656e 6774 6820  nches..s_length 
-00000730: 3d20 3230 2a31 3220 2320 6c65 6e67 7468  = 20*12 # length
-00000740: 206f 6620 7365 636f 6e64 6172 7920 6d65   of secondary me
-00000750: 6d62 6572 7320 696e 2069 6e63 6865 730d  mbers in inches.
-00000760: 0a0d 0a23 2053 7570 706f 7274 2074 7970  ...# Support typ
-00000770: 6573 2061 7265 2064 6573 6967 6e61 7465  es are designate
-00000780: 6420 6279 2074 7570 6c65 7320 7265 7072  d by tuples repr
-00000790: 6573 656e 7469 6e67 2028 5478 2c20 5479  esenting (Tx, Ty
-000007a0: 2c20 527a 292e 0d0a 2320 4120 3020 696e  , Rz)...# A 0 in
-000007b0: 6469 6361 7465 7320 7468 6520 6465 6772  dicates the degr
-000007c0: 6565 206f 6620 6672 6565 646f 6d20 6973  ee of freedom is
-000007d0: 2075 6e72 6573 7472 6169 6e65 6420 7768   unrestrained wh
-000007e0: 696c 6520 6120 3120 696e 6469 6361 7465  ile a 1 indicate
-000007f0: 7320 6120 0d0a 2320 7265 7374 7261 696e  s a ..# restrain
-00000800: 6564 2064 6567 7265 6520 6f66 2066 7265  ed degree of fre
-00000810: 6564 6f6d 2e0d 0a70 5f73 7570 706f 7274  edom...p_support
-00000820: 203d 205b 5b30 2c20 2831 2c20 312c 2030   = [[0, (1, 1, 0
-00000830: 295d 2c20 5b70 5f6c 656e 6774 682c 2028  )], [p_length, (
-00000840: 312c 2031 2c20 3029 5d5d 0d0a 735f 7375  1, 1, 0)]]..s_su
-00000850: 7070 6f72 7420 3d20 5b5b 302c 2028 312c  pport = [[0, (1,
-00000860: 2031 2c20 3029 5d2c 205b 735f 6c65 6e67   1, 0)], [s_leng
-00000870: 7468 2c20 2831 2c20 312c 2030 295d 5d0d  th, (1, 1, 0)]].
-00000880: 0a0d 0a70 5f67 6972 6465 7231 203d 2050  ...p_girder1 = P
-00000890: 7269 6d61 7279 4d65 6d62 6572 2870 5f6c  rimaryMember(p_l
-000008a0: 656e 6774 682c 2077 3136 7832 362c 2070  ength, w16x26, p
-000008b0: 5f73 7570 706f 7274 290d 0a70 5f67 6972  _support)..p_gir
-000008c0: 6465 7232 203d 2050 7269 6d61 7279 4d65  der2 = PrimaryMe
-000008d0: 6d62 6572 2870 5f6c 656e 6774 682c 2077  mber(p_length, w
-000008e0: 3136 7832 362c 2070 5f73 7570 706f 7274  16x26, p_support
-000008f0: 290d 0a73 5f62 6561 6d31 203d 2053 6563  )..s_beam1 = Sec
-00000900: 6f6e 6461 7279 4d65 6d62 6572 2873 5f6c  ondaryMember(s_l
-00000910: 656e 6774 682c 2077 3132 7831 362c 2073  ength, w12x16, s
-00000920: 5f73 7570 706f 7274 290d 0a73 5f62 6561  _support)..s_bea
-00000930: 6d32 203d 2053 6563 6f6e 6461 7279 4d65  m2 = SecondaryMe
-00000940: 6d62 6572 2873 5f6c 656e 6774 682c 2077  mber(s_length, w
-00000950: 3132 7831 362c 2073 5f73 7570 706f 7274  12x16, s_support
-00000960: 290d 0a73 5f6a 6f69 7374 3120 3d20 5365  )..s_joist1 = Se
-00000970: 636f 6e64 6172 794d 656d 6265 7228 735f  condaryMember(s_
-00000980: 6c65 6e67 7468 2c20 6b5f 3134 6b31 2c20  length, k_14k1, 
-00000990: 735f 7375 7070 6f72 7429 0d0a 735f 6a6f  s_support)..s_jo
-000009a0: 6973 7432 203d 2053 6563 6f6e 6461 7279  ist2 = Secondary
-000009b0: 4d65 6d62 6572 2873 5f6c 656e 6774 682c  Member(s_length,
-000009c0: 206b 5f31 346b 312c 2073 5f73 7570 706f   k_14k1, s_suppo
-000009d0: 7274 290d 0a73 5f6a 6f69 7374 3320 3d20  rt)..s_joist3 = 
-000009e0: 5365 636f 6e64 6172 794d 656d 6265 7228  SecondaryMember(
-000009f0: 735f 6c65 6e67 7468 2c20 6b5f 3134 6b31  s_length, k_14k1
-00000a00: 2c20 735f 7375 7070 6f72 7429 0d0a 0d0a  , s_support)....
-00000a10: 705f 6672 616d 696e 6720 3d20 5072 696d  p_framing = Prim
-00000a20: 6172 7946 7261 6d69 6e67 285b 705f 6769  aryFraming([p_gi
-00000a30: 7264 6572 312c 2070 5f67 6972 6465 7232  rder1, p_girder2
-00000a40: 5d29 0d0a 735f 6672 616d 696e 6720 3d20  ])..s_framing = 
-00000a50: 5365 636f 6e64 6172 7946 7261 6d69 6e67  SecondaryFraming
-00000a60: 285b 735f 6265 616d 312c 2073 5f6a 6f69  ([s_beam1, s_joi
-00000a70: 7374 312c 2073 5f6a 6f69 7374 322c 2073  st1, s_joist2, s
-00000a80: 5f6a 6f69 7374 332c 2073 5f62 6561 6d32  _joist3, s_beam2
-00000a90: 5d29 0d0a 6060 600d 0a4e 6f74 6520 7468  ])..```..Note th
-00000aa0: 6174 2065 6163 6820 6d65 6d62 6572 2073  at each member s
-00000ab0: 686f 756c 6420 6265 2069 6e64 6976 6964  hould be individ
-00000ac0: 7561 6c6c 7920 6465 6669 6e65 6420 6173  ually defined as
-00000ad0: 2073 686f 776e 2061 626f 7665 2e20 4f74   shown above. Ot
-00000ae0: 6865 7277 6973 652c 0d0a 7468 6520 6c6f  herwise,..the lo
-00000af0: 6164 696e 6773 2077 696c 6c20 6e6f 7420  adings will not 
-00000b00: 6265 2061 7070 6c69 6564 2063 6f72 7265  be applied corre
-00000b10: 6374 6c79 2074 6f20 7468 6520 6d65 6d62  ctly to the memb
-00000b20: 6572 732e 0d0a 0d0a 5468 6520 726f 6f66  ers.....The roof
-00000b30: 2073 6c6f 7065 2063 616e 206f 7074 696f   slope can optio
-00000b40: 6e61 6c6c 7920 6265 2073 6574 2069 6e20  nally be set in 
-00000b50: 7468 6520 6060 6053 6563 6f6e 6461 7279  the ```Secondary
-00000b60: 4672 616d 696e 6760 6060 206f 626a 6563  Framing``` objec
-00000b70: 7420 6279 0d0a 7573 696e 6720 7468 6520  t by..using the 
-00000b80: 6b65 7977 6f72 6420 6060 6073 6c6f 7065  keyword ```slope
-00000b90: 6060 6020 616e 6420 656e 7465 7269 6e67  ``` and entering
-00000ba0: 2074 6865 2072 6f6f 6620 736c 6f70 6520   the roof slope 
-00000bb0: 696e 2069 6e63 6865 732f 666f 6f74 2e20  in inches/foot. 
-00000bc0: 5468 650d 0a64 6566 6175 6c74 2076 616c  The..default val
-00000bd0: 7565 2069 7320 6060 6030 2e32 3560 6060  ue is ```0.25```
-00000be0: 2e0d 0a0d 0a4e 6578 742c 2064 6566 696e  .....Next, defin
-00000bf0: 6520 7468 6520 6c6f 6164 696e 6720 696e  e the loading in
-00000c00: 2074 6865 2072 6f6f 6620 6261 792e 0d0a   the roof bay...
-00000c10: 6060 6070 7974 686f 6e0d 0a70 5f66 7261  ```python..p_fra
-00000c20: 6d69 6e67 203d 2050 7269 6d61 7279 4672  ming = PrimaryFr
-00000c30: 616d 696e 6728 5b70 5f67 6972 6465 7231  aming([p_girder1
-00000c40: 2c20 705f 6769 7264 6572 325d 290d 0a73  , p_girder2])..s
-00000c50: 5f66 7261 6d69 6e67 203d 2053 6563 6f6e  _framing = Secon
-00000c60: 6461 7279 4672 616d 696e 6728 5b73 5f62  daryFraming([s_b
-00000c70: 6561 6d31 2c20 735f 6a6f 6973 7431 2c20  eam1, s_joist1, 
-00000c80: 735f 6a6f 6973 7432 2c20 735f 6a6f 6973  s_joist2, s_jois
-00000c90: 7433 2c20 735f 6265 616d 325d 290d 0a0d  t3, s_beam2])...
-00000ca0: 0a71 5f64 6c20 3d20 3230 2f31 3030 302f  .q_dl = 20/1000/
-00000cb0: 3134 3420 2320 5375 7266 6163 6520 6465  144 # Surface de
-00000cc0: 6164 206c 6f61 6420 696e 206b 7369 0d0a  ad load in ksi..
-00000cd0: 715f 726c 203d 2032 322e 342f 3130 3030  q_rl = 22.4/1000
-00000ce0: 2f31 3434 2023 2053 7572 6661 6365 2072  /144 # Surface r
-00000cf0: 6169 6e20 6c6f 6164 2061 7420 7365 636f  ain load at seco
-00000d00: 6e64 6172 7920 6472 6169 6e61 6765 2069  ndary drainage i
-00000d10: 6e6c 6574 2069 6e20 6b73 690d 0a0d 0a6c  nlet in ksi....l
-00000d20: 6f61 6469 6e67 203d 204c 6f61 6469 6e67  oading = Loading
-00000d30: 2871 5f64 6c2c 2071 5f72 6c29 0d0a 6060  (q_dl, q_rl)..``
-00000d40: 600d 0a54 6865 2069 6e70 7574 2072 6169  `..The input rai
-00000d50: 6e20 6c6f 6164 2073 686f 756c 6420 696e  n load should in
-00000d60: 636c 7564 6520 7468 6520 7374 6174 6963  clude the static
-00000d70: 2068 6561 6420 616e 6420 7468 6520 6879   head and the hy
-00000d80: 6472 6175 6c69 6320 6865 6164 2c20 6275  draulic head, bu
-00000d90: 740d 0a6e 6f20 706f 6e64 696e 6720 6865  t..no ponding he
-00000da0: 6164 2e0d 0a0d 0a46 696e 616c 6c79 2c20  ad.....Finally, 
-00000db0: 6465 6669 6e65 2074 6865 2060 6060 506f  define the ```Po
-00000dc0: 6e64 5079 4d6f 6465 6c60 6060 206f 626a  ndPyModel``` obj
-00000dd0: 6563 7420 616e 6420 616e 616c 797a 6520  ect and analyze 
-00000de0: 7468 6520 6d6f 6465 6c2e 0d0a 6060 6070  the model...```p
-00000df0: 7974 686f 6e0d 0a70 6f6e 6470 795f 6d6f  ython..pondpy_mo
-00000e00: 6465 6c20 3d20 506f 6e64 5079 4d6f 6465  del = PondPyMode
-00000e10: 6c28 705f 6672 616d 696e 672c 2073 5f66  l(p_framing, s_f
-00000e20: 7261 6d69 6e67 2c20 6c6f 6164 696e 6729  raming, loading)
-00000e30: 0d0a 0d0a 706f 6e64 7079 5f6d 6f64 656c  ....pondpy_model
-00000e40: 2e70 6572 666f 726d 5f61 6e61 6c79 7369  .perform_analysi
-00000e50: 7328 290d 0a60 6060 0d0a 4f70 7469 6f6e  s()..```..Option
-00000e60: 616c 2061 7267 756d 656e 7473 2066 6f72  al arguments for
-00000e70: 2074 6865 2060 6060 506f 6e64 5079 4d6f   the ```PondPyMo
-00000e80: 6465 6c60 6060 2069 6e63 6c75 6465 3a0d  del``` include:.
-00000e90: 0a0d 0a2d 2060 6060 6d69 7272 6f72 6564  ...- ```mirrored
-00000ea0: 5f6c 6566 7460 6060 3a20 626f 6f6c 2069  _left```: bool i
-00000eb0: 6e64 6963 6174 696e 6720 7768 6574 6865  ndicating whethe
-00000ec0: 7220 7468 6520 726f 6f66 2062 6179 2069  r the roof bay i
-00000ed0: 7320 6d69 7272 6f72 6564 0d0a 2020 2020  s mirrored..    
-00000ee0: 6f6e 2074 6865 206c 6566 7420 7369 6465  on the left side
-00000ef0: 3b20 6465 6661 756c 7420 6973 2060 6060  ; default is ```
-00000f00: 4661 6c73 6560 6060 0d0a 0d0a 2d20 6060  False```....- ``
-00000f10: 606d 6972 726f 7265 645f 7269 6768 7460  `mirrored_right`
-00000f20: 6060 203a 2062 6f6f 6c20 696e 6469 6361  `` : bool indica
-00000f30: 7469 6e67 2077 6865 7468 6572 2074 6865  ting whether the
-00000f40: 2072 6f6f 6620 6261 7920 6973 206d 6972   roof bay is mir
-00000f50: 726f 7265 640d 0a20 2020 206f 6e20 7468  rored..    on th
-00000f60: 6520 7269 6768 7420 7369 6465 3b20 6465  e right side; de
-00000f70: 6661 756c 7420 6973 2060 6060 4661 6c73  fault is ```Fals
-00000f80: 6560 6060 0d0a 0d0a 2d20 6060 6073 746f  e```....- ```sto
-00000f90: 705f 6372 6974 6572 696f 6e60 6060 203a  p_criterion``` :
-00000fa0: 2066 6c6f 6174 2069 6e64 6963 6174 696e   float indicatin
-00000fb0: 6720 7468 6520 6572 726f 7220 696e 2074  g the error in t
-00000fc0: 6f74 616c 2069 6d70 6f75 6e64 6564 0d0a  otal impounded..
-00000fd0: 2020 2020 7761 7465 7220 7765 6967 6874      water weight
-00000fe0: 2061 7420 7768 6963 6820 7468 6520 6974   at which the it
-00000ff0: 6572 6174 6976 6520 616e 616c 7973 6973  erative analysis
-00001000: 2073 686f 756c 6420 6265 2074 6572 6d69   should be termi
-00001010: 6e61 7465 643b 0d0a 2020 2020 6465 6661  nated;..    defa
-00001020: 756c 7420 6973 2060 6060 302e 3030 3031  ult is ```0.0001
-00001030: 6060 600d 0a0d 0a2d 2060 6060 6d61 785f  ```....- ```max_
-00001040: 6974 6572 6060 6020 3a20 696e 7420 696e  iter``` : int in
-00001050: 6469 6361 7469 6e67 2074 6865 206d 6178  dicating the max
-00001060: 696d 756d 206e 756d 6265 7220 6f66 2069  imum number of i
-00001070: 7465 7261 7469 6f6e 7320 7468 6174 0d0a  terations that..
-00001080: 2020 2020 7368 6f75 6c64 2062 6520 7065      should be pe
-00001090: 7266 6f72 6d65 643b 2064 6566 6175 6c74  rformed; default
-000010a0: 2069 7320 6060 6035 3060 6060 0d0a 2020   is ```50```..  
-000010b0: 2020 0d0a 2d20 6060 6073 686f 775f 7265    ..- ```show_re
-000010c0: 7375 6c74 7360 6060 203a 2062 6f6f 6c20  sults``` : bool 
-000010d0: 696e 6469 6361 7469 6e67 2077 6865 7468  indicating wheth
-000010e0: 6572 2074 6865 2069 7465 7261 7469 6f6e  er the iteration
-000010f0: 2072 6573 756c 7473 2073 686f 756c 640d   results should.
-00001100: 0a20 2020 2062 6520 7072 696e 7465 6420  .    be printed 
-00001110: 746f 2074 6865 2074 6572 6d69 6e61 6c20  to the terminal 
-00001120: 7570 6f6e 2063 6f6d 706c 6574 696f 6e20  upon completion 
-00001130: 6f66 2074 6865 2061 6e61 6c79 7369 733b  of the analysis;
-00001140: 0d0a 2020 2020 6465 6661 756c 7420 6973  ..    default is
-00001150: 2060 6060 5472 7565 6060 600d 0a0d 0a23   ```True```....#
-00001160: 2323 2041 6e61 6c79 7369 7320 5265 7375  ## Analysis Resu
-00001170: 6c74 730d 0a45 6163 6820 7072 696d 6172  lts..Each primar
-00001180: 7920 616e 6420 7365 636f 6e64 6172 7920  y and secondary 
-00001190: 6d65 6d62 6572 2069 7320 7265 7072 6573  member is repres
-000011a0: 656e 7465 6420 7769 7468 696e 2074 6865  ented within the
-000011b0: 2050 6f6e 6450 794d 6f64 656c 206f 626a   PondPyModel obj
-000011c0: 6563 740d 0a62 7920 6120 4265 616d 4d6f  ect..by a BeamMo
-000011d0: 6465 6c20 6f62 6a65 6374 2e20 4173 2073  del object. As s
-000011e0: 7563 6820 6120 6772 6561 7420 6465 616c  uch a great deal
-000011f0: 206f 6620 616e 616c 7973 6973 2072 6573   of analysis res
-00001200: 756c 7473 2063 616e 2062 6520 6f62 7461  ults can be obta
-00001210: 696e 6564 0d0a 6661 6972 6c79 2065 6173  ined..fairly eas
-00001220: 696c 7920 6f6e 6365 2074 6865 2061 6e61  ily once the ana
-00001230: 6c79 7369 7320 6973 2063 6f6d 706c 6574  lysis is complet
-00001240: 652e 0d0a 0d0a 2d20 546f 2061 6363 6573  e.....- To acces
-00001250: 7320 7468 6520 6465 666c 6563 7465 6420  s the deflected 
-00001260: 7368 6170 652c 2073 6865 6172 2066 6f72  shape, shear for
-00001270: 6365 2064 6961 6772 616d 2c20 6f72 2062  ce diagram, or b
-00001280: 656e 6469 6e67 206d 6f6d 656e 7420 6469  ending moment di
-00001290: 6167 7261 6d0d 0a20 206f 6620 6120 7061  agram..  of a pa
-000012a0: 7274 6963 756c 6172 206d 656d 6265 722c  rticular member,
-000012b0: 2075 7365 2074 6865 2066 6f6c 6c6f 7769   use the followi
-000012c0: 6e67 2063 616c 6c73 3a0d 0a20 2060 6060  ng calls:..  ```
-000012d0: 7079 7468 6f6e 0d0a 2020 6d65 6d62 6572  python..  member
-000012e0: 203d 2070 6f6e 6470 795f 6d6f 6465 6c2e   = pondpy_model.
-000012f0: 726f 6f66 5f62 6179 5f6d 6f64 656c 2e73  roof_bay_model.s
-00001300: 6563 6f6e 6461 7279 5f6d 656d 6265 7273  econdary_members
-00001310: 5b30 5d0d 0a20 2062 6d64 203d 206d 656d  [0]..  bmd = mem
-00001320: 6265 722e 706c 6f74 5f62 6d64 2829 0d0a  ber.plot_bmd()..
-00001330: 2020 626d 642e 7368 6f77 2829 0d0a 2020    bmd.show()..  
-00001340: 6060 600d 0a20 2054 6865 2073 6865 6172  ```..  The shear
-00001350: 2066 6f72 6365 2064 6961 6772 616d 2061   force diagram a
-00001360: 6e64 2064 6566 6c65 6374 6564 2073 6861  nd deflected sha
-00001370: 7065 2063 616e 2062 6520 6163 6365 7373  pe can be access
-00001380: 6564 2069 6e20 6120 7369 6d69 6c61 720d  ed in a similar.
-00001390: 0a20 2066 6173 6869 6f6e 2e0d 0a0d 0a2d  .  fashion.....-
-000013a0: 2054 6865 2073 7570 706f 7274 2072 6561   The support rea
-000013b0: 6374 696f 6e73 2063 616e 2062 6520 6f62  ctions can be ob
-000013c0: 7461 696e 6564 2061 7320 666f 6c6c 6f77  tained as follow
-000013d0: 733a 0d0a 2020 6060 6070 7974 686f 6e0d  s:..  ```python.
-000013e0: 0a20 2073 7570 706f 7274 5f6e 6f64 6573  .  support_nodes
-000013f0: 203d 206d 656d 6265 722e 7375 7070 6f72   = member.suppor
-00001400: 745f 6e6f 6465 730d 0a20 2073 7570 706f  t_nodes..  suppo
-00001410: 7274 5f72 6561 6374 696f 6e73 203d 205b  rt_reactions = [
-00001420: 6d65 6d62 6572 2e73 7570 706f 7274 5f72  member.support_r
-00001430: 6561 6374 696f 6e73 5b6e 6f64 655d 2066  eactions[node] f
-00001440: 6f72 206e 6f64 6520 696e 2073 7570 706f  or node in suppo
-00001450: 7274 5f6e 6f64 6573 5d0d 0a20 2060 6060  rt_nodes]..  ```
-00001460: 0d0a 0d0a 5365 7665 7261 6c20 6f74 6865  ....Several othe
-00001470: 7220 6174 7472 6962 7574 6573 206f 6620  r attributes of 
-00001480: 7468 6520 4265 616d 4d6f 6465 6c20 6f62  the BeamModel ob
-00001490: 6a65 6374 2063 616e 2062 6520 6163 6365  ject can be acce
-000014a0: 7373 6564 2069 6e20 6120 7369 6d69 6c61  ssed in a simila
-000014b0: 720d 0a66 6173 6869 6f6e 2e0d 0a0d 0a4e  r..fashion.....N
-000014c0: 6f74 6520 7468 6174 206f 6e6c 7920 7468  ote that only th
-000014d0: 6520 6669 6e61 6c20 616e 616c 7973 6973  e final analysis
-000014e0: 2072 6573 756c 7473 2063 616e 2063 7572   results can cur
-000014f0: 7265 6e74 6c79 2062 6520 6163 6365 7373  rently be access
-00001500: 6564 2e0d 0a0d 0a23 2323 2041 6464 6974  ed.....### Addit
-00001510: 696f 6e61 6c20 496e 666f 726d 6174 696f  ional Informatio
-00001520: 6e0d 0a2d 205b 446f 6375 6d65 6e74 6174  n..- [Documentat
-00001530: 696f 6e5d 2868 7474 7073 3a2f 2f70 6f6e  ion](https://pon
-00001540: 6470 792e 7265 6164 7468 6564 6f63 732e  dpy.readthedocs.
-00001550: 696f 2f65 6e2f 6c61 7465 7374 2f29 0d0a  io/en/latest/)..
-00001560: 2d20 5b50 7950 4920 4469 7374 7269 6275  - [PyPI Distribu
-00001570: 7469 6f6e 5d28 6874 7470 733a 2f2f 7079  tion](https://py
-00001580: 7069 2e6f 7267 2f70 726f 6a65 6374 2f70  pi.org/project/p
-00001590: 6f6e 6470 792f 290d 0a                   ondpy/)..
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0d0a 2020 2020 3c69 6d67 2073 7263  ">..    <img src
+00000020: 3d22 646f 6373 2f73 6f75 7263 652f 706f  ="docs/source/po
+00000030: 6e64 7079 2e73 7667 2220 616c 743d 224c  ndpy.svg" alt="L
+00000040: 6f67 6f22 2077 6964 7468 3d22 3530 3022  ogo" width="500"
+00000050: 202f 3e0d 0a3c 2f70 3e0d 0a0d 0a3c 7020   />..</p>....<p 
+00000060: 616c 6967 6e3d 2263 656e 7465 7222 3e0d  align="center">.
+00000070: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00000080: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000090: 2f6d 6174 7468 6577 2d75 7073 6861 772f  /matthew-upshaw/
+000000a0: 706f 6e64 7079 2f61 6374 696f 6e73 2f77  pondpy/actions/w
+000000b0: 6f72 6b66 6c6f 7773 2f74 6573 7473 2e79  orkflows/tests.y
+000000c0: 6d6c 223e 3c69 6d67 2061 6c74 3d22 5465  ml"><img alt="Te
+000000d0: 7374 7322 2073 7263 3d22 6874 7470 733a  sts" src="https:
+000000e0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6174  //github.com/mat
+000000f0: 7468 6577 2d75 7073 6861 772f 706f 6e64  thew-upshaw/pond
+00000100: 7079 2f61 6374 696f 6e73 2f77 6f72 6b66  py/actions/workf
+00000110: 6c6f 7773 2f74 6573 7473 2e79 616d 6c2f  lows/tests.yaml/
+00000120: 6261 6467 652e 7376 6722 3e3c 2f61 3e26  badge.svg"></a>&
+00000130: 6e62 7370 3b26 6e62 7370 3b26 6e62 7370  nbsp;&nbsp;&nbsp
+00000140: 3b0d 0a20 2020 203c 6120 6872 6566 3d22  ;..    <a href="
+00000150: 6874 7470 733a 2f2f 636f 7665 7261 6c6c  https://coverall
+00000160: 732e 696f 2f67 6974 6875 622f 6d61 7474  s.io/github/matt
+00000170: 6865 772d 7570 7368 6177 2f70 6f6e 6470  hew-upshaw/pondp
+00000180: 793f 6272 616e 6368 3d6d 6169 6e22 3e3c  y?branch=main"><
+00000190: 696d 6720 616c 743d 2243 6f76 6572 6167  img alt="Coverag
+000001a0: 6520 5374 6174 7573 2220 7372 633d 2268  e Status" src="h
+000001b0: 7474 7073 3a2f 2f63 6f76 6572 616c 6c73  ttps://coveralls
+000001c0: 2e69 6f2f 7265 706f 732f 6769 7468 7562  .io/repos/github
+000001d0: 2f6d 6174 7468 6577 2d75 7073 6861 772f  /matthew-upshaw/
+000001e0: 706f 6e64 7079 2f62 6164 6765 2e73 7667  pondpy/badge.svg
+000001f0: 3f62 7261 6e63 683d 6d61 696e 2676 3d30  ?branch=main&v=0
+00000200: 2e31 2e32 223e 3c2f 613e 266e 6273 703b  .1.2"></a>&nbsp;
+00000210: 266e 6273 703b 266e 6273 703b 0d0a 2020  &nbsp;&nbsp;..  
+00000220: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000230: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d61  ://github.com/ma
+00000240: 7474 6865 772d 7570 7368 6177 2f70 6f6e  tthew-upshaw/pon
+00000250: 6470 792f 626c 6f62 2f6d 6169 6e2f 4c49  dpy/blob/main/LI
+00000260: 4345 4e53 4522 3e3c 696d 6720 616c 743d  CENSE"><img alt=
+00000270: 224c 6963 656e 7365 3a20 4d49 5422 2073  "License: MIT" s
+00000280: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000290: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000002a0: 2f4c 6963 656e 7365 2d4d 4954 2d79 656c  /License-MIT-yel
+000002b0: 6c6f 772e 7376 6722 3e3c 2f61 3e26 6e62  low.svg"></a>&nb
+000002c0: 7370 3b26 6e62 7370 3b26 6e62 7370 3b0d  sp;&nbsp;&nbsp;.
+000002d0: 0a3c 2f70 3e0d 0a0d 0a23 2049 6e74 726f  .</p>....# Intro
+000002e0: 6475 6374 696f 6e0d 0a2a 2a70 6f6e 6470  duction..**pondp
+000002f0: 792a 2a20 6973 2061 2070 6163 6b61 6765  y** is a package
+00000300: 2062 7569 6c74 2074 6f20 6169 6420 696e   built to aid in
+00000310: 2074 6865 2064 6573 6967 6e20 6f66 206c   the design of l
+00000320: 6f77 2d73 6c6f 7065 2072 6f6f 6620 6261  ow-slope roof ba
+00000330: 7973 2066 6f72 200d 0a70 6f6e 6469 6e67  ys for ..ponding
+00000340: 2073 7461 6269 6c69 7479 2061 6e64 2069   stability and i
+00000350: 6d70 6f75 6e64 6564 2072 6169 6e20 6c6f  mpounded rain lo
+00000360: 6164 696e 672e 2049 7420 7574 696c 697a  ading. It utiliz
+00000370: 6573 2061 2073 6572 6965 7320 6f66 0d0a  es a series of..
+00000380: 7075 7270 6f73 652d 6275 696c 7420 6669  purpose-built fi
+00000390: 6e69 7465 2065 6c65 6d65 6e74 2061 6e64  nite element and
+000003a0: 2070 6f6e 6469 6e67 2061 6e61 6c79 7369   ponding analysi
+000003b0: 7320 636c 6173 7365 7320 616e 6420 6d65  s classes and me
+000003c0: 7468 6f64 7320 746f 2062 650d 0a61 7320  thods to be..as 
+000003d0: 696e 7475 6974 6976 6520 6173 2070 6f73  intuitive as pos
+000003e0: 7369 626c 6520 666f 7220 7468 6520 6d6f  sible for the mo
+000003f0: 6465 726e 2065 6e67 696e 6565 722e 0d0a  dern engineer...
+00000400: 0d0a 2323 2320 496e 7374 616c 6c61 7469  ..### Installati
+00000410: 6f6e 0d0a 496e 7374 616c 6c20 706f 6e64  on..Install pond
+00000420: 7079 2077 6974 6820 7069 703a 0d0a 6060  py with pip:..``
+00000430: 6062 6173 680d 0a70 6970 2069 6e73 7461  `bash..pip insta
+00000440: 6c6c 2070 6f6e 6470 790d 0a60 6060 0d0a  ll pondpy..```..
+00000450: 0d0a 2323 2320 5573 6167 650d 0a54 6865  ..### Usage..The
+00000460: 2050 6f6e 6450 794d 6f64 656c 2063 6c61   PondPyModel cla
+00000470: 7373 2069 7320 6465 7369 676e 6564 2074  ss is designed t
+00000480: 6f20 776f 726b 2077 6974 6820 7365 7665  o work with seve
+00000490: 7261 6c20 7075 7270 6f73 652d 6275 696c  ral purpose-buil
+000004a0: 7420 636c 6173 7365 730d 0a74 6861 7420  t classes..that 
+000004b0: 6865 6c70 2074 6865 2075 7365 7220 6f72  help the user or
+000004c0: 6761 6e69 7a65 2074 6865 6972 2069 6e70  ganize their inp
+000004d0: 7574 2069 6e74 6f20 6120 666f 726d 2074  ut into a form t
+000004e0: 6861 7420 6172 6520 7265 6164 696c 7920  hat are readily 
+000004f0: 7574 696c 697a 6564 0d0a 746f 2062 7569  utilized..to bui
+00000500: 6c64 2061 6e64 2061 6e61 6c79 7a65 2074  ld and analyze t
+00000510: 6865 206d 6f64 656c 2e20 5468 6573 6520  he model. These 
+00000520: 6172 6520 7468 6520 6060 6050 7269 6d61  are the ```Prima
+00000530: 7279 4672 616d 696e 6760 6060 2c0d 0a60  ryFraming```,..`
+00000540: 6060 5365 636f 6e64 6172 7946 7261 6d69  ``SecondaryFrami
+00000550: 6e67 6060 602c 2061 6e64 2060 6060 4c6f  ng```, and ```Lo
+00000560: 6164 696e 6760 6060 2063 6c61 7373 6573  ading``` classes
+00000570: 2e20 496e 2061 6464 6974 696f 6e2c 2074  . In addition, t
+00000580: 6865 2070 6163 6b61 6765 2069 730d 0a64  he package is..d
+00000590: 6573 6967 6e65 6420 746f 2077 6f72 6b20  esigned to work 
+000005a0: 7769 7468 2074 6865 2060 6060 7374 6565  with the ```stee
+000005b0: 6c70 7960 6060 2061 6e64 2060 6060 6a6f  lpy``` and ```jo
+000005c0: 6973 7470 7960 6060 2070 6163 6b61 6765  istpy``` package
+000005d0: 732c 2074 686f 7567 6820 616e 790d 0a6f  s, though any..o
+000005e0: 626a 6563 7420 636f 6e74 6169 6e69 6e67  bject containing
+000005f0: 2074 6865 2072 6571 7569 7269 6e67 2069   the requiring i
+00000600: 6e66 6f72 6d61 7469 6f6e 2061 7474 7269  nformation attri
+00000610: 6275 7265 7320 2869 2e65 2e20 6d6f 6d65  bures (i.e. mome
+00000620: 6e74 206f 6620 696e 6572 7469 612c 0d0a  nt of inertia,..
+00000630: 6372 6f73 732d 7365 6374 696f 6e61 6c20  cross-sectional 
+00000640: 6172 6561 2c20 656c 6173 7469 6320 6d6f  area, elastic mo
+00000650: 6475 6c75 732c 2065 7463 2e29 2063 6f75  dulus, etc.) cou
+00000660: 6c64 2062 6520 7573 6564 2069 6e20 6c69  ld be used in li
+00000670: 6575 206f 6620 6569 7468 6572 0d0a 7061  eu of either..pa
+00000680: 636b 6167 652e 0d0a 0d0a 546f 2063 7265  ckage.....To cre
+00000690: 6174 6520 616e 6420 616e 616c 797a 6520  ate and analyze 
+000006a0: 6120 726f 6f66 2062 6179 206d 6f64 656c  a roof bay model
+000006b0: 2c20 6669 7273 7420 696d 706f 7274 2074  , first import t
+000006c0: 6865 2072 6571 7569 7265 6420 6465 7065  he required depe
+000006d0: 6e64 656e 6369 6573 0d0a 616e 6420 636c  ndencies..and cl
+000006e0: 6173 7365 733a 0d0a 6060 6070 7974 686f  asses:..```pytho
+000006f0: 6e0d 0a66 726f 6d20 6a6f 6973 7470 7920  n..from joistpy 
+00000700: 696d 706f 7274 2073 6a69 0d0a 6672 6f6d  import sji..from
+00000710: 2073 7465 656c 7079 2069 6d70 6f72 7420   steelpy import 
+00000720: 6169 7363 0d0a 0d0a 6672 6f6d 2070 6f6e  aisc....from pon
+00000730: 6470 792e 616e 616c 7973 6973 2e66 656d  dpy.analysis.fem
+00000740: 5f61 6e61 6c79 7369 7320 696d 706f 7274  _analysis import
+00000750: 2028 0d0a 2020 2020 5374 6565 6c42 6561   (..    SteelBea
+00000760: 6d53 697a 652c 0d0a 2020 2020 5374 6565  mSize,..    Stee
+00000770: 6c4a 6f69 7374 5369 7a65 2c0d 0a29 0d0a  lJoistSize,..)..
+00000780: 0d0a 6672 6f6d 2070 6f6e 6470 792e 616e  ..from pondpy.an
+00000790: 616c 7973 6973 2e70 6f6e 645f 616e 616c  alysis.pond_anal
+000007a0: 7973 6973 2069 6d70 6f72 7420 280d 0a20  ysis import (.. 
+000007b0: 2020 2050 7269 6d61 7279 4d65 6d62 6572     PrimaryMember
+000007c0: 2c0d 0a20 2020 2050 7269 6d61 7279 4672  ,..    PrimaryFr
+000007d0: 616d 696e 672c 0d0a 2020 2020 5365 636f  aming,..    Seco
+000007e0: 6e64 6172 794d 656d 6265 722c 0d0a 2020  ndaryMember,..  
+000007f0: 2020 5365 636f 6e64 6172 7946 7261 6d69    SecondaryFrami
+00000800: 6e67 2c0d 0a20 2020 204c 6f61 6469 6e67  ng,..    Loading
+00000810: 0d0a 290d 0a0d 0a66 726f 6d20 706f 6e64  ..)....from pond
+00000820: 7079 2e70 6f6e 6470 7920 696d 706f 7274  py.pondpy import
+00000830: 2050 6f6e 6450 794d 6f64 656c 0d0a 6060   PondPyModel..``
+00000840: 600d 0a0d 0a4e 6578 742c 2064 6566 696e  `....Next, defin
+00000850: 6520 7468 6520 7374 6565 6c20 7368 6170  e the steel shap
+00000860: 6573 2061 6e64 206a 6f69 7374 2064 6573  es and joist des
+00000870: 6967 6e61 7469 6f6e 7320 696e 2079 6f75  ignations in you
+00000880: 7220 6d6f 6465 6c2e 0d0a 6060 6070 7974  r model...```pyt
+00000890: 686f 6e0d 0a77 3132 7831 3620 3d20 5374  hon..w12x16 = St
+000008a0: 6565 6c42 6561 6d53 697a 6528 2757 3132  eelBeamSize('W12
+000008b0: 5831 3627 2c20 6169 7363 2e57 5f73 6861  X16', aisc.W_sha
+000008c0: 7065 732e 5731 3258 3136 290d 0a77 3136  pes.W12X16)..w16
+000008d0: 7832 3620 3d20 5374 6565 6c42 6561 6d53  x26 = SteelBeamS
+000008e0: 697a 6528 2757 3136 5832 3627 2c20 6169  ize('W16X26', ai
+000008f0: 7363 2e57 5f73 6861 7065 732e 5731 3658  sc.W_shapes.W16X
+00000900: 3236 290d 0a6b 5f31 346b 3120 3d20 5374  26)..k_14k1 = St
+00000910: 6565 6c4a 6f69 7374 5369 7a65 2827 3134  eelJoistSize('14
+00000920: 4b31 272c 2073 6a69 2e4b 5f53 6572 6965  K1', sji.K_Serie
+00000930: 732e 4b5f 3134 4b31 290d 0a60 6060 0d0a  s.K_14K1)..```..
+00000940: 0d0a 4e65 7874 2c20 6465 6669 6e65 2074  ..Next, define t
+00000950: 6865 2070 7269 6d61 7279 2061 6e64 2073  he primary and s
+00000960: 6563 6f6e 6461 7279 2066 7261 6d69 6e67  econdary framing
+00000970: 2069 6e20 7468 6520 726f 6f66 2062 6179   in the roof bay
+00000980: 2066 7261 6d69 6e67 2073 7973 7465 6d2e   framing system.
+00000990: 200d 0a4e 6f74 6520 7468 6174 2061 6c6c   ..Note that all
+000009a0: 2069 6e70 7574 7320 7368 6f75 6c64 2062   inputs should b
+000009b0: 6520 696e 206b 6970 7320 616e 6420 696e  e in kips and in
+000009c0: 6368 6573 2e0d 0a60 6060 7079 7468 6f6e  ches...```python
+000009d0: 0d0a 705f 6c65 6e67 7468 203d 2032 302a  ..p_length = 20*
+000009e0: 3132 2023 206c 656e 6774 6820 6f66 2070  12 # length of p
+000009f0: 7269 6d61 7279 206d 656d 6265 7273 2069  rimary members i
+00000a00: 6e20 696e 6368 6573 0d0a 735f 6c65 6e67  n inches..s_leng
+00000a10: 7468 203d 2032 302a 3132 2023 206c 656e  th = 20*12 # len
+00000a20: 6774 6820 6f66 2073 6563 6f6e 6461 7279  gth of secondary
+00000a30: 206d 656d 6265 7273 2069 6e20 696e 6368   members in inch
+00000a40: 6573 0d0a 0d0a 2320 5375 7070 6f72 7420  es....# Support 
+00000a50: 7479 7065 7320 6172 6520 6465 7369 676e  types are design
+00000a60: 6174 6564 2062 7920 7475 706c 6573 2072  ated by tuples r
+00000a70: 6570 7265 7365 6e74 696e 6720 2854 782c  epresenting (Tx,
+00000a80: 2054 792c 2052 7a29 2e0d 0a23 2041 2030   Ty, Rz)...# A 0
+00000a90: 2069 6e64 6963 6174 6573 2074 6865 2064   indicates the d
+00000aa0: 6567 7265 6520 6f66 2066 7265 6564 6f6d  egree of freedom
+00000ab0: 2069 7320 756e 7265 7374 7261 696e 6564   is unrestrained
+00000ac0: 2077 6869 6c65 2061 2031 2069 6e64 6963   while a 1 indic
+00000ad0: 6174 6573 2061 200d 0a23 2072 6573 7472  ates a ..# restr
+00000ae0: 6169 6e65 6420 6465 6772 6565 206f 6620  ained degree of 
+00000af0: 6672 6565 646f 6d2e 0d0a 705f 7375 7070  freedom...p_supp
+00000b00: 6f72 7420 3d20 5b5b 302c 2028 312c 2031  ort = [[0, (1, 1
+00000b10: 2c20 3029 5d2c 205b 705f 6c65 6e67 7468  , 0)], [p_length
+00000b20: 2c20 2831 2c20 312c 2030 295d 5d0d 0a73  , (1, 1, 0)]]..s
+00000b30: 5f73 7570 706f 7274 203d 205b 5b30 2c20  _support = [[0, 
+00000b40: 2831 2c20 312c 2030 295d 2c20 5b73 5f6c  (1, 1, 0)], [s_l
+00000b50: 656e 6774 682c 2028 312c 2031 2c20 3029  ength, (1, 1, 0)
+00000b60: 5d5d 0d0a 0d0a 705f 6769 7264 6572 3120  ]]....p_girder1 
+00000b70: 3d20 5072 696d 6172 794d 656d 6265 7228  = PrimaryMember(
+00000b80: 705f 6c65 6e67 7468 2c20 7731 3678 3236  p_length, w16x26
+00000b90: 2c20 705f 7375 7070 6f72 7429 0d0a 705f  , p_support)..p_
+00000ba0: 6769 7264 6572 3220 3d20 5072 696d 6172  girder2 = Primar
+00000bb0: 794d 656d 6265 7228 705f 6c65 6e67 7468  yMember(p_length
+00000bc0: 2c20 7731 3678 3236 2c20 705f 7375 7070  , w16x26, p_supp
+00000bd0: 6f72 7429 0d0a 735f 6265 616d 3120 3d20  ort)..s_beam1 = 
+00000be0: 5365 636f 6e64 6172 794d 656d 6265 7228  SecondaryMember(
+00000bf0: 735f 6c65 6e67 7468 2c20 7731 3278 3136  s_length, w12x16
+00000c00: 2c20 735f 7375 7070 6f72 7429 0d0a 735f  , s_support)..s_
+00000c10: 6265 616d 3220 3d20 5365 636f 6e64 6172  beam2 = Secondar
+00000c20: 794d 656d 6265 7228 735f 6c65 6e67 7468  yMember(s_length
+00000c30: 2c20 7731 3278 3136 2c20 735f 7375 7070  , w12x16, s_supp
+00000c40: 6f72 7429 0d0a 735f 6a6f 6973 7431 203d  ort)..s_joist1 =
+00000c50: 2053 6563 6f6e 6461 7279 4d65 6d62 6572   SecondaryMember
+00000c60: 2873 5f6c 656e 6774 682c 206b 5f31 346b  (s_length, k_14k
+00000c70: 312c 2073 5f73 7570 706f 7274 290d 0a73  1, s_support)..s
+00000c80: 5f6a 6f69 7374 3220 3d20 5365 636f 6e64  _joist2 = Second
+00000c90: 6172 794d 656d 6265 7228 735f 6c65 6e67  aryMember(s_leng
+00000ca0: 7468 2c20 6b5f 3134 6b31 2c20 735f 7375  th, k_14k1, s_su
+00000cb0: 7070 6f72 7429 0d0a 735f 6a6f 6973 7433  pport)..s_joist3
+00000cc0: 203d 2053 6563 6f6e 6461 7279 4d65 6d62   = SecondaryMemb
+00000cd0: 6572 2873 5f6c 656e 6774 682c 206b 5f31  er(s_length, k_1
+00000ce0: 346b 312c 2073 5f73 7570 706f 7274 290d  4k1, s_support).
+00000cf0: 0a0d 0a70 5f66 7261 6d69 6e67 203d 2050  ...p_framing = P
+00000d00: 7269 6d61 7279 4672 616d 696e 6728 5b70  rimaryFraming([p
+00000d10: 5f67 6972 6465 7231 2c20 705f 6769 7264  _girder1, p_gird
+00000d20: 6572 325d 290d 0a73 5f66 7261 6d69 6e67  er2])..s_framing
+00000d30: 203d 2053 6563 6f6e 6461 7279 4672 616d   = SecondaryFram
+00000d40: 696e 6728 5b73 5f62 6561 6d31 2c20 735f  ing([s_beam1, s_
+00000d50: 6a6f 6973 7431 2c20 735f 6a6f 6973 7432  joist1, s_joist2
+00000d60: 2c20 735f 6a6f 6973 7433 2c20 735f 6265  , s_joist3, s_be
+00000d70: 616d 325d 290d 0a60 6060 0d0a 4e6f 7465  am2])..```..Note
+00000d80: 2074 6861 7420 6561 6368 206d 656d 6265   that each membe
+00000d90: 7220 7368 6f75 6c64 2062 6520 696e 6469  r should be indi
+00000da0: 7669 6475 616c 6c79 2064 6566 696e 6564  vidually defined
+00000db0: 2061 7320 7368 6f77 6e20 6162 6f76 652e   as shown above.
+00000dc0: 204f 7468 6572 7769 7365 2c0d 0a74 6865   Otherwise,..the
+00000dd0: 206c 6f61 6469 6e67 7320 7769 6c6c 206e   loadings will n
+00000de0: 6f74 2062 6520 6170 706c 6965 6420 636f  ot be applied co
+00000df0: 7272 6563 746c 7920 746f 2074 6865 206d  rrectly to the m
+00000e00: 656d 6265 7273 2e0d 0a0d 0a54 6865 2072  embers.....The r
+00000e10: 6f6f 6620 736c 6f70 6520 6361 6e20 6f70  oof slope can op
+00000e20: 7469 6f6e 616c 6c79 2062 6520 7365 7420  tionally be set 
+00000e30: 696e 2074 6865 2060 6060 5365 636f 6e64  in the ```Second
+00000e40: 6172 7946 7261 6d69 6e67 6060 6020 6f62  aryFraming``` ob
+00000e50: 6a65 6374 2062 790d 0a75 7369 6e67 2074  ject by..using t
+00000e60: 6865 206b 6579 776f 7264 2060 6060 736c  he keyword ```sl
+00000e70: 6f70 6560 6060 2061 6e64 2065 6e74 6572  ope``` and enter
+00000e80: 696e 6720 7468 6520 726f 6f66 2073 6c6f  ing the roof slo
+00000e90: 7065 2069 6e20 696e 6368 6573 2f66 6f6f  pe in inches/foo
+00000ea0: 742e 2054 6865 0d0a 6465 6661 756c 7420  t. The..default 
+00000eb0: 7661 6c75 6520 6973 2060 6060 302e 3235  value is ```0.25
+00000ec0: 6060 602e 0d0a 0d0a 4e65 7874 2c20 6465  ```.....Next, de
+00000ed0: 6669 6e65 2074 6865 206c 6f61 6469 6e67  fine the loading
+00000ee0: 2069 6e20 7468 6520 726f 6f66 2062 6179   in the roof bay
+00000ef0: 2e0d 0a60 6060 7079 7468 6f6e 0d0a 705f  ...```python..p_
+00000f00: 6672 616d 696e 6720 3d20 5072 696d 6172  framing = Primar
+00000f10: 7946 7261 6d69 6e67 285b 705f 6769 7264  yFraming([p_gird
+00000f20: 6572 312c 2070 5f67 6972 6465 7232 5d29  er1, p_girder2])
+00000f30: 0d0a 735f 6672 616d 696e 6720 3d20 5365  ..s_framing = Se
+00000f40: 636f 6e64 6172 7946 7261 6d69 6e67 285b  condaryFraming([
+00000f50: 735f 6265 616d 312c 2073 5f6a 6f69 7374  s_beam1, s_joist
+00000f60: 312c 2073 5f6a 6f69 7374 322c 2073 5f6a  1, s_joist2, s_j
+00000f70: 6f69 7374 332c 2073 5f62 6561 6d32 5d29  oist3, s_beam2])
+00000f80: 0d0a 0d0a 715f 646c 203d 2032 302f 3130  ....q_dl = 20/10
+00000f90: 3030 2f31 3434 2023 2053 7572 6661 6365  00/144 # Surface
+00000fa0: 2064 6561 6420 6c6f 6164 2069 6e20 6b73   dead load in ks
+00000fb0: 690d 0a71 5f72 6c20 3d20 3232 2e34 2f31  i..q_rl = 22.4/1
+00000fc0: 3030 302f 3134 3420 2320 5375 7266 6163  000/144 # Surfac
+00000fd0: 6520 7261 696e 206c 6f61 6420 6174 2073  e rain load at s
+00000fe0: 6563 6f6e 6461 7279 2064 7261 696e 6167  econdary drainag
+00000ff0: 6520 696e 6c65 7420 696e 206b 7369 0d0a  e inlet in ksi..
+00001000: 0d0a 6c6f 6164 696e 6720 3d20 4c6f 6164  ..loading = Load
+00001010: 696e 6728 715f 646c 2c20 715f 726c 290d  ing(q_dl, q_rl).
+00001020: 0a60 6060 0d0a 5468 6520 696e 7075 7420  .```..The input 
+00001030: 7261 696e 206c 6f61 6420 7368 6f75 6c64  rain load should
+00001040: 2069 6e63 6c75 6465 2074 6865 2073 7461   include the sta
+00001050: 7469 6320 6865 6164 2061 6e64 2074 6865  tic head and the
+00001060: 2068 7964 7261 756c 6963 2068 6561 642c   hydraulic head,
+00001070: 2062 7574 0d0a 6e6f 2070 6f6e 6469 6e67   but..no ponding
+00001080: 2068 6561 642e 0d0a 0d0a 4669 6e61 6c6c   head.....Finall
+00001090: 792c 2064 6566 696e 6520 7468 6520 6060  y, define the ``
+000010a0: 6050 6f6e 6450 794d 6f64 656c 6060 6020  `PondPyModel``` 
+000010b0: 6f62 6a65 6374 2061 6e64 2061 6e61 6c79  object and analy
+000010c0: 7a65 2074 6865 206d 6f64 656c 2e0d 0a60  ze the model...`
+000010d0: 6060 7079 7468 6f6e 0d0a 706f 6e64 7079  ``python..pondpy
+000010e0: 5f6d 6f64 656c 203d 2050 6f6e 6450 794d  _model = PondPyM
+000010f0: 6f64 656c 2870 5f66 7261 6d69 6e67 2c20  odel(p_framing, 
+00001100: 735f 6672 616d 696e 672c 206c 6f61 6469  s_framing, loadi
+00001110: 6e67 290d 0a0d 0a70 6f6e 6470 795f 6d6f  ng)....pondpy_mo
+00001120: 6465 6c2e 7065 7266 6f72 6d5f 616e 616c  del.perform_anal
+00001130: 7973 6973 2829 0d0a 6060 600d 0a4f 7074  ysis()..```..Opt
+00001140: 696f 6e61 6c20 6172 6775 6d65 6e74 7320  ional arguments 
+00001150: 666f 7220 7468 6520 6060 6050 6f6e 6450  for the ```PondP
+00001160: 794d 6f64 656c 6060 6020 696e 636c 7564  yModel``` includ
+00001170: 653a 0d0a 0d0a 2d20 6060 606d 6972 726f  e:....- ```mirro
+00001180: 7265 645f 6c65 6674 6060 603a 2062 6f6f  red_left```: boo
+00001190: 6c20 696e 6469 6361 7469 6e67 2077 6865  l indicating whe
+000011a0: 7468 6572 2074 6865 2072 6f6f 6620 6261  ther the roof ba
+000011b0: 7920 6973 206d 6972 726f 7265 640d 0a20  y is mirrored.. 
+000011c0: 2020 206f 6e20 7468 6520 6c65 6674 2073     on the left s
+000011d0: 6964 653b 2064 6566 6175 6c74 2069 7320  ide; default is 
+000011e0: 6060 6046 616c 7365 6060 600d 0a0d 0a2d  ```False```....-
+000011f0: 2060 6060 6d69 7272 6f72 6564 5f72 6967   ```mirrored_rig
+00001200: 6874 6060 6020 3a20 626f 6f6c 2069 6e64  ht``` : bool ind
+00001210: 6963 6174 696e 6720 7768 6574 6865 7220  icating whether 
+00001220: 7468 6520 726f 6f66 2062 6179 2069 7320  the roof bay is 
+00001230: 6d69 7272 6f72 6564 0d0a 2020 2020 6f6e  mirrored..    on
+00001240: 2074 6865 2072 6967 6874 2073 6964 653b   the right side;
+00001250: 2064 6566 6175 6c74 2069 7320 6060 6046   default is ```F
+00001260: 616c 7365 6060 600d 0a0d 0a2d 2060 6060  alse```....- ```
+00001270: 7374 6f70 5f63 7269 7465 7269 6f6e 6060  stop_criterion``
+00001280: 6020 3a20 666c 6f61 7420 696e 6469 6361  ` : float indica
+00001290: 7469 6e67 2074 6865 2065 7272 6f72 2069  ting the error i
+000012a0: 6e20 746f 7461 6c20 696d 706f 756e 6465  n total impounde
+000012b0: 640d 0a20 2020 2077 6174 6572 2077 6569  d..    water wei
+000012c0: 6768 7420 6174 2077 6869 6368 2074 6865  ght at which the
+000012d0: 2069 7465 7261 7469 7665 2061 6e61 6c79   iterative analy
+000012e0: 7369 7320 7368 6f75 6c64 2062 6520 7465  sis should be te
+000012f0: 726d 696e 6174 6564 3b0d 0a20 2020 2064  rminated;..    d
+00001300: 6566 6175 6c74 2069 7320 6060 6030 2e30  efault is ```0.0
+00001310: 3030 3160 6060 0d0a 0d0a 2d20 6060 606d  001```....- ```m
+00001320: 6178 5f69 7465 7260 6060 203a 2069 6e74  ax_iter``` : int
+00001330: 2069 6e64 6963 6174 696e 6720 7468 6520   indicating the 
+00001340: 6d61 7869 6d75 6d20 6e75 6d62 6572 206f  maximum number o
+00001350: 6620 6974 6572 6174 696f 6e73 2074 6861  f iterations tha
+00001360: 740d 0a20 2020 2073 686f 756c 6420 6265  t..    should be
+00001370: 2070 6572 666f 726d 6564 3b20 6465 6661   performed; defa
+00001380: 756c 7420 6973 2060 6060 3530 6060 600d  ult is ```50```.
+00001390: 0a20 2020 200d 0a2d 2060 6060 7368 6f77  .    ..- ```show
+000013a0: 5f72 6573 756c 7473 6060 6020 3a20 626f  _results``` : bo
+000013b0: 6f6c 2069 6e64 6963 6174 696e 6720 7768  ol indicating wh
+000013c0: 6574 6865 7220 7468 6520 6974 6572 6174  ether the iterat
+000013d0: 696f 6e20 7265 7375 6c74 7320 7368 6f75  ion results shou
+000013e0: 6c64 0d0a 2020 2020 6265 2070 7269 6e74  ld..    be print
+000013f0: 6564 2074 6f20 7468 6520 7465 726d 696e  ed to the termin
+00001400: 616c 2075 706f 6e20 636f 6d70 6c65 7469  al upon completi
+00001410: 6f6e 206f 6620 7468 6520 616e 616c 7973  on of the analys
+00001420: 6973 3b0d 0a20 2020 2064 6566 6175 6c74  is;..    default
+00001430: 2069 7320 6060 6054 7275 6560 6060 0d0a   is ```True```..
+00001440: 0d0a 2323 2320 416e 616c 7973 6973 2052  ..### Analysis R
+00001450: 6573 756c 7473 0d0a 4561 6368 2070 7269  esults..Each pri
+00001460: 6d61 7279 2061 6e64 2073 6563 6f6e 6461  mary and seconda
+00001470: 7279 206d 656d 6265 7220 6973 2072 6570  ry member is rep
+00001480: 7265 7365 6e74 6564 2077 6974 6869 6e20  resented within 
+00001490: 7468 6520 506f 6e64 5079 4d6f 6465 6c20  the PondPyModel 
+000014a0: 6f62 6a65 6374 0d0a 6279 2061 2042 6561  object..by a Bea
+000014b0: 6d4d 6f64 656c 206f 626a 6563 742e 2041  mModel object. A
+000014c0: 7320 7375 6368 2061 2067 7265 6174 2064  s such a great d
+000014d0: 6561 6c20 6f66 2061 6e61 6c79 7369 7320  eal of analysis 
+000014e0: 7265 7375 6c74 7320 6361 6e20 6265 206f  results can be o
+000014f0: 6274 6169 6e65 640d 0a66 6169 726c 7920  btained..fairly 
+00001500: 6561 7369 6c79 206f 6e63 6520 7468 6520  easily once the 
+00001510: 616e 616c 7973 6973 2069 7320 636f 6d70  analysis is comp
+00001520: 6c65 7465 2e0d 0a0d 0a2d 2054 6f20 6163  lete.....- To ac
+00001530: 6365 7373 2074 6865 2064 6566 6c65 6374  cess the deflect
+00001540: 6564 2073 6861 7065 2c20 7368 6561 7220  ed shape, shear 
+00001550: 666f 7263 6520 6469 6167 7261 6d2c 206f  force diagram, o
+00001560: 7220 6265 6e64 696e 6720 6d6f 6d65 6e74  r bending moment
+00001570: 2064 6961 6772 616d 0d0a 2020 6f66 2061   diagram..  of a
+00001580: 2070 6172 7469 6375 6c61 7220 6d65 6d62   particular memb
+00001590: 6572 2c20 7573 6520 7468 6520 666f 6c6c  er, use the foll
+000015a0: 6f77 696e 6720 6361 6c6c 733a 0d0a 2020  owing calls:..  
+000015b0: 6060 6070 7974 686f 6e0d 0a20 206d 656d  ```python..  mem
+000015c0: 6265 7220 3d20 706f 6e64 7079 5f6d 6f64  ber = pondpy_mod
+000015d0: 656c 2e72 6f6f 665f 6261 795f 6d6f 6465  el.roof_bay_mode
+000015e0: 6c2e 7365 636f 6e64 6172 795f 6d65 6d62  l.secondary_memb
+000015f0: 6572 735b 305d 0d0a 2020 626d 6420 3d20  ers[0]..  bmd = 
+00001600: 6d65 6d62 6572 2e70 6c6f 745f 626d 6428  member.plot_bmd(
+00001610: 290d 0a20 2062 6d64 2e73 686f 7728 290d  )..  bmd.show().
+00001620: 0a20 2060 6060 0d0a 2020 5468 6520 7368  .  ```..  The sh
+00001630: 6561 7220 666f 7263 6520 6469 6167 7261  ear force diagra
+00001640: 6d20 616e 6420 6465 666c 6563 7465 6420  m and deflected 
+00001650: 7368 6170 6520 6361 6e20 6265 2061 6363  shape can be acc
+00001660: 6573 7365 6420 696e 2061 2073 696d 696c  essed in a simil
+00001670: 6172 0d0a 2020 6661 7368 696f 6e20 7573  ar..  fashion us
+00001680: 696e 6720 7468 6520 6060 6070 6c6f 745f  ing the ```plot_
+00001690: 7366 6428 2960 6060 2061 6e64 2060 6060  sfd()``` and ```
+000016a0: 706c 6f74 5f64 6566 6c65 6374 6564 5f73  plot_deflected_s
+000016b0: 6861 7065 2829 6060 6020 6d65 7468 6f64  hape()``` method
+000016c0: 732e 0d0a 0d0a 2020 5468 6520 6465 666c  s.....  The defl
+000016d0: 6563 7465 6420 7368 6170 652c 2073 6865  ected shape, she
+000016e0: 6172 2066 6f72 6365 2064 6961 6772 616d  ar force diagram
+000016f0: 2c20 616e 6420 6265 6e64 696e 6720 6d6f  , and bending mo
+00001700: 6d65 6e74 2064 6961 6772 616d 2070 6c6f  ment diagram plo
+00001710: 7473 0d0a 2020 666f 7220 616c 6c20 6d65  ts..  for all me
+00001720: 6d62 6572 7320 6361 6e20 616c 6c20 6265  mbers can all be
+00001730: 2067 656e 6572 6174 6564 2062 7920 7573   generated by us
+00001740: 696e 6720 7468 6520 6060 6052 6f6f 6642  ing the ```RoofB
+00001750: 6179 4d6f 6465 6c60 6060 2773 0d0a 2020  ayModel```'s..  
+00001760: 6060 6067 656e 6572 6174 655f 706c 6f74  ```generate_plot
+00001770: 7328 2960 6060 206d 6574 686f 642e 0d0a  s()``` method...
+00001780: 0d0a 2020 6060 6070 7974 686f 6e0d 0a20  ..  ```python.. 
+00001790: 2070 6c6f 7473 203d 2070 6f6e 6470 795f   plots = pondpy_
+000017a0: 6d6f 6465 6c2e 726f 6f66 5f62 6179 5f6d  model.roof_bay_m
+000017b0: 6f64 656c 2e67 656e 6572 6174 655f 706c  odel.generate_pl
+000017c0: 6f74 7328 290d 0a20 2060 6060 0d0a 0d0a  ots()..  ```....
+000017d0: 2020 5468 6973 206d 6574 686f 6420 7265    This method re
+000017e0: 7475 726e 7320 6120 6060 6064 6963 7460  turns a ```dict`
+000017f0: 6060 206f 626a 6563 7420 7769 7468 206b  `` object with k
+00001800: 6579 7320 6060 6062 6d64 6060 602c 2060  eys ```bmd```, `
+00001810: 6060 7366 6460 6060 2c20 616e 640d 0a20  ``sfd```, and.. 
+00001820: 2060 6060 6465 666c 6060 2c20 6561 6368   ```defl``, each
+00001830: 206f 6620 7768 6963 6820 6973 2061 7373   of which is ass
+00001840: 6f63 6961 7465 6420 7769 7468 2061 2073  ociated with a s
+00001850: 7562 2d64 6963 7469 6f6e 6172 7920 7769  ub-dictionary wi
+00001860: 7468 206b 6579 730d 0a20 2060 6060 5072  th keys..  ```Pr
+00001870: 696d 6172 7960 6060 2061 6e64 2060 6060  imary``` and ```
+00001880: 5365 636f 6e64 6172 7960 6060 2e20 4561  Secondary```. Ea
+00001890: 6368 2073 7562 2d64 6963 7469 6f6e 6172  ch sub-dictionar
+000018a0: 7920 636f 6e74 6169 6e73 2061 206c 6973  y contains a lis
+000018b0: 7420 6f66 0d0a 2020 7468 6520 6173 736f  t of..  the asso
+000018c0: 6369 6174 6564 2070 6c6f 7420 666f 7220  ciated plot for 
+000018d0: 6561 6368 2070 7269 6d61 7279 206f 7220  each primary or 
+000018e0: 7365 636f 6e64 6172 7920 6d65 6d62 6572  secondary member
+000018f0: 2c20 6173 2061 7070 6c69 6361 626c 652e  , as applicable.
+00001900: 0d0a 0d0a 2d20 5468 6520 7375 7070 6f72  ....- The suppor
+00001910: 7420 7265 6163 7469 6f6e 7320 6361 6e20  t reactions can 
+00001920: 6265 206f 6274 6169 6e65 6420 6173 2066  be obtained as f
+00001930: 6f6c 6c6f 7773 3a0d 0a20 2060 6060 7079  ollows:..  ```py
+00001940: 7468 6f6e 0d0a 2020 7375 7070 6f72 745f  thon..  support_
+00001950: 6e6f 6465 7320 3d20 6d65 6d62 6572 2e73  nodes = member.s
+00001960: 7570 706f 7274 5f6e 6f64 6573 0d0a 2020  upport_nodes..  
+00001970: 7375 7070 6f72 745f 7265 6163 7469 6f6e  support_reaction
+00001980: 7320 3d20 5b6d 656d 6265 722e 7375 7070  s = [member.supp
+00001990: 6f72 745f 7265 6163 7469 6f6e 735b 6e6f  ort_reactions[no
+000019a0: 6465 5d20 666f 7220 6e6f 6465 2069 6e20  de] for node in 
+000019b0: 7375 7070 6f72 745f 6e6f 6465 735d 0d0a  support_nodes]..
+000019c0: 2020 6060 600d 0a0d 0a53 6576 6572 616c    ```....Several
+000019d0: 206f 7468 6572 2061 7474 7269 6275 7465   other attribute
+000019e0: 7320 6f66 2074 6865 2042 6561 6d4d 6f64  s of the BeamMod
+000019f0: 656c 206f 626a 6563 7420 6361 6e20 6265  el object can be
+00001a00: 2061 6363 6573 7365 6420 696e 2061 2073   accessed in a s
+00001a10: 696d 696c 6172 0d0a 6661 7368 696f 6e2e  imilar..fashion.
+00001a20: 0d0a 0d0a 4e6f 7465 2074 6861 7420 6f6e  ....Note that on
+00001a30: 6c79 2074 6865 2066 696e 616c 2061 6e61  ly the final ana
+00001a40: 6c79 7369 7320 7265 7375 6c74 7320 6361  lysis results ca
+00001a50: 6e20 6375 7272 656e 746c 7920 6265 2061  n currently be a
+00001a60: 6363 6573 7365 642e 0d0a 0d0a 2323 2320  ccessed.....### 
+00001a70: 4164 6469 7469 6f6e 616c 2049 6e66 6f72  Additional Infor
+00001a80: 6d61 7469 6f6e 0d0a 2d20 5b44 6f63 756d  mation..- [Docum
+00001a90: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
+00001aa0: 2f2f 706f 6e64 7079 2e72 6561 6474 6865  //pondpy.readthe
+00001ab0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00001ac0: 742f 290d 0a2d 205b 5079 5049 2044 6973  t/)..- [PyPI Dis
+00001ad0: 7472 6962 7574 696f 6e5d 2868 7474 7073  tribution](https
+00001ae0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00001af0: 6563 742f 706f 6e64 7079 2f29 0d0a       ect/pondpy/)..
```

### Comparing `pondpy-0.1.2/PKG-INFO` & `pondpy-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 706f 6e64  : 2.1.Name: pond
 00000020: 7079 0a56 6572 7369 6f6e 3a20 302e 312e  py.Version: 0.1.
-00000030: 320a 5375 6d6d 6172 793a 2050 6163 6b61  2.Summary: Packa
+00000030: 330a 5375 6d6d 6172 793a 2050 6163 6b61  3.Summary: Packa
 00000040: 6765 2074 6f20 6169 6420 696e 2074 6865  ge to aid in the
 00000050: 2064 6573 6967 6e20 6f66 206c 6f77 2d73   design of low-s
 00000060: 6c6f 7065 2072 6f6f 6620 7379 7374 656d  lope roof system
 00000070: 7320 666f 7220 706f 6e64 696e 6720 7374  s for ponding st
 00000080: 6162 696c 6974 7920 616e 6420 696d 706f  ability and impo
 00000090: 756e 6465 6420 7261 696e 206c 6f61 642e  unded rain load.
 000000a0: 0a4c 6963 656e 7365 3a20 4d49 540a 4175  .License: MIT.Au
@@ -21,356 +21,441 @@
 00000140: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
 00000150: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
 00000160: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
 00000170: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
 00000180: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
 00000190: 3a20 5079 7468 6f6e 203a 3a20 332e 3132  : Python :: 3.12
 000001a0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000001b0: 6a6f 6973 7470 7920 283d 3d30 2e31 2e34  joistpy (==0.1.4
+000001b0: 6a6f 6973 7470 7920 283d 3d31 2e30 2e30  joistpy (==1.0.0
 000001c0: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
 000001d0: 206d 6174 706c 6f74 6c69 6220 283d 3d33   matplotlib (==3
 000001e0: 2e39 2e30 290a 5265 7175 6972 6573 2d44  .9.0).Requires-D
 000001f0: 6973 743a 206e 756d 7079 2028 3d3d 312e  ist: numpy (==1.
 00000200: 3236 2e34 290a 5265 7175 6972 6573 2d44  26.4).Requires-D
 00000210: 6973 743a 2073 6369 7079 2028 3d3d 312e  ist: scipy (==1.
 00000220: 3133 2e31 290a 5265 7175 6972 6573 2d44  13.1).Requires-D
 00000230: 6973 743a 2073 7465 656c 7079 2028 3d3d  ist: steelpy (==
 00000240: 312e 312e 3129 0a44 6573 6372 6970 7469  1.1.1).Descripti
 00000250: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
 00000260: 2074 6578 742f 6d61 726b 646f 776e 0a0a   text/markdown..
-00000270: 2320 506f 6e64 5079 0a50 6f6e 6450 7920  # PondPy.PondPy 
-00000280: 6973 2061 2070 6163 6b61 6765 2062 7569  is a package bui
-00000290: 6c74 2074 6f20 6169 6420 696e 2074 6865  lt to aid in the
-000002a0: 2064 6573 6967 6e20 6f66 206c 6f77 2d73   design of low-s
-000002b0: 6c6f 7065 2072 6f6f 6620 6261 7973 2066  lope roof bays f
-000002c0: 6f72 200a 706f 6e64 696e 6720 7374 6162  or .ponding stab
-000002d0: 696c 6974 7920 616e 6420 696d 706f 756e  ility and impoun
-000002e0: 6465 6420 7261 696e 206c 6f61 6469 6e67  ded rain loading
-000002f0: 2e20 4974 2075 7469 6c69 7a65 7320 6120  . It utilizes a 
-00000300: 7365 7269 6573 206f 660a 7075 7270 6f73  series of.purpos
-00000310: 652d 6275 696c 7420 6669 6e69 7465 2065  e-built finite e
-00000320: 6c65 6d65 6e74 2061 6e64 2070 6f6e 6469  lement and pondi
-00000330: 6e67 2061 6e61 6c79 7369 7320 636c 6173  ng analysis clas
-00000340: 7365 7320 616e 6420 6d65 7468 6f64 7320  ses and methods 
-00000350: 746f 2062 650a 6173 2069 6e74 7569 7469  to be.as intuiti
-00000360: 7665 2061 7320 706f 7373 6962 6c65 2066  ve as possible f
-00000370: 6f72 2074 6865 206d 6f64 6572 6e20 656e  or the modern en
-00000380: 6769 6e65 6572 2e0a 0a23 2323 2049 6e73  gineer...### Ins
-00000390: 7461 6c6c 6174 696f 6e0a 496e 7374 616c  tallation.Instal
-000003a0: 6c20 706f 6e64 7079 2077 6974 6820 7069  l pondpy with pi
-000003b0: 703a 0a60 6060 6261 7368 0a70 6970 2069  p:.```bash.pip i
-000003c0: 6e73 7461 6c6c 2070 6f6e 6470 790a 6060  nstall pondpy.``
-000003d0: 600a 0a23 2323 2055 7361 6765 0a54 6865  `..### Usage.The
-000003e0: 2050 6f6e 6450 794d 6f64 656c 2063 6c61   PondPyModel cla
-000003f0: 7373 2069 7320 6465 7369 676e 6564 2074  ss is designed t
-00000400: 6f20 776f 726b 2077 6974 6820 7365 7665  o work with seve
-00000410: 7261 6c20 7075 7270 6f73 652d 6275 696c  ral purpose-buil
-00000420: 7420 636c 6173 7365 730a 7468 6174 2068  t classes.that h
-00000430: 656c 7020 7468 6520 7573 6572 206f 7267  elp the user org
-00000440: 616e 697a 6520 7468 6569 7220 696e 7075  anize their inpu
-00000450: 7420 696e 746f 2061 2066 6f72 6d20 7468  t into a form th
-00000460: 6174 2061 7265 2072 6561 6469 6c79 2075  at are readily u
-00000470: 7469 6c69 7a65 640a 746f 2062 7569 6c64  tilized.to build
-00000480: 2061 6e64 2061 6e61 6c79 7a65 2074 6865   and analyze the
-00000490: 206d 6f64 656c 2e20 5468 6573 6520 6172   model. These ar
-000004a0: 6520 7468 6520 6060 6050 7269 6d61 7279  e the ```Primary
-000004b0: 4672 616d 696e 6760 6060 2c0a 6060 6053  Framing```,.```S
-000004c0: 6563 6f6e 6461 7279 4672 616d 696e 6760  econdaryFraming`
-000004d0: 6060 2c20 616e 6420 6060 604c 6f61 6469  ``, and ```Loadi
-000004e0: 6e67 6060 6020 636c 6173 7365 732e 2049  ng``` classes. I
-000004f0: 6e20 6164 6469 7469 6f6e 2c20 7468 6520  n addition, the 
-00000500: 7061 636b 6167 6520 6973 0a64 6573 6967  package is.desig
-00000510: 6e65 6420 746f 2077 6f72 6b20 7769 7468  ned to work with
-00000520: 2074 6865 2060 6060 7374 6565 6c70 7960   the ```steelpy`
-00000530: 6060 2061 6e64 2060 6060 6a6f 6973 7470  `` and ```joistp
-00000540: 7960 6060 2070 6163 6b61 6765 732c 2074  y``` packages, t
-00000550: 686f 7567 6820 616e 790a 6f62 6a65 6374  hough any.object
-00000560: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
-00000570: 7265 7175 6972 696e 6720 696e 666f 726d  requiring inform
-00000580: 6174 696f 6e20 6174 7472 6962 7572 6573  ation attribures
-00000590: 2028 692e 652e 206d 6f6d 656e 7420 6f66   (i.e. moment of
-000005a0: 2069 6e65 7274 6961 2c0a 6372 6f73 732d   inertia,.cross-
-000005b0: 7365 6374 696f 6e61 6c20 6172 6561 2c20  sectional area, 
-000005c0: 656c 6173 7469 6320 6d6f 6475 6c75 732c  elastic modulus,
-000005d0: 2065 7463 2e29 2063 6f75 6c64 2062 6520   etc.) could be 
-000005e0: 7573 6564 2069 6e20 6c69 6575 206f 6620  used in lieu of 
-000005f0: 6569 7468 6572 0a70 6163 6b61 6765 2e0a  either.package..
-00000600: 0a54 6f20 6372 6561 7465 2061 6e64 2061  .To create and a
-00000610: 6e61 6c79 7a65 2061 2072 6f6f 6620 6261  nalyze a roof ba
-00000620: 7920 6d6f 6465 6c2c 2066 6972 7374 2069  y model, first i
-00000630: 6d70 6f72 7420 7468 6520 7265 7175 6972  mport the requir
-00000640: 6564 2064 6570 656e 6465 6e63 6965 730a  ed dependencies.
-00000650: 616e 6420 636c 6173 7365 733a 0a60 6060  and classes:.```
-00000660: 7079 7468 6f6e 0a66 726f 6d20 6a6f 6973  python.from jois
-00000670: 7470 7920 696d 706f 7274 2073 6a69 0a66  tpy import sji.f
-00000680: 726f 6d20 7374 6565 6c70 7920 696d 706f  rom steelpy impo
-00000690: 7274 2061 6973 630a 0a66 726f 6d20 706f  rt aisc..from po
-000006a0: 6e64 7079 2e61 6e61 6c79 7369 732e 6665  ndpy.analysis.fe
-000006b0: 6d5f 616e 616c 7973 6973 2069 6d70 6f72  m_analysis impor
-000006c0: 7420 280a 2020 2020 5374 6565 6c42 6561  t (.    SteelBea
-000006d0: 6d53 697a 652c 0a20 2020 2053 7465 656c  mSize,.    Steel
-000006e0: 4a6f 6973 7453 697a 652c 0a29 0a0a 6672  JoistSize,.)..fr
-000006f0: 6f6d 2070 6f6e 6470 792e 616e 616c 7973  om pondpy.analys
-00000700: 6973 2e70 6f6e 645f 616e 616c 7973 6973  is.pond_analysis
-00000710: 2069 6d70 6f72 7420 280a 2020 2020 5072   import (.    Pr
-00000720: 696d 6172 794d 656d 6265 722c 0a20 2020  imaryMember,.   
-00000730: 2050 7269 6d61 7279 4672 616d 696e 672c   PrimaryFraming,
-00000740: 0a20 2020 2053 6563 6f6e 6461 7279 4d65  .    SecondaryMe
-00000750: 6d62 6572 2c0a 2020 2020 5365 636f 6e64  mber,.    Second
-00000760: 6172 7946 7261 6d69 6e67 2c0a 2020 2020  aryFraming,.    
-00000770: 4c6f 6164 696e 670a 290a 0a66 726f 6d20  Loading.)..from 
-00000780: 706f 6e64 7079 2e70 6f6e 6470 7920 696d  pondpy.pondpy im
-00000790: 706f 7274 2050 6f6e 6450 794d 6f64 656c  port PondPyModel
-000007a0: 0a60 6060 0a0a 4e65 7874 2c20 6465 6669  .```..Next, defi
-000007b0: 6e65 2074 6865 2073 7465 656c 2073 6861  ne the steel sha
-000007c0: 7065 7320 616e 6420 6a6f 6973 7420 6465  pes and joist de
-000007d0: 7369 676e 6174 696f 6e73 2069 6e20 796f  signations in yo
-000007e0: 7572 206d 6f64 656c 2e0a 6060 6070 7974  ur model..```pyt
-000007f0: 686f 6e0a 7731 3278 3136 203d 2053 7465  hon.w12x16 = Ste
-00000800: 656c 4265 616d 5369 7a65 2827 5731 3258  elBeamSize('W12X
-00000810: 3136 272c 2061 6973 632e 575f 7368 6170  16', aisc.W_shap
-00000820: 6573 2e57 3132 5831 3629 0a77 3136 7832  es.W12X16).w16x2
-00000830: 3620 3d20 5374 6565 6c42 6561 6d53 697a  6 = SteelBeamSiz
-00000840: 6528 2757 3136 5832 3627 2c20 6169 7363  e('W16X26', aisc
-00000850: 2e57 5f73 6861 7065 732e 5731 3658 3236  .W_shapes.W16X26
-00000860: 290a 6b5f 3134 6b31 203d 2053 7465 656c  ).k_14k1 = Steel
-00000870: 4a6f 6973 7453 697a 6528 2731 344b 3127  JoistSize('14K1'
-00000880: 2c20 736a 692e 4b5f 5365 7269 6573 2e4b  , sji.K_Series.K
-00000890: 5f31 344b 3129 0a60 6060 0a0a 4e65 7874  _14K1).```..Next
-000008a0: 2c20 6465 6669 6e65 2074 6865 2070 7269  , define the pri
-000008b0: 6d61 7279 2061 6e64 2073 6563 6f6e 6461  mary and seconda
-000008c0: 7279 2066 7261 6d69 6e67 2069 6e20 7468  ry framing in th
-000008d0: 6520 726f 6f66 2062 6179 2066 7261 6d69  e roof bay frami
-000008e0: 6e67 2073 7973 7465 6d2e 200a 4e6f 7465  ng system. .Note
-000008f0: 2074 6861 7420 616c 6c20 696e 7075 7473   that all inputs
-00000900: 2073 686f 756c 6420 6265 2069 6e20 6b69   should be in ki
-00000910: 7073 2061 6e64 2069 6e63 6865 732e 0a60  ps and inches..`
-00000920: 6060 7079 7468 6f6e 0a70 5f6c 656e 6774  ``python.p_lengt
-00000930: 6820 3d20 3230 2a31 3220 2320 6c65 6e67  h = 20*12 # leng
-00000940: 7468 206f 6620 7072 696d 6172 7920 6d65  th of primary me
-00000950: 6d62 6572 7320 696e 2069 6e63 6865 730a  mbers in inches.
-00000960: 735f 6c65 6e67 7468 203d 2032 302a 3132  s_length = 20*12
-00000970: 2023 206c 656e 6774 6820 6f66 2073 6563   # length of sec
-00000980: 6f6e 6461 7279 206d 656d 6265 7273 2069  ondary members i
-00000990: 6e20 696e 6368 6573 0a0a 2320 5375 7070  n inches..# Supp
-000009a0: 6f72 7420 7479 7065 7320 6172 6520 6465  ort types are de
-000009b0: 7369 676e 6174 6564 2062 7920 7475 706c  signated by tupl
-000009c0: 6573 2072 6570 7265 7365 6e74 696e 6720  es representing 
-000009d0: 2854 782c 2054 792c 2052 7a29 2e0a 2320  (Tx, Ty, Rz)..# 
-000009e0: 4120 3020 696e 6469 6361 7465 7320 7468  A 0 indicates th
-000009f0: 6520 6465 6772 6565 206f 6620 6672 6565  e degree of free
-00000a00: 646f 6d20 6973 2075 6e72 6573 7472 6169  dom is unrestrai
-00000a10: 6e65 6420 7768 696c 6520 6120 3120 696e  ned while a 1 in
-00000a20: 6469 6361 7465 7320 6120 0a23 2072 6573  dicates a .# res
-00000a30: 7472 6169 6e65 6420 6465 6772 6565 206f  trained degree o
-00000a40: 6620 6672 6565 646f 6d2e 0a70 5f73 7570  f freedom..p_sup
-00000a50: 706f 7274 203d 205b 5b30 2c20 2831 2c20  port = [[0, (1, 
-00000a60: 312c 2030 295d 2c20 5b70 5f6c 656e 6774  1, 0)], [p_lengt
-00000a70: 682c 2028 312c 2031 2c20 3029 5d5d 0a73  h, (1, 1, 0)]].s
-00000a80: 5f73 7570 706f 7274 203d 205b 5b30 2c20  _support = [[0, 
-00000a90: 2831 2c20 312c 2030 295d 2c20 5b73 5f6c  (1, 1, 0)], [s_l
-00000aa0: 656e 6774 682c 2028 312c 2031 2c20 3029  ength, (1, 1, 0)
-00000ab0: 5d5d 0a0a 705f 6769 7264 6572 3120 3d20  ]]..p_girder1 = 
-00000ac0: 5072 696d 6172 794d 656d 6265 7228 705f  PrimaryMember(p_
-00000ad0: 6c65 6e67 7468 2c20 7731 3678 3236 2c20  length, w16x26, 
-00000ae0: 705f 7375 7070 6f72 7429 0a70 5f67 6972  p_support).p_gir
-00000af0: 6465 7232 203d 2050 7269 6d61 7279 4d65  der2 = PrimaryMe
-00000b00: 6d62 6572 2870 5f6c 656e 6774 682c 2077  mber(p_length, w
-00000b10: 3136 7832 362c 2070 5f73 7570 706f 7274  16x26, p_support
-00000b20: 290a 735f 6265 616d 3120 3d20 5365 636f  ).s_beam1 = Seco
-00000b30: 6e64 6172 794d 656d 6265 7228 735f 6c65  ndaryMember(s_le
-00000b40: 6e67 7468 2c20 7731 3278 3136 2c20 735f  ngth, w12x16, s_
-00000b50: 7375 7070 6f72 7429 0a73 5f62 6561 6d32  support).s_beam2
-00000b60: 203d 2053 6563 6f6e 6461 7279 4d65 6d62   = SecondaryMemb
-00000b70: 6572 2873 5f6c 656e 6774 682c 2077 3132  er(s_length, w12
-00000b80: 7831 362c 2073 5f73 7570 706f 7274 290a  x16, s_support).
-00000b90: 735f 6a6f 6973 7431 203d 2053 6563 6f6e  s_joist1 = Secon
-00000ba0: 6461 7279 4d65 6d62 6572 2873 5f6c 656e  daryMember(s_len
-00000bb0: 6774 682c 206b 5f31 346b 312c 2073 5f73  gth, k_14k1, s_s
-00000bc0: 7570 706f 7274 290a 735f 6a6f 6973 7432  upport).s_joist2
-00000bd0: 203d 2053 6563 6f6e 6461 7279 4d65 6d62   = SecondaryMemb
-00000be0: 6572 2873 5f6c 656e 6774 682c 206b 5f31  er(s_length, k_1
-00000bf0: 346b 312c 2073 5f73 7570 706f 7274 290a  4k1, s_support).
-00000c00: 735f 6a6f 6973 7433 203d 2053 6563 6f6e  s_joist3 = Secon
-00000c10: 6461 7279 4d65 6d62 6572 2873 5f6c 656e  daryMember(s_len
-00000c20: 6774 682c 206b 5f31 346b 312c 2073 5f73  gth, k_14k1, s_s
-00000c30: 7570 706f 7274 290a 0a70 5f66 7261 6d69  upport)..p_frami
-00000c40: 6e67 203d 2050 7269 6d61 7279 4672 616d  ng = PrimaryFram
-00000c50: 696e 6728 5b70 5f67 6972 6465 7231 2c20  ing([p_girder1, 
-00000c60: 705f 6769 7264 6572 325d 290a 735f 6672  p_girder2]).s_fr
-00000c70: 616d 696e 6720 3d20 5365 636f 6e64 6172  aming = Secondar
-00000c80: 7946 7261 6d69 6e67 285b 735f 6265 616d  yFraming([s_beam
-00000c90: 312c 2073 5f6a 6f69 7374 312c 2073 5f6a  1, s_joist1, s_j
-00000ca0: 6f69 7374 322c 2073 5f6a 6f69 7374 332c  oist2, s_joist3,
-00000cb0: 2073 5f62 6561 6d32 5d29 0a60 6060 0a4e   s_beam2]).```.N
-00000cc0: 6f74 6520 7468 6174 2065 6163 6820 6d65  ote that each me
-00000cd0: 6d62 6572 2073 686f 756c 6420 6265 2069  mber should be i
-00000ce0: 6e64 6976 6964 7561 6c6c 7920 6465 6669  ndividually defi
-00000cf0: 6e65 6420 6173 2073 686f 776e 2061 626f  ned as shown abo
-00000d00: 7665 2e20 4f74 6865 7277 6973 652c 0a74  ve. Otherwise,.t
-00000d10: 6865 206c 6f61 6469 6e67 7320 7769 6c6c  he loadings will
-00000d20: 206e 6f74 2062 6520 6170 706c 6965 6420   not be applied 
-00000d30: 636f 7272 6563 746c 7920 746f 2074 6865  correctly to the
-00000d40: 206d 656d 6265 7273 2e0a 0a54 6865 2072   members...The r
-00000d50: 6f6f 6620 736c 6f70 6520 6361 6e20 6f70  oof slope can op
-00000d60: 7469 6f6e 616c 6c79 2062 6520 7365 7420  tionally be set 
-00000d70: 696e 2074 6865 2060 6060 5365 636f 6e64  in the ```Second
-00000d80: 6172 7946 7261 6d69 6e67 6060 6020 6f62  aryFraming``` ob
-00000d90: 6a65 6374 2062 790a 7573 696e 6720 7468  ject by.using th
-00000da0: 6520 6b65 7977 6f72 6420 6060 6073 6c6f  e keyword ```slo
-00000db0: 7065 6060 6020 616e 6420 656e 7465 7269  pe``` and enteri
-00000dc0: 6e67 2074 6865 2072 6f6f 6620 736c 6f70  ng the roof slop
-00000dd0: 6520 696e 2069 6e63 6865 732f 666f 6f74  e in inches/foot
-00000de0: 2e20 5468 650a 6465 6661 756c 7420 7661  . The.default va
-00000df0: 6c75 6520 6973 2060 6060 302e 3235 6060  lue is ```0.25``
-00000e00: 602e 0a0a 4e65 7874 2c20 6465 6669 6e65  `...Next, define
-00000e10: 2074 6865 206c 6f61 6469 6e67 2069 6e20   the loading in 
-00000e20: 7468 6520 726f 6f66 2062 6179 2e0a 6060  the roof bay..``
-00000e30: 6070 7974 686f 6e0a 705f 6672 616d 696e  `python.p_framin
-00000e40: 6720 3d20 5072 696d 6172 7946 7261 6d69  g = PrimaryFrami
-00000e50: 6e67 285b 705f 6769 7264 6572 312c 2070  ng([p_girder1, p
-00000e60: 5f67 6972 6465 7232 5d29 0a73 5f66 7261  _girder2]).s_fra
-00000e70: 6d69 6e67 203d 2053 6563 6f6e 6461 7279  ming = Secondary
-00000e80: 4672 616d 696e 6728 5b73 5f62 6561 6d31  Framing([s_beam1
-00000e90: 2c20 735f 6a6f 6973 7431 2c20 735f 6a6f  , s_joist1, s_jo
-00000ea0: 6973 7432 2c20 735f 6a6f 6973 7433 2c20  ist2, s_joist3, 
-00000eb0: 735f 6265 616d 325d 290a 0a71 5f64 6c20  s_beam2])..q_dl 
-00000ec0: 3d20 3230 2f31 3030 302f 3134 3420 2320  = 20/1000/144 # 
-00000ed0: 5375 7266 6163 6520 6465 6164 206c 6f61  Surface dead loa
-00000ee0: 6420 696e 206b 7369 0a71 5f72 6c20 3d20  d in ksi.q_rl = 
-00000ef0: 3232 2e34 2f31 3030 302f 3134 3420 2320  22.4/1000/144 # 
-00000f00: 5375 7266 6163 6520 7261 696e 206c 6f61  Surface rain loa
-00000f10: 6420 6174 2073 6563 6f6e 6461 7279 2064  d at secondary d
-00000f20: 7261 696e 6167 6520 696e 6c65 7420 696e  rainage inlet in
-00000f30: 206b 7369 0a0a 6c6f 6164 696e 6720 3d20   ksi..loading = 
-00000f40: 4c6f 6164 696e 6728 715f 646c 2c20 715f  Loading(q_dl, q_
-00000f50: 726c 290a 6060 600a 5468 6520 696e 7075  rl).```.The inpu
-00000f60: 7420 7261 696e 206c 6f61 6420 7368 6f75  t rain load shou
-00000f70: 6c64 2069 6e63 6c75 6465 2074 6865 2073  ld include the s
-00000f80: 7461 7469 6320 6865 6164 2061 6e64 2074  tatic head and t
-00000f90: 6865 2068 7964 7261 756c 6963 2068 6561  he hydraulic hea
-00000fa0: 642c 2062 7574 0a6e 6f20 706f 6e64 696e  d, but.no pondin
-00000fb0: 6720 6865 6164 2e0a 0a46 696e 616c 6c79  g head...Finally
-00000fc0: 2c20 6465 6669 6e65 2074 6865 2060 6060  , define the ```
-00000fd0: 506f 6e64 5079 4d6f 6465 6c60 6060 206f  PondPyModel``` o
-00000fe0: 626a 6563 7420 616e 6420 616e 616c 797a  bject and analyz
-00000ff0: 6520 7468 6520 6d6f 6465 6c2e 0a60 6060  e the model..```
-00001000: 7079 7468 6f6e 0a70 6f6e 6470 795f 6d6f  python.pondpy_mo
-00001010: 6465 6c20 3d20 506f 6e64 5079 4d6f 6465  del = PondPyMode
-00001020: 6c28 705f 6672 616d 696e 672c 2073 5f66  l(p_framing, s_f
-00001030: 7261 6d69 6e67 2c20 6c6f 6164 696e 6729  raming, loading)
-00001040: 0a0a 706f 6e64 7079 5f6d 6f64 656c 2e70  ..pondpy_model.p
-00001050: 6572 666f 726d 5f61 6e61 6c79 7369 7328  erform_analysis(
-00001060: 290a 6060 600a 4f70 7469 6f6e 616c 2061  ).```.Optional a
-00001070: 7267 756d 656e 7473 2066 6f72 2074 6865  rguments for the
-00001080: 2060 6060 506f 6e64 5079 4d6f 6465 6c60   ```PondPyModel`
-00001090: 6060 2069 6e63 6c75 6465 3a0a 0a2d 2060  `` include:..- `
-000010a0: 6060 6d69 7272 6f72 6564 5f6c 6566 7460  ``mirrored_left`
-000010b0: 6060 3a20 626f 6f6c 2069 6e64 6963 6174  ``: bool indicat
-000010c0: 696e 6720 7768 6574 6865 7220 7468 6520  ing whether the 
-000010d0: 726f 6f66 2062 6179 2069 7320 6d69 7272  roof bay is mirr
-000010e0: 6f72 6564 0a20 2020 206f 6e20 7468 6520  ored.    on the 
-000010f0: 6c65 6674 2073 6964 653b 2064 6566 6175  left side; defau
-00001100: 6c74 2069 7320 6060 6046 616c 7365 6060  lt is ```False``
-00001110: 600a 0a2d 2060 6060 6d69 7272 6f72 6564  `..- ```mirrored
-00001120: 5f72 6967 6874 6060 6020 3a20 626f 6f6c  _right``` : bool
-00001130: 2069 6e64 6963 6174 696e 6720 7768 6574   indicating whet
-00001140: 6865 7220 7468 6520 726f 6f66 2062 6179  her the roof bay
-00001150: 2069 7320 6d69 7272 6f72 6564 0a20 2020   is mirrored.   
-00001160: 206f 6e20 7468 6520 7269 6768 7420 7369   on the right si
-00001170: 6465 3b20 6465 6661 756c 7420 6973 2060  de; default is `
-00001180: 6060 4661 6c73 6560 6060 0a0a 2d20 6060  ``False```..- ``
-00001190: 6073 746f 705f 6372 6974 6572 696f 6e60  `stop_criterion`
-000011a0: 6060 203a 2066 6c6f 6174 2069 6e64 6963  `` : float indic
-000011b0: 6174 696e 6720 7468 6520 6572 726f 7220  ating the error 
-000011c0: 696e 2074 6f74 616c 2069 6d70 6f75 6e64  in total impound
-000011d0: 6564 0a20 2020 2077 6174 6572 2077 6569  ed.    water wei
-000011e0: 6768 7420 6174 2077 6869 6368 2074 6865  ght at which the
-000011f0: 2069 7465 7261 7469 7665 2061 6e61 6c79   iterative analy
-00001200: 7369 7320 7368 6f75 6c64 2062 6520 7465  sis should be te
-00001210: 726d 696e 6174 6564 3b0a 2020 2020 6465  rminated;.    de
-00001220: 6661 756c 7420 6973 2060 6060 302e 3030  fault is ```0.00
-00001230: 3031 6060 600a 0a2d 2060 6060 6d61 785f  01```..- ```max_
-00001240: 6974 6572 6060 6020 3a20 696e 7420 696e  iter``` : int in
-00001250: 6469 6361 7469 6e67 2074 6865 206d 6178  dicating the max
-00001260: 696d 756d 206e 756d 6265 7220 6f66 2069  imum number of i
-00001270: 7465 7261 7469 6f6e 7320 7468 6174 0a20  terations that. 
-00001280: 2020 2073 686f 756c 6420 6265 2070 6572     should be per
-00001290: 666f 726d 6564 3b20 6465 6661 756c 7420  formed; default 
-000012a0: 6973 2060 6060 3530 6060 600a 2020 2020  is ```50```.    
-000012b0: 0a2d 2060 6060 7368 6f77 5f72 6573 756c  .- ```show_resul
-000012c0: 7473 6060 6020 3a20 626f 6f6c 2069 6e64  ts``` : bool ind
-000012d0: 6963 6174 696e 6720 7768 6574 6865 7220  icating whether 
-000012e0: 7468 6520 6974 6572 6174 696f 6e20 7265  the iteration re
-000012f0: 7375 6c74 7320 7368 6f75 6c64 0a20 2020  sults should.   
-00001300: 2062 6520 7072 696e 7465 6420 746f 2074   be printed to t
-00001310: 6865 2074 6572 6d69 6e61 6c20 7570 6f6e  he terminal upon
-00001320: 2063 6f6d 706c 6574 696f 6e20 6f66 2074   completion of t
-00001330: 6865 2061 6e61 6c79 7369 733b 0a20 2020  he analysis;.   
-00001340: 2064 6566 6175 6c74 2069 7320 6060 6054   default is ```T
-00001350: 7275 6560 6060 0a0a 2323 2320 416e 616c  rue```..### Anal
-00001360: 7973 6973 2052 6573 756c 7473 0a45 6163  ysis Results.Eac
-00001370: 6820 7072 696d 6172 7920 616e 6420 7365  h primary and se
-00001380: 636f 6e64 6172 7920 6d65 6d62 6572 2069  condary member i
-00001390: 7320 7265 7072 6573 656e 7465 6420 7769  s represented wi
-000013a0: 7468 696e 2074 6865 2050 6f6e 6450 794d  thin the PondPyM
-000013b0: 6f64 656c 206f 626a 6563 740a 6279 2061  odel object.by a
-000013c0: 2042 6561 6d4d 6f64 656c 206f 626a 6563   BeamModel objec
-000013d0: 742e 2041 7320 7375 6368 2061 2067 7265  t. As such a gre
-000013e0: 6174 2064 6561 6c20 6f66 2061 6e61 6c79  at deal of analy
-000013f0: 7369 7320 7265 7375 6c74 7320 6361 6e20  sis results can 
-00001400: 6265 206f 6274 6169 6e65 640a 6661 6972  be obtained.fair
-00001410: 6c79 2065 6173 696c 7920 6f6e 6365 2074  ly easily once t
-00001420: 6865 2061 6e61 6c79 7369 7320 6973 2063  he analysis is c
-00001430: 6f6d 706c 6574 652e 0a0a 2d20 546f 2061  omplete...- To a
-00001440: 6363 6573 7320 7468 6520 6465 666c 6563  ccess the deflec
-00001450: 7465 6420 7368 6170 652c 2073 6865 6172  ted shape, shear
-00001460: 2066 6f72 6365 2064 6961 6772 616d 2c20   force diagram, 
-00001470: 6f72 2062 656e 6469 6e67 206d 6f6d 656e  or bending momen
-00001480: 7420 6469 6167 7261 6d0a 2020 6f66 2061  t diagram.  of a
-00001490: 2070 6172 7469 6375 6c61 7220 6d65 6d62   particular memb
-000014a0: 6572 2c20 7573 6520 7468 6520 666f 6c6c  er, use the foll
-000014b0: 6f77 696e 6720 6361 6c6c 733a 0a20 2060  owing calls:.  `
-000014c0: 6060 7079 7468 6f6e 0a20 206d 656d 6265  ``python.  membe
-000014d0: 7220 3d20 706f 6e64 7079 5f6d 6f64 656c  r = pondpy_model
-000014e0: 2e72 6f6f 665f 6261 795f 6d6f 6465 6c2e  .roof_bay_model.
-000014f0: 7365 636f 6e64 6172 795f 6d65 6d62 6572  secondary_member
-00001500: 735b 305d 0a20 2062 6d64 203d 206d 656d  s[0].  bmd = mem
-00001510: 6265 722e 706c 6f74 5f62 6d64 2829 0a20  ber.plot_bmd(). 
-00001520: 2062 6d64 2e73 686f 7728 290a 2020 6060   bmd.show().  ``
-00001530: 600a 2020 5468 6520 7368 6561 7220 666f  `.  The shear fo
-00001540: 7263 6520 6469 6167 7261 6d20 616e 6420  rce diagram and 
-00001550: 6465 666c 6563 7465 6420 7368 6170 6520  deflected shape 
-00001560: 6361 6e20 6265 2061 6363 6573 7365 6420  can be accessed 
-00001570: 696e 2061 2073 696d 696c 6172 0a20 2066  in a similar.  f
-00001580: 6173 6869 6f6e 2e0a 0a2d 2054 6865 2073  ashion...- The s
-00001590: 7570 706f 7274 2072 6561 6374 696f 6e73  upport reactions
-000015a0: 2063 616e 2062 6520 6f62 7461 696e 6564   can be obtained
-000015b0: 2061 7320 666f 6c6c 6f77 733a 0a20 2060   as follows:.  `
-000015c0: 6060 7079 7468 6f6e 0a20 2073 7570 706f  ``python.  suppo
-000015d0: 7274 5f6e 6f64 6573 203d 206d 656d 6265  rt_nodes = membe
-000015e0: 722e 7375 7070 6f72 745f 6e6f 6465 730a  r.support_nodes.
-000015f0: 2020 7375 7070 6f72 745f 7265 6163 7469    support_reacti
-00001600: 6f6e 7320 3d20 5b6d 656d 6265 722e 7375  ons = [member.su
-00001610: 7070 6f72 745f 7265 6163 7469 6f6e 735b  pport_reactions[
-00001620: 6e6f 6465 5d20 666f 7220 6e6f 6465 2069  node] for node i
-00001630: 6e20 7375 7070 6f72 745f 6e6f 6465 735d  n support_nodes]
-00001640: 0a20 2060 6060 0a0a 5365 7665 7261 6c20  .  ```..Several 
-00001650: 6f74 6865 7220 6174 7472 6962 7574 6573  other attributes
-00001660: 206f 6620 7468 6520 4265 616d 4d6f 6465   of the BeamMode
-00001670: 6c20 6f62 6a65 6374 2063 616e 2062 6520  l object can be 
-00001680: 6163 6365 7373 6564 2069 6e20 6120 7369  accessed in a si
-00001690: 6d69 6c61 720a 6661 7368 696f 6e2e 0a0a  milar.fashion...
-000016a0: 4e6f 7465 2074 6861 7420 6f6e 6c79 2074  Note that only t
-000016b0: 6865 2066 696e 616c 2061 6e61 6c79 7369  he final analysi
-000016c0: 7320 7265 7375 6c74 7320 6361 6e20 6375  s results can cu
-000016d0: 7272 656e 746c 7920 6265 2061 6363 6573  rrently be acces
-000016e0: 7365 642e 0a0a 2323 2320 4164 6469 7469  sed...### Additi
-000016f0: 6f6e 616c 2049 6e66 6f72 6d61 7469 6f6e  onal Information
-00001700: 0a2d 205b 446f 6375 6d65 6e74 6174 696f  .- [Documentatio
-00001710: 6e5d 2868 7474 7073 3a2f 2f70 6f6e 6470  n](https://pondp
-00001720: 792e 7265 6164 7468 6564 6f63 732e 696f  y.readthedocs.io
-00001730: 2f65 6e2f 6c61 7465 7374 2f29 0a2d 205b  /en/latest/).- [
-00001740: 5079 5049 2044 6973 7472 6962 7574 696f  PyPI Distributio
-00001750: 6e5d 2868 7474 7073 3a2f 2f70 7970 692e  n](https://pypi.
-00001760: 6f72 672f 7072 6f6a 6563 742f 706f 6e64  org/project/pond
-00001770: 7079 2f29 0a0a                           py/)..
+00000270: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000280: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
+00000290: 2264 6f63 732f 736f 7572 6365 2f70 6f6e  "docs/source/pon
+000002a0: 6470 792e 7376 6722 2061 6c74 3d22 4c6f  dpy.svg" alt="Lo
+000002b0: 676f 2220 7769 6474 683d 2235 3030 2220  go" width="500" 
+000002c0: 2f3e 0a3c 2f70 3e0a 0a3c 7020 616c 6967  />.</p>..<p alig
+000002d0: 6e3d 2263 656e 7465 7222 3e0a 2020 2020  n="center">.    
+000002e0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000002f0: 2f67 6974 6875 622e 636f 6d2f 6d61 7474  /github.com/matt
+00000300: 6865 772d 7570 7368 6177 2f70 6f6e 6470  hew-upshaw/pondp
+00000310: 792f 6163 7469 6f6e 732f 776f 726b 666c  y/actions/workfl
+00000320: 6f77 732f 7465 7374 732e 796d 6c22 3e3c  ows/tests.yml"><
+00000330: 696d 6720 616c 743d 2254 6573 7473 2220  img alt="Tests" 
+00000340: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+00000350: 6875 622e 636f 6d2f 6d61 7474 6865 772d  hub.com/matthew-
+00000360: 7570 7368 6177 2f70 6f6e 6470 792f 6163  upshaw/pondpy/ac
+00000370: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000380: 7465 7374 732e 7961 6d6c 2f62 6164 6765  tests.yaml/badge
+00000390: 2e73 7667 223e 3c2f 613e 266e 6273 703b  .svg"></a>&nbsp;
+000003a0: 266e 6273 703b 266e 6273 703b 0a20 2020  &nbsp;&nbsp;.   
+000003b0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000003c0: 2f2f 636f 7665 7261 6c6c 732e 696f 2f67  //coveralls.io/g
+000003d0: 6974 6875 622f 6d61 7474 6865 772d 7570  ithub/matthew-up
+000003e0: 7368 6177 2f70 6f6e 6470 793f 6272 616e  shaw/pondpy?bran
+000003f0: 6368 3d6d 6169 6e22 3e3c 696d 6720 616c  ch=main"><img al
+00000400: 743d 2243 6f76 6572 6167 6520 5374 6174  t="Coverage Stat
+00000410: 7573 2220 7372 633d 2268 7474 7073 3a2f  us" src="https:/
+00000420: 2f63 6f76 6572 616c 6c73 2e69 6f2f 7265  /coveralls.io/re
+00000430: 706f 732f 6769 7468 7562 2f6d 6174 7468  pos/github/matth
+00000440: 6577 2d75 7073 6861 772f 706f 6e64 7079  ew-upshaw/pondpy
+00000450: 2f62 6164 6765 2e73 7667 3f62 7261 6e63  /badge.svg?branc
+00000460: 683d 6d61 696e 2676 3d30 2e31 2e32 223e  h=main&v=0.1.2">
+00000470: 3c2f 613e 266e 6273 703b 266e 6273 703b  </a>&nbsp;&nbsp;
+00000480: 266e 6273 703b 0a20 2020 203c 6120 6872  &nbsp;.    <a hr
+00000490: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000004a0: 7562 2e63 6f6d 2f6d 6174 7468 6577 2d75  ub.com/matthew-u
+000004b0: 7073 6861 772f 706f 6e64 7079 2f62 6c6f  pshaw/pondpy/blo
+000004c0: 622f 6d61 696e 2f4c 4943 454e 5345 223e  b/main/LICENSE">
+000004d0: 3c69 6d67 2061 6c74 3d22 4c69 6365 6e73  <img alt="Licens
+000004e0: 653a 204d 4954 2220 7372 633d 2268 7474  e: MIT" src="htt
+000004f0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000500: 2e69 6f2f 6261 6467 652f 4c69 6365 6e73  .io/badge/Licens
+00000510: 652d 4d49 542d 7965 6c6c 6f77 2e73 7667  e-MIT-yellow.svg
+00000520: 223e 3c2f 613e 266e 6273 703b 266e 6273  "></a>&nbsp;&nbs
+00000530: 703b 266e 6273 703b 0a3c 2f70 3e0a 0a23  p;&nbsp;.</p>..#
+00000540: 2049 6e74 726f 6475 6374 696f 6e0a 2a2a   Introduction.**
+00000550: 706f 6e64 7079 2a2a 2069 7320 6120 7061  pondpy** is a pa
+00000560: 636b 6167 6520 6275 696c 7420 746f 2061  ckage built to a
+00000570: 6964 2069 6e20 7468 6520 6465 7369 676e  id in the design
+00000580: 206f 6620 6c6f 772d 736c 6f70 6520 726f   of low-slope ro
+00000590: 6f66 2062 6179 7320 666f 7220 0a70 6f6e  of bays for .pon
+000005a0: 6469 6e67 2073 7461 6269 6c69 7479 2061  ding stability a
+000005b0: 6e64 2069 6d70 6f75 6e64 6564 2072 6169  nd impounded rai
+000005c0: 6e20 6c6f 6164 696e 672e 2049 7420 7574  n loading. It ut
+000005d0: 696c 697a 6573 2061 2073 6572 6965 7320  ilizes a series 
+000005e0: 6f66 0a70 7572 706f 7365 2d62 7569 6c74  of.purpose-built
+000005f0: 2066 696e 6974 6520 656c 656d 656e 7420   finite element 
+00000600: 616e 6420 706f 6e64 696e 6720 616e 616c  and ponding anal
+00000610: 7973 6973 2063 6c61 7373 6573 2061 6e64  ysis classes and
+00000620: 206d 6574 686f 6473 2074 6f20 6265 0a61   methods to be.a
+00000630: 7320 696e 7475 6974 6976 6520 6173 2070  s intuitive as p
+00000640: 6f73 7369 626c 6520 666f 7220 7468 6520  ossible for the 
+00000650: 6d6f 6465 726e 2065 6e67 696e 6565 722e  modern engineer.
+00000660: 0a0a 2323 2320 496e 7374 616c 6c61 7469  ..### Installati
+00000670: 6f6e 0a49 6e73 7461 6c6c 2070 6f6e 6470  on.Install pondp
+00000680: 7920 7769 7468 2070 6970 3a0a 6060 6062  y with pip:.```b
+00000690: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
+000006a0: 706f 6e64 7079 0a60 6060 0a0a 2323 2320  pondpy.```..### 
+000006b0: 5573 6167 650a 5468 6520 506f 6e64 5079  Usage.The PondPy
+000006c0: 4d6f 6465 6c20 636c 6173 7320 6973 2064  Model class is d
+000006d0: 6573 6967 6e65 6420 746f 2077 6f72 6b20  esigned to work 
+000006e0: 7769 7468 2073 6576 6572 616c 2070 7572  with several pur
+000006f0: 706f 7365 2d62 7569 6c74 2063 6c61 7373  pose-built class
+00000700: 6573 0a74 6861 7420 6865 6c70 2074 6865  es.that help the
+00000710: 2075 7365 7220 6f72 6761 6e69 7a65 2074   user organize t
+00000720: 6865 6972 2069 6e70 7574 2069 6e74 6f20  heir input into 
+00000730: 6120 666f 726d 2074 6861 7420 6172 6520  a form that are 
+00000740: 7265 6164 696c 7920 7574 696c 697a 6564  readily utilized
+00000750: 0a74 6f20 6275 696c 6420 616e 6420 616e  .to build and an
+00000760: 616c 797a 6520 7468 6520 6d6f 6465 6c2e  alyze the model.
+00000770: 2054 6865 7365 2061 7265 2074 6865 2060   These are the `
+00000780: 6060 5072 696d 6172 7946 7261 6d69 6e67  ``PrimaryFraming
+00000790: 6060 602c 0a60 6060 5365 636f 6e64 6172  ```,.```Secondar
+000007a0: 7946 7261 6d69 6e67 6060 602c 2061 6e64  yFraming```, and
+000007b0: 2060 6060 4c6f 6164 696e 6760 6060 2063   ```Loading``` c
+000007c0: 6c61 7373 6573 2e20 496e 2061 6464 6974  lasses. In addit
+000007d0: 696f 6e2c 2074 6865 2070 6163 6b61 6765  ion, the package
+000007e0: 2069 730a 6465 7369 676e 6564 2074 6f20   is.designed to 
+000007f0: 776f 726b 2077 6974 6820 7468 6520 6060  work with the ``
+00000800: 6073 7465 656c 7079 6060 6020 616e 6420  `steelpy``` and 
+00000810: 6060 606a 6f69 7374 7079 6060 6020 7061  ```joistpy``` pa
+00000820: 636b 6167 6573 2c20 7468 6f75 6768 2061  ckages, though a
+00000830: 6e79 0a6f 626a 6563 7420 636f 6e74 6169  ny.object contai
+00000840: 6e69 6e67 2074 6865 2072 6571 7569 7269  ning the requiri
+00000850: 6e67 2069 6e66 6f72 6d61 7469 6f6e 2061  ng information a
+00000860: 7474 7269 6275 7265 7320 2869 2e65 2e20  ttribures (i.e. 
+00000870: 6d6f 6d65 6e74 206f 6620 696e 6572 7469  moment of inerti
+00000880: 612c 0a63 726f 7373 2d73 6563 7469 6f6e  a,.cross-section
+00000890: 616c 2061 7265 612c 2065 6c61 7374 6963  al area, elastic
+000008a0: 206d 6f64 756c 7573 2c20 6574 632e 2920   modulus, etc.) 
+000008b0: 636f 756c 6420 6265 2075 7365 6420 696e  could be used in
+000008c0: 206c 6965 7520 6f66 2065 6974 6865 720a   lieu of either.
+000008d0: 7061 636b 6167 652e 0a0a 546f 2063 7265  package...To cre
+000008e0: 6174 6520 616e 6420 616e 616c 797a 6520  ate and analyze 
+000008f0: 6120 726f 6f66 2062 6179 206d 6f64 656c  a roof bay model
+00000900: 2c20 6669 7273 7420 696d 706f 7274 2074  , first import t
+00000910: 6865 2072 6571 7569 7265 6420 6465 7065  he required depe
+00000920: 6e64 656e 6369 6573 0a61 6e64 2063 6c61  ndencies.and cla
+00000930: 7373 6573 3a0a 6060 6070 7974 686f 6e0a  sses:.```python.
+00000940: 6672 6f6d 206a 6f69 7374 7079 2069 6d70  from joistpy imp
+00000950: 6f72 7420 736a 690a 6672 6f6d 2073 7465  ort sji.from ste
+00000960: 656c 7079 2069 6d70 6f72 7420 6169 7363  elpy import aisc
+00000970: 0a0a 6672 6f6d 2070 6f6e 6470 792e 616e  ..from pondpy.an
+00000980: 616c 7973 6973 2e66 656d 5f61 6e61 6c79  alysis.fem_analy
+00000990: 7369 7320 696d 706f 7274 2028 0a20 2020  sis import (.   
+000009a0: 2053 7465 656c 4265 616d 5369 7a65 2c0a   SteelBeamSize,.
+000009b0: 2020 2020 5374 6565 6c4a 6f69 7374 5369      SteelJoistSi
+000009c0: 7a65 2c0a 290a 0a66 726f 6d20 706f 6e64  ze,.)..from pond
+000009d0: 7079 2e61 6e61 6c79 7369 732e 706f 6e64  py.analysis.pond
+000009e0: 5f61 6e61 6c79 7369 7320 696d 706f 7274  _analysis import
+000009f0: 2028 0a20 2020 2050 7269 6d61 7279 4d65   (.    PrimaryMe
+00000a00: 6d62 6572 2c0a 2020 2020 5072 696d 6172  mber,.    Primar
+00000a10: 7946 7261 6d69 6e67 2c0a 2020 2020 5365  yFraming,.    Se
+00000a20: 636f 6e64 6172 794d 656d 6265 722c 0a20  condaryMember,. 
+00000a30: 2020 2053 6563 6f6e 6461 7279 4672 616d     SecondaryFram
+00000a40: 696e 672c 0a20 2020 204c 6f61 6469 6e67  ing,.    Loading
+00000a50: 0a29 0a0a 6672 6f6d 2070 6f6e 6470 792e  .)..from pondpy.
+00000a60: 706f 6e64 7079 2069 6d70 6f72 7420 506f  pondpy import Po
+00000a70: 6e64 5079 4d6f 6465 6c0a 6060 600a 0a4e  ndPyModel.```..N
+00000a80: 6578 742c 2064 6566 696e 6520 7468 6520  ext, define the 
+00000a90: 7374 6565 6c20 7368 6170 6573 2061 6e64  steel shapes and
+00000aa0: 206a 6f69 7374 2064 6573 6967 6e61 7469   joist designati
+00000ab0: 6f6e 7320 696e 2079 6f75 7220 6d6f 6465  ons in your mode
+00000ac0: 6c2e 0a60 6060 7079 7468 6f6e 0a77 3132  l..```python.w12
+00000ad0: 7831 3620 3d20 5374 6565 6c42 6561 6d53  x16 = SteelBeamS
+00000ae0: 697a 6528 2757 3132 5831 3627 2c20 6169  ize('W12X16', ai
+00000af0: 7363 2e57 5f73 6861 7065 732e 5731 3258  sc.W_shapes.W12X
+00000b00: 3136 290a 7731 3678 3236 203d 2053 7465  16).w16x26 = Ste
+00000b10: 656c 4265 616d 5369 7a65 2827 5731 3658  elBeamSize('W16X
+00000b20: 3236 272c 2061 6973 632e 575f 7368 6170  26', aisc.W_shap
+00000b30: 6573 2e57 3136 5832 3629 0a6b 5f31 346b  es.W16X26).k_14k
+00000b40: 3120 3d20 5374 6565 6c4a 6f69 7374 5369  1 = SteelJoistSi
+00000b50: 7a65 2827 3134 4b31 272c 2073 6a69 2e4b  ze('14K1', sji.K
+00000b60: 5f53 6572 6965 732e 4b5f 3134 4b31 290a  _Series.K_14K1).
+00000b70: 6060 600a 0a4e 6578 742c 2064 6566 696e  ```..Next, defin
+00000b80: 6520 7468 6520 7072 696d 6172 7920 616e  e the primary an
+00000b90: 6420 7365 636f 6e64 6172 7920 6672 616d  d secondary fram
+00000ba0: 696e 6720 696e 2074 6865 2072 6f6f 6620  ing in the roof 
+00000bb0: 6261 7920 6672 616d 696e 6720 7379 7374  bay framing syst
+00000bc0: 656d 2e20 0a4e 6f74 6520 7468 6174 2061  em. .Note that a
+00000bd0: 6c6c 2069 6e70 7574 7320 7368 6f75 6c64  ll inputs should
+00000be0: 2062 6520 696e 206b 6970 7320 616e 6420   be in kips and 
+00000bf0: 696e 6368 6573 2e0a 6060 6070 7974 686f  inches..```pytho
+00000c00: 6e0a 705f 6c65 6e67 7468 203d 2032 302a  n.p_length = 20*
+00000c10: 3132 2023 206c 656e 6774 6820 6f66 2070  12 # length of p
+00000c20: 7269 6d61 7279 206d 656d 6265 7273 2069  rimary members i
+00000c30: 6e20 696e 6368 6573 0a73 5f6c 656e 6774  n inches.s_lengt
+00000c40: 6820 3d20 3230 2a31 3220 2320 6c65 6e67  h = 20*12 # leng
+00000c50: 7468 206f 6620 7365 636f 6e64 6172 7920  th of secondary 
+00000c60: 6d65 6d62 6572 7320 696e 2069 6e63 6865  members in inche
+00000c70: 730a 0a23 2053 7570 706f 7274 2074 7970  s..# Support typ
+00000c80: 6573 2061 7265 2064 6573 6967 6e61 7465  es are designate
+00000c90: 6420 6279 2074 7570 6c65 7320 7265 7072  d by tuples repr
+00000ca0: 6573 656e 7469 6e67 2028 5478 2c20 5479  esenting (Tx, Ty
+00000cb0: 2c20 527a 292e 0a23 2041 2030 2069 6e64  , Rz)..# A 0 ind
+00000cc0: 6963 6174 6573 2074 6865 2064 6567 7265  icates the degre
+00000cd0: 6520 6f66 2066 7265 6564 6f6d 2069 7320  e of freedom is 
+00000ce0: 756e 7265 7374 7261 696e 6564 2077 6869  unrestrained whi
+00000cf0: 6c65 2061 2031 2069 6e64 6963 6174 6573  le a 1 indicates
+00000d00: 2061 200a 2320 7265 7374 7261 696e 6564   a .# restrained
+00000d10: 2064 6567 7265 6520 6f66 2066 7265 6564   degree of freed
+00000d20: 6f6d 2e0a 705f 7375 7070 6f72 7420 3d20  om..p_support = 
+00000d30: 5b5b 302c 2028 312c 2031 2c20 3029 5d2c  [[0, (1, 1, 0)],
+00000d40: 205b 705f 6c65 6e67 7468 2c20 2831 2c20   [p_length, (1, 
+00000d50: 312c 2030 295d 5d0a 735f 7375 7070 6f72  1, 0)]].s_suppor
+00000d60: 7420 3d20 5b5b 302c 2028 312c 2031 2c20  t = [[0, (1, 1, 
+00000d70: 3029 5d2c 205b 735f 6c65 6e67 7468 2c20  0)], [s_length, 
+00000d80: 2831 2c20 312c 2030 295d 5d0a 0a70 5f67  (1, 1, 0)]]..p_g
+00000d90: 6972 6465 7231 203d 2050 7269 6d61 7279  irder1 = Primary
+00000da0: 4d65 6d62 6572 2870 5f6c 656e 6774 682c  Member(p_length,
+00000db0: 2077 3136 7832 362c 2070 5f73 7570 706f   w16x26, p_suppo
+00000dc0: 7274 290a 705f 6769 7264 6572 3220 3d20  rt).p_girder2 = 
+00000dd0: 5072 696d 6172 794d 656d 6265 7228 705f  PrimaryMember(p_
+00000de0: 6c65 6e67 7468 2c20 7731 3678 3236 2c20  length, w16x26, 
+00000df0: 705f 7375 7070 6f72 7429 0a73 5f62 6561  p_support).s_bea
+00000e00: 6d31 203d 2053 6563 6f6e 6461 7279 4d65  m1 = SecondaryMe
+00000e10: 6d62 6572 2873 5f6c 656e 6774 682c 2077  mber(s_length, w
+00000e20: 3132 7831 362c 2073 5f73 7570 706f 7274  12x16, s_support
+00000e30: 290a 735f 6265 616d 3220 3d20 5365 636f  ).s_beam2 = Seco
+00000e40: 6e64 6172 794d 656d 6265 7228 735f 6c65  ndaryMember(s_le
+00000e50: 6e67 7468 2c20 7731 3278 3136 2c20 735f  ngth, w12x16, s_
+00000e60: 7375 7070 6f72 7429 0a73 5f6a 6f69 7374  support).s_joist
+00000e70: 3120 3d20 5365 636f 6e64 6172 794d 656d  1 = SecondaryMem
+00000e80: 6265 7228 735f 6c65 6e67 7468 2c20 6b5f  ber(s_length, k_
+00000e90: 3134 6b31 2c20 735f 7375 7070 6f72 7429  14k1, s_support)
+00000ea0: 0a73 5f6a 6f69 7374 3220 3d20 5365 636f  .s_joist2 = Seco
+00000eb0: 6e64 6172 794d 656d 6265 7228 735f 6c65  ndaryMember(s_le
+00000ec0: 6e67 7468 2c20 6b5f 3134 6b31 2c20 735f  ngth, k_14k1, s_
+00000ed0: 7375 7070 6f72 7429 0a73 5f6a 6f69 7374  support).s_joist
+00000ee0: 3320 3d20 5365 636f 6e64 6172 794d 656d  3 = SecondaryMem
+00000ef0: 6265 7228 735f 6c65 6e67 7468 2c20 6b5f  ber(s_length, k_
+00000f00: 3134 6b31 2c20 735f 7375 7070 6f72 7429  14k1, s_support)
+00000f10: 0a0a 705f 6672 616d 696e 6720 3d20 5072  ..p_framing = Pr
+00000f20: 696d 6172 7946 7261 6d69 6e67 285b 705f  imaryFraming([p_
+00000f30: 6769 7264 6572 312c 2070 5f67 6972 6465  girder1, p_girde
+00000f40: 7232 5d29 0a73 5f66 7261 6d69 6e67 203d  r2]).s_framing =
+00000f50: 2053 6563 6f6e 6461 7279 4672 616d 696e   SecondaryFramin
+00000f60: 6728 5b73 5f62 6561 6d31 2c20 735f 6a6f  g([s_beam1, s_jo
+00000f70: 6973 7431 2c20 735f 6a6f 6973 7432 2c20  ist1, s_joist2, 
+00000f80: 735f 6a6f 6973 7433 2c20 735f 6265 616d  s_joist3, s_beam
+00000f90: 325d 290a 6060 600a 4e6f 7465 2074 6861  2]).```.Note tha
+00000fa0: 7420 6561 6368 206d 656d 6265 7220 7368  t each member sh
+00000fb0: 6f75 6c64 2062 6520 696e 6469 7669 6475  ould be individu
+00000fc0: 616c 6c79 2064 6566 696e 6564 2061 7320  ally defined as 
+00000fd0: 7368 6f77 6e20 6162 6f76 652e 204f 7468  shown above. Oth
+00000fe0: 6572 7769 7365 2c0a 7468 6520 6c6f 6164  erwise,.the load
+00000ff0: 696e 6773 2077 696c 6c20 6e6f 7420 6265  ings will not be
+00001000: 2061 7070 6c69 6564 2063 6f72 7265 6374   applied correct
+00001010: 6c79 2074 6f20 7468 6520 6d65 6d62 6572  ly to the member
+00001020: 732e 0a0a 5468 6520 726f 6f66 2073 6c6f  s...The roof slo
+00001030: 7065 2063 616e 206f 7074 696f 6e61 6c6c  pe can optionall
+00001040: 7920 6265 2073 6574 2069 6e20 7468 6520  y be set in the 
+00001050: 6060 6053 6563 6f6e 6461 7279 4672 616d  ```SecondaryFram
+00001060: 696e 6760 6060 206f 626a 6563 7420 6279  ing``` object by
+00001070: 0a75 7369 6e67 2074 6865 206b 6579 776f  .using the keywo
+00001080: 7264 2060 6060 736c 6f70 6560 6060 2061  rd ```slope``` a
+00001090: 6e64 2065 6e74 6572 696e 6720 7468 6520  nd entering the 
+000010a0: 726f 6f66 2073 6c6f 7065 2069 6e20 696e  roof slope in in
+000010b0: 6368 6573 2f66 6f6f 742e 2054 6865 0a64  ches/foot. The.d
+000010c0: 6566 6175 6c74 2076 616c 7565 2069 7320  efault value is 
+000010d0: 6060 6030 2e32 3560 6060 2e0a 0a4e 6578  ```0.25```...Nex
+000010e0: 742c 2064 6566 696e 6520 7468 6520 6c6f  t, define the lo
+000010f0: 6164 696e 6720 696e 2074 6865 2072 6f6f  ading in the roo
+00001100: 6620 6261 792e 0a60 6060 7079 7468 6f6e  f bay..```python
+00001110: 0a70 5f66 7261 6d69 6e67 203d 2050 7269  .p_framing = Pri
+00001120: 6d61 7279 4672 616d 696e 6728 5b70 5f67  maryFraming([p_g
+00001130: 6972 6465 7231 2c20 705f 6769 7264 6572  irder1, p_girder
+00001140: 325d 290a 735f 6672 616d 696e 6720 3d20  2]).s_framing = 
+00001150: 5365 636f 6e64 6172 7946 7261 6d69 6e67  SecondaryFraming
+00001160: 285b 735f 6265 616d 312c 2073 5f6a 6f69  ([s_beam1, s_joi
+00001170: 7374 312c 2073 5f6a 6f69 7374 322c 2073  st1, s_joist2, s
+00001180: 5f6a 6f69 7374 332c 2073 5f62 6561 6d32  _joist3, s_beam2
+00001190: 5d29 0a0a 715f 646c 203d 2032 302f 3130  ])..q_dl = 20/10
+000011a0: 3030 2f31 3434 2023 2053 7572 6661 6365  00/144 # Surface
+000011b0: 2064 6561 6420 6c6f 6164 2069 6e20 6b73   dead load in ks
+000011c0: 690a 715f 726c 203d 2032 322e 342f 3130  i.q_rl = 22.4/10
+000011d0: 3030 2f31 3434 2023 2053 7572 6661 6365  00/144 # Surface
+000011e0: 2072 6169 6e20 6c6f 6164 2061 7420 7365   rain load at se
+000011f0: 636f 6e64 6172 7920 6472 6169 6e61 6765  condary drainage
+00001200: 2069 6e6c 6574 2069 6e20 6b73 690a 0a6c   inlet in ksi..l
+00001210: 6f61 6469 6e67 203d 204c 6f61 6469 6e67  oading = Loading
+00001220: 2871 5f64 6c2c 2071 5f72 6c29 0a60 6060  (q_dl, q_rl).```
+00001230: 0a54 6865 2069 6e70 7574 2072 6169 6e20  .The input rain 
+00001240: 6c6f 6164 2073 686f 756c 6420 696e 636c  load should incl
+00001250: 7564 6520 7468 6520 7374 6174 6963 2068  ude the static h
+00001260: 6561 6420 616e 6420 7468 6520 6879 6472  ead and the hydr
+00001270: 6175 6c69 6320 6865 6164 2c20 6275 740a  aulic head, but.
+00001280: 6e6f 2070 6f6e 6469 6e67 2068 6561 642e  no ponding head.
+00001290: 0a0a 4669 6e61 6c6c 792c 2064 6566 696e  ..Finally, defin
+000012a0: 6520 7468 6520 6060 6050 6f6e 6450 794d  e the ```PondPyM
+000012b0: 6f64 656c 6060 6020 6f62 6a65 6374 2061  odel``` object a
+000012c0: 6e64 2061 6e61 6c79 7a65 2074 6865 206d  nd analyze the m
+000012d0: 6f64 656c 2e0a 6060 6070 7974 686f 6e0a  odel..```python.
+000012e0: 706f 6e64 7079 5f6d 6f64 656c 203d 2050  pondpy_model = P
+000012f0: 6f6e 6450 794d 6f64 656c 2870 5f66 7261  ondPyModel(p_fra
+00001300: 6d69 6e67 2c20 735f 6672 616d 696e 672c  ming, s_framing,
+00001310: 206c 6f61 6469 6e67 290a 0a70 6f6e 6470   loading)..pondp
+00001320: 795f 6d6f 6465 6c2e 7065 7266 6f72 6d5f  y_model.perform_
+00001330: 616e 616c 7973 6973 2829 0a60 6060 0a4f  analysis().```.O
+00001340: 7074 696f 6e61 6c20 6172 6775 6d65 6e74  ptional argument
+00001350: 7320 666f 7220 7468 6520 6060 6050 6f6e  s for the ```Pon
+00001360: 6450 794d 6f64 656c 6060 6020 696e 636c  dPyModel``` incl
+00001370: 7564 653a 0a0a 2d20 6060 606d 6972 726f  ude:..- ```mirro
+00001380: 7265 645f 6c65 6674 6060 603a 2062 6f6f  red_left```: boo
+00001390: 6c20 696e 6469 6361 7469 6e67 2077 6865  l indicating whe
+000013a0: 7468 6572 2074 6865 2072 6f6f 6620 6261  ther the roof ba
+000013b0: 7920 6973 206d 6972 726f 7265 640a 2020  y is mirrored.  
+000013c0: 2020 6f6e 2074 6865 206c 6566 7420 7369    on the left si
+000013d0: 6465 3b20 6465 6661 756c 7420 6973 2060  de; default is `
+000013e0: 6060 4661 6c73 6560 6060 0a0a 2d20 6060  ``False```..- ``
+000013f0: 606d 6972 726f 7265 645f 7269 6768 7460  `mirrored_right`
+00001400: 6060 203a 2062 6f6f 6c20 696e 6469 6361  `` : bool indica
+00001410: 7469 6e67 2077 6865 7468 6572 2074 6865  ting whether the
+00001420: 2072 6f6f 6620 6261 7920 6973 206d 6972   roof bay is mir
+00001430: 726f 7265 640a 2020 2020 6f6e 2074 6865  rored.    on the
+00001440: 2072 6967 6874 2073 6964 653b 2064 6566   right side; def
+00001450: 6175 6c74 2069 7320 6060 6046 616c 7365  ault is ```False
+00001460: 6060 600a 0a2d 2060 6060 7374 6f70 5f63  ```..- ```stop_c
+00001470: 7269 7465 7269 6f6e 6060 6020 3a20 666c  riterion``` : fl
+00001480: 6f61 7420 696e 6469 6361 7469 6e67 2074  oat indicating t
+00001490: 6865 2065 7272 6f72 2069 6e20 746f 7461  he error in tota
+000014a0: 6c20 696d 706f 756e 6465 640a 2020 2020  l impounded.    
+000014b0: 7761 7465 7220 7765 6967 6874 2061 7420  water weight at 
+000014c0: 7768 6963 6820 7468 6520 6974 6572 6174  which the iterat
+000014d0: 6976 6520 616e 616c 7973 6973 2073 686f  ive analysis sho
+000014e0: 756c 6420 6265 2074 6572 6d69 6e61 7465  uld be terminate
+000014f0: 643b 0a20 2020 2064 6566 6175 6c74 2069  d;.    default i
+00001500: 7320 6060 6030 2e30 3030 3160 6060 0a0a  s ```0.0001```..
+00001510: 2d20 6060 606d 6178 5f69 7465 7260 6060  - ```max_iter```
+00001520: 203a 2069 6e74 2069 6e64 6963 6174 696e   : int indicatin
+00001530: 6720 7468 6520 6d61 7869 6d75 6d20 6e75  g the maximum nu
+00001540: 6d62 6572 206f 6620 6974 6572 6174 696f  mber of iteratio
+00001550: 6e73 2074 6861 740a 2020 2020 7368 6f75  ns that.    shou
+00001560: 6c64 2062 6520 7065 7266 6f72 6d65 643b  ld be performed;
+00001570: 2064 6566 6175 6c74 2069 7320 6060 6035   default is ```5
+00001580: 3060 6060 0a20 2020 200a 2d20 6060 6073  0```.    .- ```s
+00001590: 686f 775f 7265 7375 6c74 7360 6060 203a  how_results``` :
+000015a0: 2062 6f6f 6c20 696e 6469 6361 7469 6e67   bool indicating
+000015b0: 2077 6865 7468 6572 2074 6865 2069 7465   whether the ite
+000015c0: 7261 7469 6f6e 2072 6573 756c 7473 2073  ration results s
+000015d0: 686f 756c 640a 2020 2020 6265 2070 7269  hould.    be pri
+000015e0: 6e74 6564 2074 6f20 7468 6520 7465 726d  nted to the term
+000015f0: 696e 616c 2075 706f 6e20 636f 6d70 6c65  inal upon comple
+00001600: 7469 6f6e 206f 6620 7468 6520 616e 616c  tion of the anal
+00001610: 7973 6973 3b0a 2020 2020 6465 6661 756c  ysis;.    defaul
+00001620: 7420 6973 2060 6060 5472 7565 6060 600a  t is ```True```.
+00001630: 0a23 2323 2041 6e61 6c79 7369 7320 5265  .### Analysis Re
+00001640: 7375 6c74 730a 4561 6368 2070 7269 6d61  sults.Each prima
+00001650: 7279 2061 6e64 2073 6563 6f6e 6461 7279  ry and secondary
+00001660: 206d 656d 6265 7220 6973 2072 6570 7265   member is repre
+00001670: 7365 6e74 6564 2077 6974 6869 6e20 7468  sented within th
+00001680: 6520 506f 6e64 5079 4d6f 6465 6c20 6f62  e PondPyModel ob
+00001690: 6a65 6374 0a62 7920 6120 4265 616d 4d6f  ject.by a BeamMo
+000016a0: 6465 6c20 6f62 6a65 6374 2e20 4173 2073  del object. As s
+000016b0: 7563 6820 6120 6772 6561 7420 6465 616c  uch a great deal
+000016c0: 206f 6620 616e 616c 7973 6973 2072 6573   of analysis res
+000016d0: 756c 7473 2063 616e 2062 6520 6f62 7461  ults can be obta
+000016e0: 696e 6564 0a66 6169 726c 7920 6561 7369  ined.fairly easi
+000016f0: 6c79 206f 6e63 6520 7468 6520 616e 616c  ly once the anal
+00001700: 7973 6973 2069 7320 636f 6d70 6c65 7465  ysis is complete
+00001710: 2e0a 0a2d 2054 6f20 6163 6365 7373 2074  ...- To access t
+00001720: 6865 2064 6566 6c65 6374 6564 2073 6861  he deflected sha
+00001730: 7065 2c20 7368 6561 7220 666f 7263 6520  pe, shear force 
+00001740: 6469 6167 7261 6d2c 206f 7220 6265 6e64  diagram, or bend
+00001750: 696e 6720 6d6f 6d65 6e74 2064 6961 6772  ing moment diagr
+00001760: 616d 0a20 206f 6620 6120 7061 7274 6963  am.  of a partic
+00001770: 756c 6172 206d 656d 6265 722c 2075 7365  ular member, use
+00001780: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00001790: 616c 6c73 3a0a 2020 6060 6070 7974 686f  alls:.  ```pytho
+000017a0: 6e0a 2020 6d65 6d62 6572 203d 2070 6f6e  n.  member = pon
+000017b0: 6470 795f 6d6f 6465 6c2e 726f 6f66 5f62  dpy_model.roof_b
+000017c0: 6179 5f6d 6f64 656c 2e73 6563 6f6e 6461  ay_model.seconda
+000017d0: 7279 5f6d 656d 6265 7273 5b30 5d0a 2020  ry_members[0].  
+000017e0: 626d 6420 3d20 6d65 6d62 6572 2e70 6c6f  bmd = member.plo
+000017f0: 745f 626d 6428 290a 2020 626d 642e 7368  t_bmd().  bmd.sh
+00001800: 6f77 2829 0a20 2060 6060 0a20 2054 6865  ow().  ```.  The
+00001810: 2073 6865 6172 2066 6f72 6365 2064 6961   shear force dia
+00001820: 6772 616d 2061 6e64 2064 6566 6c65 6374  gram and deflect
+00001830: 6564 2073 6861 7065 2063 616e 2062 6520  ed shape can be 
+00001840: 6163 6365 7373 6564 2069 6e20 6120 7369  accessed in a si
+00001850: 6d69 6c61 720a 2020 6661 7368 696f 6e20  milar.  fashion 
+00001860: 7573 696e 6720 7468 6520 6060 6070 6c6f  using the ```plo
+00001870: 745f 7366 6428 2960 6060 2061 6e64 2060  t_sfd()``` and `
+00001880: 6060 706c 6f74 5f64 6566 6c65 6374 6564  ``plot_deflected
+00001890: 5f73 6861 7065 2829 6060 6020 6d65 7468  _shape()``` meth
+000018a0: 6f64 732e 0a0a 2020 5468 6520 6465 666c  ods...  The defl
+000018b0: 6563 7465 6420 7368 6170 652c 2073 6865  ected shape, she
+000018c0: 6172 2066 6f72 6365 2064 6961 6772 616d  ar force diagram
+000018d0: 2c20 616e 6420 6265 6e64 696e 6720 6d6f  , and bending mo
+000018e0: 6d65 6e74 2064 6961 6772 616d 2070 6c6f  ment diagram plo
+000018f0: 7473 0a20 2066 6f72 2061 6c6c 206d 656d  ts.  for all mem
+00001900: 6265 7273 2063 616e 2061 6c6c 2062 6520  bers can all be 
+00001910: 6765 6e65 7261 7465 6420 6279 2075 7369  generated by usi
+00001920: 6e67 2074 6865 2060 6060 526f 6f66 4261  ng the ```RoofBa
+00001930: 794d 6f64 656c 6060 6027 730a 2020 6060  yModel```'s.  ``
+00001940: 6067 656e 6572 6174 655f 706c 6f74 7328  `generate_plots(
+00001950: 2960 6060 206d 6574 686f 642e 0a0a 2020  )``` method...  
+00001960: 6060 6070 7974 686f 6e0a 2020 706c 6f74  ```python.  plot
+00001970: 7320 3d20 706f 6e64 7079 5f6d 6f64 656c  s = pondpy_model
+00001980: 2e72 6f6f 665f 6261 795f 6d6f 6465 6c2e  .roof_bay_model.
+00001990: 6765 6e65 7261 7465 5f70 6c6f 7473 2829  generate_plots()
+000019a0: 0a20 2060 6060 0a0a 2020 5468 6973 206d  .  ```..  This m
+000019b0: 6574 686f 6420 7265 7475 726e 7320 6120  ethod returns a 
+000019c0: 6060 6064 6963 7460 6060 206f 626a 6563  ```dict``` objec
+000019d0: 7420 7769 7468 206b 6579 7320 6060 6062  t with keys ```b
+000019e0: 6d64 6060 602c 2060 6060 7366 6460 6060  md```, ```sfd```
+000019f0: 2c20 616e 640a 2020 6060 6064 6566 6c60  , and.  ```defl`
+00001a00: 602c 2065 6163 6820 6f66 2077 6869 6368  `, each of which
+00001a10: 2069 7320 6173 736f 6369 6174 6564 2077   is associated w
+00001a20: 6974 6820 6120 7375 622d 6469 6374 696f  ith a sub-dictio
+00001a30: 6e61 7279 2077 6974 6820 6b65 7973 0a20  nary with keys. 
+00001a40: 2060 6060 5072 696d 6172 7960 6060 2061   ```Primary``` a
+00001a50: 6e64 2060 6060 5365 636f 6e64 6172 7960  nd ```Secondary`
+00001a60: 6060 2e20 4561 6368 2073 7562 2d64 6963  ``. Each sub-dic
+00001a70: 7469 6f6e 6172 7920 636f 6e74 6169 6e73  tionary contains
+00001a80: 2061 206c 6973 7420 6f66 0a20 2074 6865   a list of.  the
+00001a90: 2061 7373 6f63 6961 7465 6420 706c 6f74   associated plot
+00001aa0: 2066 6f72 2065 6163 6820 7072 696d 6172   for each primar
+00001ab0: 7920 6f72 2073 6563 6f6e 6461 7279 206d  y or secondary m
+00001ac0: 656d 6265 722c 2061 7320 6170 706c 6963  ember, as applic
+00001ad0: 6162 6c65 2e0a 0a2d 2054 6865 2073 7570  able...- The sup
+00001ae0: 706f 7274 2072 6561 6374 696f 6e73 2063  port reactions c
+00001af0: 616e 2062 6520 6f62 7461 696e 6564 2061  an be obtained a
+00001b00: 7320 666f 6c6c 6f77 733a 0a20 2060 6060  s follows:.  ```
+00001b10: 7079 7468 6f6e 0a20 2073 7570 706f 7274  python.  support
+00001b20: 5f6e 6f64 6573 203d 206d 656d 6265 722e  _nodes = member.
+00001b30: 7375 7070 6f72 745f 6e6f 6465 730a 2020  support_nodes.  
+00001b40: 7375 7070 6f72 745f 7265 6163 7469 6f6e  support_reaction
+00001b50: 7320 3d20 5b6d 656d 6265 722e 7375 7070  s = [member.supp
+00001b60: 6f72 745f 7265 6163 7469 6f6e 735b 6e6f  ort_reactions[no
+00001b70: 6465 5d20 666f 7220 6e6f 6465 2069 6e20  de] for node in 
+00001b80: 7375 7070 6f72 745f 6e6f 6465 735d 0a20  support_nodes]. 
+00001b90: 2060 6060 0a0a 5365 7665 7261 6c20 6f74   ```..Several ot
+00001ba0: 6865 7220 6174 7472 6962 7574 6573 206f  her attributes o
+00001bb0: 6620 7468 6520 4265 616d 4d6f 6465 6c20  f the BeamModel 
+00001bc0: 6f62 6a65 6374 2063 616e 2062 6520 6163  object can be ac
+00001bd0: 6365 7373 6564 2069 6e20 6120 7369 6d69  cessed in a simi
+00001be0: 6c61 720a 6661 7368 696f 6e2e 0a0a 4e6f  lar.fashion...No
+00001bf0: 7465 2074 6861 7420 6f6e 6c79 2074 6865  te that only the
+00001c00: 2066 696e 616c 2061 6e61 6c79 7369 7320   final analysis 
+00001c10: 7265 7375 6c74 7320 6361 6e20 6375 7272  results can curr
+00001c20: 656e 746c 7920 6265 2061 6363 6573 7365  ently be accesse
+00001c30: 642e 0a0a 2323 2320 4164 6469 7469 6f6e  d...### Addition
+00001c40: 616c 2049 6e66 6f72 6d61 7469 6f6e 0a2d  al Information.-
+00001c50: 205b 446f 6375 6d65 6e74 6174 696f 6e5d   [Documentation]
+00001c60: 2868 7474 7073 3a2f 2f70 6f6e 6470 792e  (https://pondpy.
+00001c70: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00001c80: 6e2f 6c61 7465 7374 2f29 0a2d 205b 5079  n/latest/).- [Py
+00001c90: 5049 2044 6973 7472 6962 7574 696f 6e5d  PI Distribution]
+00001ca0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+00001cb0: 672f 7072 6f6a 6563 742f 706f 6e64 7079  g/project/pondpy
+00001cc0: 2f29 0a0a                                /)..
```

