# Comparing `tmp/geospann-0.1.1.tar.gz` & `tmp/geospann-0.1.2.tar.gz`

## Comparing `geospann-0.1.1.tar` & `geospann-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 geospann-0.1.1/.pypirc
--rw-r--r--   0        0        0  1032391 2020-02-02 00:00:00.000000 geospann-0.1.1/Example_realdata.ipynb
--rw-r--r--   0        0        0   366374 2020-02-02 00:00:00.000000 geospann-0.1.1/Example_simulation.ipynb
--rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 geospann-0.1.1/Example_simulation.md
--rw-r--r--   0        0        0    64623 2020-02-02 00:00:00.000000 geospann-0.1.1/Running_time.ipynb
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geospann-0.1.1/.idea/.gitignore
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 geospann-0.1.1/.idea/.name
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 geospann-0.1.1/.idea/NN-GLS.iml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 geospann-0.1.1/.idea/misc.xml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 geospann-0.1.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 geospann-0.1.1/.idea/vcs.xml
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 geospann-0.1.1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 geospann-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0  1032391 2020-02-02 00:00:00.000000 geospann-0.1.1/.ipynb_checkpoints/Example_realdata-checkpoint.ipynb
--rw-r--r--   0        0        0   366374 2020-02-02 00:00:00.000000 geospann-0.1.1/.ipynb_checkpoints/Example_simulation-checkpoint.ipynb
--rw-r--r--   0        0        0    64623 2020-02-02 00:00:00.000000 geospann-0.1.1/.ipynb_checkpoints/Running_time-checkpoint.ipynb
--rw-r--r--   0        0        0    97026 2020-02-02 00:00:00.000000 geospann-0.1.1/data/Normalized_PM2.5_20190605.csv
--rw-r--r--   0        0        0   180525 2020-02-02 00:00:00.000000 geospann-0.1.1/data/US_heat_0605.png
--rwxr-xr-x   0        0        0  1112364 2020-02-02 00:00:00.000000 geospann-0.1.1/data/covariate0605.csv
--rwxr-xr-x   0        0        0    32432 2020-02-02 00:00:00.000000 geospann-0.1.1/data/pm25_0605.csv
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 geospann-0.1.1/data/running_time.csv
--rw-r--r--   0        0        0    93119 2020-02-02 00:00:00.000000 geospann-0.1.1/data/output_figures/output_10_0.png
--rw-r--r--   0        0        0    34117 2020-02-02 00:00:00.000000 geospann-0.1.1/data/output_figures/output_7_0.png
--rw-r--r--   0        0        0    53531 2020-02-02 00:00:00.000000 geospann-0.1.1/data/output_figures/output_8_0.png
--rw-r--r--   0        0        0    84381 2020-02-02 00:00:00.000000 geospann-0.1.1/data/output_figures/output_9_0.png
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 geospann-0.1.1/geospaNN/__init__.py
--rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 geospann-0.1.1/geospaNN/main.py
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 geospann-0.1.1/geospaNN/model.py
--rw-r--r--   0        0        0    19215 2020-02-02 00:00:00.000000 geospann-0.1.1/geospaNN/utils.py
--rw-r--r--   0        0        0    13446 2020-02-02 00:00:00.000000 geospann-0.1.1/tests/test.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 geospann-0.1.1/LICENSE
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 geospann-0.1.1/README.md
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 geospann-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 geospann-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 geospann-0.1.2/.pypirc
+-rw-r--r--   0        0        0  1032391 2020-02-02 00:00:00.000000 geospann-0.1.2/Example_realdata.ipynb
+-rw-r--r--   0        0        0   366374 2020-02-02 00:00:00.000000 geospann-0.1.2/Example_simulation.ipynb
+-rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 geospann-0.1.2/Example_simulation.md
+-rw-r--r--   0        0        0    64623 2020-02-02 00:00:00.000000 geospann-0.1.2/Running_time.ipynb
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geospann-0.1.2/.idea/.gitignore
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 geospann-0.1.2/.idea/.name
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 geospann-0.1.2/.idea/NN-GLS.iml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 geospann-0.1.2/.idea/misc.xml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 geospann-0.1.2/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 geospann-0.1.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 geospann-0.1.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 geospann-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0  1032391 2020-02-02 00:00:00.000000 geospann-0.1.2/.ipynb_checkpoints/Example_realdata-checkpoint.ipynb
+-rw-r--r--   0        0        0   366374 2020-02-02 00:00:00.000000 geospann-0.1.2/.ipynb_checkpoints/Example_simulation-checkpoint.ipynb
+-rw-r--r--   0        0        0    64623 2020-02-02 00:00:00.000000 geospann-0.1.2/.ipynb_checkpoints/Running_time-checkpoint.ipynb
+-rw-r--r--   0        0        0    97026 2020-02-02 00:00:00.000000 geospann-0.1.2/data/Normalized_PM2.5_20190605.csv
+-rw-r--r--   0        0        0   180525 2020-02-02 00:00:00.000000 geospann-0.1.2/data/US_heat_0605.png
+-rwxr-xr-x   0        0        0  1112364 2020-02-02 00:00:00.000000 geospann-0.1.2/data/covariate0605.csv
+-rw-r--r--   0        0        0   259168 2020-02-02 00:00:00.000000 geospann-0.1.2/data/nngls.png
+-rwxr-xr-x   0        0        0    32432 2020-02-02 00:00:00.000000 geospann-0.1.2/data/pm25_0605.csv
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 geospann-0.1.2/data/running_time.csv
+-rw-r--r--   0        0        0    93119 2020-02-02 00:00:00.000000 geospann-0.1.2/data/output_figures/output_10_0.png
+-rw-r--r--   0        0        0    34117 2020-02-02 00:00:00.000000 geospann-0.1.2/data/output_figures/output_7_0.png
+-rw-r--r--   0        0        0    53531 2020-02-02 00:00:00.000000 geospann-0.1.2/data/output_figures/output_8_0.png
+-rw-r--r--   0        0        0    84381 2020-02-02 00:00:00.000000 geospann-0.1.2/data/output_figures/output_9_0.png
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 geospann-0.1.2/geospaNN/__init__.py
+-rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 geospann-0.1.2/geospaNN/main.py
+-rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 geospann-0.1.2/geospaNN/model.py
+-rw-r--r--   0        0        0    37612 2020-02-02 00:00:00.000000 geospann-0.1.2/geospaNN/utils.py
+-rw-r--r--   0        0        0    13446 2020-02-02 00:00:00.000000 geospann-0.1.2/tests/test.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 geospann-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8441 2020-02-02 00:00:00.000000 geospann-0.1.2/README.md
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 geospann-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 geospann-0.1.2/PKG-INFO
```

### Comparing `geospann-0.1.1/Example_realdata.ipynb` & `geospann-0.1.2/Example_realdata.ipynb`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/Example_simulation.ipynb` & `geospann-0.1.2/Example_simulation.ipynb`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/Example_simulation.md` & `geospann-0.1.2/Example_simulation.md`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/Running_time.ipynb` & `geospann-0.1.2/Running_time.ipynb`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/.idea/workspace.xml` & `geospann-0.1.2/.idea/workspace.xml`

 * *Files 7% similar despite different names*

#### Comparing `geospann-0.1.1/.idea/workspace.xml` & `geospann-0.1.2/.idea/workspace.xml`

```diff
@@ -1,14 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
     <list default="true" id="55b6d3ef-0094-4559-b139-f97e41838c95" name="Changes" comment="">
