# Comparing `tmp/json_criteria-0.1.2.tar.gz` & `tmp/json_criteria-0.2.0.tar.gz`

## Comparing `json_criteria-0.1.2.tar` & `json_criteria-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 json_criteria-0.1.2/.vscode/settings.json
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 json_criteria-0.1.2/examples/nested_mult_conds.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 json_criteria-0.1.2/examples/simple_one_cond.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 json_criteria-0.1.2/src/json_criteria/__init__.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 json_criteria-0.1.2/src/json_criteria/all_meet_criteria.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 json_criteria-0.1.2/src/json_criteria/any_meet_criteria.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 json_criteria-0.1.2/src/json_criteria/apply_using_criteria.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 json_criteria-0.1.2/src/json_criteria/combine_criteria.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 json_criteria-0.1.2/src/json_criteria/filter_using_criteria.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 json_criteria-0.1.2/src/json_criteria/find_using_criteria.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 json_criteria-0.1.2/src/json_criteria/get_all_criteria.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 json_criteria-0.1.2/src/json_criteria/meets_criteria.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 json_criteria-0.1.2/src/json_criteria/internal/__init__.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 json_criteria-0.1.2/src/json_criteria/internal/compare.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 json_criteria-0.1.2/src/json_criteria/internal/meets_crit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 json_criteria-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 json_criteria-0.1.2/tests/test_all_meet_criteria.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 json_criteria-0.1.2/tests/test_any_meet_criteria.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 json_criteria-0.1.2/tests/test_apply_using_criteria.py
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 json_criteria-0.1.2/tests/test_combine_criteria.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 json_criteria-0.1.2/tests/test_filter_using_criteria.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 json_criteria-0.1.2/tests/test_find_using_criteria.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 json_criteria-0.1.2/tests/test_get_all_criteria.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 json_criteria-0.1.2/tests/test_meets_criteria.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 json_criteria-0.1.2/tests/internal/__init__.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 json_criteria-0.1.2/tests/internal/test_compare.py
--rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 json_criteria-0.1.2/tests/internal/test_meets_crit.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 json_criteria-0.1.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 json_criteria-0.1.2/LICENSE
--rw-r--r--   0        0        0    14704 2020-02-02 00:00:00.000000 json_criteria-0.1.2/README.md
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 json_criteria-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    15567 2020-02-02 00:00:00.000000 json_criteria-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 json_criteria-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 json_criteria-0.2.0/examples/nested_mult_conds.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 json_criteria-0.2.0/examples/simple_custom_op.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 json_criteria-0.2.0/examples/simple_one_cond.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 json_criteria-0.2.0/src/json_criteria/__init__.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 json_criteria-0.2.0/src/json_criteria/all_meet_criteria.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 json_criteria-0.2.0/src/json_criteria/any_meet_criteria.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 json_criteria-0.2.0/src/json_criteria/apply_using_criteria.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 json_criteria-0.2.0/src/json_criteria/combine_criteria.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 json_criteria-0.2.0/src/json_criteria/config.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 json_criteria-0.2.0/src/json_criteria/filter_using_criteria.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 json_criteria-0.2.0/src/json_criteria/find_using_criteria.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 json_criteria-0.2.0/src/json_criteria/get_all_criteria.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 json_criteria-0.2.0/src/json_criteria/meets_criteria.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 json_criteria-0.2.0/src/json_criteria/internal/__init__.py
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 json_criteria-0.2.0/src/json_criteria/internal/compare.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 json_criteria-0.2.0/src/json_criteria/internal/meets_crit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 json_criteria-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 json_criteria-0.2.0/tests/test_all_meet_criteria.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 json_criteria-0.2.0/tests/test_any_meet_criteria.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 json_criteria-0.2.0/tests/test_apply_using_criteria.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 json_criteria-0.2.0/tests/test_combine_criteria.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 json_criteria-0.2.0/tests/test_filter_using_criteria.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 json_criteria-0.2.0/tests/test_find_using_criteria.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 json_criteria-0.2.0/tests/test_get_all_criteria.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 json_criteria-0.2.0/tests/test_meets_criteria.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 json_criteria-0.2.0/tests/internal/__init__.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 json_criteria-0.2.0/tests/internal/test_compare.py
+-rw-r--r--   0        0        0    10315 2020-02-02 00:00:00.000000 json_criteria-0.2.0/tests/internal/test_meets_crit.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 json_criteria-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 json_criteria-0.2.0/LICENSE
+-rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 json_criteria-0.2.0/README.md
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 json_criteria-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    16977 2020-02-02 00:00:00.000000 json_criteria-0.2.0/PKG-INFO
```

### Comparing `json_criteria-0.1.2/src/json_criteria/all_meet_criteria.py` & `json_criteria-0.2.0/src/json_criteria/filter_using_criteria.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-from typing import Dict, Any, List
+from typing import Dict, Any, List, Optional
 from .internal import meets_crit
