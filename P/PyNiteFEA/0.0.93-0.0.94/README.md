# Comparing `tmp/PyNiteFEA-0.0.93.tar.gz` & `tmp/pynitefea-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNiteFEA-0.0.93.tar", last modified: Tue Mar 12 23:24:11 2024, max compression
+gzip compressed data, was "pynitefea-0.0.94.tar", last modified: Sun Apr 28 03:36:25 2024, max compression
```

## Comparing `PyNiteFEA-0.0.93.tar` & `pynitefea-0.0.94.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:24:11.610487 PyNiteFEA-0.0.93/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-03-12 23:24:11.610487 PyNiteFEA-0.0.93/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:24:11.606487 PyNiteFEA-0.0.93/PyNite/
--rw-r--r--   0 runner    (1001) docker     (127)    56021 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/Analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/BeamSegY.py
--rw-r--r--   0 runner    (1001) docker     (127)    13637 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/BeamSegZ.py
--rw-r--r--   0 runner    (1001) docker     (127)   116362 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/FEModel3D.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/FixedEndReactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/LoadCombo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/MainStyleSheet.css
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/Material.py
--rw-r--r--   0 runner    (1001) docker     (127)    86326 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/Member3D.py
--rw-r--r--   0 runner    (1001) docker     (127)    68556 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/Mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/Node3D.py
--rw-r--r--   0 runner    (1001) docker     (127)    16388 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/PhysMember.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/Plastic Beam.py
--rw-r--r--   0 runner    (1001) docker     (127)    35580 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/Plate3D.py
--rw-r--r--   0 runner    (1001) docker     (127)    32588 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/Quad3D.py
--rw-r--r--   0 runner    (1001) docker     (127)    26019 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/Report_Template.html
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/Reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/Section.py
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/Spring3D.py
--rw-r--r--   0 runner    (1001) docker     (127)    92930 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/Visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    69302 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/Visualization_PyVista.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/PyNite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:24:11.606487 PyNiteFEA-0.0.93/PyNiteFEA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-03-12 23:24:11.000000 PyNiteFEA-0.0.93/PyNiteFEA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-12 23:24:11.000000 PyNiteFEA-0.0.93/PyNiteFEA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 23:24:11.000000 PyNiteFEA-0.0.93/PyNiteFEA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-12 23:24:11.000000 PyNiteFEA-0.0.93/PyNiteFEA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-12 23:24:11.000000 PyNiteFEA-0.0.93/PyNiteFEA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10244 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 23:24:11.610487 PyNiteFEA-0.0.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-12 23:24:03.000000 PyNiteFEA-0.0.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:36:25.305327 pynitefea-0.0.94/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-28 03:36:14.000000 pynitefea-0.0.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-28 03:36:25.301327 pynitefea-0.0.94/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:36:25.301327 pynitefea-0.0.94/PyNite/
+-rw-r--r--   0 runner    (1001) docker     (127)    56021 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/Analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/BeamSegY.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13637 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/BeamSegZ.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116523 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/FEModel3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/FixedEndReactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/LoadCombo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/MainStyleSheet.css
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/Material.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86351 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/Member3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68721 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/Mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/Node3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16403 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/PhysMember.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/Plastic Beam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35605 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/Plate3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32608 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/Quad3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58036 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/Rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26019 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/Report_Template.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/Reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/Section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8894 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/Spring3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92930 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/Visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-28 03:36:14.000000 pynitefea-0.0.94/PyNite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 03:36:25.301327 pynitefea-0.0.94/PyNiteFEA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-28 03:36:25.000000 pynitefea-0.0.94/PyNiteFEA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-28 03:36:25.000000 pynitefea-0.0.94/PyNiteFEA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 03:36:25.000000 pynitefea-0.0.94/PyNiteFEA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-28 03:36:25.000000 pynitefea-0.0.94/PyNiteFEA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 03:36:25.000000 pynitefea-0.0.94/PyNiteFEA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-04-28 03:36:14.000000 pynitefea-0.0.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 03:36:25.305327 pynitefea-0.0.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-28 03:36:14.000000 pynitefea-0.0.94/setup.py
```

### Comparing `PyNiteFEA-0.0.93/LICENSE` & `pynitefea-0.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.93/PKG-INFO` & `pynitefea-0.0.94/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: PyNiteFEA
-Version: 0.0.93
+Version: 0.0.94
 Summary: A simple elastic 3D structural finite element library for Python.
 Home-page: https://github.com/JWock82/PyNite.git
 Author: D. Craig Brinck, PE, SE
 Author-email: Building.Code@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: PrettyTable
-Provides-Extra: sparse-solver
-Requires-Dist: scipy; extra == "sparse-solver"
+Provides-Extra: sparse
+Requires-Dist: scipy; extra == "sparse"
 Provides-Extra: plotting
 Requires-Dist: matplotlib; extra == "plotting"
-Provides-Extra: visualization
-Requires-Dist: vtk; extra == "visualization"
-Provides-Extra: visualization-screenshots
-Requires-Dist: IPython; extra == "visualization-screenshots"
+Provides-Extra: vtk
+Requires-Dist: vtk; extra == "vtk"
+Requires-Dist: IPython; extra == "vtk"
+Provides-Extra: pyvista
+Requires-Dist: vtk; extra == "pyvista"
+Requires-Dist: pyvista[all,trame]; extra == "pyvista"
+Requires-Dist: trame_jupyter_extension; extra == "pyvista"
+Requires-Dist: ipywidgets; extra == "pyvista"
 Provides-Extra: reporting
 Requires-Dist: pdfkit; extra == "reporting"
 Requires-Dist: Jinja2; extra == "reporting"
-Provides-Extra: reviewing-derivations
-Requires-Dist: jupyterlab; extra == "reviewing-derivations"
-Requires-Dist: sympy; extra == "reviewing-derivations"
+Provides-Extra: derivations
+Requires-Dist: jupyterlab; extra == "derivations"
+Requires-Dist: sympy; extra == "derivations"
 
 <div align="center">
   <img src="https://github.com/JWock82/PyNite/raw/main/Resources/Full Logo No Buffer.png" width=40% align="center"/>
   <br>
   <h1>Simple Finite Element Analysis in Python</h1>
 </div>
 
@@ -87,14 +91,19 @@
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Civils.ai (https://civils.ai/1/free-3D-finite-element-structural-analysis)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.94
+* Added rendering via `Pyvista`. This greatly simplified the rendering code and provided a fresh look to the rendereings. Renderings in jupyter are now interactive. Global axes are also now shown in rendereings. To use `Pyvista` instead of `VTK`, use the new `Rendering` library rather than the old `Visualization` library. Rendering via `VTK` directly is still available.
+* Bug fix for member self-weight. The program was throwing exceptions instead of calculating member self-weight. Added a unit test to help prevent this issue from occuring again as code changes.
+* Refactored `material` to be `material_name` in the code. The prior naming convention caused confusion which led to the self-weight bug.
+
 v0.0.93
 * Fixed phantom reactions showing up at unsupported nodes. If there was a support defined at a node, the program was summing reactions for all directions at the node, rather than just the supported directions. This caused the program to report "extra" reaction directions at any supported node (if the user queried them). Element forces/stresses were not affected as this was a post-processing reaction summing issue. Reactions for supported directions were summed correctly, except in the case of nodes with both spring supports and other supports. Only unsupported directions, and nodes with both spring supports and other supports, were showing phantom reactions. This bug also caused statics checks to fail from time to time.
 * Reorganized physical member code to match member code more consistently.
 
 v0.0.92
 * Added member self-weight calculations via `FEModel3D.add_member_self_weight()`. This only applies to members. This feature does not calculate self-weight for plate and quad elements.
```

### Comparing `PyNiteFEA-0.0.93/PyNite/Analysis.py` & `pynitefea-0.0.94/PyNite/Analysis.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.93/PyNite/BeamSegY.py` & `pynitefea-0.0.94/PyNite/BeamSegY.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.93/PyNite/BeamSegZ.py` & `pynitefea-0.0.94/PyNite/BeamSegZ.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.93/PyNite/FEModel3D.py` & `pynitefea-0.0.94/PyNite/FEModel3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,24 +275,24 @@
         
         # Flag the model as unsolved
         self.solution = None
 
         # Return the spring name
         return name
 
-    def add_member(self, name, i_node, j_node, material, Iy=None, Iz=None, J=None, A=None, aux_node=None, tension_only=False, comp_only=False, section_name=None):
+    def add_member(self, name, i_node, j_node, material_name, Iy=None, Iz=None, J=None, A=None, aux_node=None, tension_only=False, comp_only=False, section_name=None):
         """Adds a new physical member to the model.
 
         :param name: A unique user-defined name for the member. If ``None`` or ``""``, a name will be automatically assigned
         :type name: str
         :param i_node: The name of the i-node (start node).
         :type i_node: str
         :param j_node: The name of the j-node (end node).
         :type j_node: str
-        :param material: The name of the material of the member.
+        :param material_name: The name of the material of the member.
         :type material: str
         :param Iy: The moment of inertia of the member about its local y-axis.
         :type Iy: number
         :param Iz: The moment of inertia of the member about its local z-axis.
         :type Iz: number
         :param J: The polar moment of inertia of the member.
         :type J: number
@@ -320,28 +320,28 @@
             count = 1
             while name in self.Members: 
                 name = "M" + str(len(self.Members)+count)
                 count += 1
                 
         # Create a new member
         if aux_node == None:
-            new_member = PhysMember(name, self.Nodes[i_node], self.Nodes[j_node], material, self, Iy, Iz, J, A, tension_only=tension_only, comp_only=comp_only, section_name=section_name)
+            new_member = PhysMember(name, self.Nodes[i_node], self.Nodes[j_node], material_name, self, Iy, Iz, J, A, tension_only=tension_only, comp_only=comp_only, section_name=section_name)
         else:
-            new_member = PhysMember(name, self.Nodes[i_node], self.Nodes[j_node], material, self, Iy, Iz, J, A, aux_node=self.AuxNodes[aux_node], tension_only=tension_only, comp_only=comp_only, section_name=section_name)
+            new_member = PhysMember(name, self.Nodes[i_node], self.Nodes[j_node], material_name, self, Iy, Iz, J, A, aux_node=self.AuxNodes[aux_node], tension_only=tension_only, comp_only=comp_only, section_name=section_name)
         
         # Add the new member to the list
         self.Members[name] = new_member
         
         # Flag the model as unsolved
         self.solution = None
 
         # Return the member name
         return name
 
-    def add_plate(self, name, i_node, j_node, m_node, n_node, t, material, kx_mod=1.0, ky_mod=1.0):
+    def add_plate(self, name, i_node, j_node, m_node, n_node, t, material_name, kx_mod=1.0, ky_mod=1.0):
         """Adds a new rectangular plate to the model. The plate formulation for in-plane (membrane)
         stiffness is based on an isoparametric formulation. For bending, it is based on a 12-term
         polynomial formulation. This element must be rectangular, and must not be used where a
         thick plate formulation is needed. For a more versatile plate element that can handle
         distortion and thick plate conditions, consider using the `add_quad` method instead.
 
         :param name: A unique user-defined name for the plate. If None or "", a name will be
@@ -353,16 +353,16 @@
         :type j_node: str
         :param m_node: The name of the m-node.
         :type m_node: str
         :param n_node: The name of the n-node.
         :type n_node: str
         :param t: The thickness of the element.
         :type t: number
-        :param material: The name of the material for the element.
-        :type material: str
+        :param material_name: The name of the material for the element.
+        :type material_name: str
         :param kx_mod: Stiffness modification factor for in-plane stiffness in the element's local
                        x-direction, defaults to 1 (no modification).
         :type kx_mod: number, optional
         :param ky_mod: Stiffness modification factor for in-plane stiffness in the element's local
                        y-direction, defaults to 1 (no modification).
         :type ky_mod: number, optional
         :raises NameError: Occurs when the specified name already exists in the model.
@@ -379,26 +379,26 @@
             count = 1
             while name in self.Plates: 
                 name = "P" + str(len(self.Plates)+count)
                 count += 1
         
         # Create a new plate
         new_plate = Plate3D(name, self.Nodes[i_node], self.Nodes[j_node], self.Nodes[m_node],
-                           self.Nodes[n_node], t, material, self, kx_mod, ky_mod)
+                           self.Nodes[n_node], t, material_name, self, kx_mod, ky_mod)
         
         # Add the new plate to the list
         self.Plates[name] = new_plate
 
         # Flag the model as unsolved
         self.solution = None
         
         # Return the plate name
         return name
 
-    def add_quad(self, name, i_node, j_node, m_node, n_node, t, material, kx_mod=1.0, ky_mod=1.0):
+    def add_quad(self, name, i_node, j_node, m_node, n_node, t, material_name, kx_mod=1.0, ky_mod=1.0):
         """Adds a new quadrilateral to the model. The quad formulation for in-plane (membrane)
         stiffness is based on an isoparametric formulation. For bending, it is based on an MITC4
         formulation. This element handles distortion relatively well, and is appropriate for thick
         and thin plates. One limitation with this element is that it does a poor job of reporting
         corner stresses. Corner forces, however are very accurate. Center stresses are very
         accurate as well. For cases where corner stress results are important, consider using the
         `add_plate` method instead.
@@ -412,16 +412,16 @@
         :type j_node: str
         :param m_node: The name of the m-node.
         :type m_node: str
         :param n_node: The name of the n-node.
         :type n_node: str
         :param t: The thickness of the element.
         :type t: number
-        :param material: The name of the material for the element.
-        :type material: str
+        :param material_name: The name of the material for the element.
+        :type material_name: str
         :param kx_mod: Stiffness modification factor for in-plane stiffness in the element's local
             x-direction, defaults to 1 (no modification).
         :type kx_mod: number, optional
         :param ky_mod: Stiffness modification factor for in-plane stiffness in the element's local
             y-direction, defaults to 1 (no modification).
         :type ky_mod: number, optional
         :raises NameError: Occurs when the specified name already exists in the model.
@@ -438,40 +438,40 @@
             count = 1
             while name in self.Quads: 
                 name = "Q" + str(len(self.Quads) + count)
                 count += 1
         
         # Create a new member
         new_quad = Quad3D(name, self.Nodes[i_node], self.Nodes[j_node], self.Nodes[m_node],
-                         self.Nodes[n_node], t, material, self, kx_mod, ky_mod)
+                         self.Nodes[n_node], t, material_name, self, kx_mod, ky_mod)
         
         # Add the new member to the list
         self.Quads[name] = new_quad
 
         # Flag the model as unsolved
         self.solution = None
         
         #Return the quad name
         return name
 
-    def add_rectangle_mesh(self, name, mesh_size, width, height, thickness, material, kx_mod=1.0, ky_mod=1.0, origin=[0, 0, 0], plane='XY', x_control=None, y_control=None, start_node=None, start_element = None, element_type='Quad'):
+    def add_rectangle_mesh(self, name, mesh_size, width, height, thickness, material_name, kx_mod=1.0, ky_mod=1.0, origin=[0, 0, 0], plane='XY', x_control=None, y_control=None, start_node=None, start_element = None, element_type='Quad'):
         """Adds a rectangular mesh of elements to the model.
 
         :param name: A unique name for the mesh.
         :type name: str
         :param mesh_size: The desired mesh size.
         :type mesh_size: number
         :param width: The overall width of the rectangular mesh measured along its local x-axis.
         :type width: number
         :param height: The overall height of the rectangular mesh measured along its local y-axis.
         :type height: number
         :param thickness: The thickness of each element in the mesh.
         :type thickness: number
-        :param material: The name of the material for elements in the mesh.
-        :type material: str
+        :param material_name: The name of the material for elements in the mesh.
+        :type material_name: str
         :param kx_mod: Stiffness modification factor for in-plane stiffness in the element's local x-direction. Defaults to 1.0 (no modification).
         :type kx_mod: float, optional
         :param ky_mod: Stiffness modification factor for in-plane stiffness in the element's local y-direction. Defaults to 1.0 (no modification).
         :type ky_mod: float, optional
         :param origin: The origin of the regtangular mesh's local coordinate system. Defaults to [0, 0, 0]
         :type origin: list, optional
         :param plane: The plane the mesh will be parallel to. Options are 'XY', 'YZ', and 'XZ'. Defaults to 'XY'.
@@ -504,43 +504,43 @@
             start_node = self.unique_name(self.Nodes, 'N')
         if element_type == 'Rect' and start_element is None:
             start_element = self.unique_name(self.Plates, 'R')
         elif element_type == 'Quad' and start_element is None:
             start_element = self.unique_name(self.Quads, 'Q')
         
         # Create the mesh