-      <change beforePath="$PROJECT_DIR$/dist/geospaNN-0.1.0-py3-none-any.whl" beforeDir="false" afterPath="$PROJECT_DIR$/dist/geospaNN-0.1.0-py3-none-any.whl" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/dist/geospann-0.1.0.tar.gz" beforeDir="false" afterPath="$PROJECT_DIR$/dist/geospann-0.1.0.tar.gz" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
```

### Comparing `geospann-0.1.1/.ipynb_checkpoints/Example_realdata-checkpoint.ipynb` & `geospann-0.1.2/.ipynb_checkpoints/Example_realdata-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/.ipynb_checkpoints/Example_simulation-checkpoint.ipynb` & `geospann-0.1.2/.ipynb_checkpoints/Example_simulation-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/.ipynb_checkpoints/Running_time-checkpoint.ipynb` & `geospann-0.1.2/.ipynb_checkpoints/Running_time-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/data/Normalized_PM2.5_20190605.csv` & `geospann-0.1.2/data/Normalized_PM2.5_20190605.csv`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/data/US_heat_0605.png` & `geospann-0.1.2/data/US_heat_0605.png`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/data/covariate0605.csv` & `geospann-0.1.2/data/covariate0605.csv`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/data/pm25_0605.csv` & `geospann-0.1.2/data/pm25_0605.csv`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/data/running_time.csv` & `geospann-0.1.2/data/running_time.csv`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/data/output_figures/output_10_0.png` & `geospann-0.1.2/data/output_figures/output_10_0.png`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/data/output_figures/output_7_0.png` & `geospann-0.1.2/data/output_figures/output_7_0.png`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/data/output_figures/output_8_0.png` & `geospann-0.1.2/data/output_figures/output_8_0.png`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/data/output_figures/output_9_0.png` & `geospann-0.1.2/data/output_figures/output_9_0.png`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/geospaNN/main.py` & `geospann-0.1.2/geospaNN/main.py`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/geospaNN/model.py` & `geospann-0.1.2/geospaNN/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,57 @@
 from .utils import make_cov_full, distance, edit_batch, krig_pred
 
 import torch
 from torch_geometric.nn import MessagePassing
 