+from .config import Config
 
-def all_meet_criteria(records: List[Dict[str, Any]], criteria: Dict[str, Any]) -> bool:
+def filter_using_criteria(
+    records: List[Dict[str, Any]],
+    criteria: Dict[str, Any],
+    config: Optional[Config] = None
+) -> List[Dict[str, Any]]:
     """
-    Determine if all of the records meet the given criteria.
+    Filter a list of records using the given criteria.
 
     Parameters:
     - records (List[Dict[str, Any]]): The data records.
-    - criteria (Dict[str, Any]): The criteria. Should be a dictionary representing the conditions that the record must satisfy. May include nested conditions.
-
+    - criteria (Dict[str, Any]): The criteria.
+      Should be a dictionary representing the conditions
+      that the record must satisfy. May include nested conditions.
+    - config (Optional[Config]): Configuration options.
+    
     Returns:
-    - bool: Whether all of the records meet the criteria.
+    - List[Dict[str, Any]]: The filtered records that meet the criteria.
     """
-    return all(meets_crit(record, criteria) for record in records)
+    return [record for record in records if meets_crit(record, criteria, config)]
```

### Comparing `json_criteria-0.1.2/src/json_criteria/any_meet_criteria.py` & `json_criteria-0.2.0/src/json_criteria/any_meet_criteria.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-from typing import Dict, Any, List
+from typing import Dict, Any, List, Optional
 from .internal import meets_crit
+from .config import Config
 
-def any_meet_criteria(records: List[Dict[str, Any]], criteria: Dict[str, Any]) -> bool:
+def any_meet_criteria(
+    records: List[Dict[str, Any]],
+    criteria: Dict[str, Any],
+    config: Optional[Config] = None
+) -> bool:
     """
     Determine if any of the records meet the given criteria.
 
     Parameters:
     - records (List[Dict[str, Any]]): The data records.
-    - criteria (Dict[str, Any]): The criteria. Should be a dictionary representing the conditions that the record must satisfy. May include nested conditions.
-
+    - criteria (Dict[str, Any]): The criteria.
+      Should be a dictionary representing the conditions
+      that the record must satisfy. May include nested conditions.
+    - config (Optional[Config]): Configuration options.
+    
     Returns:
     - bool: Whether any of the records meet the criteria.
     """
-    return any(meets_crit(record, criteria) for record in records)
+    return any(meets_crit(record, criteria, config) for record in records)
```

### Comparing `json_criteria-0.1.2/src/json_criteria/apply_using_criteria.py` & `json_criteria-0.2.0/src/json_criteria/apply_using_criteria.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-from typing import Dict, Any, List, Callable
+from typing import Dict, Any, List, Callable, Optional
 from .internal import meets_crit
+from .config import Config
 
 def apply_using_criteria(
     records: List[Dict[str, Any]],
     criteria: Dict[str, Any],
-    func: Callable[[Dict[str, Any]], Dict[str, Any]]
+    func: Callable[[Dict[str, Any]], Dict[str, Any]],
+    config: Optional[Config] = None
 ) -> List[Dict[str, Any]]:
     """
     Apply a specified function to each record that meets the given criteria.
 
     Parameters:
     - records (List[Dict[str, Any]]): The data records.
-    - criteria (Dict[str, Any]): The criteria. Should be a dictionary representing the conditions that the record must satisfy. May include nested conditions.
+    - criteria (Dict[str, Any]): The criteria.
+      Should be a dictionary representing the conditions
+      that the record must satisfy. May include nested conditions.
     - func (Callable): Function to apply to records that meet the criteria.
-
+    - config (Optional[Config]): Configuration options.
+    
     Returns:
     - list: List of records with the specified function applied.
     """
     result_records = []
     for record in records:
