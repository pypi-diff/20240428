# Comparing `tmp/modgeosys_graph_algorithms-0.3.3.tar.gz` & `tmp/modgeosys_graph_algorithms-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modgeosys_graph_algorithms-0.3.3.tar", max compression
+gzip compressed data, was "modgeosys_graph_algorithms-0.3.9.tar", max compression
```

## Comparing `modgeosys_graph_algorithms-0.3.3.tar` & `modgeosys_graph_algorithms-0.3.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     3600 2024-04-25 00:49:12.244578 modgeosys_graph_algorithms-0.3.3/README.md
--rw-r--r--   0        0        0      489 2024-04-25 02:25:20.098921 modgeosys_graph_algorithms-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.3.3/src/modgeosys/__init__.py
--rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.3.3/src/modgeosys/graph/__init__.py
--rw-r--r--   0        0        0     3238 2024-04-24 20:58:48.758144 modgeosys_graph_algorithms-0.3.3/src/modgeosys/graph/a_star.py
--rw-r--r--   0        0        0      635 2024-04-02 16:41:14.666923 modgeosys_graph_algorithms-0.3.3/src/modgeosys/graph/distance.py
--rw-r--r--   0        0        0      176 2024-04-03 04:46:47.958690 modgeosys_graph_algorithms-0.3.3/src/modgeosys/graph/edge_validation.py
--rw-r--r--   0        0        0     1696 2024-04-06 19:04:49.983022 modgeosys_graph_algorithms-0.3.3/src/modgeosys/graph/prim.py
--rw-r--r--   0        0        0     7879 2024-04-25 02:24:01.442738 modgeosys_graph_algorithms-0.3.3/src/modgeosys/graph/types.py
--rw-r--r--   0        0        0     4687 2024-04-25 02:11:54.677048 modgeosys_graph_algorithms-0.3.3/tests/modgeosys/graph/conftest.py
--rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.3.3/tests/modgeosys/graph/generate_a_star_test_data.py
--rw-r--r--   0        0        0     8358 2024-04-25 02:14:09.417361 modgeosys_graph_algorithms-0.3.3/tests/modgeosys/graph/test_a_star.py
--rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.3.3/tests/modgeosys/graph/test_distance.py
--rw-r--r--   0        0        0    24076 2024-04-25 02:16:07.069635 modgeosys_graph_algorithms-0.3.3/tests/modgeosys/graph/test_prim.py
--rw-r--r--   0        0        0     3791 2024-04-25 02:12:47.325170 modgeosys_graph_algorithms-0.3.3/tests/modgeosys/graph/test_types.py
--rw-r--r--   0        0        0     3985 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     4224 2024-04-28 17:48:48.450848 modgeosys_graph_algorithms-0.3.9/README.md
+-rw-r--r--   0        0        0      489 2024-04-28 17:51:56.303357 modgeosys_graph_algorithms-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.3.9/src/modgeosys/__init__.py
+-rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/__init__.py
+-rw-r--r--   0        0        0     3229 2024-04-28 04:37:43.782725 modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/a_star.py
+-rw-r--r--   0        0        0      625 2024-04-28 04:54:23.937487 modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/distance.py
+-rw-r--r--   0        0        0      177 2024-04-28 17:43:46.457872 modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/edge_validation.py
+-rw-r--r--   0        0        0      418 2024-04-28 05:11:58.328061 modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/edge_weight.py
+-rw-r--r--   0        0        0     1696 2024-04-06 19:04:49.983022 modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/prim.py
+-rw-r--r--   0        0        0     7804 2024-04-28 17:47:33.322604 modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/types.py
+-rw-r--r--   0        0        0     4767 2024-04-28 16:28:12.634644 modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/conftest.py
+-rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/generate_a_star_test_data.py
+-rw-r--r--   0        0        0     8358 2024-04-27 21:40:29.497540 modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_a_star.py
+-rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_distance.py
+-rw-r--r--   0        0        0    24076 2024-04-27 21:40:29.505540 modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_prim.py
+-rw-r--r--   0        0        0     3795 2024-04-28 04:46:03.711552 modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_types.py
+-rw-r--r--   0        0        0     4609 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.3.9/PKG-INFO
```

### Comparing `modgeosys_graph_algorithms-0.3.3/README.md` & `modgeosys_graph_algorithms-0.3.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# modgeosys-graph-algorithms: Graph Algorithms
+# modgeosys-graph-algorithms: Spatial Graph Algorithms
 