+
 class CovarianceVectorConv(MessagePassing):
+    """
+    A message passing layer
+    """
     def __init__(self, neighbor_size, theta):
         super().__init__(aggr="sum")
         self.neighbor_size = neighbor_size
         self.theta = theta
 
     def forward(self, pos, edge_index, edge_attr, batch_size):
-        return self.propagate(edge_index, pos = pos, edge_attr=edge_attr)[range(batch_size),:]
+        return self.propagate(edge_index, pos=pos, edge_attr=edge_attr)[range(batch_size), :]
 
     def message(self, pos_i, pos_j, edge_attr):
         num_edges = edge_attr.shape[0]
         msg = torch.zeros(num_edges, self.neighbor_size)
         col_idc = edge_attr.flatten()
         row_idc = torch.tensor(range(num_edges))
-        msg[row_idc, col_idc] = make_cov_full(self.theta, distance(pos_i - pos_j, torch.zeros(1,2))).squeeze()
+        msg[row_idc, col_idc] = make_cov_full(distance(pos_i - pos_j, torch.zeros(1, 2)), self.theta).squeeze()
         return msg
 
+
 class InverseCovMatrixFromPositions(torch.nn.Module):
     def __init__(self, neighbor_size, coord_dimension, theta):
         super(InverseCovMatrixFromPositions, self).__init__()
         self.neighbor_size = neighbor_size
         self.coord_dimension = coord_dimension
         self.theta = theta
 
     def forward(self, neighbor_positions, edge_list):
         batch_size = neighbor_positions.shape[0]
         neighbor_positions = neighbor_positions.reshape(-1, self.neighbor_size, self.coord_dimension)
         neighbor_positions1 = neighbor_positions.unsqueeze(1)
         neighbor_positions2 = neighbor_positions.unsqueeze(2)
         dists = torch.sqrt(torch.sum((neighbor_positions1 - neighbor_positions2) ** 2, axis=-1))