-        if meets_crit(record, criteria):
+        if meets_crit(record, criteria, config):
             result_records.append(func(record))
         else:
             result_records.append(record)
     return result_records
```

### Comparing `json_criteria-0.1.2/src/json_criteria/combine_criteria.py` & `json_criteria-0.2.0/src/json_criteria/combine_criteria.py`

 * *Files identical despite different names*

### Comparing `json_criteria-0.1.2/src/json_criteria/filter_using_criteria.py` & `json_criteria-0.2.0/src/json_criteria/all_meet_criteria.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-from typing import Dict, Any, List
+from typing import Dict, Any, List, Optional
 from .internal import meets_crit
+from .config import Config
 
-def filter_using_criteria(
+def all_meet_criteria(
     records: List[Dict[str, Any]],
-    criteria: Dict[str, Any]
-) -> List[Dict[str, Any]]:
+    criteria: Dict[str, Any],
+    config: Optional[Config] = None
+) -> bool:
     """
-    Filter a list of records using the given criteria.
+    Determine if all of the records meet the given criteria.
 
     Parameters:
     - records (List[Dict[str, Any]]): The data records.
-    - criteria (Dict[str, Any]): The criteria. Should be a dictionary representing the conditions that the record must satisfy. May include nested conditions.
-
+    - criteria (Dict[str, Any]): The criteria.
+      Should be a dictionary representing the conditions
+      that the record must satisfy. May include nested conditions.
+    - config (Optional[Config]): Configuration options.
+    
     Returns:
-    - List[Dict[str, Any]]: The filtered records that meet the criteria.
+    - bool: Whether all of the records meet the criteria.
     """
-    return [record for record in records if meets_crit(record, criteria)]
+    return all(meets_crit(record, criteria, config) for record in records)
```

### Comparing `json_criteria-0.1.2/src/json_criteria/find_using_criteria.py` & `json_criteria-0.2.0/src/json_criteria/find_using_criteria.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-from typing import Dict, Any, List
+from typing import Dict, Any, List, Optional
 from .internal import meets_crit
+from .config import Config
 
 def find_using_criteria(
     records: List[Dict[str, Any]],
-    criteria: Dict[str, Any]
+    criteria: Dict[str, Any],
+    config: Optional[Config] = None
 ) -> Dict[str, Any] | None:
     """
     Find the first record that meets the given criteria. Returns `None` if none found.
 
     Parameters:
     - records (List[Dict[str, Any]]): The data records.
-    - criteria (Dict[str, Any]): The criteria. Should be a dictionary representing the conditions that the record must satisfy. May include nested conditions.
-
+    - criteria (Dict[str, Any]): The criteria.
+      Should be a dictionary representing the conditions
+      that the record must satisfy. May include nested conditions.
+    - config (Optional[Config]): Configuration options.
+    
     Returns:
     - Dict[str, Any] | None: The first record that meets the criteria, otherwise None.
     """
-    return next((record for record in records if meets_crit(record, criteria)), None)
+    return next((record for record in records if meets_crit(record, criteria, config)), None)
```

### Comparing `json_criteria-0.1.2/src/json_criteria/internal/compare.py` & `json_criteria-0.2.0/src/json_criteria/internal/compare.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Any
+from typing import Any, Optional
 import re
+from ..config import Config
 
 def compare_equal_to(record_value: Any, value: Any) -> bool:
     """Check if the record value is equal to the specified value."""
     return record_value == value
 
 def compare_not_equal_to(record_value: Any, value: Any) -> bool:
     """Check if the record value is not equal to the specified value."""
@@ -75,24 +76,29 @@
     'starts_with': compare_starts_with,
     'not_starts_with': compare_not_starts_with,
     'ends_with': compare_ends_with,
     'not_ends_with': compare_not_ends_with,
     'matches_regex': compare_matches_regex
 }
 