-A repository for [hopefully] clean, readable, and easily-called implementations of some navigation,
+A repository for [hopefully] clean, readable, and easily-called implementations of some spatial navigation,
 path planning, and obstacle avoidance algorithms I will be using in the near future, written in modern
 Python and/or Rust with Python bindings. I'll be adding more algorithm implementations over time.
 
 ## Algorithms: Currently implemented + planned
 * [A*](https://en.wikipedia.org/wiki/A*_search_algorithm) - Graph path search algorithm.
   * Code-complete in both Python and Rust.
   * Needs a more thorough test suite.
@@ -19,57 +19,60 @@
 
 ### A\*
 
 ```python
 import pickle
 from pprint import pprint
 
-from modgeosys.graph.types import Graph, length_cost_per_unit
+from modgeosys.graph.edge_weight import length_cost_per_unit
+from modgeosys.graph.types import Graph, COMPUTED_WEIGHT
 from modgeosys.graph.distance import manhattan_distance, euclidean_distance
 from modgeosys.graph.a_star import a_star
 
 # Define a toy graph.
-toy_graph = Graph.from_edge_definitions(edge_definitions=((((0.0, 0.0), (0.0, 2.0)), 2, {'cost_per_unit': 2}),
-                                                          (((0.0, 0.0), (1.0, 0.0)), 1, {'cost_per_unit': 1}),
-                                                          (((1.0, 0.0), (2.0, 1.0)), 2, {'cost_per_unit': 1}),
-                                                          (((0.0, 2.0), (2.0, 3.0)), 3, {'cost_per_unit': 3}),
-                                                          (((2.0, 1.0), (2.0, 3.0)), 2, {'cost_per_unit': 1})),
-                                        edge_weight_function=length_cost_per_unit,
-                                        heuristic_distance_function=manhattan_distance)
+toy_graph = Graph.from_edge_definitions(edge_definitions=((((0.0, 0.0), (0.0, 2.0)), COMPUTED_WEIGHT, {'cost_per_unit': 2}),
+                                                          (((0.0, 0.0), (1.0, 0.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1}),
+                                                          (((1.0, 0.0), (2.0, 1.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1}),
+                                                          (((0.0, 2.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 3}),
+                                                          (((2.0, 1.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1})),
+                                        distance_function=manhattan_distance, edge_weight_function=length_cost_per_unit)
 
 # Load a bigger graph from a pickle file.
 with open('python/data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
-    larger_graph = pickle.load(pickled_sample_larger_graph_file)
-    larger_graph.heuristic_distance_function = manhattan_distance
-    larger_graph.edge_weight_function = length_cost_per_unit
+  larger_graph = pickle.load(pickled_sample_larger_graph_file)
+  larger_graph.heuristic_distance_function = manhattan_distance
+  larger_graph.edge_weight_function = length_cost_per_unit
 
 # Call the A* function.
 toy_a_star_path = a_star(graph=toy_graph, start_node_index=0, goal_node_index=4)
-print(f'Toy A* Path:')
+print('Toy A* Path:')
 pprint(toy_a_star_path)
 print()
 larger_a_star_path = a_star(graph=larger_graph, start_node_index=0, goal_node_index=4)
-print(f'Large A* Path:')
+print('Large A* Path:')
 pprint(larger_a_star_path)
 ```
 
 ### Prim's algorithm
 
 ```python
 import pickle
 
-from modgeosys.graph.types import Graph
+from modgeosys.graph.edge_weight import length_cost_per_unit
+from modgeosys.graph.types import Graph, COMPUTED_WEIGHT
+from modgeosys.graph.distance import manhattan_distance, euclidean_distance
 from modgeosys.graph.prim import prim
 
 # Define a toy graph.
-toy_graph = Graph.from_edge_definitions(((2, ((0.0, 0.0), (0.0, 2.0))),
-                                         (1, ((0.0, 0.0), (1.0, 0.0))),
-                                         (1, ((1.0, 0.0), (2.0, 1.0))),
-                                         (3, ((0.0, 2.0), (2.0, 3.0))),
-                                         (1, ((2.0, 1.0), (2.0, 3.0)))))
+toy_graph = Graph.from_edge_definitions(edge_definitions=((((0.0, 0.0), (0.0, 2.0)), COMPUTED_WEIGHT, {'cost_per_unit': 2}),
+                                                          (((0.0, 0.0), (1.0, 0.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1}),
+                                                          (((1.0, 0.0), (2.0, 1.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1}),
+                                                          (((0.0, 2.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 3}),
+                                                          (((2.0, 1.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1})),
+                                        distance_function=manhattan_distance, edge_weight_function=length_cost_per_unit)
 
 # Load a bigger graph from a pickle file.
 with open('python/data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
   larger_graph = pickle.load(pickled_sample_larger_graph_file)
 
 # Call the Prim function.
 toy_minimum_spanning_tree = prim(graph=toy_graph, start_node_index=0)
```

### Comparing `modgeosys_graph_algorithms-0.3.3/src/modgeosys/graph/a_star.py` & `modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/a_star.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """A module containing an implementation of the A* algorithm for finding the shortest path between two nodes in a graph."""
 
 from collections.abc import Mapping
 from dataclasses import dataclass
 
 from heapdict import heapdict
 
-from modgeosys.graph.types import Edge, Graph, HeuristicDistanceCallable, NoNavigablePathError
+from modgeosys.graph.types import Edge, Graph, DistanceCallable, NoNavigablePathError
 
 
 @dataclass(order=True)
 class Hop:
     """A wrapper for an edge that includes the f() function, and the g and h values to support A*."""
     edge: Edge
     g: int | float
```

### Comparing `modgeosys_graph_algorithms-0.3.3/src/modgeosys/graph/distance.py` & `modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/distance.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Heuristic distance functions."""
+"""Distance functions."""
 
 import numpy as np
 
 from modgeosys.graph.types import Node
 
 
 def manhattan_distance(a: Node, b: Node) -> int | float:
```

### Comparing `modgeosys_graph_algorithms-0.3.3/src/modgeosys/graph/prim.py` & `modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.3/src/modgeosys/graph/types.py` & `modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """Simple and complex data types for the graph module."""
 
 import bisect
 from collections.abc import Callable, Mapping, Sequence
 from copy import deepcopy
 from dataclasses import dataclass, field
 from typing import Annotated, Literal, TypeVar
-
 import numpy as np
 import numpy.typing as npt
 
 
 NDType = TypeVar("NDType", bound=np.generic)
 Vector = Annotated[npt.NDArray[NDType], Literal["N", 1]]
 
 type NodeSequence = Sequence[Node]
 type EdgeSequence = Sequence[Edge]
-type EdgeDefinitionSequence = Sequence[tuple[tuple, tuple], int | float | None, dict]
+type EdgeDefinition = tuple[tuple, int | float | None, dict]
+type EdgeDefinitionSequence = Sequence[EdgeDefinition]
 type AdjacencyMap = Mapping[Node, Sequence[Edge]]
-type HeuristicDistanceCallable = Callable[[Node, Node], int | float]
+type DistanceCallable = Callable[[Node, Node], int | float]
 type ValidEdgeCallable = Callable[[Edge], bool]
 type EdgeWeightCallable = Callable[Graph, Edge]
 
 
+COMPUTED_WEIGHT = None
+
+
 @dataclass
 class Node:
     """A node in a graph."""
     coordinates: Vector[np.float64]
     properties: dict = field(default_factory=dict)
 
     def __post_init__(self):
@@ -110,54 +113,55 @@
 
 class Graph:
     """A graph."""
     nodes: NodeSequence = field(default_factory=list)
     edges: EdgeSequence = field(default_factory=tuple)
     properties: dict = field(default_factory=dict)
     edge_weight_function: EdgeWeightCallable | None
-    heuristic_distance_function: HeuristicDistanceCallable | None
+    heuristic_distance_function: DistanceCallable | None
 
     @classmethod
-    def from_edge_definitions(cls, edge_definitions: EdgeDefinitionSequence, properties: dict | None = None, edge_weight_function: EdgeWeightCallable | None = None, heuristic_distance_function: HeuristicDistanceCallable | None = None) -> 'Graph':
+    def from_edge_definitions(cls, edge_definitions: EdgeDefinitionSequence, properties: dict | None = None, distance_function: DistanceCallable | None = None, edge_weight_function: EdgeWeightCallable | None = None) -> 'Graph':
+        """Create a graph from a sequence of edge definitions."""
         coordinates_of_all_nodes = []
 
         for edge_definition in edge_definitions:
             for edge_node_coordinates in edge_definition[0]:
                 if edge_node_coordinates not in coordinates_of_all_nodes:
                     coordinates_of_all_nodes.append(edge_node_coordinates)
 
-        nodes = dict()
+        nodes = {}
         edges = []
 
         for edge_definition in edge_definitions:
             indices = []
             for edge_node_coordinates in edge_definition[0]:
                 index = coordinates_of_all_nodes.index(edge_node_coordinates)
                 indices.append(index)
                 nodes[index] = Node(coordinates=edge_node_coordinates)
             node_indices = frozenset(indices)
             edge = Edge(weight=edge_definition[1], node_indices=node_indices, properties=edge_definition[2])
             edges.append(edge)
 
         nodes = [nodes[index] for index in sorted(nodes)]
 
-        return cls(nodes=nodes, edges=edges, properties=properties, edge_weight_function=edge_weight_function, heuristic_distance_function=heuristic_distance_function)
+        return cls(nodes=nodes, edges=edges, properties=properties, edge_weight_function=edge_weight_function, heuristic_distance_function=distance_function)
 
-    def __init__(self, nodes: NodeSequence, edges: EdgeSequence, properties: dict | None = None, edge_weight_function: EdgeWeightCallable | None = None, heuristic_distance_function: HeuristicDistanceCallable | None = None):
+    def __init__(self, nodes: NodeSequence, edges: EdgeSequence, properties: dict | None = None, edge_weight_function: EdgeWeightCallable | None = None, heuristic_distance_function: DistanceCallable | None = None):
         """Initialize a graph."""
         self.nodes = deepcopy(nodes)
         self.edges = tuple(deepcopy(edge) for edge in edges)
         self.properties = {} if properties is None else (deepcopy(properties) if isinstance(properties, dict) else dict(properties))
         self.heuristic_distance_function = heuristic_distance_function if heuristic_distance_function else None
         if edge_weight_function:
             self.edge_weight_function = edge_weight_function
             for edge in self.edges:
                 edge.weight = self.edge_weight_function(self, edge)
         else:
-            self.edge_weight_function = None
+            self.edge_weight_function = specified_edge_weight
 
     def __repr__(self):
         return f'Graph(nodes={self.nodes}, edges={self.edges})'
 
     def __str__(self):
         return f'Graph containing these nodes: {self.nodes} and these edges: {self.edges})'
 
@@ -186,19 +190,16 @@
         for edge in self.edges:
             node_indices = list(edge.node_indices)
             adjacency_matrix[node_indices[0], node_indices[1]] = adjacency_matrix[node_indices[1], node_indices[0]] = edge.weight
 
         return adjacency_matrix
 
 
-
-def length_cost_per_unit(graph: Graph, edge: Edge) -> float:
-    cost_per_unit = edge.properties['cost_per_unit']
-    heuristic_distance = graph.heuristic_distance_function
-    attached_nodes = [graph.nodes[node_index] for node_index in edge.node_indices]
-    return cost_per_unit * heuristic_distance(attached_nodes[0], attached_nodes[1])
+def specified_edge_weight(_graph: Graph, edge: Edge) -> float:
+    """As the default edge weight function, return the current value of the edge's weight property."""
+    return edge.weight
 
 
 class NoNavigablePathError(Exception):
     """Raised when no path can be found to the goal node."""
     def __init__(self, start_node: Node, goal_node: Node='N/A'):
         super().__init__(f'No path exists between nodes {start_node} and {goal_node}.')
```

### Comparing `modgeosys_graph_algorithms-0.3.3/tests/modgeosys/graph/conftest.py` & `modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pickle
 import pytest
 
+from src.modgeosys.graph.edge_weight import length_cost_per_unit
 from src.modgeosys.graph.distance import manhattan_distance
-from src.modgeosys.graph.types import Node, Edge, Graph, length_cost_per_unit
+from src.modgeosys.graph.types import Node, Edge, Graph, COMPUTED_WEIGHT
 
 
 @pytest.fixture
 def valid_nodes():
     return [Node(properties={}, coordinates=(0.0, 0.0)), Node(properties={}, coordinates=(0.0, 2.0)), Node(properties={}, coordinates=(1.0, 0.0)), Node(properties={}, coordinates=(2.0, 1.0)), Node(properties={}, coordinates=(2.0, 3.0))]
 
 
@@ -68,21 +69,20 @@
 @pytest.fixture
 def valid_graph3(valid_nodes, valid_edges3):
     return Graph(properties={}, nodes=valid_nodes, edges=valid_edges3, heuristic_distance_function=manhattan_distance, edge_weight_function=length_cost_per_unit)
 
 
 @pytest.fixture
 def valid_graph_from_edge_definitions():
-    return Graph.from_edge_definitions(edge_definitions=((((0.0, 0.0), (0.0, 2.0)), 2, {'cost_per_unit': 2}),
-                                                         (((0.0, 0.0), (1.0, 0.0)), 1, {'cost_per_unit': 1}),
-                                                         (((1.0, 0.0), (2.0, 1.0)), 2, {'cost_per_unit': 1}),
-                                                         (((0.0, 2.0), (2.0, 3.0)), 3, {'cost_per_unit': 3}),
-                                                         (((2.0, 1.0), (2.0, 3.0)), 2, {'cost_per_unit': 1})),
-                                        edge_weight_function=length_cost_per_unit,
-                                       heuristic_distance_function=manhattan_distance)
+    return Graph.from_edge_definitions(edge_definitions=((((0.0, 0.0), (0.0, 2.0)), COMPUTED_WEIGHT, {'cost_per_unit': 2}),
+                                                         (((0.0, 0.0), (1.0, 0.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1}),
+                                                         (((1.0, 0.0), (2.0, 1.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1}),
+                                                         (((0.0, 2.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 3}),
+                                                         (((2.0, 1.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1})),
+                                       distance_function=manhattan_distance, edge_weight_function=length_cost_per_unit)
 
 
 @pytest.fixture
 def valid_graph_larger():
     with open('data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
         graph = pickle.load(pickled_sample_larger_graph_file)
         graph.heuristic_distance_function = manhattan_distance
```

### Comparing `modgeosys_graph_algorithms-0.3.3/tests/modgeosys/graph/generate_a_star_test_data.py` & `modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/generate_a_star_test_data.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.3/tests/modgeosys/graph/test_a_star.py` & `modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_a_star.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.3/tests/modgeosys/graph/test_distance.py` & `modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.3/tests/modgeosys/graph/test_prim.py` & `modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.3/tests/modgeosys/graph/test_types.py` & `modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 
 def test_graph_creation(valid_nodes, valid_edges1, valid_graph1):
     assert valid_graph1.nodes == valid_nodes
     assert valid_graph1.edges == valid_edges1
     assert valid_graph1.properties == {}
     assert valid_graph1.heuristic_distance_function is not None
-    assert valid_graph1.edge_weight_function is None
+    assert valid_graph1.edge_weight_function is not None
 
 
 def test_graph_creation_with_edge_weight_function(valid_nodes, valid_edges3_with_computed_weights, valid_graph3):
     assert valid_graph3.nodes == valid_nodes
     assert valid_graph3.edges == valid_edges3_with_computed_weights
     assert valid_graph3.properties == {}
     assert valid_graph3.heuristic_distance_function is not None
```

### Comparing `modgeosys_graph_algorithms-0.3.3/PKG-INFO` & `modgeosys_graph_algorithms-0.3.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: modgeosys-graph-algorithms
-Version: 0.3.3
+Version: 0.3.9
 Summary: 
 Author: Kevin Weller
 Author-email: klweller@icloud.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: heapdict (>=1.0.1,<2.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Description-Content-Type: text/markdown
 
-# modgeosys-graph-algorithms: Graph Algorithms
+# modgeosys-graph-algorithms: Spatial Graph Algorithms
 
-A repository for [hopefully] clean, readable, and easily-called implementations of some navigation,
+A repository for [hopefully] clean, readable, and easily-called implementations of some spatial navigation,
 path planning, and obstacle avoidance algorithms I will be using in the near future, written in modern
 Python and/or Rust with Python bindings. I'll be adding more algorithm implementations over time.
 
 ## Algorithms: Currently implemented + planned
 * [A*](https://en.wikipedia.org/wiki/A*_search_algorithm) - Graph path search algorithm.
   * Code-complete in both Python and Rust.
   * Needs a more thorough test suite.
@@ -32,57 +32,60 @@
 
 ### A\*
 
 ```python
 import pickle
 from pprint import pprint
 
-from modgeosys.graph.types import Graph, length_cost_per_unit
+from modgeosys.graph.edge_weight import length_cost_per_unit
+from modgeosys.graph.types import Graph, COMPUTED_WEIGHT
 from modgeosys.graph.distance import manhattan_distance, euclidean_distance
 from modgeosys.graph.a_star import a_star
 
 # Define a toy graph.
-toy_graph = Graph.from_edge_definitions(edge_definitions=((((0.0, 0.0), (0.0, 2.0)), 2, {'cost_per_unit': 2}),
-                                                          (((0.0, 0.0), (1.0, 0.0)), 1, {'cost_per_unit': 1}),
-                                                          (((1.0, 0.0), (2.0, 1.0)), 2, {'cost_per_unit': 1}),
-                                                          (((0.0, 2.0), (2.0, 3.0)), 3, {'cost_per_unit': 3}),
-                                                          (((2.0, 1.0), (2.0, 3.0)), 2, {'cost_per_unit': 1})),
-                                        edge_weight_function=length_cost_per_unit,
-                                        heuristic_distance_function=manhattan_distance)
+toy_graph = Graph.from_edge_definitions(edge_definitions=((((0.0, 0.0), (0.0, 2.0)), COMPUTED_WEIGHT, {'cost_per_unit': 2}),
+                                                          (((0.0, 0.0), (1.0, 0.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1}),
+                                                          (((1.0, 0.0), (2.0, 1.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1}),
+                                                          (((0.0, 2.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 3}),
+                                                          (((2.0, 1.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1})),
+                                        distance_function=manhattan_distance, edge_weight_function=length_cost_per_unit)
 
 # Load a bigger graph from a pickle file.
 with open('python/data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
-    larger_graph = pickle.load(pickled_sample_larger_graph_file)
-    larger_graph.heuristic_distance_function = manhattan_distance
-    larger_graph.edge_weight_function = length_cost_per_unit
+  larger_graph = pickle.load(pickled_sample_larger_graph_file)
+  larger_graph.heuristic_distance_function = manhattan_distance
+  larger_graph.edge_weight_function = length_cost_per_unit
 
 # Call the A* function.
 toy_a_star_path = a_star(graph=toy_graph, start_node_index=0, goal_node_index=4)
-print(f'Toy A* Path:')
+print('Toy A* Path:')
 pprint(toy_a_star_path)
 print()
 larger_a_star_path = a_star(graph=larger_graph, start_node_index=0, goal_node_index=4)
-print(f'Large A* Path:')
+print('Large A* Path:')
 pprint(larger_a_star_path)
 ```
 
 ### Prim's algorithm
 
 ```python
 import pickle
 
-from modgeosys.graph.types import Graph
+from modgeosys.graph.edge_weight import length_cost_per_unit
+from modgeosys.graph.types import Graph, COMPUTED_WEIGHT
+from modgeosys.graph.distance import manhattan_distance, euclidean_distance
 from modgeosys.graph.prim import prim
 
 # Define a toy graph.
-toy_graph = Graph.from_edge_definitions(((2, ((0.0, 0.0), (0.0, 2.0))),
-                                         (1, ((0.0, 0.0), (1.0, 0.0))),
-                                         (1, ((1.0, 0.0), (2.0, 1.0))),
-                                         (3, ((0.0, 2.0), (2.0, 3.0))),
-                                         (1, ((2.0, 1.0), (2.0, 3.0)))))
+toy_graph = Graph.from_edge_definitions(edge_definitions=((((0.0, 0.0), (0.0, 2.0)), COMPUTED_WEIGHT, {'cost_per_unit': 2}),
+                                                          (((0.0, 0.0), (1.0, 0.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1}),
+                                                          (((1.0, 0.0), (2.0, 1.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1}),
+                                                          (((0.0, 2.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 3}),
+                                                          (((2.0, 1.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1})),
+                                        distance_function=manhattan_distance, edge_weight_function=length_cost_per_unit)
 
 # Load a bigger graph from a pickle file.
 with open('python/data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
   larger_graph = pickle.load(pickled_sample_larger_graph_file)
 
 # Call the Prim function.
 toy_minimum_spanning_tree = prim(graph=toy_graph, start_node_index=0)
```