-        cov = make_cov_full(self.theta, dists, nuggets = True) #have to add nuggets (resolved)
-        #cov_final = self.theta[0]*torch.eye(self.neighbor_size).repeat(batch_size, 1, 1)
-        #for i in range(batch_size):
+        cov = make_cov_full(dists, self.theta, nuggets=True)  # have to add nuggets (resolved)
+        # cov_final = self.theta[0]*torch.eye(self.neighbor_size).repeat(batch_size, 1, 1)
+        # for i in range(batch_size):
         #    cov_final[i, edge_list[i].reshape(1, -1, 1), edge_list[i].reshape(1, 1, -1)] = \
         #        cov[i, edge_list[i].reshape(1, -1, 1), edge_list[i].reshape(1, 1, -1)]
-        #inv_cov_final = torch.linalg.inv(cov_final)
+        # inv_cov_final = torch.linalg.inv(cov_final)
         inv_cov_final = torch.linalg.inv(cov)
         return inv_cov_final
 
+
 class GatherNeighborPositionsConv(MessagePassing):
     def __init__(self, neighbor_size, coord_dimensions):
         super().__init__(aggr="sum")
         self.neighbor_size = neighbor_size
         self.coord_dimensions = coord_dimensions
 
     def forward(self, pos, edge_index, edge_attr, batch_size):
@@ -60,92 +66,95 @@
         col_idc = edge_attr.flatten() * self.coord_dimensions
         row_idc = torch.tensor(range(num_edges))
         msg[
             row_idc.unsqueeze(1), col_idc.unsqueeze(1) + torch.tensor(range(self.coord_dimensions))
         ] = pos_j
         return msg
 
+
 class GatherNeighborInfoConv(MessagePassing):
     """
     The output of node i will be a tensor of shape (neighbor_size+1,) where the j-th row contains
     the output of the (j+1)-th neighbor of node i. The first row will contain the output of node i.
     Assumes that the outputs are already computed.
     """
 
     def __init__(self, neighbor_size):
         super().__init__(aggr="sum")
         self.neighbor_size = neighbor_size
 
     def forward(self, y, edge_index, edge_attr, batch_size):
-        out = self.propagate(edge_index, y = y.reshape(-1,1), edge_attr=edge_attr)[range(batch_size),:]
+        out = self.propagate(edge_index, y=y.reshape(-1, 1), edge_attr=edge_attr)[range(batch_size), :]
         return out
 
     def message(self, y_j, edge_attr):
         num_edges = edge_attr.shape[0]
         msg = torch.zeros(num_edges, self.neighbor_size).double()
         col_idc = edge_attr.flatten()
         row_idc = torch.tensor(range(num_edges))
         msg[row_idc, col_idc] = y_j.squeeze().double()
         return msg
 
+
 class nngls(torch.nn.Module):
     def __init__(
-        self,
-        p: int,
-        neighbor_size: int,
-        coord_dimensions: int,
-        mlp: torch.nn.Module,
-        theta: tuple[float, float, float]
+            self,
+            p: int,
+            neighbor_size: int,
+            coord_dimensions: int,
+            mlp: torch.nn.Module,
+            theta: tuple[float, float, float]
     ):
         super(nngls, self).__init__()
         self.p = p
         self.neighbor_size = neighbor_size
         self.coord_dimensions = coord_dimensions
-        self.theta = torch.nn.Parameter(torch.Tensor(theta)) # split to accelerate?
+        self.theta = torch.nn.Parameter(torch.Tensor(theta))  # split to accelerate?
         self.compute_covariance_vectors = CovarianceVectorConv(neighbor_size, self.theta)
         self.compute_inverse_cov_matrices = InverseCovMatrixFromPositions(
             neighbor_size, coord_dimensions, self.theta
         )
         self.gather_neighbor_positions = GatherNeighborPositionsConv(neighbor_size, coord_dimensions)
         self.gather_neighbor_outputs = GatherNeighborInfoConv(neighbor_size)
         self.gather_neighbor_targets = GatherNeighborInfoConv(neighbor_size)
 
         # Simple MLP to map features to scalars
         self.mlp = mlp
 
     def forward(self, batch):