-def compare(record_value: Any, operator: str, value: Any) -> bool:
+def compare(record_value: Any, operator: str, value: Any, config: Optional[Config] = None) -> bool:
     """
     Compare record value with the specified value using the given operator.
 
     Parameters:
     - record_value (Any): The value from the data record.
     - operator (str): The comparison operator.
     - value (Any): The value to compare against.
+    - config (Config): Configuration options.
 
     Returns:
     - bool: The result of the comparison.
     """
 
     if operator in operator_functions:
         return operator_functions[operator](record_value, value)
 
+    # Check for Custom operators
+    if config and operator in config.custom_ops:
+        return bool(config.custom_ops[operator](record_value, value))
+
     raise ValueError(f"Unsupported operator: {operator}")
```

### Comparing `json_criteria-0.1.2/src/json_criteria/internal/meets_crit.py` & `json_criteria-0.2.0/src/json_criteria/internal/meets_crit.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,41 @@
-from typing import Dict, Any
+from typing import Dict, Any, Optional
 from .compare import compare
+from ..config import Config
 
-def meets_crit(record: Dict[str, Any], element: Dict[str, Any]) -> bool:
+def meets_crit(
+    record: Dict[str, Any],
+    element: Dict[str, Any],
+    config: Optional[Config] = None
+) -> bool:
     """
     Internal function to check if a record meets the given criteria.
 
     Parameters:
     - record (Dict[str, Any]): The data record.
     - element (Dict[str, Any]): The element of the criteria.
+    - config (Optional[Config]): Configuration options.
 
     Returns:
     - bool: Whether or not the record meets the criteria.
     """
 
     if not isinstance(element, dict):
         raise ValueError('Invalid element: must be a dictionary')
 
     # AND, OR, NOT operators
     if 'AND' in element:
-        return all(meets_crit(record, el) for el in element.get('AND', []))
+        return all(meets_crit(record, el, config) for el in element.get('AND', []))
     if 'OR' in element:
-        return any(meets_crit(record, el) for el in element.get('OR', []))
+        return any(meets_crit(record, el, config) for el in element.get('OR', []))
     if 'NOT' in element:
-        return not meets_crit(record, element.get('NOT', {}))
+        return not meets_crit(record, element.get('NOT', {}), config)
 
     # Conditions
     key = element.get('key')
     operator = element.get('op')
     value = element.get('value')
 
     if not isinstance(key, str) or not operator or value is None:
         raise ValueError(f'Invalid condition: {element}')
 
-    return compare(record.get(key), operator, value)
+    return compare(record.get(key), operator, value, config)
```

### Comparing `json_criteria-0.1.2/tests/test_all_meet_criteria.py` & `json_criteria-0.2.0/tests/test_all_meet_criteria.py`

 * *Files identical despite different names*

### Comparing `json_criteria-0.1.2/tests/test_any_meet_criteria.py` & `json_criteria-0.2.0/tests/test_any_meet_criteria.py`

 * *Files identical despite different names*

### Comparing `json_criteria-0.1.2/tests/test_apply_using_criteria.py` & `json_criteria-0.2.0/tests/test_apply_using_criteria.py`

 * *Files identical despite different names*

### Comparing `json_criteria-0.1.2/tests/test_combine_criteria.py` & `json_criteria-0.2.0/tests/test_combine_criteria.py`

 * *Files identical despite different names*

### Comparing `json_criteria-0.1.2/tests/test_find_using_criteria.py` & `json_criteria-0.2.0/tests/test_find_using_criteria.py`

 * *Files identical despite different names*

### Comparing `json_criteria-0.1.2/tests/test_get_all_criteria.py` & `json_criteria-0.2.0/tests/test_get_all_criteria.py`

 * *Files identical despite different names*

### Comparing `json_criteria-0.1.2/tests/internal/test_meets_crit.py` & `json_criteria-0.2.0/tests/internal/test_meets_crit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 
 from src.json_criteria.internal import meets_crit
+from src.json_criteria import Config
 
 class TestMeetsCrit(unittest.TestCase):
     def test_basic(self):
         record = { 'name': 'Joe' , 'age': 30 }
         criteria = { 'key': 'age', 'op': 'equal_to', 'value': 30 }
         result = meets_crit(record, criteria)
         self.assertTrue(result)
@@ -256,9 +257,17 @@
 
     def test_in_false(self):
         record = { 'name': 'Joe' , 'age': 30 }
         criteria = {'key': 'age', 'op': 'in', 'value': [28, 29, 31] }
         result = meets_crit(record, criteria)
         self.assertFalse(result)
 