-        new_mesh = RectangleMesh(mesh_size, width, height, thickness, material, self, kx_mod,
+        new_mesh = RectangleMesh(mesh_size, width, height, thickness, material_name, self, kx_mod,
                                  ky_mod, origin, plane, x_control, y_control, start_node,
                                  start_element, element_type=element_type)
 
         # Add the new mesh to the `Meshes` dictionary
         self.Meshes[name] = new_mesh
 
         # Flag the model as unsolved
         self.solution = None
         
         #Return the mesh's name
         return name
     
-    def add_annulus_mesh(self, name, mesh_size, outer_radius, inner_radius, thickness, material, kx_mod=1.0, 
+    def add_annulus_mesh(self, name, mesh_size, outer_radius, inner_radius, thickness, material_name, kx_mod=1.0, 
             ky_mod=1.0, origin=[0, 0, 0], axis='Y', start_node=None, start_element=None):
         """Adds a mesh of quadrilaterals forming an annulus (a donut).
 
         :param name: A unique name for the mesh.
         :type name: str
         :param mesh_size: The target mesh size.
         :type mesh_size: float
         :param outer_radius: The radius to the outside of the annulus.
         :type outer_radius: float
         :param inner_radius: The radius to the inside of the annulus.
         :type inner_radius: float
         :param thickness: Element thickness.
         :type thickness: float
-        :param material: The name of the element material.
-        :type material: str
+        :param material_name: The name of the element material.
+        :type material_name: str
         :param kx_mod: Stiffness modification factor for radial stiffness in the element's local
                        x-direction. Default is 1.0 (no modification).
         :type kx_mod: float, optional
         :param ky_mod: Stiffness modification factor for meridional stiffness in the element's
                        local y-direction. Default is 1.0 (no modification).
         :type ky_mod: float, optional
         :param origin: The origin of the mesh. The default is [0, 0, 0].
@@ -569,43 +569,43 @@
         # Identify the starting node and element
         if start_node is None:
             start_node = self.unique_name(self.Nodes, 'N')
         if start_element is None:
             start_element = self.unique_name(self.Quads, 'Q')
         
         # Create a new mesh
-        new_mesh = AnnulusMesh(mesh_size, outer_radius, inner_radius, thickness, material, self,
+        new_mesh = AnnulusMesh(mesh_size, outer_radius, inner_radius, thickness, material_name, self,
                                kx_mod, ky_mod, origin, axis, start_node, start_element)
 
         # Add the new mesh to the `Meshes` dictionary
         self.Meshes[name] = new_mesh
 
         # Flag the model as unsolved
         self.solution = None
         
         #Return the mesh's name
         return name
 
-    def add_frustrum_mesh(self, name, mesh_size, large_radius, small_radius, height, thickness,material, kx_mod=1.0, ky_mod=1.0, origin=[0, 0, 0], axis='Y', start_node=None, start_element=None):
+    def add_frustrum_mesh(self, name, mesh_size, large_radius, small_radius, height, thickness,material_name, kx_mod=1.0, ky_mod=1.0, origin=[0, 0, 0], axis='Y', start_node=None, start_element=None):
         """Adds a mesh of quadrilaterals forming a frustrum (a cone intersected by a horizontal plane).
 
         :param name: A unique name for the mesh.
         :type name: str
         :param mesh_size: The target mesh size
         :type mesh_size: number
         :param large_radius: The larger of the two end radii.
         :type large_radius: number
         :param small_radius: The smaller of the two end radii.
         :type small_radius: number
         :param height: The height of the frustrum.
         :type height: number
         :param thickness: The thickness of the elements.
         :type thickness: number
-        :param material: The name of the element material.
-        :type material: str
+        :param material_name: The name of the element material.
+        :type material_name: str
         :param kx_mod: Stiffness modification factor for radial stiffness in each element's local x-direction, defaults to 1 (no modification).
         :type kx_mod: number, optional
         :param ky_mod: Stiffness modification factor for meridional stiffness in each element's local y-direction, defaults to 1 (no modification).
         :type ky_mod: number, optional
         :param origin: The origin of the mesh, defaults to [0, 0, 0].
         :type origin: list, optional
         :param axis: The global axis about which the mesh will be generated, defaults to 'Y'.
@@ -631,43 +631,43 @@
         # Identify the starting node and element
         if start_node is None:
             start_node = self.unique_name(self.Nodes, 'N')
         if start_element is None:
             start_element = self.unique_name(self.Quads, 'Q')
         
         # Create a new mesh
-        new_mesh = FrustrumMesh(mesh_size, large_radius, small_radius, height, thickness, material,
+        new_mesh = FrustrumMesh(mesh_size, large_radius, small_radius, height, thickness, material_name,
                                 self, kx_mod, ky_mod, origin, axis, start_node, start_element)
 
         # Add the new mesh to the `Meshes` dictionary
         self.Meshes[name] = new_mesh
 
         # Flag the model as unsolved
         self.solution = None
         
         #Return the mesh's name
         return name
     
-    def add_cylinder_mesh(self, name, mesh_size, radius, height, thickness, material, kx_mod=1,
+    def add_cylinder_mesh(self, name, mesh_size, radius, height, thickness, material_name, kx_mod=1,
                           ky_mod=1, origin=[0, 0, 0], axis='Y', num_elements=None, start_node=None,
                           start_element=None, element_type='Quad'):
         """Adds a mesh of elements forming a cylinder.
 
         :param name: A unique name for the mesh.
         :type name: str
         :param mesh_size: The target mesh size.
         :type mesh_size: float
         :param radius: The radius of the cylinder.
         :type radius: float
         :param height: The height of the cylinder.
         :type height: float
         :param thickness: Element thickness.
         :type thickness: float
-        :param material: The name of the element material.
-        :type material: str
+        :param material_name: The name of the element material.
+        :type material_name: str
         :param kx_mod: Stiffness modification factor for hoop stiffness in each element's local
                        x-direction. Defaults to 1.0 (no modification).
         :type kx_mod: int, optional
         :param ky_mod: Stiffness modification factor for meridional stiffness in each element's
                        local y-direction. Defaults to 1.0 (no modification).
         :type ky_mod: int, optional
         :param origin: The origin [X, Y, Z] of the mesh. Defaults to [0, 0, 0].
@@ -707,15 +707,15 @@
             start_node = self.unique_name(self.Nodes, 'N')
         if element_type == 'Rect' and start_element is None:
             start_element = self.unique_name(self.Plates, 'R')
         elif element_type == 'Quad' and start_element is None:
             start_element = self.unique_name(self.Quads, 'Q')
         
         # Create a new mesh
-        new_mesh = CylinderMesh(mesh_size, radius, height, thickness, material, self,
+        new_mesh = CylinderMesh(mesh_size, radius, height, thickness, material_name, self,
                                kx_mod, ky_mod, origin, axis, start_node, start_element,
                                num_elements, element_type)
 
         # Add the new mesh to the `Meshes` dictionary
         self.Meshes[name] = new_mesh
 
         # Flag the model as unsolved
@@ -1173,15 +1173,15 @@
         :type case: str, optional
         """
 
         # Step through each member in the model
         for member in self.Members.values():
 
             # Calculate the self weight of the member
-            self_weight = factor*member.material.rho*member.A
+            self_weight = factor*self.Materials[member.material_name].rho*member.A
 
             # Add the self-weight load to the member
             self.add_member_dist_load(member.name, global_direction, self_weight, self_weight, case=case)
         
         # No need to flag the model as unsolved. That has already been taken care of by our call to `add_member_dist_load`
 
     def add_plate_surface_pressure(self, plate_name, pressure, case='Case 1'):
```

### Comparing `PyNiteFEA-0.0.93/PyNite/FixedEndReactions.py` & `pynitefea-0.0.94/PyNite/FixedEndReactions.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.93/PyNite/LoadCombo.py` & `pynitefea-0.0.94/PyNite/LoadCombo.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.93/PyNite/MainStyleSheet.css` & `pynitefea-0.0.94/PyNite/MainStyleSheet.css`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.93/PyNite/Member3D.py` & `pynitefea-0.0.94/PyNite/Member3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,26 +18,26 @@
     """
 
     # '__plt' is used to store the 'pyplot' from matplotlib once it gets imported. Setting it to 'None' for now allows
     # us to defer importing it until it's actually needed.
     __plt = None
 
 #%%
-    def __init__(self, name, i_node, j_node, material, model, Iy, Iz, J, A, auxNode=None,
+    def __init__(self, name, i_node, j_node, material_name, model, Iy, Iz, J, A, auxNode=None,
                  tension_only=False, comp_only=False, section_name=None):
         """
         Initializes a new member.
         """
         self.name = name      # A unique name for the member given by the user
         self.ID = None        # Unique index number for the member assigned by the program
         self.i_node = i_node  # The element's i-node
         self.j_node = j_node  # The element's j-node
-        self.material = material  # The element's material
-        self.E = model.Materials[material].E   # The modulus of elasticity of the element
-        self.G = model.Materials[material].G   # The shear modulus of the element
+        self.material_name = material_name  # The element's material
+        self.E = model.Materials[material_name].E   # The modulus of elasticity of the element
+        self.G = model.Materials[material_name].G   # The shear modulus of the element
 
         # Section properties
         if section_name is None:
             self.section = None
             self.A = A            # The cross-sectional area
             self.Iy = Iy          # The y-axis moment of inertia
             self.Iz = Iz          # The z-axis moment of inertia
```

### Comparing `PyNiteFEA-0.0.93/PyNite/Mesh.py` & `pynitefea-0.0.94/PyNite/Mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 #%%
 class Mesh():
     """
     A parent class for meshes to inherit from.
     """
 
-    def __init__(self, thickness, material, model, kx_mod=1, ky_mod=1, start_node='N1', start_element='Q1'):
+    def __init__(self, thickness, material_name, model, kx_mod=1, ky_mod=1, start_node='N1', start_element='Q1'):
 
         self.thickness = thickness          # Thickness
-        self.material = material            # The name of the element material
+        self.material_name = material_name            # The name of the element material
         self.model = model                  # Meshes need a link to the model they belong to
         self.kx_mod = kx_mod                # Local x stiffness modification factor for elements in the mesh
         self.ky_mod = ky_mod                # Local y stiffness modification factor for elements in the mesh
         self.start_node = start_node        # The name of the first node in the mesh
         self.last_node = None               # The name of the last node in the mesh
         self.start_element = start_element  # The name of the first element in the mesh
         self.last_element = None            # The name of the last element in the mesh
@@ -358,29 +358,29 @@
             
         # Return the smallest value encountered from all the elements
         return M_min
     
 #%%
 class RectangleMesh(Mesh):
 
-    def __init__(self, mesh_size, width, height, thickness, material, model, kx_mod=1, ky_mod=1, origin=[0, 0, 0], plane='XY', x_control=None, y_control=None, start_node='N1', start_element='Q1', element_type='Quad'):
+    def __init__(self, mesh_size, width, height, thickness, material_name, model, kx_mod=1, ky_mod=1, origin=[0, 0, 0], plane='XY', x_control=None, y_control=None, start_node='N1', start_element='Q1', element_type='Quad'):
         """
         A rectangular mesh of elements.
 
         Parameters
         ----------
         mesh_size : number
             Desired mesh size.
         width : number
             The overall width of the mesh measured along its local x-axis.
         height : number
             The overall height of the mesh measured along its local y-axis.
         thickness : number
             Element thickness.
-        material : string
+        material_name : string
             The name of the element material.
         model : FEModel3D
             The model the mesh belongs to.
         kx_mod : number
             Stiffness modification factor for in-plane stiffness in the element's local
             x-direction. Default value is 1.0 (no modification).
         ky_mod : number
@@ -406,15 +406,15 @@
 
         Returns
         -------
         A new rectangular mesh object.
 
         """
         
-        super().__init__(thickness, material, model, kx_mod, ky_mod, start_node, start_element)
+        super().__init__(thickness, material_name, model, kx_mod, ky_mod, start_node, start_element)
         self.mesh_size = mesh_size
         self.width = width
         self.height = height
         self.origin = origin
         self.plane = plane
 
         if x_control is None: self.x_control = []
@@ -588,21 +588,21 @@
             n += 1
             
             if element_type == 'Quad':
                 self.elements[element_name] = Quad3D(element_name, self.nodes['N' + str(i_node + node_offset)],
                                                                    self.nodes['N' + str(j_node + node_offset)],
                                                                    self.nodes['N' + str(m_node + node_offset)],
                                                                    self.nodes['N' + str(n_node + node_offset)],
-                                                                   self.thickness, self.material, self.model, self.kx_mod, self.ky_mod)
+                                                                   self.thickness, self.material_name, self.model, self.kx_mod, self.ky_mod)
             else:
                 self.elements[element_name] = Plate3D(element_name, self.nodes['N' + str(i_node + node_offset)],
                                                                     self.nodes['N' + str(j_node + node_offset)],
                                                                     self.nodes['N' + str(m_node + node_offset)],
                                                                     self.nodes['N' + str(n_node + node_offset)],
-                                                                    self.thickness, self.material, self.model, self.kx_mod, self.ky_mod)
+                                                                    self.thickness, self.material_name, self.model, self.kx_mod, self.ky_mod)
 
         # Initialize a list of nodes and associated elements that fall within opening boundaries
         # that will be deleted
         node_del_list = []
         element_del_list = []
 
         # Go back through the mesh and delete any nodes that are in the openings
@@ -762,18 +762,18 @@
 
 #%%           
 class AnnulusMesh(Mesh):
     """
     A mesh of quadrilaterals forming an annulus (a donut).
     """
 
-    def __init__(self, mesh_size, outer_radius, inner_radius, thickness, material, model, kx_mod=1,
+    def __init__(self, mesh_size, outer_radius, inner_radius, thickness, material_name, model, kx_mod=1,
         ky_mod=1, origin=[0, 0, 0], axis='Y', start_node='N1', start_element='Q1'):
 
-        super().__init__(thickness, material, model, kx_mod, ky_mod, start_node, start_element)
+        super().__init__(thickness, material_name, model, kx_mod, ky_mod, start_node, start_element)
 
         self.inner_radius = inner_radius
         self.outer_radius = outer_radius
         self.mesh_size = mesh_size
         self.origin = origin
         self.axis = axis
 
@@ -808,22 +808,22 @@
             if b_circ > 3*mesh_size:
                 transition = True
             else:
                 transition = False
         
             # Create a mesh of nodes for the ring
             if transition == True:
-                ring = AnnulusTransRingMesh(r_inner + h_rad, r_inner, n_circ, self.thickness, self.material, self.model, self.kx_mod, self.ky_mod,
+                ring = AnnulusTransRingMesh(r_inner + h_rad, r_inner, n_circ, self.thickness, self.material_name, self.model, self.kx_mod, self.ky_mod,
                                             self.origin, self.axis, 'N' + str(n), 'Q' + str(q))
                 n += 3*n_circ
                 q += 4*n_circ
                 n_circ *= 3
                 self.num_quads_outer = n_circ
             else:
-                ring = AnnulusRingMesh(r_inner + h_rad, r_inner, n_circ, self.thickness, self.material, self.model, self.kx_mod, self.ky_mod, self.origin,
+                ring = AnnulusRingMesh(r_inner + h_rad, r_inner, n_circ, self.thickness, self.material_name, self.model, self.kx_mod, self.ky_mod, self.origin,
                                        self.axis, 'N' + str(n), 'Q' + str(q))
                 n += n_circ
                 q += n_circ
         
             # Add the newly generated nodes and elements to the overall mesh. Note that if duplicate
             # keys exist, the `.update()` method will overwrite them with the newly generated key value
             # pairs. This works in our favor by automatically eliminating duplicate nodes from the
@@ -859,18 +859,18 @@
 
 #%%
 class AnnulusRingMesh(Mesh):
     """
     A mesh of quadrilaterals forming an annular ring (a donut).
     """
 
-    def __init__(self, outer_radius, inner_radius, num_quads, thickness, material, model, kx_mod=1, ky_mod=1,
+    def __init__(self, outer_radius, inner_radius, num_quads, thickness, material_name, model, kx_mod=1, ky_mod=1,
                  origin=[0, 0, 0], axis='Y', start_node='N1', start_element='Q1'):
 
-        super().__init__(thickness, material, model, kx_mod, ky_mod, start_node=start_node,
+        super().__init__(thickness, material_name, model, kx_mod, ky_mod, start_node=start_node,
                          start_element=start_element)
 
         self.inner_radius = inner_radius
         self.outer_radius = outer_radius
         self.n = num_quads
         self.Xo = origin[0]
         self.Yo = origin[1]
@@ -962,15 +962,15 @@
                 m_node = 1
                 j_node = 1 + n
 
             self.elements[element_name] = Quad3D(element_name, self.nodes['N' + str(i_node + node_offset)],
                                                                self.nodes['N' + str(j_node + node_offset)],
                                                                self.nodes['N' + str(m_node + node_offset)],
                                                                self.nodes['N' + str(n_node + node_offset)],
-                                                               self.thickness, self.material, self.model, self.kx_mod, self.ky_mod)
+                                                               self.thickness, self.material_name, self.model, self.kx_mod, self.ky_mod)
 
         # Add the nodes and elements to the model
         for node in self.nodes.values():
             self.model.Nodes[node.name] = node
         
         # Add the elements to the model
         for element in self.elements.values():
@@ -985,25 +985,25 @@
 #%%
 class AnnulusTransRingMesh(Mesh):
     """
     A mesh of quadrilaterals forming an annular ring (a donut) with the mesh getting finer on the outer
     edge.
     """
 
-    def __init__(self, outer_radius, inner_radius, num_inner_quads, thickness, material, model,
+    def __init__(self, outer_radius, inner_radius, num_inner_quads, thickness, material_name, model,
                  kx_mod=1, ky_mod=1, origin=[0, 0, 0], axis='Y', start_node='N1',
                  start_element='Q1'):
         """
         Parameters
         ----------
         direction : array
             A vector indicating the direction normal to the ring.
         """
 
-        super().__init__(thickness, material, model, kx_mod, ky_mod, start_node=start_node,
+        super().__init__(thickness, material_name, model, kx_mod, ky_mod, start_node=start_node,
                          start_element=start_element)
 
         self.inner_radius = inner_radius
         self.outer_radius = (inner_radius + outer_radius)/2
         self.r3 = outer_radius
         self.n = num_inner_quads
         self.Xo = origin[0]
@@ -1140,15 +1140,15 @@
                     m_node = 1
                     j_node = 1 + 3*n
 
             self.elements[element_name] = Quad3D(element_name, self.nodes['N' + str(i_node + node_offset)],
                                                                self.nodes['N' + str(j_node + node_offset)],
                                                                self.nodes['N' + str(m_node + node_offset)],
                                                                self.nodes['N' + str(n_node + node_offset)],
-                                                               self.thickness, self.material, self.model, self.kx_mod, self.ky_mod)
+                                                               self.thickness, self.material_name, self.model, self.kx_mod, self.ky_mod)
 
         # Add the nodes and elements to the model
         for node in self.nodes.values():
             self.model.Nodes[node.name] = node
         
         for element in self.elements.values():
             if element.type == 'Quad':
@@ -1161,19 +1161,19 @@
 
 #%%
 class FrustrumMesh(AnnulusMesh):
     """
     A mesh of quadrilaterals forming a frustrum (a cone intersected by a horizontal plane).
     """
 
-    def __init__(self, mesh_size, large_radius, small_radius, height, thickness, material, model, kx_mod=1, ky_mod=1,
+    def __init__(self, mesh_size, large_radius, small_radius, height, thickness, material_name, model, kx_mod=1, ky_mod=1,
                  origin=[0, 0, 0], axis='Y', start_node='N1', start_element='Q1'):
         
         # Create an annulus mesh
-        super().__init__(mesh_size, large_radius, small_radius, thickness, material, model, kx_mod,
+        super().__init__(mesh_size, large_radius, small_radius, thickness, material_name, model, kx_mod,
                          ky_mod, origin, axis, start_node, start_element)
         
         self.height = height
     
     def generate(self):
 
         super().generate()
@@ -1212,15 +1212,15 @@
         specified. Otherwise it will be used to mesh the circumference too.
     radius : number
         The radius of the cylinder to the element centers
     height : number
         Total height of the cylinder.
     thickness : number
         Element thickness.
-    material : string
+    material_name : string
         The name of the element material.
     kx_mod : number
         Stiffness modification factor for in-plane stiffness in the element's local
         x-direction. Default value is 1.0 (no modification).
     ky_mod : number
         Stiffness modification factor for in-plane stiffness in the element's local
         y-direction. Default value is 1.0 (no modification).
@@ -1236,18 +1236,18 @@
         The number of quadrilaterals to divide the circumference into. If this value is omitted
         `mesh_size` will be used instead to calculate the number of quadrilaterals in the
         circumference. The default is `None`.
     element_type : string
         The type of element to use for the mesh: 'Quad' or 'Rect'
     """
 
-    def __init__(self, mesh_size, radius, height, thickness, material, model, kx_mod=1, ky_mod=1,origin=[0, 0, 0], axis='Y', start_node='N1', start_element='Q1', num_elements=None, element_type='Quad'):
+    def __init__(self, mesh_size, radius, height, thickness, material_name, model, kx_mod=1, ky_mod=1,origin=[0, 0, 0], axis='Y', start_node='N1', start_element='Q1', num_elements=None, element_type='Quad'):
 
         # Inherit properties and methods from the parent `Mesh` class
-        super().__init__(thickness, material, model, kx_mod, ky_mod, start_node, start_element)
+        super().__init__(thickness, material_name, model, kx_mod, ky_mod, start_node, start_element)
 
         # Define a few new additional class properties related to cylinders
         self.radius = radius
         self.h = height
         self.mesh_size = mesh_size
         self.origin = origin
         self.axis = axis
@@ -1266,15 +1266,15 @@
         # Generate the mesh
         self.generate()
     
     def generate(self):
         
         # Get the mesh thickness and the material name
         thickness = self.thickness
-        material = self.material
+        material_name = self.material_name
 
         mesh_size = self.mesh_size  # Desired mesh size
         num_elements = self.num_elements  # Number of quadrilaterals in each course of the ring
         n = self.num_elements  # Total number of elements in the mesh (initialized for a single ring at the moment)
 
         radius = self.radius
         h = self.h
@@ -1301,19 +1301,19 @@
 
             height = h - y  #Remaining height to be meshed
             # Number of times the plate height fits in the remaining unmeshed height, resulting at least one element
             n_vert = max(int(abs(height)/mesh_size),1)
             h_y = height/n_vert             # Element height in the vertical direction
             # Create a mesh of nodes for the ring
             if self.axis == 'Y':
-                ring = CylinderRingMesh(radius, h_y, num_elements, thickness, material, self.model, 1, 1, [0, y, 0], self.axis, 'N' + str(n), 'Q' + str(q), element_type)
+                ring = CylinderRingMesh(radius, h_y, num_elements, thickness, material_name, self.model, 1, 1, [0, y, 0], self.axis, 'N' + str(n), 'Q' + str(q), element_type)
             elif self.axis == 'X':
-                ring = CylinderRingMesh(radius, h_y, num_elements, thickness, material, self.model, 1, 1, [y, 0, 0], self.axis, 'N' + str(n), 'Q' + str(q), element_type)
+                ring = CylinderRingMesh(radius, h_y, num_elements, thickness, material_name, self.model, 1, 1, [y, 0, 0], self.axis, 'N' + str(n), 'Q' + str(q), element_type)
             elif self.axis == 'Z':
-                ring = CylinderRingMesh(radius, h_y, num_elements, thickness, material, self.model, 1, 1, [0, 0, y], self.axis, 'N' + str(n), 'Q' + str(q), element_type)
+                ring = CylinderRingMesh(radius, h_y, num_elements, thickness, material_name, self.model, 1, 1, [0, 0, y], self.axis, 'N' + str(n), 'Q' + str(q), element_type)
 
             n += num_elements
             q += num_elements
         
             # Add the newly generated nodes and elements to the overall mesh. Note that if duplicate keys exist, the `.update()` method will overwrite them with the newly generated key value pairs. This works in our favor by automatically eliminating duplicate nodes at the shared boundaries between rings.
             self.nodes.update(ring.nodes)
             self.elements.update(ring.elements)
@@ -1352,15 +1352,15 @@
         Radius to the center of the plates in the cylindrical ring.
     height : number
         Height of the cylindrical ring.
     num_elements : number
         Number of elements used to generate the cylindrical ring.
     thickness : number
         Element thickness.
-    material : string
+    material_name : string
         The name of the element material.
     kx_mod : number
         Stiffness modification factor for in-plane stiffness in the element's local
         x-direction. Default value is 1.0 (no modification).
     ky_mod : number
         Stiffness modification factor for in-plane stiffness in the element's local
         y-direction. Default value is 1.0 (no modification).
@@ -1377,19 +1377,19 @@
         single letter followed by a number (e.g. 'Q32'). The mesh will begin numbering elements
         from this number. The default is 'Q1'.
     num_elements : number
         The number of elements to divide the circumference into.
     
     """
 
-    def __init__(self, radius, height, num_elements, thickness, material, model, kx_mod=1, ky_mod=1,
+    def __init__(self, radius, height, num_elements, thickness, material_name, model, kx_mod=1, ky_mod=1,
                  origin=[0, 0, 0], axis='Y', start_node='N1', start_element='Q1',
                  element_type='Quad'):
 
-        super().__init__(thickness, material, model, kx_mod, ky_mod, start_node=start_node, start_element=start_element)
+        super().__init__(thickness, material_name, model, kx_mod, ky_mod, start_node=start_node, start_element=start_element)
 
         self.radius = radius
         self.height = height
         self.num_elements = num_elements
         self.Xo = origin[0]
         self.Yo = origin[1]
         self.Zo = origin[2]
@@ -1499,21 +1499,21 @@
 
             # Create the element and add it to the `elements` dictionary
             if self.element_type == 'Quad':
                 self.elements[element_name] = Quad3D(element_name, self.nodes['N' + str(i_node + node_offset)],
                                                      self.nodes['N' + str(j_node + node_offset)],
                                                      self.nodes['N' + str(m_node + node_offset)],
                                                      self.nodes['N' + str(n_node + node_offset)],
-                                                     self.thickness, self.material, self.model, self.kx_mod, self.ky_mod)
+                                                     self.thickness, self.material_name, self.model, self.kx_mod, self.ky_mod)
             elif self.element_type == 'Rect':
                 self.elements[element_name] = Plate3D(element_name, self.nodes['N' + str(i_node + node_offset)],
                                                       self.nodes['N' + str(j_node + node_offset)],
                                                       self.nodes['N' + str(m_node + node_offset)],
                                                       self.nodes['N' + str(n_node + node_offset)],
-                                                      self.thickness, self.material, self.model, self.kx_mod, self.ky_mod)
+                                                      self.thickness, self.material_name, self.model, self.kx_mod, self.ky_mod)
         
         # Add the nodes and elements to the model
         for node in self.nodes.values():
             self.model.Nodes[node.name] = node
         
         for element in self.elements.values():
             if element.type == 'Quad':
```

### Comparing `PyNiteFEA-0.0.93/PyNite/Node3D.py` & `pynitefea-0.0.94/PyNite/Node3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.93/PyNite/PhysMember.py` & `pynitefea-0.0.94/PyNite/PhysMember.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     """
     A physical member.
 
     Physical members can detect internal nodes and subdivide themselves into sub-members at those
     nodes.
     """
 
-    def __init__(self, name, i_node, j_node, material, model, Iy, Iz, J, A, aux_node=None,
+    def __init__(self, name, i_node, j_node, material_name, model, Iy, Iz, J, A, aux_node=None,
                  tension_only=False, comp_only=False, section_name=None):
         
-        super().__init__(name, i_node, j_node, material, model, Iy, Iz, J, A, aux_node, tension_only, comp_only, section_name)
+        super().__init__(name, i_node, j_node, material_name, model, Iy, Iz, J, A, aux_node, tension_only, comp_only, section_name)
         self.sub_members = {}
 
     def descritize(self):
         """
         Subdivides the physical member into sub-members at each node along the physical member
         """
 
@@ -75,15 +75,15 @@
             j_node = int_nodes[i+1][0]
             xi = int_nodes[i][1]
             xj = int_nodes[i+1][1]
 
             # Create a new sub-member
             if self.section is None: section_name = None
             else: section_name = self.section.name
-            new_sub_member = Member3D(name, i_node, j_node, self.material, self.model, self.Iy, self.Iz, self.J, self.A, self.auxNode, self.tension_only, self.comp_only, section_name)
+            new_sub_member = Member3D(name, i_node, j_node, self.material_name, self.model, self.Iy, self.Iz, self.J, self.A, self.auxNode, self.tension_only, self.comp_only, section_name)
             
             # Flag the sub-member as active
             for combo_name in self.model.LoadCombos.keys():
                 new_sub_member.active[combo_name] = True
 
             # Apply end releases if applicable
             if i == 0:
```

### Comparing `PyNiteFEA-0.0.93/PyNite/Plastic Beam.py` & `pynitefea-0.0.94/PyNite/Plastic Beam.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.93/PyNite/Plate3D.py` & `pynitefea-0.0.94/PyNite/Plate3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from numpy import zeros, array, matmul, cross, add
 from numpy.linalg import inv, norm, det
 
 #%%
 class Plate3D():
 
-    def __init__(self, name, i_node, j_node, m_node, n_node, t, material, model, kx_mod=1.0,
+    def __init__(self, name, i_node, j_node, m_node, n_node, t, material_name, model, kx_mod=1.0,
                  ky_mod=1.0):
         """
         A rectangular plate element
 
         Parameters
         ----------
         name : string
@@ -19,15 +19,15 @@
             The plate's j-node
         m_node : Node3D
             The plate's m-node
         n_node : Node3D
             The plate's n-node
         t : number
             Plate thickness
-        material : string
+        material_name : string
             The name of the plate material
         kx_mod : number
             Modification factor for stiffness in the plate's local x-direction. Default value is
             1.0, which indicates no stiffness modification (100% stiffness).
         ky_mod : number
             Modification factor for stiffness in the plate's local y-direction. Default value is
             1.0, which indicates no stiffness modification (100% stiffness).
@@ -52,18 +52,18 @@
         self.pressures = []  # A list of surface pressures [pressure, case='Case 1']
 
         # Plates need a link to the model they belong to
         self.model = model
 
         # Get material properties for the plate from the model
         try:
-            self.E = self.model.Materials[material].E
-            self.nu = self.model.Materials[material].nu
+            self.E = self.model.Materials[material_name].E
+            self.nu = self.model.Materials[material_name].nu
         except:
-            raise KeyError('Please define the material ' + str(material) + ' before assigning it to plates.')
+            raise KeyError('Please define the material ' + str(material_name) + ' before assigning it to plates.')
     
     def width(self):
         """
         Returns the width of the plate along its local x-axis
         """
         return self.i_node.distance(self.j_node)
```

### Comparing `PyNiteFEA-0.0.93/PyNite/Quad3D.py` & `pynitefea-0.0.94/PyNite/Quad3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     This element performs well for thick and thin plates, and for skewed plates. Element center
     stresses and corner FORCES converge rapidly; however, corner STRESSES are more representative
     of center stresses. Minor errors are introduced into the solution due to the drilling
     approximation. Orthotropic behavior is limited to acting along the plate's local axes.
     """
 
 #%%
-    def __init__(self, name, i_node, j_node, m_node, n_node, t, material, model, kx_mod=1.0,
+    def __init__(self, name, i_node, j_node, m_node, n_node, t, material_name, model, kx_mod=1.0,
                  ky_mod=1.0):
 
         self.name = name
         self.ID = None
         self.type = 'Quad'
 
         self.i_node = i_node
@@ -41,18 +41,18 @@
         self.pressures = []  # A list of surface pressures [pressure, case='Case 1']
     
         # Quads need a link to the model they belong to
         self.model = model
 
         # Get material properties for the plate from the model
         try:
-            self.E = self.model.Materials[material].E
-            self.nu = self.model.Materials[material].nu
+            self.E = self.model.Materials[material_name].E
+            self.nu = self.model.Materials[material_name].nu
         except:
-            raise KeyError('Please define the material ' + str(material) + ' before assigning it to plates.')
+            raise KeyError('Please define the material ' + str(material_name) + ' before assigning it to plates.')
 
 #%%
     def _local_coords(self):
         '''
         Calculates or recalculates and stores the local (x, y) coordinates for each node of the
         quadrilateral.
         '''
```

### Comparing `PyNiteFEA-0.0.93/PyNite/Report_Template.html` & `pynitefea-0.0.94/PyNite/Report_Template.html`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.93/PyNite/Reporting.py` & `pynitefea-0.0.94/PyNite/Reporting.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.93/PyNite/Section.py` & `pynitefea-0.0.94/PyNite/Section.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 import numpy as np
 
 class Section():
 
-    def __init__(self, model, name, A, Iy, Iz, J, material):
+    def __init__(self, model, name, A, Iy, Iz, J, material_name):
         
         self.model = model
         self.name = name
         self.A = A
         self.Iy = Iy
         self.Iz = Iz
         self.J = J
-        self.material = material
-        self.fy = model.Materials[material].fy
+        self.material_name = material_name
+        self.fy = model.Materials[material_name].fy
     
     def Phi(self):
         pass
 
     def G(self, fx, my, mz):
         """Returns the gradient to the yield surface at a given point using numerical differentiation. This is a default solution. For a better solution, overwrite this method with a more precies one in the material/shape specific child class that inherits from this class.
         """
@@ -35,18 +35,18 @@
                          [0],
                          [0],
                          [dPhi_dmy],
                          [dPhi_dmz]])
 
 class SteelSection(Section):
 
-    def __init__(self, model, name, A, Iy, Iz, J, Zy, Zz, material):
+    def __init__(self, model, name, A, Iy, Iz, J, Zy, Zz, material_name):
 
         # Basic section properties
-        super().__init__(model, name, A, Iy, Iz, J, material)
+        super().__init__(model, name, A, Iy, Iz, J, material_name)
 
         # Additional section properties for steel
         self.ry = (Iy/A)**0.5
         self.rz = (Iz/A)**0.5
         self.Zy = Zy
         self.Zz = Zz
```

### Comparing `PyNiteFEA-0.0.93/PyNite/Spring3D.py` & `pynitefea-0.0.94/PyNite/Spring3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
 #%%
     def __init__(self, name, i_node, j_node, ks, LoadCombos={'Combo 1':LoadCombo('Combo 1', factors={'Case 1':1.0})},
                  tension_only=False, comp_only=False):
         '''
         Initializes a new spring.
         '''
-        self.name = name    # A unique name for the spring given by the user
-        self.ID = None      # Unique index number for the spring assigned by the program
+        self.name = name      # A unique name for the spring given by the user
+        self.ID = None        # Unique index number for the spring assigned by the program
         self.i_node = i_node  # The spring's i-node
         self.j_node = j_node  # The spring's j-node
-        self.ks = ks        # The spring constant (force/displacement)
+        self.ks = ks          # The spring constant (force/displacement)
         self.LoadCombos = LoadCombos # The dictionary of load combinations in the model this spring belongs to
         self.tension_only = tension_only # Indicates whether the spring is tension-only
         self.comp_only = comp_only # Indicates whether the spring is compression-only
 
         # Springs need to track whether they are active or not for any given load combination.
         # They may become inactive for a load combination during a tension/compression-only
         # analysis. This dictionary will be used when the model is solved.
```

### Comparing `PyNiteFEA-0.0.93/PyNite/Visualization.py` & `pynitefea-0.0.94/PyNite/Visualization.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.93/PyNite/Visualization_PyVista.py` & `pynitefea-0.0.94/PyNite/Rendering.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 
 from json import load
 import warnings
 
 from IPython.display import Image
-from numpy import array, empty, append, cross, zeros
-from numpy.linalg import norm
+import numpy as np
 import pyvista as pv
+import math
+
+# Allow for 3D interaction within jupyter notebook using trame
+try:
+    pv.global_theme.trame.jupyter_extension_enabled = True
+except:
+    # Ignore the exception that is produced if we are not running the code via jupyter
+    pass
+pv.set_jupyter_backend('trame')
 
 class Renderer:
     """Used to render finite element models.
     """
 
     scalar = None
 
@@ -34,14 +42,22 @@
         self.plotter = pv.Plotter()
         self.plotter.set_background('white')  # Setting background color
         # self.plotter.add_logo_widget('./Resources/Full Logo No Buffer - Transparent.png')
         # self.plotter.view_isometric()
         self.plotter.view_xy()
         self.plotter.show_axes()
 
+        # Initialize load labels
+        self._load_label_points = []
+        self._load_labels = []
+
+        # Initialize spring labels
+        self._spring_label_points = []
+        self._spring_labels = []
+
     @property
     def window_width(self):
         return self.plotter.window_size[0]
 
     @window_width.setter
     def window_width(self, width):
         height = self.plotter.window_size[1]
@@ -142,15 +158,15 @@
     def scalar_bar_text_size(self):
         return self._scalar_bar_text_size
     
     @scalar_bar_text_size.setter
     def scalar_bar_text_size(self, text_size):
         self._scalar_bar_text_size = text_size
 
-    def render_model(self, interact=True, reset_camera=True):
+    def render_model(self, reset_camera=True):
         """
         Renders the model in a window
 
         Parameters
         ----------
         interact : bool
             Suppresses interacting with the window if set to `False`. This can be used to capture a
@@ -159,41 +175,41 @@
             Resets the camera if set to `True`. Default is `True`.
         """
 
         # Update the plotter with the latest geometry
         self.update(reset_camera)
 
         # Render the model (code execution will pause here until the user closes the window)
-        self.plotter.show(title='Pynite - Simple Finite Element Analysis for Python', window_size=None, interactive=True, auto_close=None, interactive_update=False, full_screen=None, screenshot=False, return_img=False, cpos=None, jupyter_backend=None, return_viewer=False, return_cpos=None, before_close_callback=None)
+        self.plotter.show(title='Pynite - Simple Finite Element Analysis for Python')
 
-    def screenshot(self, filepath='console', interact=True, reset_camera=True):
-        """
-        Renders the model in a window. When the window is closed a screenshot is captured.
+    def screenshot(self, filepath='./Pynite_Image.png', interact=True, reset_camera=True):
+        """Saves a screenshot of the rendered model. Press `q` to capture the screenshot after positioning the view. Pressing the close button in the corner of the window will ignore the positioning.
 
-        Parameters
-        ----------
-        filepath : string
-            Sends a screenshot to the specified filepath. The screenshot will be taken when the
-            user closes out of the render window.
-        interact : bool
-            Suppresses interacting with the window if set to `False`. This can be used to capture a
-            screenshot without pausing the program for the user to interact. Default is `True`.
-        reset_camera : bool
-            Resets the camera if set to `True`. Default is `True`.
+        :param filepath: The filepath to write the image to. When set to 'jupyter', the resulting plot is placed inline in a jupyter notebook. Defaults to 'jupyter'.
+        :type filepath: str, optional
+        :param interact: When set to `True` the user can set the scene before the screenshot is taken. Once the scene is set, press 'q' to take the screenshot. Defaults to `True`
+        :type interact: bool, optional
+        :param reset_camera: Resets the plotter's camera. Defaults to `True`
+        :type reset_camera: bool, optional
         """
 
         # Update the plotter with the latest geometry
         self.update(reset_camera)
 
         # Show the plotter for interaction
         if interact == True:
-            self.plotter.show(auto_close=False)
+            # Use `q` for `quit` to take the screenshot. The window will not close until the `X` in
+            # the corner of the window is hit.
+            self.plotter.show(title='Pynite - Simple Finite Element Anlaysis for Python', screenshot=filepath)
+        else:
+            # Don't bother showing the image before capturing the screenshot
+            self.plotter.off_screen = True
 
-        # Render the model (code execution will pause here until the user closes the window)
-        self.plotter.show(title='Pynite - Simple Finite Element Analysis for Python', window_size=None, interactive=True, auto_close=None, interactive_update=False, full_screen=None, screenshot=filepath, return_img=False, cpos=None, jupyter_backend=None, return_viewer=False, return_cpos=None, before_close_callback=None)
+            # Save the screenshot
+            self.plotter.screenshot(filename=filepath)
 
     def update(self, reset_camera=True):
         """
         Builds or rebuilds the pyvista plotter
 
         Parameters
         ----------
@@ -207,108 +223,102 @@
                             ' not load cases.')
         if self.model.LoadCombos == {} and self.render_loads == True and self.case == None:
             self.render_loads = False
             warnings.warn('Unable to render load combination. No load combinations defined.', UserWarning)
 
         # Clear out the old plot (if any)
         self.plotter.clear()
+
+        # Clear out internally stored labels (if any)
+        self._load_label_points = []
+        self._load_labels = []
+
+        self._spring_label_points = []
+        self._spring_labels = []
         
         # Check if nodes are to be rendered
         if self.render_nodes == True:
 
             if self.theme == 'print':
                 color = 'black'
             else:
                 color = 'grey'
 
             # Plot each node in the model
             for node in self.model.Nodes.values():
-                self.plot_node(node, self.annotation_size, color)
+                self.plot_node(node, color)
             
             # Plot each auxiliary node in the model
             for aux_node in self.model.AuxNodes.values():
-                self.plot_node(aux_node, self.annotation_size, color)
+                self.plot_node(aux_node, color)
         
         # Render node labels
         label_points = [[node.X, node.Y, node.Z] for node in self.model.Nodes.values()]
         labels = [node.name for node in self.model.Nodes.values()]
-        self.plotter.add_point_labels(label_points, labels, italic=False, bold=False, font_size=24, text_color='grey', font_family=None, shadow=False, show_points=True, point_color=None, point_size=None, name=None, shape_color=None, shape=None, fill_shape=True, margin=3, shape_opacity=1.0, pickable=False, render_points_as_spheres=True, tolerance=0.001, reset_camera=None, always_visible=False, render=True)
+        
+        self.plotter.add_point_labels(label_points, labels, bold=False, text_color='black', show_points=True, point_color='grey', point_size=5, shape=None, render_points_as_spheres=True)
+
+        # Check if there are springs in the model
+        if self.model.Springs:
 
-        # Create a visual spring for each spring in the model
-        # vis_springs = []
-        # for spring in self.model.Springs.values():
-        #     vis_springs.append(VisSpring(spring, self.model.Nodes, self.annotation_size))    
-    
-        # Create a visual member for each member in the model
-        # vis_members = []
-        # for member in self.model.Members.values():
-        #     vis_members.append(VisMember(member, self.model.Nodes, self.annotation_size, self.theme))
+            # Render the springs
+            for spring in self.model.Springs.values():
+                self.plot_spring(spring, self.annotation_size, 'grey')
+            
+            # Render the spring labels
+            self.plotter.add_point_labels(self._spring_label_points, self._spring_labels, text_color='black', bold=False, shape=None, render_points_as_spheres=False)
         
+        # Render the members
         for member in self.model.Members.values():
             self.plot_member(member)
 
         # Render the member labels
         label_points = [[(member.i_node.X+member.j_node.X)/2, (member.i_node.Y+member.j_node.Y)/2, (member.i_node.Z+member.j_node.Z)/2] for member in self.model.Members.values()]
         labels = [member.name for member in self.model.Members.values()]
-        self.plotter.add_point_labels(label_points, labels, italic=False, bold=False, font_size=24, text_color='grey', font_family=None, shadow=False, show_points=False, point_color=None, point_size=None, name=None, shape_color=None, shape=None, fill_shape=True, margin=3, shape_opacity=1.0, pickable=False, render_points_as_spheres=True, tolerance=0.001, reset_camera=None, always_visible=False, render=True)
-
-        # Add actors for each spring
-        # for vis_spring in vis_springs:
-        
-        #     # Add the spring
-        #     self.plotter.add_mesh(vis_spring.mesh)
-
-        #     if self.labels == True:
-
-        #         # Add the actor for the spring label
-        #         self.plotter.add_mesh(vis_spring.text_mesh)  
-
-        # Add actors for each member
-        # for vis_member in vis_members:
-            
-        #     # Add the actor for the member
-        #     self.plotter.add_mesh(vis_member.mesh)
-
-        #     if self.labels == True:
-                
-        #         # Add the actor for the member label
-        #         self.plotter.add_mesh(vis_member.text_mesh)
+        self.plotter.add_point_labels(label_points, labels, bold=False, text_color='black', show_points=False, shape=None, render_points_as_spheres=False)
 
         # Render the deformed shape if requested
         if self.deformed_shape == True:
 
             # Render deformed nodes
-            for node in self.model.Nodes.values():
-                self.plot_deformed_node(node, self.deformed_scale)
+            # for node in self.model.Nodes.values():
+            #     self.plot_deformed_node(node, self.deformed_scale)
             
             # Render deformed members
             for member in self.model.Members.values():
                 self.plot_deformed_member(member, self.deformed_scale)
+            
+            # Render deformed springs
+            for spring in self.model.Springs.values():
+                self.plot_deformed_spring(spring, self.deformed_scale, self.combo_name)
 
             # _DeformedShape(self.model, self.deformed_scale, self.annotation_size, self.combo_name, self.render_nodes, self.theme)
 
-        # # Render the loads if requested
-        # if (self.combo_name != None or self.case != None) and self.render_loads != False:
-        #     _RenderLoads(self.model, renderer, self.annotation_size, self.combo_name, self.case, self.theme)
+        # Render the loads if requested
+        if (self.combo_name != None or self.case != None) and self.render_loads != False:
+
+            # Plot the loads
+            self.plot_loads()
+
+            # Plot the load labels
+            self.plotter.add_point_labels(self._load_label_points, self._load_labels, bold=False, text_color='green', show_points=False, shape=None, render_points_as_spheres=False)
         
         # Render the plates and quads, if present
         if self.model.Quads or self.model.Plates:
-            self.plot_plates(self.deformed_shape, self.deformed_scale, self.color_map, self.scalar_bar, self.scalar_bar_text_size, self.combo_name, self.theme)
-
-        # Set the window's background color
-        # if self.theme == 'default':
-        #     renderer.SetBackground(0, 0, 128)  # Blue
-        # elif self.theme == 'print':
-        #     renderer.SetBackground(255, 255, 255)  # White
+            self.plot_plates(self.deformed_shape, self.deformed_scale, self.color_map, self.combo_name)
+        
+        # Determine whether to show or hide the scalar bar
+        # if self._scalar_bar == False:
+        #     self.plotter.scalar_bar.VisibilityOff()
             
         # Reset the camera if requested by the user
         if reset_camera:
             self.plotter.reset_camera()
     
-    def plot_node(self, node, size, color='grey'):
+    def plot_node(self, node, color='grey'):
         """Adds a node to the plotter
 
         :param node: node
         :type node: Node3D
         """
       
         # Get the node's position
@@ -318,135 +328,163 @@
 
         # Generate any supports that occur at the node
         # Check for a fixed suppport
         if node.support_DX and node.support_DY and node.support_DZ and node.support_RX and node.support_RY and node.support_RZ:
             
             # Create a cube using PyVista
             self.plotter.add_mesh(pv.Cube(center=(node.X, node.Y, node.Z),
-                                          x_length=size*2,
-                                          y_length=size*2,
-                                          z_length=size*2))
+                                          x_length=self.annotation_size*2,
+                                          y_length=self.annotation_size*2,
+                                          z_length=self.annotation_size*2),
+                                  color=color)
         
         # Check for a pinned support
         elif node.support_DX and node.support_DY and node.support_DZ and not node.support_RX and not node.support_RY and not node.support_RZ:
             
             # Create a cone using PyVista's Cone function
-            self.plotter.add_mesh(pv.Cone(center=(node.X, node.Y-size, node.Z),
+            self.plotter.add_mesh(pv.Cone(center=(node.X, node.Y - self.annotation_size, node.Z),
                                           direction=(0, 1, 0),
-                                          height=size*2,
-                                          radius=size*2))
+                                          height=self.annotation_size*2,
+                                          radius=self.annotation_size*2),
+                                  color=color)
 
         # Other support conditions
         else:
 
             # Generate a sphere for the node
-            #sphere = pv.Sphere(center=(X, Y, Z), radius=size/2)
-            #self.plotter.add_mesh(sphere, name='Node: '+node.name)
+            # sphere = pv.Sphere(center=(X, Y, Z), radius=0.4*self.annotation_size)
+            # self.plotter.add_mesh(sphere, name='Node: '+ node.name, color=color)
             
             # Restrained against X translation
             if node.support_DX:
 
                 # Line showing support direction
-                self.plotter.add_mesh((node.X-size, node.Y, node.Z),
-                                      (node.X+size, node.Y, node.Z))
+                self.plotter.add_mesh(pv.Line((node.X - self.annotation_size, node.Y, node.Z),
+                                              (node.X + self.annotation_size, node.Y, node.Z)),
+                                      color=color)
 
                 # Cones at both ends
-                self.plotter.add_mesh(pv.Cone(center=(node.X-size, node.Y, node.Z),
-                                        direction=(1, 0, 0),
-                                        height=size*0.6,
-                                        radius=size*0.3))
-                self.plotter.add_mesh(pv.Cone(center=(node.X+size, node.Y, node.Z),
-                                        direction=(-1, 0, 0),
-                                        height=size*0.6,
-                                        radius=size*0.3))
+                self.plotter.add_mesh(pv.Cone(center=(node.X - self.annotation_size, node.Y,
+                                                      node.Z),
+                                              direction=(1, 0, 0), height=self.annotation_size*0.6,
+                                              radius=self.annotation_size*0.3),
+                                      color=color)
+                self.plotter.add_mesh(pv.Cone(center=(node.X + self.annotation_size, node.Y,
+                                                      node.Z),
+                                              direction=(-1, 0, 0),
+                                              height=self.annotation_size*0.6,
+                                              radius=self.annotation_size*0.3),
+                                      color=color)
             
             # Restrained against Y translation
             if node.support_DY:
 
                 # Line showing support direction
-                self.plotter.add_mesh(pv.Line((node.X, node.Y-size, node.Z),
-                                              (node.X, node.Y+size, node.Z)))
+                self.plotter.add_mesh(pv.Line((node.X, node.Y - self.annotation_size, node.Z),
+                                              (node.X, node.Y + self.annotation_size, node.Z)),
+                                      color=color)
 
                 # Cones at both ends
-                self.plotter.add_mesh(pv.Cone(center=(node.X, node.Y-size, node.Z),
-                                              direction=(0, 1, 0),
-                                              height=size*0.6,
-                                              radius=size*0.3))
-                self.plotter.add_mesh(pv.Cone(center=(node.X, node.Y+size, node.Z),
-                                              direction=(0, -1, 0),
-                                              height=size*0.6,
-                                              radius=size*0.3))
+                self.plotter.add_mesh(pv.Cone(center=(node.X, node.Y - self.annotation_size,
+                                                      node.Z), direction=(0, 1, 0),
+                                                      height=self.annotation_size*0.6,
+                                                      radius=self.annotation_size*0.3),
+                                      color=color)
+                self.plotter.add_mesh(pv.Cone(center=(node.X, node.Y + self.annotation_size,
+                                                      node.Z),
+                                                      direction=(0, -1, 0),
+                                                      height=self.annotation_size*0.6,
+                                                      radius=self.annotation_size*0.3),
+                                      color=color)
             
             # Restrained against Z translation
             if node.support_DZ:
 
                 # Line showing support direction
-                self.plotter.add_mesh(pv.Line((node.X, node.Y, node.Z-size),
-                                              (node.X, node.Y, node.Z+size)))
+                self.plotter.add_mesh(pv.Line((node.X, node.Y, node.Z-self.annotation_size),
+                                              (node.X, node.Y, node.Z+self.annotation_size)),
+                                      color=color)
 
                 # Cones at both ends
-                self.plotter.add_mesh(pv.Cone(center=(node.X, node.Y, node.Z-size),
+                self.plotter.add_mesh(pv.Cone(center=(node.X, node.Y, node.Z-self.annotation_size),
                                               direction=(0, 0, 1),
-                                              height=size*0.6,
-                                              radius=size*0.3))
-                self.plotter.add_mesh(pv.Cone(center=(node.X, node.Y, node.Z+size),
+                                              height=self.annotation_size*0.6,
+                                              radius=self.annotation_size*0.3),
+                                      color=color)
+                self.plotter.add_mesh(pv.Cone(center=(node.X, node.Y, node.Z+self.annotation_size),
                                               direction=(0, 0, -1),
-                                              height=size*0.6,
-                                              radius=size*0.3))
+                                              height=self.annotation_size*0.6,
+                                              radius=self.annotation_size*0.3),
+                                      color=color)
             
             # Restrained against X rotation
             if node.support_RX:
 
                 # Line showing support direction
-                self.plotter.add_mesh(pv.Line((node.X-1.6*size, node.Y, node.Z),
-                                              (node.X+1.6*size, node.Y, node.Z)))
+                self.plotter.add_mesh(pv.Line((node.X-1.6*self.annotation_size, node.Y, node.Z),
+                                              (node.X+1.6*self.annotation_size, node.Y, node.Z)),
+                                      color=color)
 
                 # Cubes at both ends
-                self.plotter.add_mesh(pv.Cube(center=(node.X-1.9*size, node.Y, node.Z),
-                                              x_length=size*0.6,
-                                              y_length=size*0.6,
-                                              z_length=size*0.6))
-                self.plotter.add_mesh(pv.Cube(center=(node.X+1.9 *size, node.Y, node.Z),
-                                              x_length=size*0.6,
-                                              y_length=size*0.6,
-                                              z_length=size*0.6))
+                self.plotter.add_mesh(pv.Cube(center=(node.X-1.9*self.annotation_size, node.Y,
+                                                      node.Z),
+                                              x_length=self.annotation_size*0.6,
+                                              y_length=self.annotation_size*0.6,
+                                              z_length=self.annotation_size*0.6),
+                                      color=color)
+                self.plotter.add_mesh(pv.Cube(center=(node.X+1.9 *self.annotation_size, node.Y,
+                                                      node.Z),
+                                              x_length=self.annotation_size*0.6,
+                                              y_length=self.annotation_size*0.6,
+                                              z_length=self.annotation_size*0.6),
+                                      color=color)
 
             # Restrained against rotation about the Y-axis
             if node.support_RY:
 
                 # Line showing support direction
-                self.plotter.add_mesh(pv.Line((node.X, node.Y-1.6*size, node.Z),
-                                              (node.X, node.Y+1.6*size, node.Z)))
+                self.plotter.add_mesh(pv.Line((node.X, node.Y-1.6*self.annotation_size, node.Z),
+                                              (node.X, node.Y+1.6*self.annotation_size, node.Z)),
+                                      color=color)
 
                 # Cubes at both ends
-                self.plotter.add_mesh(pv.Cube(center=(node.X, node.Y-1.9*size, node.Z),
-                                              x_length=size*0.6,
-                                              y_length=size*0.6,
-                                              z_length=size*0.6))
-                self.plotter.add_mesh(pv.Cube(center=(node.X, node.Y+1.9*size, node.Z),
-                                              x_length=size*0.6,
-                                              y_length=size*0.6,
-                                              z_length=size*0.6))
+                self.plotter.add_mesh(pv.Cube(center=(node.X, node.Y-1.9*self.annotation_size,
+                                                      node.Z),
+                                              x_length=self.annotation_size*0.6,
+                                              y_length=self.annotation_size*0.6,
+                                              z_length=self.annotation_size*0.6),
+                                      color=color)
+                self.plotter.add_mesh(pv.Cube(center=(node.X, node.Y+1.9*self.annotation_size,
+                                                      node.Z),
+                                              x_length=self.annotation_size*0.6,
+                                              y_length=self.annotation_size*0.6,
+                                              z_length=self.annotation_size*0.6),
+                                      color=color)
             
             # Restrained against rotation about the Z-axis
             if node.support_RZ:
 
                 # Line showing support direction
-                self.plotter.add_mesh(pv.Line((node.X, node.Y, node.Z-1.6*size),
-                                              (node.X, node.Y, node.Z+1.6*size)))
+                self.plotter.add_mesh(pv.Line((node.X, node.Y, node.Z-1.6*self.annotation_size),
+                                              (node.X, node.Y, node.Z+1.6*self.annotation_size)),
+                                      color=color)
 
                 # Cubes at both ends
-                self.plotter.add_mesh(pv.Cube(center=(node.X, node.Y, node.Z-1.9*size),
-                                              x_length=size*0.6,
-                                              y_length=size*0.6,
-                                              z_length=size*0.6))
-                self.plotter.add_mesh(pv.Cube(center=(node.X, node.Y, node.Z+1.9*size),
-                                              x_length=size*0.6,
-                                              y_length=size*0.6,
-                                              z_length=size*0.6))
+                self.plotter.add_mesh(pv.Cube(center=(node.X, node.Y,
+                                                      node.Z-1.9*self.annotation_size),
+                                              x_length=self.annotation_size*0.6,
+                                              y_length=self.annotation_size*0.6,
+                                              z_length=self.annotation_size*0.6),
+                                      color=color)
+                self.plotter.add_mesh(pv.Cube(center=(node.X, node.Y,
+                                                      node.Z+1.9*self.annotation_size),
+                                              x_length=self.annotation_size*0.6,
+                                              y_length=self.annotation_size*0.6,
+                                              z_length=self.annotation_size*0.6),
+                                      color=color)
 
     def plot_member(self, member, theme='default'):
     
         # Generate a line for the member
         line = pv.Line()
 
         Xi = member.i_node.X
@@ -459,50 +497,37 @@
         Zj = member.j_node.Z
         line.points[1] = [Xj, Yj, Zj]
 
         self.plotter.add_mesh(line, color='black', line_width=2)
 
     def plot_spring(self, spring, size, color='grey'):
         
-        # Create points for the line source
-        points = zeros((2, 3))  # 2 points in 3D
-        line = pv.Line(points)
-
-        # Step through each node in the model and find the position of the i-node and j-node
+        # Find the position of the i-node and j-node
         i_node = spring.i_node
         j_node = spring.j_node
         Xi, Yi, Zi = i_node.X, i_node.Y, i_node.Z
-        line.points[0] = [Xi, Yi, Zi]
         Xj, Yj, Zj = j_node.X, j_node.Y, j_node.Z
-        line.points[1] = [Xj, Yj, Zj]
 
-        # Create the PyVista actors
-        actor = pv.PolyData(line).tube(radius=0.1)
-        label = pv.VectorText(spring.name)
-
-        # Set up an actor for the spring label
-        lblActor = pv.Follower(label)
-        lblActor.scale(size, size, size)
-        lblActor.position = [(Xi+Xj)/2, (Yi+Yj)/2, (Zi+Zj)/2]
-
-        # Add some color
+        # Create the line
+        line = pv.Line((Xi, Yi, Zi), (Xj, Yj, Zj))
+        
+        # Change the color
         if color is None:
-            actor.point_data["color"] = array([255, 0, 255])  # Magenta
-            lblActor.point_data["color"] = array([255, 0, 255])
+            line.plot(color='magenta')
         elif color == 'black':
-            actor.point_data["color"] = array([0, 0, 0])  # Black
-            lblActor.point_data["color"] = array([0, 0, 0])
+            line.plot(color='black')
 
-        # Plot the actors
-        plotter = pv.Plotter()
-        plotter.add_mesh(actor)
-        plotter.add_mesh(lblActor)
-        plotter.show()
+        # Add the spring label to the list of labels
+        self._spring_labels.append(spring.name)
+        self._spring_label_points.append([(Xi+Xj)/2, (Yi+Yj)/2, (Zi+Zj)/2])
+
+        # Add the line to the plotter
+        self.plotter.add_mesh(line)
             
-    def plot_plates(self, deformed_shape, deformed_scale, color_map, scalar_bar, scalar_bar_text_size, combo_name, theme='default'):
+    def plot_plates(self, deformed_shape, deformed_scale, color_map, combo_name):
         
         # Start a list of vertices
         plate_vertices = []
 
         # Start a list of plates (faces) for the mesh.
         plate_faces = []
         
@@ -560,406 +585,562 @@
                 plate_results.append(r2)
                 plate_results.append(r3)
 
             # Move on to the next plate in our lists to repeat the process
             i+=1
 
         # Add the vertices and the faces to our lists
-        plate_vertices = array(plate_vertices)
-        plate_faces = array(plate_faces)
+        plate_vertices = np.array(plate_vertices)
+        plate_faces = np.array(plate_faces)
 
         # Create a new PyVista dataset to store plate data
         plate_polydata = pv.PolyData(plate_vertices, plate_faces)
 
         # Add the results as point data to the PyVista dataset
         if color_map:
             
             plate_polydata = plate_polydata.separate_cells()
-            plate_polydata['Contours'] = array(plate_results)
+            plate_polydata['Contours'] = np.array(plate_results)
             
             # Add the scalar bar for the contours
-            if scalar_bar:
+            if self._scalar_bar == True:
                 self.plotter.add_mesh(plate_polydata, scalars='Contours', show_edges=True)
             else:
                 self.plotter.add_mesh(plate_polydata)
+
         else:
             self.plotter.add_mesh(plate_polydata)
       
-    def plot_deformed_node(self, node, scale_factor):
+    def plot_deformed_node(self, node, scale_factor, color='grey'):
 
         # Calculate the node's deformed position
         newX = node.X + scale_factor * (node.DX[self.combo_name])
         newY = node.Y + scale_factor * (node.DY[self.combo_name])
         newZ = node.Z + scale_factor * (node.DZ[self.combo_name])
 
         # Generate a sphere source for the node in its deformed position
-        sphere = pv.Sphere(radius=0.6 * self.annotation_size, center=[newX, newY, newZ])
+        sphere = pv.Sphere(radius=0.4*self.annotation_size, center=[newX, newY, newZ])
 
         # Add the mesh to the plotter
-        self.plotter.add_mesh(sphere)
+        self.plotter.add_mesh(sphere, color=color)
   
     def plot_deformed_member(self, member, scale_factor):
         
         # Determine if this member is active for each load combination
         if member.active:
         
             L = member.L() # Member length
             T = member.T() # Member local transformation matrix
         
-            cos_x = array([T[0, 0:3]]) # Direction cosines of local x-axis
-            cos_y = array([T[1, 0:3]]) # Direction cosines of local y-axis
-            cos_z = array([T[2, 0:3]]) # Direction cosines of local z-axis
+            cos_x = np.array([T[0, 0:3]]) # Direction cosines of local x-axis
+            cos_y = np.array([T[1, 0:3]]) # Direction cosines of local y-axis
+            cos_z = np.array([T[2, 0:3]]) # Direction cosines of local z-axis
 
             # Find the initial position of the local i-node
             Xi = member.i_node.X
             Yi = member.i_node.Y
             Zi = member.i_node.Z
         
             # Calculate the local y-axis displacements at 20 points along the member's length
-            DY_plot = empty((0, 3))
+            DY_plot = np.empty((0, 3))
             for i in range(20):
                     
                 # Calculate the local y-direction displacement
                 dy_tot = member.deflection('dy', L / 19 * i, self.combo_name)
             
                 # Calculate the scaled displacement in global coordinates
-                DY_plot = append(DY_plot, dy_tot * cos_y * scale_factor, axis=0)
+                DY_plot = np.append(DY_plot, dy_tot * cos_y * scale_factor, axis=0)
         
             # Calculate the local z-axis displacements at 20 points along the member's length
-            DZ_plot = empty((0, 3)) 
+            DZ_plot = np.empty((0, 3)) 
             for i in range(20):
                     
                 # Calculate the local z-direction displacement
                 dz_tot = member.deflection('dz', L / 19 * i, self.combo_name)
             
                 # Calculate the scaled displacement in global coordinates
-                DZ_plot = append(DZ_plot, dz_tot * cos_z * scale_factor, axis=0)
+                DZ_plot = np.append(DZ_plot, dz_tot * cos_z * scale_factor, axis=0)
         
             # Calculate the local x-axis displacements at 20 points along the member's length
-            DX_plot = empty((0, 3)) 
+            DX_plot = np.empty((0, 3)) 
             for i in range(20):
                     
                 # Displacements in local coordinates
                 dx_tot = [[Xi, Yi, Zi]] + (L / 19 * i + member.deflection('dx', L / 19 * i, self.combo_name) * scale_factor) * cos_x
                     
                 # Magnified displacements in global coordinates
-                DX_plot = append(DX_plot, dx_tot, axis=0)
+                DX_plot = np.append(DX_plot, dx_tot, axis=0)
             
             # Sum the component displacements to obtain overall displacement
             D_plot = DY_plot + DZ_plot + DX_plot
             
             # Create lines connecting the points
             for i in range(len(D_plot)-1):
                 line = pv.Line(D_plot[i], D_plot[i+1])
                 self.plotter.add_mesh(line, color='red', line_width=2)
-                                  
-# class VisDeformedSpring():
     
-#     def __init__(self, spring, nodes, scale_factor, combo_name='Combo 1'):
+    def plot_deformed_spring(self, spring, scale_factor, combo_name='Combo 1'):
+
+        # Determine if the spring is active for the load combination
+        if spring.active[combo_name]:
+
+            # Get the spring's i-node and j-node
+            i_node = spring.i_node
+            j_node = spring.j_node
+            
+            # Calculate the deformed positions of the spring's end points
+            Xi = i_node.X + i_node.DX[combo_name]*scale_factor
+            Yi = i_node.Y + i_node.DY[combo_name]*scale_factor
+            Zi = i_node.Z + i_node.DZ[combo_name]*scale_factor
+            
+            Xj = j_node.X + j_node.DX[combo_name]*scale_factor
+            Yj = j_node.Y + j_node.DY[combo_name]*scale_factor
+            Zj = j_node.Z + j_node.DZ[combo_name]*scale_factor
+            
+            # Plot a line for the deformed spring
+            self.plotter.add_mesh(pv.Line((Xi, Yi, Zi), (Xj, Yj, Zj)))
+
+    def plot_pt_load(self, position, direction, length, label_text=None, color='green'):
 
-#         # Determine if this spring is active for each load combination
-#         self.active = spring.active
+        # Create a unit vector in the direction of the 'direction' vector
+        unitVector = direction/np.linalg.norm(direction)
         
-#         # Generate a line source for the spring
-#         self.source = vtk.vtkLineSource()
+        # Determine if the load is positive or negative
+        if length == 0:
+            sign = 1
+        else:
+            sign = abs(length)/length
+
+        # Generate the tip of the load arrow
+        tip_length = abs(length) / 4
+        radius = abs(length) / 16
+        tip = pv.Cone(center=(position[0] - tip_length*sign*unitVector[0]/2,
+                              position[1] - tip_length*sign*unitVector[1]/2,
+                              position[2] - tip_length*sign*unitVector[2]/2),
+                              direction=(direction[0]*sign, direction[1]*sign, direction[2]*sign),
+                              height=tip_length, radius=radius)
+
+        # Plot the tip
+        self.plotter.add_mesh(tip, color=color)
+
+        # Create the shaft (you'll need to specify the second point)
+        X_tail = position[0] - unitVector[0]*length
+        Y_tail = position[1] - unitVector[1]*length
+        Z_tail = position[2] - unitVector[2]*length
+        shaft = pv.Line(pointa=position, pointb=(X_tail, Y_tail, Z_tail))
+        
+        # Save the data necessary to create the load's label
+        if label_text is not None:
+            self._load_labels.append(sig_fig_round(label_text, 3))
+            self._load_label_points.append([X_tail, Y_tail, Z_tail])
+        
+        # Plot the shaft
+        self.plotter.add_mesh(shaft, line_width=2, color=color)                         
+
+    def plot_dist_load(self, position1, position2, direction, length1, length2, label_text1, label_text2, color='green'):
+
+        # Calculate the length of the distributed load
+        load_length = ((position2[0] - position1[0])**2 + (position2[1] - position1[1])**2 + (position2[2] - position1[2])**2)**0.5
+
+        # Find the direction cosines for the line the load acts on
+        line_dir_cos = [(position2[0] - position1[0])/load_length,
+                        (position2[1] - position1[1])/load_length,
+                        (position2[2] - position1[2])/load_length]
+
+        # Find the direction cosines for the direction the load acts in
+        dir_dir_cos = direction/np.linalg.norm(direction)
+
+        # Create point loads at intervals roughly equal to 75% of the load's largest length
+        # Add text labels to the first and last load arrow
+        if load_length > 0:
+            num_steps = int(round(0.75 * load_length/max(abs(length1), abs(length2)), 0))
+        else:
+            num_steps = 0
+
+        num_steps = max(num_steps, 1)
+        step = load_length/num_steps
+
+        for i in range(num_steps + 1):
+
+            # Calculate the position (X, Y, Z) of this load arrow's point
+            position = (position1[0] + i*step*line_dir_cos[0],
+                        position1[1] + i*step*line_dir_cos[1],
+                        position1[2] + i*step*line_dir_cos[2])
+
+            # Determine the length of this load arrow
+            length = length1 + (length2 - length1)/load_length*i*step
+
+            # Determine the label's text
+            if i == 0:
+                label_text = label_text1
+            elif i == num_steps:
+                label_text = label_text2
+            else:
+                label_text = None
+
+            # Plot the load arrow
+            self.plot_pt_load(position, dir_dir_cos, length, label_text, color)
+
+        # Draw a line between the first and last load arrow's tails (using cylinder here for better visualization)
+        tail_line = pv.Line(position1 - dir_dir_cos*length1, position2 - dir_dir_cos*length2)
+
+        # Combine all geometry into a single PolyData object
+        self.plotter.add_mesh(tail_line, color=color)
+
+    def plot_moment(self, center, direction, radius, label_text=None, color='green'):
+
+        # Convert the direction vector into a unit vector
+        v1 = direction/np.linalg.norm(direction)
+
+        # Find any vector perpendicular to the moment direction vector. This will serve as a
+        # vector from the center of the arc pointing to the tail of the moment arc.
+        v2 = _PerpVector(v1)
         
-#         # Find the deformed position of the local i-node
-#         # Step through each node
-#         for node in nodes.values():
-      
-#             # Check to see if the current node is the i-node
-#             if node.name == spring.i_node.name:
-#                 Xi = node.X + node.DX[combo_name]*scale_factor
-#                 Yi = node.Y + node.DY[combo_name]*scale_factor
-#                 Zi = node.Z + node.DZ[combo_name]*scale_factor
-#                 self.source.SetPoint1(Xi, Yi, Zi)
-        
-#             # Check to see if the current node is the i-node
-#             if node.name == spring.j_node.name:
-#                 Xj = node.X + node.DX[combo_name]*scale_factor
-#                 Yj = node.Y + node.DY[combo_name]*scale_factor
-#                 Zj = node.Z + node.DZ[combo_name]*scale_factor
-#                 self.source.SetPoint2(Xj, Yj, Zj)
-        
-#         self.source.Update()
-    
-# class VisPtLoad():
-#     '''
-#     Creates a point load for the viewer
-#     '''
-    
-#     def __init__(self, position, direction, length, label_text=None, annotation_size=5, color=None):
-#         '''
-#         Constructor.
-      
-#         Parameters
-#         ----------
-#         position : tuple
-#           A tuple of X, Y and Z coordinates for the point of the load arrow: (X, Y, Z).
-#         direction : tuple
-#           A tuple indicating the direction vector for the load arrow: (i, j, k).
-#         length : number
-#           The length of the load arrow.
-#         tip_length : number
-#           The height of the arrow head.
-#         label_text : string
-#           Text that will show up at the tail of the arrow. If set to 'None' no text will be displayed.
-#         '''
-      
-#         # Create a unit vector in the direction of the 'direction' vector
-#         unitVector = direction/norm(direction)
-      
-#         # Create a 'vtkAppendPolyData' filter to append the tip and shaft together into a single dataset
-#         self.polydata = vtk.vtkAppendPolyData()
-      
-#         # Determine if the load is positive or negative
-#         if length == 0:
-#             sign = 1
-#         else:
-#             sign = abs(length)/length
-      
-#         # Generate the tip of the load arrow
-#         tip_length = abs(length)/4
-#         radius = abs(length)/16
-#         tip = vtk.vtkConeSource()
-#         tip.SetCenter(position[0] - tip_length*sign*0.5*unitVector[0], \
-#                       position[1] - tip_length*sign*0.5*unitVector[1], \
-#                       position[2] - tip_length*sign*0.5*unitVector[2])
-#         tip.SetDirection([direction[0]*sign, direction[1]*sign, direction[2]*sign])
-#         tip.SetHeight(tip_length)
-#         tip.SetRadius(radius)
-#         tip.Update()
-      
-#         # Add the arrow tip to the append filter
-#         self.polydata.AddInputData(tip.GetOutput())
+        # Generate the arc for the moment
+        arc = pv.CircularArcFromNormal(center, resolution=20, normal=v1, angle=215, polar=v2*radius)
         
-#         # Create the shaft
-#         shaft = vtk.vtkLineSource()
-#         shaft.SetPoint1(position)
-#         shaft.SetPoint2((position[0]-length*unitVector[0], position[1]-length*unitVector[1], position[2]-length*unitVector[2]))
-#         shaft.Update()
-      
-#         # Copy and append the shaft data to the append filter
-#         self.polydata.AddInputData(shaft.GetOutput())
-#         self.polydata.Update()
-      
-#         # Create a mapper and actor
-#         mapper = vtk.vtkPolyDataMapper()
-#         mapper.SetInputConnection(self.polydata.GetOutputPort())
-#         self.actor = vtk.vtkActor()
-#         if color is None: self.actor.GetProperty().SetColor(0, 255, 0) # Green
-#         elif color == 'black': self.actor.GetProperty().SetColor(0, 0, 0)  # Black
-#         self.actor.SetMapper(mapper)
-      
-#         # Create the label if needed
-#         if label_text != None:
-      
-#             # Create the label and set its text
-#             self.label = vtk.vtkVectorText()
-#             self.label.SetText(label_text)
-        
-#             # Set up a mapper for the label
-#             lblMapper = vtk.vtkPolyDataMapper()
-#             lblMapper.SetInputConnection(self.label.GetOutputPort())
-        
-#             # Set up an actor for the label
-#             self.lblActor = vtk.vtkFollower()
-#             self.lblActor.SetMapper(lblMapper)
-#             self.lblActor.SetScale(annotation_size, annotation_size, annotation_size)
-#             self.lblActor.SetPosition(position[0] - (length - 0.6*annotation_size)*unitVector[0], \
-#                                       position[1] - (length - 0.6*annotation_size)*unitVector[1], \
-#                                       position[2] - (length - 0.6*annotation_size)*unitVector[2])
-#             if color is None: self.lblActor.GetProperty().SetColor(0, 255, 0)  # Green
-#             elif color == 'black': self.lblActor.GetProperty().SetColor(0, 0, 0)  # Black
-      
-# class VisDistLoad():
-#     '''
-#     Creates a distributed load for the viewer
-#     '''
-    
-#     def __init__(self, position1, position2, direction, length1, length2, label_text1, label_text2, annotation_size=5, color=None):
-#         '''
-#         Constructor.
-#         '''
-      
-#         # Calculate the length of the distributed load
-#         loadLength = ((position2[0]-position1[0])**2 + (position2[1]-position1[1])**2 + (position2[2]-position1[2])**2)**0.5
-      
-#         # Find the direction cosines for the line the load acts on
-#         lineDirCos = [(position2[0]-position1[0])/loadLength, (position2[1]-position1[1])/loadLength, (position2[2]-position1[2])/loadLength]
-      
-#         # Find the direction cosines for the direction the load acts in
-#         dirDirCos = direction/norm(direction)
-      
-#         # Create point loads at intervals roughly equal to 75% of the load's largest length (magnitude)
-#         # Add text labels to the first and last load arrow
-#         if loadLength > 0:
-#             num_steps = int(round(0.75*loadLength/max(abs(length1), abs(length2)), 0))
-#         else:
-#             num_steps = 0
-
-#         num_steps = max(num_steps, 1)
-#         step = loadLength/num_steps
-#         ptLoads = []
-      
-#         for i in range(num_steps + 1):
-      
-#             # Calculate the position (X, Y, Z) of this load arrow's point
-#             position = (position1[0] + i*step*lineDirCos[0], position1[1] + i*step*lineDirCos[1], position1[2] + i*step*lineDirCos[2])
+        # Add the arc to the plot
+        self.plotter.add_mesh(arc, line_width=2, color=color)
+
+        # Generate the arrow tip at the end of the arc
+        tip_length = radius/4
+        cone_radius = radius/16
+        cone_direction = -np.cross(v1, arc.center - arc.points[-1])
+        tip = pv.Cone(center=arc.points[-1], direction=cone_direction, height=tip_length,
+                      radius=cone_radius)
+
+        # Add the tip to the plot
+        self.plotter.add_mesh(tip, color=color)
+
+        # Create the text label
+        if label_text:
+            text_pos = center + (radius + 0.25*self.annotation_size)*v2
+            self._load_label_points.append(text_pos)
+            self._load_labels.append(label_text)
+
+    def plot_area_load(self, position0, position1, position2, position3, direction, length, label_text, color='green'):
+
+        # Find the direction cosines for the direction the load acts in
+        dir_dir_cos = direction / np.linalg.norm(direction)
+
+        # Find the positions of the tails of all the arrows at the corners
+        self.p0 = position0 - dir_dir_cos * length
+        self.p1 = position1 - dir_dir_cos * length
+        self.p2 = position2 - dir_dir_cos * length
+        self.p3 = position3 - dir_dir_cos * length
+
+        # Plot the area load arrows
+        self.plot_pt_load(position0, dir_dir_cos, length, label_text, color)
+        self.plot_pt_load(position1, dir_dir_cos, length, color=color)
+        self.plot_pt_load(position2, dir_dir_cos, length, color=color)
+        self.plot_pt_load(position3, dir_dir_cos, length, color=color)
+
+        # Create the area load polygon (quad)
+        quad = pv.Quadrilateral([self.p0, self.p1, self.p2, self.p3])
+
+        self.plotter.add_mesh(quad, color=color)
+
+    def _calc_max_loads(self):
+
+        max_pt_load = 0
+        max_moment = 0
+        max_dist_load = 0
+        max_area_load = 0
         
-#             # Determine the length of this load arrow
-#             length = length1 + (length2 - length1)/loadLength*i*step
+        # Find the requested load combination or load case
+        if self.case == None:
         
-#             # Determine the label's text
-#             if i == 0:
-#                 label_text = label_text1
-#             elif i == num_steps:
-#                 label_text = label_text2
-        
-#             # Create the load arrow
-#             ptLoads.append(VisPtLoad(position, direction, length, label_text, annotation_size=annotation_size))
-          
-#         # Draw a line between the first and last load arrow's tails
-#         tail_line = vtk.vtkLineSource()
-#         tail_line.SetPoint1((position1[0] - length1*dirDirCos[0], position1[1] - length1*dirDirCos[1], position1[2] - length1*dirDirCos[2]))
-#         tail_line.SetPoint2((position2[0] - length2*dirDirCos[0], position2[1] - length2*dirDirCos[1], position2[2] - length2*dirDirCos[2]))
-      
-#         # Combine all the geometry into one 'vtkPolyData' object
-#         self.polydata = vtk.vtkAppendPolyData()
-#         for arrow in ptLoads:
-#             arrow.polydata.Update()
-#             self.polydata.AddInputData(arrow.polydata.GetOutput())
-        
-#         tail_line.Update()
-#         self.polydata.AddInputData(tail_line.GetOutput())
-#         self.polydata.Update()
-      
-#         # Create a mapper and actor for the geometry
-#         mapper = vtk.vtkPolyDataMapper()
-#         mapper.SetInputConnection(self.polydata.GetOutputPort())
-#         self.actor = vtk.vtkActor()
-#         if color is None: self.actor.GetProperty().SetColor(0, 255, 0)  # Green
-#         elif color == 'black': self.actor.GetProperty().SetColor(0, 0, 0)  # Black
-#         self.actor.SetMapper(mapper)
-      
-#         # Get the actors for the labels
-#         self.lblActors = [ptLoads[0].lblActor, ptLoads[len(ptLoads) - 1].lblActor]
+            # Step through each node
+            for node in self.model.Nodes.values():
+        
+                # Step through each nodal load to find the largest one
+                for load in node.NodeLoads:
+                
+                    # Find the largest loads in the load combination
+                    if load[2] in self.model.LoadCombos[self.combo_name].factors:
+                        if load[0] == 'FX' or load[0] == 'FY' or load[0] == 'FZ':
+                            if abs(load[1]*self.model.LoadCombos[self.combo_name].factors[load[2]]) > max_pt_load:
+                                max_pt_load = abs(load[1]*self.model.LoadCombos[self.combo_name].factors[load[2]])
+                        else:
+                            if abs(load[1]*self.model.LoadCombos[self.combo_name].factors[load[2]]) > max_moment:
+                                max_moment = abs(load[1]*self.model.LoadCombos[self.combo_name].factors[load[2]])
+        
+            # Step through each member
+            for member in self.model.Members.values():
+        
+                # Step through each member point load
+                for load in member.PtLoads:
+                    
+                    # Find and store the largest point load and moment in the load combination
+                    if load[3] in self.model.LoadCombos[self.combo_name].factors:
+            
+                        if (load[0] == 'Fx' or load[0] == 'Fy' or load[0] == 'Fz'
+                        or  load[0] == 'FX' or load[0] == 'FY' or load[0] == 'FZ'):
+                            if abs(load[1]*self.model.LoadCombos[self.combo_name].factors[load[3]]) > max_pt_load:
+                                max_pt_load = abs(load[1]*self.model.LoadCombos[self.combo_name].factors[load[3]])
+                        else:
+                            if abs(load[1]*self.model.LoadCombos[self.combo_name].factors[load[3]]) > max_moment:
+                                max_moment = abs(load[1]*self.model.LoadCombos[self.combo_name].factors[load[3]])
+        
+                # Step through each member distributed load
+                for load in member.DistLoads:
+            
+                    #Find and store the largest distributed load in the load combination
+                    if load[5] in self.model.LoadCombos[self.combo_name].factors:
+            
+                        if abs(load[1]*self.model.LoadCombos[self.combo_name].factors[load[5]]) > max_dist_load:
+                            max_dist_load = abs(load[1]*self.model.LoadCombos[self.combo_name].factors[load[5]])
+                        if abs(load[2]*self.model.LoadCombos[self.combo_name].factors[load[5]]) > max_dist_load:
+                            max_dist_load = abs(load[2]*self.model.LoadCombos[self.combo_name].factors[load[5]])
+        
+            # Step through each plate
+            for plate in self.model.Plates.values():
+        
+                # Step through each plate load
+                for load in plate.pressures:
+            
+                    if load[1] in self.model.LoadCombos[self.combo_name].factors:
+                        if abs(load[0]*self.model.LoadCombos[self.combo_name].factors[load[1]]) > max_area_load:
+                            max_area_load = abs(load[0]*self.model.LoadCombos[self.combo_name].factors[load[1]])
+        
+            # Step through each quad
+            for quad in self.model.Quads.values():
+        
+                # Step through each plate load
+                for load in quad.pressures:
+            
+                    # Check to see if the load case is in the requested load combination
+                    if load[1] in self.model.LoadCombos[self.combo_name].factors:
+                        if abs(load[0]*self.model.LoadCombos[self.combo_name].factors[load[1]]) > max_area_load:
+                            max_area_load = abs(load[0]*self.model.LoadCombos[self.combo_name].factors[load[1]])
+        
+        # Behavior if case has been specified
+        else:
+            
+            # Step through each node
+            for node in self.model.Nodes.values():
+        
+                # Step through each nodal load to find the largest one
+                for load in node.NodeLoads:
+                
+                    # Find the largest loads in the load case
+                    if load[2] == self.case:
+                        if load[0] == 'FX' or load[0] == 'FY' or load[0] == 'FZ':
+                            if abs(load[1]) > max_pt_load:
+                                max_pt_load = abs(load[1])
+                        else:
+                            if abs(load[1]) > max_moment:
+                                max_moment = abs(load[1])
+        
+            # Step through each member
+            for member in self.model.Members.values():
+        
+                # Step through each member point load
+                for load in member.PtLoads:
+                
+                    # Find and store the largest point load and moment in the load case
+                    if load[3] == self.case:
+                
+                        if (load[0] == 'Fx' or load[0] == 'Fy' or load[0] == 'Fz'
+                        or  load[0] == 'FX' or load[0] == 'FY' or load[0] == 'FZ'):
+                            if abs(load[1]) > max_pt_load:
+                                max_pt_load = abs(load[1])
+                        else:
+                            if abs(load[1]) > max_moment:
+                                max_moment = abs(load[1])
+            
+                # Step through each member distributed load
+                for load in member.DistLoads:
+            
+                    # Find and store the largest distributed load in the load case
+                    if load[5] == self.case:
+                
+                        if abs(load[1]) > max_dist_load:
+                            max_dist_load = abs(load[1])
+                        if abs(load[2]) > max_dist_load:
+                            max_dist_load = abs(load[2])
+                
+                # Step through each plate
+                for plate in self.model.Plates.values():
+            
+                    # Step through each plate load
+                    for load in plate.pressures:
+            
+                        if load[1] == self.case:
+                
+                            if abs(load[0]) > max_area_load:
+                                max_area_load = abs(load[0])
+            
+            # Step through each quad
+            for quad in self.model.Quads.values():
+        
+                # Step through each plate load
+                for load in quad.pressures:
+            
+                    if load[1] == self.case:
+            
+                        if abs(load[0]) > max_area_load:
+                            max_area_load = abs(load[0])
+            
+        # Return the maximum loads for the load combo or load case
+        return max_pt_load, max_moment, max_dist_load, max_area_load
 
-# class VisMoment():
-#     '''
-#     Creates a concentrated moment for the viewer
-#     '''
-    
-#     def __init__(self, center, direction, radius, label_text=None, annotation_size=5, color=None):
-#         '''
-#         Constructor.
-      
-#         Parameters
-#         ----------
-#         center : tuple
-#           A tuple of X, Y and Z coordinates for center of the moment: (X, Y, Z).
-#         direction : tuple
-#           A tuple indicating the direction vector for the moment: (i, j, k).
-#         radius : number
-#           The radius of the moment.
-#         tip_length : number
-#           The height of the arrow head.
-#         label_text : string
-#           Text that will show up at the tail of the moment. If set to 'None' no text will be displayed.
-#         '''
+    def plot_loads(self):
       
-#         # Create an append filter to store load polydata in
-#         self.polydata = vtk.vtkAppendPolyData()
+        # Get the maximum load magnitudes that will be used to normalize the display scale
+        max_pt_load, max_moment, max_dist_load, max_area_load = self._calc_max_loads()
         
-#         # Find a vector perpendicular to the directional unit vector
-#         v1 = direction/norm(direction)  # v1 = The directional unit vector for the moment
-#         v2 = _PerpVector(v1)             # v2 = A unit vector perpendicular to v1
-#         v3 = cross(v1, v2)
-#         v3 = v3/norm(v3)                # v3 = A unit vector perpendicular to v1 and v2
-      
-#         # Generate an arc for the moment
-#         Xc, Yc, Zc = center
-#         arc = vtk.vtkArcSource()
-#         arc.SetCenter(Xc, Yc, Zc)
-#         arc.SetPoint1(Xc + v2[0]*radius, Yc + v2[1]*radius, Zc + v2[2]*radius)
-#         arc.SetPoint2(Xc + v3[0]*radius, Yc + v3[1]*radius, Zc + v3[2]*radius)
-#         arc.SetNegative(True)
-#         arc.SetResolution(20)
-#         arc.Update()
-#         self.polydata.AddInputData(arc.GetOutput())
-      
-#         # Generate the arrow tip at the end of the arc
-#         tip_length = radius/2
-#         cone_radius = radius/8
-#         tip = vtk.vtkConeSource()
-#         tip.SetCenter(arc.GetPoint1()[0], arc.GetPoint1()[1], arc.GetPoint1()[2])
-#         tip.SetDirection(cross(v1, v2))
-#         tip.SetHeight(tip_length)
-#         tip.SetRadius(cone_radius)
-#         tip.Update()
-#         self.polydata.AddInputData(tip.GetOutput())
-      
-#         # Update the polydata one last time now that we're done appending items to it
-#         self.polydata.Update()
-      
-#         # Create the text label
-#         label = vtk.vtkVectorText()
-#         label.SetText(label_text)
-#         lblMapper = vtk.vtkPolyDataMapper()
-#         lblMapper.SetInputConnection(label.GetOutputPort())
-#         self.lblActor = vtk.vtkFollower()
-#         self.lblActor.SetMapper(lblMapper)
-#         self.lblActor.SetScale(annotation_size, annotation_size, annotation_size)
-#         self.lblActor.SetPosition(Xc + v3[0]*(radius + 0.25*annotation_size), \
-#                                   Yc + v3[1]*(radius + 0.25*annotation_size), \
-#                                   Zc + v3[2]*(radius + 0.25*annotation_size))
-#         if color is None: self.lblActor.GetProperty().SetColor(0, 255, 0)  # Green
-#         elif color == 'black': self.lblActor.GetProperty().SetColor(0, 0, 0)  # Black
-
-# class VisAreaLoad():
-#     '''
-#     Creates an area load for the viewer
-#     '''
-    
-#     def __init__(self, position0, position1, position2, position3, direction, length, label_text, annotation_size=5, theme='default'):
-#         '''
-#         Constructor
-#         '''
-      
-#         # Create a point load for each corner of the area load
-#         ptLoads = []
-#         ptLoads.append(VisPtLoad(position0, direction, length, label_text, annotation_size=annotation_size))
-#         ptLoads.append(VisPtLoad(position1, direction, length, label_text, annotation_size=annotation_size))
-#         ptLoads.append(VisPtLoad(position2, direction, length, label_text, annotation_size=annotation_size))
-#         ptLoads.append(VisPtLoad(position3, direction, length, label_text, annotation_size=annotation_size))
-      
-#         # Find the direction cosines for the direction the load acts in
-#         dirDirCos = direction/norm(direction)
-      
-#         # Find the positions of the tails of all the arrows at the corners of the area load. This is
-#         # where we will place the polygon.
-#         self.p0 = position0 - dirDirCos*length
-#         self.p1 = position1 - dirDirCos*length
-#         self.p2 = position2 - dirDirCos*length
-#         self.p3 = position3 - dirDirCos*length
-      
-#         # Combine all geometry into one 'vtkPolyData' object
-#         self.polydata = vtk.vtkAppendPolyData()
-#         for arrow in ptLoads:
-#             self.polydata.AddInputData(arrow.polydata.GetOutput())
-#         self.polydata.Update()
-      
-#         # Add a label
-#         self.label_actor = ptLoads[0].lblActor
+        # Display the requested load combination, or 'Combo 1' if no load combo or case has been
+        # specified
+        if self.case is None:
+            # Store model.LoadCombos[combo].factors under a simpler name for use below
+            load_factors = self.model.LoadCombos[self.combo_name].factors
+        else:
+            # Set up a load combination dictionary that represents the load case
+            load_factors = {self.case: 1}
+        
+        # Step through each node
+        for node in self.model.Nodes.values():
+        
+            # Step through and display each nodal load
+            for load in node.NodeLoads:
+            
+                # Determine if this load is part of the requested LoadCombo or case
+                if load[2] in load_factors:
+                
+                    # Calculate the factored value for this load and it's sign (positive or
+                    # negative)
+                    load_value = load[1]*load_factors[load[2]]
+                    if load_value != 0:
+                        sign = load_value/abs(load_value)
+                    else:
+                        sign = 1
+                    
+                    # Determine the direction of this load
+                    if load[0] == 'FX' or load[0] == 'MX': direction = (sign*1, 0, 0)
+                    elif load[0] == 'FY' or load[0] == 'MY': direction = (0, sign*1, 0)
+                    elif load[0] == 'FZ' or load[0] == 'MZ': direction = (0, 0, sign*1)
+
+                    # Display the load
+                    if load[0] in {'FX', 'FY', 'FZ'}:
+                        self.plot_pt_load((node.X, node.Y, node.Z), direction,
+                                          load_value/max_pt_load*5*self.annotation_size,
+                                          load_value, 'green')
+                    elif load[0] in {'MX', 'MY', 'MZ'}:
+                        self.plot_moment((node.X, node.Y, node.Z), direction, abs(load_value/max_moment)*2.5*self.annotation_size, str(load_value), 'green')
+        
+        # Step through each member
+        for member in self.model.Members.values():
+        
+            # Get the direction cosines for the member's local axes
+            dir_cos = member.T()[0:3, 0:3]
+        
+            # Get the starting point for the member
+            x_start, y_start, z_start = member.i_node.X, member.i_node.Y, member.i_node.Z
+        
+            # Step through each member point load
+            for load in member.PtLoads:
+        
+                # Determine if this load is part of the requested load combination
+                if load[3] in load_factors:
+            
+                    # Calculate the factored value for this load and it's sign (positive or negative)
+                    load_value = load[1]*load_factors[load[3]]
+                    sign = load_value/abs(load_value)
+            
+                    # Calculate the load's location in 3D space
+                    x = load[2]
+                    position = [x_start + dir_cos[0, 0]*x, y_start + dir_cos[0, 1]*x, z_start + dir_cos[0, 2]*x]
+            
+                    # Display the load
+                    if load[0] == 'Fx':
+                        self.plot_pt_load(position, dir_cos[0, :], load_value/max_pt_load*5*self.annotation_size, load_value)
+                    elif load[0] == 'Fy':
+                        self.plot_pt_load(position, dir_cos[1, :], load_value/max_pt_load*5*self.annotation_size, load_value)
+                    elif load[0] == 'Fz':
+                        self.plot_pt_load(position, dir_cos[2, :], load_value/max_pt_load*5*self.annotation_size, load_value)
+                    elif load[0] == 'Mx':
+                        self.plot_moment(position, dir_cos[0, :]*sign, abs(load_value)/max_moment*2.5*self.annotation_size, str(load_value))
+                    elif load[0] == 'My':
+                        self.plot_moment(position, dir_cos[1, :]*sign, abs(load_value)/max_moment*2.5*self.annotation_size, str(load_value))
+                    elif load[0] == 'Mz':
+                        self.plot_moment(position, dir_cos[2, :]*sign, abs(load_value)/max_moment*2.5*self.annotation_size, str(load_value))
+                    elif load[0] == 'FX':
+                        self.plot_pt_load(position, [1, 0, 0], load_value/max_pt_load*5*self.annotation_size, load_value)
+                    elif load[0] == 'FY':
+                        self.plot_pt_load(position, [0, 1, 0], load_value/max_pt_load*5*self.annotation_size, load_value)
+                    elif load[0] == 'FZ':
+                        self.plot_pt_load(position, [0, 0, 1], load_value/max_pt_load*5*self.annotation_size, load_value)
+                    elif load[0] == 'MX':
+                        self.plot_moment(position, [1*sign, 0, 0], abs(load_value)/max_moment*2.5*self.annotation_size, str(load_value))
+                    elif load[0] == 'MY':
+                        self.plot_moment(position, [0, 1*sign, 0], abs(load_value)/max_moment*2.5*self.annotation_size, str(load_value))
+                    elif load[0] == 'MZ':
+                        self.plot_moment(position, [0, 0, 1*sign], abs(load_value)/max_moment*2.5*self.annotation_size, str(load_value))
+        
+            # Step through each member distributed load
+            for load in member.DistLoads:
+        
+                # Determine if this load is part of the requested load combination
+                if load[5] in load_factors:
+            
+                    # Calculate the factored value for this load and it's sign (positive or negative)
+                    w1 = load[1]*load_factors[load[5]]
+                    w2 = load[2]*load_factors[load[5]]
+            
+                    # Calculate the loads location in 3D space
+                    x1 = load[3]
+                    x2 = load[4]
+                    position1 = [x_start + dir_cos[0, 0]*x1, y_start + dir_cos[0, 1]*x1, z_start + dir_cos[0, 2]*x1]
+                    position2 = [x_start + dir_cos[0, 0]*x2, y_start + dir_cos[0, 1]*x2, z_start + dir_cos[0, 2]*x2]
+                    
+                    # Display the load
+                    if load[0] in {'Fx', 'Fy', 'Fz', 'FX', 'FY', 'FZ'}:
 
-#         # Add color to the area load label
-#         if theme == 'print':
-#             self.label_actor.GetProperty().SetColor(255/255, 0/255, 0/255)  # red
-#         elif theme == 'default':
-#             self.label_actor.GetProperty().SetColor(0/255, 255/255, 0/255)  # green
+                        # Determine the load direction
+                        if load[0] == 'Fx': direction = dir_cos[0, :]
+                        elif load[0] == 'Fy': direction = dir_cos[1, :]
+                        elif load[0] == 'Fz': direction = dir_cos[2, :]
+                        elif load[0] == 'FX': direction = [1, 0, 0]
+                        elif load[0] == 'FY': direction = [0, 1, 0]
+                        elif load[0] == 'FZ': direction = [0, 0, 1]
+
+                        # Plot the distributed load
+                        self.plot_dist_load(position1, position2, direction, w1/max_dist_load*5*self.annotation_size, w2/max_dist_load*5*self.annotation_size, str(sig_fig_round(w1, 3)), str(sig_fig_round(w2, 3)), 'green')
+        
+        # Step through each plate
+        for plate in list(self.model.Plates.values()) + list(self.model.Quads.values()):
+        
+            # Get the direction cosines for the plate's local z-axis
+            dir_cos = plate.T()[0:3, 0:3]
+            dir_cos = dir_cos[2]
+        
+            # Step through each plate load
+            for load in plate.pressures:
+        
+                # Determine if this load is part of the requested load combination
+                if load[1] in load_factors:
+            
+                    # Calculate the factored value for this load
+                    load_value = load[0]*load_factors[load[1]]
+                    
+                    # Find the sign for this load. Intercept any divide by zero errors
+                    if load[0] == 0:
+                        sign = 1
+                    else:
+                        sign = abs(load[0])/load[0]
+            
+                    # Find the position of the load's 4 corners
+                    position0 = [plate.i_node.X, plate.i_node.Y, plate.i_node.Z]
+                    position1 = [plate.j_node.X, plate.j_node.Y, plate.j_node.Z]
+                    position2 = [plate.m_node.X, plate.m_node.Y, plate.m_node.Z]
+                    position3 = [plate.n_node.X, plate.n_node.Y, plate.n_node.Z]
+            
+                    # Create an area load and get its data
+                    self.plot_area_load(position0, position1, position2, position3, dir_cos*sign, load_value/max_area_load*5*self.annotation_size, str(sig_fig_round(load_value, 3)), color='green')
 
 def _PerpVector(v):
     '''
     Returns a unit vector perpendicular to v=[i, j, k]
     '''
     
     i = v[0]
@@ -981,15 +1162,15 @@
         k2 = 1
     else:
         i2 = 1
         j2 = 1
         k2 = -(i*i2+j*j2)/k
     
     # Return the unit vector
-    return [i2, j2, k2]/norm([i2, j2, k2])
+    return [i2, j2, k2]/np.linalg.norm([i2, j2, k2])
 
 def _PrepContour(model, stress_type='Mx', combo_name='Combo 1'):
 
     if stress_type != None:
     
         # Erase any previous contours
         for node in model.Nodes.values():
@@ -1064,442 +1245,21 @@
       
         # Average the values at each node to obtain a smoothed contour
         for node in model.Nodes.values():
             # Prevent divide by zero errors for nodes with no contour values
             if node.contour != []:
                 node.contour = sum(node.contour)/len(node.contour)
 
-# def _DeformedShape(model, scale_factor, annotation_size, combo_name, render_nodes=True, theme='default'):
-#     '''
-#     Renders the deformed shape of a model.
-    
-#     Parameters
-#     ----------
-#     model : FEModel3D
-#         Finite element model to be rendered.
-#     scale_factor : number
-#         The scale factor to apply to the model deformations.
-#     annotation_size : number
-#         Controls the height of text displayed with the model. The units used for `annotation_size` are
-#         the same as those used for lengths in the model. Sizes of other objects (such as nodes) are
-#         related to this value.
-#     combo_name : string
-#         The load case used for rendering the deflected shape.
-    
-#     Returns
-#     -------
-#     None.
-#     '''
-    
-#     # Create an empty PolyData
-#     polydata = pv.PolyData()
-        
-#     # Add the springs to the PolyData
-#     for spring in model.Springs.values():
-#         # Only add the spring if it is active for the given load combination
-#         if spring.active[combo_name]:
-#             vis_spring = VisDeformedSpring(spring, model.Nodes, scale_factor, combo_name)
-#             polydata += vis_spring.source.GetOutput()
-            
-#     # Adjust the color
-#     if theme == 'default':
-#         color = [255, 255, 0]  # Yellow
-#     elif theme == 'print':
-#         color = [26, 26, 26]  # Dark Grey
-#     else:
-#         color = [255, 255, 255]  # White
-    
-#     # Create a PyVista actor for the PolyData
-#     actor = pv.PolyData(polydata).plot(color=color)
-
-
-# def _RenderLoads(model, renderer, annotation_size, combo_name, case, theme='default'):
-
-#     # Create an append filter to store all the polydata in. This will allow us to use fewer actors to
-#     # display all the loads, which will greatly improve rendering speed as the user interacts. VTK
-#     # becomes very slow when a large number of actors are used.
-#     polydata = vtk.vtkAppendPolyData()
-    
-#     # Polygons are treated as cells in VTK. Create a cell array to store all the area load polygons
-#     # in. We'll also create a list of points to store the polygon points in. The polydata for these
-#     # polygons will be stored separately from the other load data.
-#     polygons = vtk.vtkCellArray()
-#     polygon_points = vtk.vtkPoints()
-#     polygon_polydata = vtk.vtkPolyData()
-    
-#     # Get the maximum load magnitudes that will be used to normalize the display scale
-#     max_pt_load, max_moment, max_dist_load, max_area_load = _MaxLoads(model, combo_name, case)
-    
-#     # Display the requested load combination, or 'Combo 1' if no load combo or case has been
-#     # specified
-#     if case == None:
-#         # Store model.LoadCombos[combo].factors under a simpler name for use below
-#         load_factors = model.LoadCombos[combo_name].factors
-#     else:
-#         # Set up a load combination dictionary that represents the load case
-#         load_factors = {case: 1}
-    
-#     # Step through each node
-#     for node in model.Nodes.values():
-    
-#         # Step through and display each nodal load
-#         for load in node.NodeLoads:
-          
-#             # Determine if this load is part of the requested LoadCombo or case
-#             if load[2] in load_factors:
-              
-#                 # Calculate the factored value for this load and it's sign (positive or negative)
-#                 load_value = load[1]*load_factors[load[2]]
-#                 if load_value != 0:
-#                     sign = load_value/abs(load_value)
-#                 else:
-#                     sign = 1
-                
-#                 # Display the load
-#                 if load[0] == 'FX':
-#                     ptLoad = VisPtLoad((node.X - 0.6*annotation_size*sign, node.Y, node.Z), [1, 0, 0], load_value/max_pt_load*5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'FY':
-#                     ptLoad = VisPtLoad((node.X, node.Y - 0.6*annotation_size*sign, node.Z), [0, 1, 0], load_value/max_pt_load*5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'FZ':
-#                     ptLoad = VisPtLoad((node.X, node.Y, node.Z - 0.6*annotation_size*sign), [0, 0, 1], load_value/max_pt_load*5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'MX':
-#                     ptLoad = VisMoment((node.X, node.Y, node.Z), (1*sign, 0, 0), abs(load_value)/max_moment*2.5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'MY':
-#                     ptLoad = VisMoment((node.X, node.Y, node.Z), (0, 1*sign, 0), abs(load_value)/max_moment*2.5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'MZ':
-#                     ptLoad = VisMoment((node.X, node.Y, node.Z), (0, 0, 1*sign), abs(load_value)/max_moment*2.5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-                
-#                 polydata.AddInputData(ptLoad.polydata.GetOutput())
-#                 renderer.AddActor(ptLoad.lblActor)
-#                 ptLoad.lblActor.SetCamera(renderer.GetActiveCamera())
-    
-#     # Step through each member
-#     for member in model.Members.values():
-    
-#         # Get the direction cosines for the member's local axes
-#         dir_cos = member.T()[0:3, 0:3]
-      
-#         # Get the starting point for the member
-#         x_start, y_start, z_start = member.i_node.X, member.i_node.Y, member.i_node.Z
-      
-#         # Step through each member point load
-#         for load in member.PtLoads:
-      
-#             # Determine if this load is part of the requested load combination
-#             if load[3] in load_factors:
-        
-#                 # Calculate the factored value for this load and it's sign (positive or negative)
-#                 load_value = load[1]*load_factors[load[3]]
-#                 sign = load_value/abs(load_value)
-          
-#                 # Calculate the load's location in 3D space
-#                 x = load[2]
-#                 position = [x_start + dir_cos[0, 0]*x, y_start + dir_cos[0, 1]*x, z_start + dir_cos[0, 2]*x]
-          
-#                 # Display the load
-#                 if load[0] == 'Fx':
-#                     ptLoad = VisPtLoad(position, dir_cos[0, :], load_value/max_pt_load*5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'Fy':
-#                     ptLoad = VisPtLoad(position, dir_cos[1, :], load_value/max_pt_load*5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'Fz':
-#                     ptLoad = VisPtLoad(position, dir_cos[2, :], load_value/max_pt_load*5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'Mx':
-#                     ptLoad = VisMoment(position, dir_cos[0, :]*sign, abs(load_value)/max_moment*2.5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'My':
-#                     ptLoad = VisMoment(position, dir_cos[1, :]*sign, abs(load_value)/max_moment*2.5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'Mz':
-#                     ptLoad = VisMoment(position, dir_cos[2, :]*sign, abs(load_value)/max_moment*2.5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'FX':
-#                     ptLoad = VisPtLoad(position, [1, 0, 0], load_value/max_pt_load*5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'FY':
-#                     ptLoad = VisPtLoad(position, [0, 1, 0], load_value/max_pt_load*5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'FZ':
-#                     ptLoad = VisPtLoad(position, [0, 0, 1], load_value/max_pt_load*5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'MX':
-#                     ptLoad = VisMoment(position, [1*sign, 0, 0], abs(load_value)/max_moment*2.5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'MY':
-#                     ptLoad = VisMoment(position, [0, 1*sign, 0], abs(load_value)/max_moment*2.5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-#                 elif load[0] == 'MZ':
-#                     ptLoad = VisMoment(position, [0, 0, 1*sign], abs(load_value)/max_moment*2.5*annotation_size, '{:.3g}'.format(load_value), annotation_size)
-            
-#                 polydata.AddInputData(ptLoad.polydata.GetOutput())
-#                 renderer.AddActor(ptLoad.lblActor)
-#                 ptLoad.lblActor.SetCamera(renderer.GetActiveCamera())
-    
-#         # Step through each member distributed load
-#         for load in member.DistLoads:
-    
-#             # Determine if this load is part of the requested load combination
-#             if load[5] in load_factors:
-        
-#                 # Calculate the factored value for this load and it's sign (positive or negative)
-#                 w1 = load[1]*load_factors[load[5]]
-#                 w2 = load[2]*load_factors[load[5]]
-          
-#                 # Calculate the loads location in 3D space
-#                 x1 = load[3]
-#                 x2 = load[4]
-#                 position1 = [x_start + dir_cos[0, 0]*x1, y_start + dir_cos[0, 1]*x1, z_start + dir_cos[0, 2]*x1]
-#                 position2 = [x_start + dir_cos[0, 0]*x2, y_start + dir_cos[0, 1]*x2, z_start + dir_cos[0, 2]*x2]
-                
-#                 # Display the load
-#                 if load[0] == 'Fx':
-#                     distLoad = VisDistLoad(position1, position2, dir_cos[0, :], w1/max_dist_load*5*annotation_size, w2/max_dist_load*5*annotation_size, '{:.3g}'.format(w1), '{:.3g}'.format(w2), annotation_size)
-#                 elif load[0] == 'Fy':
-#                     distLoad = VisDistLoad(position1, position2, dir_cos[1, :], w1/max_dist_load*5*annotation_size, w2/max_dist_load*5*annotation_size, '{:.3g}'.format(w1), '{:.3g}'.format(w2), annotation_size)
-#                 elif load[0] == 'Fz':
-#                     distLoad = VisDistLoad(position1, position2, dir_cos[2, :], w1/max_dist_load*5*annotation_size, w2/max_dist_load*5*annotation_size, '{:.3g}'.format(w1), '{:.3g}'.format(w2), annotation_size)
-#                 elif load[0] == 'FX':
-#                     distLoad = VisDistLoad(position1, position2, [1, 0, 0], w1/max_dist_load*5*annotation_size, w2/max_dist_load*5*annotation_size, '{:.3g}'.format(w1), '{:.3g}'.format(w2), annotation_size)
-#                 elif load[0] == 'FY':
-#                     distLoad = VisDistLoad(position1, position2, [0, 1, 0], w1/max_dist_load*5*annotation_size, w2/max_dist_load*5*annotation_size, '{:.3g}'.format(w1), '{:.3g}'.format(w2), annotation_size)
-#                 elif load[0] == 'FZ':
-#                     distLoad = VisDistLoad(position1, position2, [0, 0, 1], w1/max_dist_load*5*annotation_size, w2/max_dist_load*5*annotation_size, '{:.3g}'.format(w1), '{:.3g}'.format(w2), annotation_size)
-               
-#                 polydata.AddInputData(distLoad.polydata.GetOutput())
-#                 renderer.AddActor(distLoad.lblActors[0])
-#                 renderer.AddActor(distLoad.lblActors[1])
-#                 distLoad.lblActors[0].SetCamera(renderer.GetActiveCamera())
-#                 distLoad.lblActors[1].SetCamera(renderer.GetActiveCamera())   
-    
-#     # Step through each plate
-#     i = 0
-#     for plate in list(model.Plates.values()) + list(model.Quads.values()):
-    
-#         # Get the direction cosines for the plate's local z-axis
-#         dir_cos = plate.T()[0:3, 0:3]
-#         dir_cos = dir_cos[2]
-      
-#         # Step through each plate load
-#         for load in plate.pressures:
-      
-#             # Determine if this load is part of the requested load combination
-#             if load[1] in load_factors:
-        
-#                 # Calculate the factored value for this load
-#                 load_value = load[0]*load_factors[load[1]]
-                
-#                 # Find the sign for this load. Intercept any divide by zero errors
-#                 if load[0] == 0:
-#                     sign = 1
-#                 else:
-#                     sign = abs(load[0])/load[0]
-          
-#                 # Find the position of the load's 4 corners
-#                 position0 = [plate.i_node.X, plate.i_node.Y, plate.i_node.Z]
-#                 position1 = [plate.j_node.X, plate.j_node.Y, plate.j_node.Z]
-#                 position2 = [plate.m_node.X, plate.m_node.Y, plate.m_node.Z]
-#                 position3 = [plate.n_node.X, plate.n_node.Y, plate.n_node.Z]
-          
-#                 # Create an area load and get its data
-#                 area_load = VisAreaLoad(position0, position1, position2, position3, dir_cos*sign, abs(load_value)/max_area_load*5*annotation_size, '{:.3g}'.format(load_value), annotation_size, theme)
-          
-#                 # Add the area load's arrows to the overall load polydata
-#                 polydata.AddInputData(area_load.polydata.GetOutput())
-          
-#                 # Add the 4 points at the corners of this area load to the list of points
-#                 polygon_points.InsertNextPoint(area_load.p0[0], area_load.p0[1], area_load.p0[2])
-#                 polygon_points.InsertNextPoint(area_load.p1[0], area_load.p1[1], area_load.p1[2])
-#                 polygon_points.InsertNextPoint(area_load.p2[0], area_load.p2[1], area_load.p2[2])
-#                 polygon_points.InsertNextPoint(area_load.p3[0], area_load.p3[1], area_load.p3[2])
-          
-#                 # Create a polygon based on the four points we just defined.
-#                 # The 1st number in `SetId()` is the local point id
-#                 # The 2nd number in `SetId()` is the global point id
-#                 polygon = vtk.vtkPolygon()
-#                 polygon.GetPointIds().SetNumberOfIds(4)
-#                 polygon.GetPointIds().SetId(0, i*4)
-#                 polygon.GetPointIds().SetId(1, i*4 + 1)
-#                 polygon.GetPointIds().SetId(2, i*4 + 2)
-#                 polygon.GetPointIds().SetId(3, i*4 + 3)
-          
-#                 # Add the polygon to the list of polygons
-#                 polygons.InsertNextCell(polygon)
-                
-#                 # Add the load label
-#                 renderer.AddActor(area_load.label_actor)
-          
-#                 # Set the text to follow the camera as the user interacts
-#                 area_load.label_actor.SetCamera(renderer.GetActiveCamera())
-          
-#                 # `i` keeps track of the next polygon's ID. We've just added a polygon, so `i` needs to
-#                 # go up 1.
-#                 i += 1
-        
-#                 # Create polygon polydata from all the points and polygons we just defined
-#                 polygon_polydata.SetPoints(polygon_points)
-#                 polygon_polydata.SetPolys(polygons)
-    
-#     # Set up an actor and mapper for the loads
-#     load_mapper = vtk.vtkPolyDataMapper()
-#     load_mapper.SetInputConnection(polydata.GetOutputPort())
-#     load_actor = vtk.vtkActor()
-#     load_actor.SetMapper(load_mapper)
-
-#     # Colorize the loads
-#     if theme == 'default':
-#         load_actor.GetProperty().SetColor(0/255, 255/255, 0/255)  # Green
-#     elif theme == 'print':
-#         load_actor.GetProperty().SetColor(255/255, 0/255, 0/255)  # Red
-
-#     # Add the load actor to the renderer
-#     renderer.AddActor(load_actor)
-    
-#     # Set up an actor and a mapper for the area load polygons
-#     polygon_mapper = vtk.vtkPolyDataMapper()
-#     polygon_mapper.SetInputData(polygon_polydata)
-#     polygon_actor = vtk.vtkActor()
-
-#     # polygon_actor.GetProperty().SetOpacity(0.5)      # 50% opacity
-#     polygon_actor.SetMapper(polygon_mapper)
-#     renderer.AddActor(polygon_actor)
-    
-#     # Set the color of the area load polygons
-#     if theme == 'default':
-#         polygon_actor.GetProperty().SetColor(0/255, 255/255, 0/255)  # Green
-#     elif theme == 'print':
-#         polygon_actor.GetProperty().SetColor(255/255, 0/255, 0/255)  # Red
-
-def _MaxLoads(model, combo_name=None, case=None):
-
-    max_pt_load = 0
-    max_moment = 0
-    max_dist_load = 0
-    max_area_load = 0
-    
-    # Find the requested load combination or load case
-    if case == None:
-    
-        # Step through each node
-        for node in model.Nodes.values():
-      
-            # Step through each nodal load to find the largest one
-            for load in node.NodeLoads:
-              
-                # Find the largest loads in the load combination
-                if load[2] in model.LoadCombos[combo_name].factors:
-                    if load[0] == 'FX' or load[0] == 'FY' or load[0] == 'FZ':
-                        if abs(load[1]*model.LoadCombos[combo_name].factors[load[2]]) > max_pt_load:
-                            max_pt_load = abs(load[1]*model.LoadCombos[combo_name].factors[load[2]])
-                    else:
-                        if abs(load[1]*model.LoadCombos[combo_name].factors[load[2]]) > max_moment:
-                            max_moment = abs(load[1]*model.LoadCombos[combo_name].factors[load[2]])
-    
-        # Step through each member
-        for member in model.Members.values():
-      
-            # Step through each member point load
-            for load in member.PtLoads:
-                
-                # Find and store the largest point load and moment in the load combination
-                if load[3] in model.LoadCombos[combo_name].factors:
-          
-                    if (load[0] == 'Fx' or load[0] == 'Fy' or load[0] == 'Fz'
-                    or  load[0] == 'FX' or load[0] == 'FY' or load[0] == 'FZ'):
-                        if abs(load[1]*model.LoadCombos[combo_name].factors[load[3]]) > max_pt_load:
-                            max_pt_load = abs(load[1]*model.LoadCombos[combo_name].factors[load[3]])
-                    else:
-                        if abs(load[1]*model.LoadCombos[combo_name].factors[load[3]]) > max_moment:
-                            max_moment = abs(load[1]*model.LoadCombos[combo_name].factors[load[3]])
-      
-            # Step through each member distributed load
-            for load in member.DistLoads:
-        
-                #Find and store the largest distributed load in the load combination
-                if load[5] in model.LoadCombos[combo_name].factors:
-          
-                    if abs(load[1]*model.LoadCombos[combo_name].factors[load[5]]) > max_dist_load:
-                        max_dist_load = abs(load[1]*model.LoadCombos[combo_name].factors[load[5]])
-                    if abs(load[2]*model.LoadCombos[combo_name].factors[load[5]]) > max_dist_load:
-                        max_dist_load = abs(load[2]*model.LoadCombos[combo_name].factors[load[5]])
-      
-        # Step through each plate
-        for plate in model.Plates.values():
-      
-            # Step through each plate load
-            for load in plate.pressures:
-        
-                if load[1] in model.LoadCombos[combo_name].factors:
-                    if abs(load[0]*model.LoadCombos[combo_name].factors[load[1]]) > max_area_load:
-                        max_area_load = abs(load[0]*model.LoadCombos[combo_name].factors[load[1]])
-      
-        # Step through each quad
-        for quad in model.Quads.values():
-      
-            # Step through each plate load
-            for load in quad.pressures:
-        
-                # Check to see if the load case is in the requested load combination
-                if load[1] in model.LoadCombos[combo_name].factors:
-                    if abs(load[0]*model.LoadCombos[combo_name].factors[load[1]]) > max_area_load:
-                        max_area_load = abs(load[0]*model.LoadCombos[combo_name].factors[load[1]])
-      
-    # Behavior if case has been specified
-    else:
-        
-        # Step through each node
-        for node in model.Nodes.values():
-      
-            # Step through each nodal load to find the largest one
-            for load in node.NodeLoads:
-              
-                # Find the largest loads in the load case
-                if load[2] == case:
-                    if load[0] == 'FX' or load[0] == 'FY' or load[0] == 'FZ':
-                        if abs(load[1]) > max_pt_load:
-                            max_pt_load = abs(load[1])
-                    else:
-                        if abs(load[1]) > max_moment:
-                            max_moment = abs(load[1])
-      
-        # Step through each member
-        for member in model.Members.values():
-      
-            # Step through each member point load
-            for load in member.PtLoads:
-              
-                # Find and store the largest point load and moment in the load case
-                if load[3] == case:
-            
-                    if (load[0] == 'Fx' or load[0] == 'Fy' or load[0] == 'Fz'
-                    or  load[0] == 'FX' or load[0] == 'FY' or load[0] == 'FZ'):
-                        if abs(load[1]) > max_pt_load:
-                            max_pt_load = abs(load[1])
-                    else:
-                        if abs(load[1]) > max_moment:
-                            max_moment = abs(load[1])
-        
-            # Step through each member distributed load
-            for load in member.DistLoads:
-          
-                # Find and store the largest distributed load in the load case
-                if load[5] == case:
-            
-                    if abs(load[1]) > max_dist_load:
-                        max_dist_load = abs(load[1])
-                    if abs(load[2]) > max_dist_load:
-                        max_dist_load = abs(load[2])
-            
-            # Step through each plate
-            for plate in model.Plates.values():
-          
-                # Step through each plate load
-                for load in plate.pressures:
-          
-                    if load[1] == case:
-            
-                        if abs(load[0]) > max_area_load:
-                            max_area_load = abs(load[0])
-          
-        # Step through each quad
-        for quad in model.Quads.values():
-      
-            # Step through each plate load
-            for load in quad.pressures:
-        
-                if load[1] == case:
-          
-                    if abs(load[0]) > max_area_load:
-                        max_area_load = abs(load[0])
-        
-    # Return the maximum loads in the load combination or load case
-    return max_pt_load, max_moment, max_dist_load, max_area_load
+def sig_fig_round(number, sig_figs):
+    if number == 0:
+        return 0
+
+    # Calculate the magnitude of the number
+    magnitude = math.floor(math.log10(abs(number)))
+
+    # Calculate the number of decimal places to round to
+    decimal_places = sig_figs - 1 - magnitude
+
+    # Round the number to the specified number of decimal places
+    rounded_number = round(number, decimal_places)
+
+    return rounded_number
```

### Comparing `PyNiteFEA-0.0.93/PyNiteFEA.egg-info/PKG-INFO` & `pynitefea-0.0.94/PyNiteFEA.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: PyNiteFEA
-Version: 0.0.93
+Version: 0.0.94
 Summary: A simple elastic 3D structural finite element library for Python.
 Home-page: https://github.com/JWock82/PyNite.git
 Author: D. Craig Brinck, PE, SE
 Author-email: Building.Code@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: PrettyTable
-Provides-Extra: sparse-solver
-Requires-Dist: scipy; extra == "sparse-solver"
+Provides-Extra: sparse
+Requires-Dist: scipy; extra == "sparse"
 Provides-Extra: plotting
 Requires-Dist: matplotlib; extra == "plotting"
-Provides-Extra: visualization
-Requires-Dist: vtk; extra == "visualization"
-Provides-Extra: visualization-screenshots
-Requires-Dist: IPython; extra == "visualization-screenshots"
+Provides-Extra: vtk
+Requires-Dist: vtk; extra == "vtk"
+Requires-Dist: IPython; extra == "vtk"
+Provides-Extra: pyvista
+Requires-Dist: vtk; extra == "pyvista"
+Requires-Dist: pyvista[all,trame]; extra == "pyvista"
+Requires-Dist: trame_jupyter_extension; extra == "pyvista"
+Requires-Dist: ipywidgets; extra == "pyvista"
 Provides-Extra: reporting
 Requires-Dist: pdfkit; extra == "reporting"
 Requires-Dist: Jinja2; extra == "reporting"
-Provides-Extra: reviewing-derivations
-Requires-Dist: jupyterlab; extra == "reviewing-derivations"
-Requires-Dist: sympy; extra == "reviewing-derivations"
+Provides-Extra: derivations
+Requires-Dist: jupyterlab; extra == "derivations"
+Requires-Dist: sympy; extra == "derivations"
 
 <div align="center">
   <img src="https://github.com/JWock82/PyNite/raw/main/Resources/Full Logo No Buffer.png" width=40% align="center"/>
   <br>
   <h1>Simple Finite Element Analysis in Python</h1>
 </div>
 
@@ -87,14 +91,19 @@
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Civils.ai (https://civils.ai/1/free-3D-finite-element-structural-analysis)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.94
+* Added rendering via `Pyvista`. This greatly simplified the rendering code and provided a fresh look to the rendereings. Renderings in jupyter are now interactive. Global axes are also now shown in rendereings. To use `Pyvista` instead of `VTK`, use the new `Rendering` library rather than the old `Visualization` library. Rendering via `VTK` directly is still available.
+* Bug fix for member self-weight. The program was throwing exceptions instead of calculating member self-weight. Added a unit test to help prevent this issue from occuring again as code changes.
+* Refactored `material` to be `material_name` in the code. The prior naming convention caused confusion which led to the self-weight bug.
+
 v0.0.93
 * Fixed phantom reactions showing up at unsupported nodes. If there was a support defined at a node, the program was summing reactions for all directions at the node, rather than just the supported directions. This caused the program to report "extra" reaction directions at any supported node (if the user queried them). Element forces/stresses were not affected as this was a post-processing reaction summing issue. Reactions for supported directions were summed correctly, except in the case of nodes with both spring supports and other supports. Only unsupported directions, and nodes with both spring supports and other supports, were showing phantom reactions. This bug also caused statics checks to fail from time to time.
 * Reorganized physical member code to match member code more consistently.
 
 v0.0.92
 * Added member self-weight calculations via `FEModel3D.add_member_self_weight()`. This only applies to members. This feature does not calculate self-weight for plate and quad elements.
```

### Comparing `PyNiteFEA-0.0.93/PyNiteFEA.egg-info/SOURCES.txt` & `pynitefea-0.0.94/PyNiteFEA.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 PyNite/Member3D.py
 PyNite/Mesh.py
 PyNite/Node3D.py
 PyNite/PhysMember.py
 PyNite/Plastic Beam.py
 PyNite/Plate3D.py
 PyNite/Quad3D.py
+PyNite/Rendering.py
 PyNite/Report_Template.html
 PyNite/Reporting.py
 PyNite/Section.py
 PyNite/Spring3D.py
 PyNite/Visualization.py
-PyNite/Visualization_PyVista.py
 PyNite/__init__.py
 PyNiteFEA.egg-info/PKG-INFO
 PyNiteFEA.egg-info/SOURCES.txt
 PyNiteFEA.egg-info/dependency_links.txt
 PyNiteFEA.egg-info/requires.txt
 PyNiteFEA.egg-info/top_level.txt
```

### Comparing `PyNiteFEA-0.0.93/README.md` & `pynitefea-0.0.94/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,19 @@
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Civils.ai (https://civils.ai/1/free-3D-finite-element-structural-analysis)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.94
+* Added rendering via `Pyvista`. This greatly simplified the rendering code and provided a fresh look to the rendereings. Renderings in jupyter are now interactive. Global axes are also now shown in rendereings. To use `Pyvista` instead of `VTK`, use the new `Rendering` library rather than the old `Visualization` library. Rendering via `VTK` directly is still available.
+* Bug fix for member self-weight. The program was throwing exceptions instead of calculating member self-weight. Added a unit test to help prevent this issue from occuring again as code changes.
+* Refactored `material` to be `material_name` in the code. The prior naming convention caused confusion which led to the self-weight bug.
+
 v0.0.93
 * Fixed phantom reactions showing up at unsupported nodes. If there was a support defined at a node, the program was summing reactions for all directions at the node, rather than just the supported directions. This caused the program to report "extra" reaction directions at any supported node (if the user queried them). Element forces/stresses were not affected as this was a post-processing reaction summing issue. Reactions for supported directions were summed correctly, except in the case of nodes with both spring supports and other supports. Only unsupported directions, and nodes with both spring supports and other supports, were showing phantom reactions. This bug also caused statics checks to fail from time to time.
 * Reorganized physical member code to match member code more consistently.
 
 v0.0.92
 * Added member self-weight calculations via `FEModel3D.add_member_self_weight()`. This only applies to members. This feature does not calculate self-weight for plate and quad elements.
```

### Comparing `PyNiteFEA-0.0.93/setup.py` & `pynitefea-0.0.94/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyNiteFEA",
-    version="0.0.93",
+    version="0.0.94",
     author="D. Craig Brinck, PE, SE",
     author_email="Building.Code@outlook.com",
     description="A simple elastic 3D structural finite element library for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JWock82/PyNite.git",
     packages=setuptools.find_packages(include=['PyNite', 'Pynite.*']),
@@ -20,17 +20,17 @@
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'numpy',
         'PrettyTable'
     ],
     extras_require = {
-        'Sparse Solver': ['scipy'],
-        'Plotting': ['matplotlib'],
-        'Visualization':  ['vtk'],
-        'Visualization Screenshots': ['IPython'],
-        'Reporting': ['pdfkit', 'Jinja2'],
-        'Reviewing Derivations': ['jupyterlab', 'sympy']
+        'sparse': ['scipy'],
+        'plotting': ['matplotlib'],
+        'vtk':  ['vtk', 'IPython'],
+        'pyvista': ['vtk', 'pyvista[all,trame]', 'trame_jupyter_extension', 'ipywidgets'],
+        'reporting': ['pdfkit', 'Jinja2'],
+        'derivations': ['jupyterlab', 'sympy']
     },
     include_package_data = True,
-    python_requires = '>=3.6',
+    python_requires = '>=3.7',
 )
```