-        if 'batch_size' not in batch.keys:
-            batch.batch_size = batch.x.shape[0] #### can improve
+        if 'batch_size' not in batch.keys: #### use batch.keys() in higher version of torch_geom
+            batch.batch_size = batch.x.shape[0]  #### can improve
         batch = edit_batch(batch)
         Cov_i_Ni = self.compute_covariance_vectors(batch.pos, batch.edge_index, batch.edge_attr, batch.batch_size)
         coord_neighbor = self.gather_neighbor_positions(batch.pos, batch.edge_index, batch.edge_attr, batch.batch_size)
         Inv_Cov_Ni_Ni = self.compute_inverse_cov_matrices(coord_neighbor, batch.edge_list)
 
         B_i = torch.matmul(Inv_Cov_Ni_Ni, Cov_i_Ni.unsqueeze(2)).squeeze()
-        F_i = self.theta[0] + self.theta[2] - torch.sum(B_i * Cov_i_Ni, dim = 1)
+        F_i = self.theta[0] + self.theta[2] - torch.sum(B_i * Cov_i_Ni, dim=1)
 
         y_neighbor = self.gather_neighbor_outputs(batch.y, batch.edge_index, batch.edge_attr, batch.batch_size)
-        y_decor = (batch.y[range(batch.batch_size)] - torch.sum(y_neighbor * B_i, dim = 1))/torch.sqrt(F_i)
+        y_decor = (batch.y[range(batch.batch_size)] - torch.sum(y_neighbor * B_i, dim=1)) / torch.sqrt(F_i)
         batch.o = self.mlp(batch.x).squeeze()
         o_neighbor = self.gather_neighbor_outputs(batch.o, batch.edge_index, batch.edge_attr, batch.batch_size)
         o_decor = (batch.o[range(batch.batch_size)] - torch.sum(o_neighbor * B_i, dim=1)) / torch.sqrt(F_i)
         preds = batch.o
 
         return y_decor, o_decor, preds
 
     def estimate(self, X):
         with torch.no_grad():
             return self.mlp(X).squeeze()
 
-    def predict(self, data_train, data_test, CI = False, **kwargs):
+    def predict(self, data_train, data_test, CI=False, **kwargs):
         with torch.no_grad():
             w_train = data_train.y - self.estimate(data_train.x)
             if CI:
                 w_test, w_u, w_l = krig_pred(w_train, data_train.pos, data_test.pos, self.theta, **kwargs)
                 estimation_test = self.estimate(data_test.x)
                 return [estimation_test + w_test, estimation_test + w_u, estimation_test + w_l]
             else:
                 w_test, _, _ = krig_pred(w_train, data_train.pos, data_test.pos, self.theta, **kwargs)
                 estimation_test = self.estimate(data_test.x)
                 return estimation_test + w_test
 
-__all__ = ['nngls']
+
+__all__ = ['nngls']
```

### Comparing `geospann-0.1.1/tests/test.py` & `geospann-0.1.2/tests/test.py`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/LICENSE` & `geospann-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geospann-0.1.1/pyproject.toml` & `geospann-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geospaNN"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Wentao Zhan", email="wzhan3@jhu.edu" },
+    { name="Abhirup Datta", email="abhidatta@jhu.edu" }
 ]
 maintainers = [
     { name="Wentao Zhan", email="wzhan3@jhu.edu" },
 ]
 description = "A PyThon implementation of NNGLS"
 readme = "README.md"
 requires-python = ">=3.9"
@@ -23,18 +24,18 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Mathematics",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    'torch==2.0.0',
-    'torch_scatter>=2.1.0',
-    'torch_sparse>=0.6.0',
-    'torch_geometric==2.3.0',
     'numpy', 'scipy', 'scikit-learn',
+    'torch>=2.0.0',
+    'torch_sparse>=0.6.18',
+    'torch_scatter>=2.1.2',
+    'torch_geometric>=2.3.0'
 ]
 
 [project.urls]
 Homepage = "https://github.com/WentaoZhan1998/NN-GLS"
 Repository = "https://github.com/WentaoZhan1998/NN-GLS.git"
 Issues = "https://github.com/WentaoZhan1998/NN-GLS/issues"
```