+    def test_custom_op(self):
+        def custom1(record_value, value):
+            return record_value + value == 100
+        record = { 'name': 'Joe' , 'age': 30 }
+        criteria = {'key': 'age', 'op': 'custom1', 'value': 70 }
+        result = meets_crit(record, criteria, Config(custom_ops = { 'custom1': custom1 }))
+        self.assertTrue(result)
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `json_criteria-0.1.2/.gitignore` & `json_criteria-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `json_criteria-0.1.2/LICENSE` & `json_criteria-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `json_criteria-0.1.2/README.md` & `json_criteria-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # json-criteria
 
-`json-criteria` is a lightweight, dependency-free Python library designed for evaluating data against serializable JSON criteria. This library supports multiple operators and nested conditions, providing a flexible and powerful tool for condition-based decision-making.
+`json-criteria` is a lightweight, dependency-free Python library designed for evaluating data against serializable JSON criteria. It offers a variety of built-in operators, supports custom operators, and can handle complex nested conditions, making it a valuable and flexible tool for condition-based decision-making.
 
 ## Why use `json-criteria`?
 
 * **Serialization to JSON**
   * The criteria used by `json-criteria` can be easily serialized to JSON format. This enables the persistence of criteria, making it suitable for storage in databases or external configurations.
 * **Dynamic Criteria Adjustment**
   * Since the criteria is stored as JSON, it allows for dynamic adjustments without the need for code deployment. Criteria can be modified or extended as needed, providing the ability to adapt application behavior without code changes.
@@ -65,29 +65,47 @@
 }
 
 # Check if the record meets the criteria
 # `result` will be True
 result = meets_criteria(record, criteria)
 ```
 
-These examples demonstrate the simplicity and power of `json_criteria` in handling both basic and intricate conditions for evaluating data. The library's support for nested conditions enables the representation of complex logical structures, making it a valuable tool for decision-making in various scenarios.
+### Simple Custom Operator
+
+Pass in a `Config` object to specify custom operators.
+
+```python
+from json_criteria import meets_criteria, Config
+
+def custom1(record_value, value):
+    return record_value + value == 60
+
+record = { 'name': 'Joe', 'age': 30 }
+criteria = { 'key': 'age', 'op': 'custom1', 'value': 30 }
+config = Config(custom_ops = { 'custom1': custom1 })
+
+# `result` will be True
+result = meets_criteria(record, criteria, config)
+```
+
+These examples demonstrate the simplicity and flexibility of `json_criteria` in handling both basic and intricate conditions for evaluating data. The library's support for nested conditions enables the representation of complex logical structures, making it a valuable tool for decision-making in various scenarios.
 
 ## Criteria
 
 Criteria in `json-criteria` are represented as dictionaries, specifying the conditions that record(s) must satisfy. This allows for flexible and expressive criteria, supporting both simple conditions and intricate logical structures with AND, OR, and NOT operators.
 
 A condition is composed of three fundamental components:
 
 * `key`: The key to be evaluated.
 * `op`: The operator indicating the comparison type.
 * `value`: The expected value for the specified key.
 
 Additional keys, such as `id` and `description`, can be included without impacting functionality. This feature provides the flexibility to add context or relevant information to the criteria.
 
-### Supported Operators:
+### Built-In Operators:
 
 * `equal_to`
 * `not_equal_to`
 * `greater_than`
 * `less_than`
 * `greater_than_or_equal_to`
 * `less_than_or_equal_to`
@@ -242,15 +260,15 @@
 #     ]
 # }
 result = combine_criteria('AND', [criteria1, criteria2])
 ```
 
 ### `filter_using_criteria`
 
-Filter a list of records based on the given criteria. This function provides a powerful mechanism for selectively extracting records that meet specific conditions, enhancing the flexibility of data filtering.
+Filter a list of records based on the given criteria. This function provides a mechanism for selectively extracting records that meet specific conditions, enhancing the flexibility of data filtering.
 
 ```python
 from json_criteria import filter_using_criteria
 
 # Define a list of employee records
 employee_records = [
     {'name': 'Alice', 'age': 28, 'department': 'Engineering', 'is_manager': False},
@@ -305,15 +323,15 @@
 # Find the first employee record meeting the criteria
 # `result` will be: {'name': 'Bob', 'age': 35, 'department': 'Marketing', 'is_manager': True}
 result = find_using_criteria(employee_records, criteria)
 ```
 
 ### `get_all_criteria`
 
-Given a record and a list of criteria, retrieve all criteria that the record meets. This function is useful for analyzing and identifying the specific criteria that a record satisfies within a given list.
+Given a record and a list of criteria, get all criteria that the record meets. This function is useful for analyzing and identifying the specific criteria that a record satisfies within a given list.
 
 ```python
 from json_criteria import get_all_criteria
 
 # Define a user
 user = {
     'name': 'Alice',
@@ -397,10 +415,34 @@
 }
 
 # Check if the user record meets the specified criteria
 # `result` will be True
 result = meets_criteria(user_record, criteria)
 ```
 
+### Configuration
+
+Configuring `json-criteria` is optional. By default, the library works without any additional setup. However, if you want to customize the behavior, such as adding custom operators, you can create a `Config` object and pass it to the library function being called. Available configuration options are detailed below.
+
+#### custom_ops
+
+This option allows you to define custom operators. To use it, provide a dictionary where the keys are the operator names, and the values are the corresponding operator functions. Each operator function receives two arguments:
+
+1. `record_value`: The value from the data record.
+2. `value`: The value specified in the criteria.
+
+```python
+from json_criteria import Config
+
+def same_len(record_value, value):
+    return len(record_value) == len(value)
+
+config = Config(custom_ops = { 'same_len': same_len })
+```
+
 ## Contributing Guide
 
 I welcome all pull requests. Please make sure you add appropriate test cases for any features added.
+
+To run tests: `python3 -m unittest`
+
+To lint: `pylint src`
```

### Comparing `json_criteria-0.1.2/pyproject.toml` & `json_criteria-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "json-criteria"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Matthew Fay" },
 ]
 description = "Python library designed for evaluating data against serializable JSON criteria"
 keywords = ["json", "criteria", "persistence", "serialization", "serialized", "serializable", "rules", "decisions", "decision-making", "decision making", "conditions", "nested", "nested conditions", "operators", "logic", "eligibility", "dynamic adjustment", "data evaluation", "evaluation", "comparison", "compare", "adaptable", "flexible", "flexibility", "maintainable", "maintainability", "dependency-free"]
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `json_criteria-0.1.2/PKG-INFO` & `json_criteria-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: json-criteria
-Version: 0.1.2
+Version: 0.2.0
 Summary: Python library designed for evaluating data against serializable JSON criteria
 Project-URL: Homepage, https://github.com/MatthewFay/json-criteria
 Project-URL: Issues, https://github.com/MatthewFay/json-criteria/issues
 Author: Matthew Fay
 License-File: LICENSE
 Keywords: adaptable,compare,comparison,conditions,criteria,data evaluation,decision making,decision-making,decisions,dependency-free,dynamic adjustment,eligibility,evaluation,flexibility,flexible,json,logic,maintainability,maintainable,nested,nested conditions,operators,persistence,rules,serializable,serialization,serialized
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # json-criteria
 
-`json-criteria` is a lightweight, dependency-free Python library designed for evaluating data against serializable JSON criteria. This library supports multiple operators and nested conditions, providing a flexible and powerful tool for condition-based decision-making.
+`json-criteria` is a lightweight, dependency-free Python library designed for evaluating data against serializable JSON criteria. It offers a variety of built-in operators, supports custom operators, and can handle complex nested conditions, making it a valuable and flexible tool for condition-based decision-making.
 
 ## Why use `json-criteria`?
 
 * **Serialization to JSON**
   * The criteria used by `json-criteria` can be easily serialized to JSON format. This enables the persistence of criteria, making it suitable for storage in databases or external configurations.
 * **Dynamic Criteria Adjustment**
   * Since the criteria is stored as JSON, it allows for dynamic adjustments without the need for code deployment. Criteria can be modified or extended as needed, providing the ability to adapt application behavior without code changes.
@@ -80,29 +80,47 @@
 }
 
 # Check if the record meets the criteria
 # `result` will be True
 result = meets_criteria(record, criteria)
 ```
 
-These examples demonstrate the simplicity and power of `json_criteria` in handling both basic and intricate conditions for evaluating data. The library's support for nested conditions enables the representation of complex logical structures, making it a valuable tool for decision-making in various scenarios.
+### Simple Custom Operator
+
+Pass in a `Config` object to specify custom operators.
+
+```python
+from json_criteria import meets_criteria, Config
+
+def custom1(record_value, value):
+    return record_value + value == 60
+
+record = { 'name': 'Joe', 'age': 30 }
+criteria = { 'key': 'age', 'op': 'custom1', 'value': 30 }
+config = Config(custom_ops = { 'custom1': custom1 })
+
+# `result` will be True
+result = meets_criteria(record, criteria, config)
+```
+
+These examples demonstrate the simplicity and flexibility of `json_criteria` in handling both basic and intricate conditions for evaluating data. The library's support for nested conditions enables the representation of complex logical structures, making it a valuable tool for decision-making in various scenarios.
 
 ## Criteria
 
 Criteria in `json-criteria` are represented as dictionaries, specifying the conditions that record(s) must satisfy. This allows for flexible and expressive criteria, supporting both simple conditions and intricate logical structures with AND, OR, and NOT operators.
 
 A condition is composed of three fundamental components:
 
 * `key`: The key to be evaluated.
 * `op`: The operator indicating the comparison type.
 * `value`: The expected value for the specified key.
 
 Additional keys, such as `id` and `description`, can be included without impacting functionality. This feature provides the flexibility to add context or relevant information to the criteria.
 
-### Supported Operators:
+### Built-In Operators:
 
 * `equal_to`
 * `not_equal_to`
 * `greater_than`
 * `less_than`
 * `greater_than_or_equal_to`
 * `less_than_or_equal_to`
@@ -257,15 +275,15 @@
 #     ]
 # }
 result = combine_criteria('AND', [criteria1, criteria2])
 ```
 
 ### `filter_using_criteria`
 
-Filter a list of records based on the given criteria. This function provides a powerful mechanism for selectively extracting records that meet specific conditions, enhancing the flexibility of data filtering.
+Filter a list of records based on the given criteria. This function provides a mechanism for selectively extracting records that meet specific conditions, enhancing the flexibility of data filtering.
 
 ```python
 from json_criteria import filter_using_criteria
 
 # Define a list of employee records
 employee_records = [
     {'name': 'Alice', 'age': 28, 'department': 'Engineering', 'is_manager': False},
@@ -320,15 +338,15 @@
 # Find the first employee record meeting the criteria
 # `result` will be: {'name': 'Bob', 'age': 35, 'department': 'Marketing', 'is_manager': True}
 result = find_using_criteria(employee_records, criteria)
 ```
 
 ### `get_all_criteria`
 
-Given a record and a list of criteria, retrieve all criteria that the record meets. This function is useful for analyzing and identifying the specific criteria that a record satisfies within a given list.
+Given a record and a list of criteria, get all criteria that the record meets. This function is useful for analyzing and identifying the specific criteria that a record satisfies within a given list.
 
 ```python
 from json_criteria import get_all_criteria
 
 # Define a user
 user = {
     'name': 'Alice',
@@ -412,10 +430,34 @@
 }
 
 # Check if the user record meets the specified criteria
 # `result` will be True
 result = meets_criteria(user_record, criteria)
 ```
 
+### Configuration
+
+Configuring `json-criteria` is optional. By default, the library works without any additional setup. However, if you want to customize the behavior, such as adding custom operators, you can create a `Config` object and pass it to the library function being called. Available configuration options are detailed below.
+
+#### custom_ops
+
+This option allows you to define custom operators. To use it, provide a dictionary where the keys are the operator names, and the values are the corresponding operator functions. Each operator function receives two arguments:
+
+1. `record_value`: The value from the data record.
+2. `value`: The value specified in the criteria.
+
+```python
+from json_criteria import Config
+
+def same_len(record_value, value):
+    return len(record_value) == len(value)
+
+config = Config(custom_ops = { 'same_len': same_len })
+```
+
 ## Contributing Guide
 
 I welcome all pull requests. Please make sure you add appropriate test cases for any features added.
+
+To run tests: `python3 -m unittest`
+
+To lint: `pylint src`
```

