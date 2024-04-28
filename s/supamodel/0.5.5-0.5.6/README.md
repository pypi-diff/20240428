# Comparing `tmp/supamodel-0.5.5.tar.gz` & `tmp/supamodel-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supamodel-0.5.5.tar", max compression
+gzip compressed data, was "supamodel-0.5.6.tar", max compression
```

## Comparing `supamodel-0.5.5.tar` & `supamodel-0.5.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3741 2024-04-15 21:10:14.946524 supamodel-0.5.5/README.md
--rw-r--r--   0        0        0      869 2024-04-25 21:27:44.857148 supamodel-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      190 2024-04-15 21:10:14.947301 supamodel-0.5.5/supamodel/__init__.py
--rw-r--r--   0        0        0     8349 2024-04-15 21:10:14.947482 supamodel-0.5.5/supamodel/_abc.py
--rw-r--r--   0        0        0      291 2024-04-16 02:36:19.549095 supamodel-0.5.5/supamodel/_client.py
--rw-r--r--   0        0        0     8016 2024-04-15 21:10:14.947711 supamodel-0.5.5/supamodel/_core.py
--rw-r--r--   0        0        0      674 2024-04-15 21:10:14.947815 supamodel-0.5.5/supamodel/_logging.py
--rw-r--r--   0        0        0      335 2024-04-15 21:10:14.947906 supamodel-0.5.5/supamodel/_types.py
--rw-r--r--   0        0        0     1488 2024-04-15 21:10:14.948025 supamodel-0.5.5/supamodel/config.py
--rw-r--r--   0        0        0     2284 2024-04-15 21:10:14.948124 supamodel-0.5.5/supamodel/enums.py
--rw-r--r--   0        0        0      321 2024-04-15 21:10:14.948205 supamodel-0.5.5/supamodel/errors.py
--rw-r--r--   0        0        0     1432 2024-04-15 21:10:14.948303 supamodel-0.5.5/supamodel/exceptions.py
--rw-r--r--   0        0        0     8307 2024-04-15 21:10:14.948494 supamodel-0.5.5/supamodel/supa.py
--rw-r--r--   0        0        0     4187 2024-04-15 21:10:14.948633 supamodel-0.5.5/supamodel/supa_builder.py
--rw-r--r--   0        0        0        0 2024-04-15 21:10:14.948743 supamodel-0.5.5/supamodel/trading/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 21:10:14.948807 supamodel-0.5.5/supamodel/trading/assets.py
--rw-r--r--   0        0        0     3690 2024-04-15 21:10:14.949133 supamodel-0.5.5/supamodel/trading/clock.py
--rw-r--r--   0        0        0     3464 2024-04-15 23:57:47.194613 supamodel-0.5.5/supamodel/trading/exchange.py
--rw-r--r--   0        0        0     1336 2024-04-15 21:10:14.949430 supamodel-0.5.5/supamodel/trading/market_data.py
--rw-r--r--   0        0        0     1865 2024-04-15 21:10:14.949520 supamodel-0.5.5/supamodel/trading/order_management.py
--rw-r--r--   0        0        0     1832 2024-04-15 21:10:14.949609 supamodel-0.5.5/supamodel/trading/portfolio.py
--rw-r--r--   0        0        0    11732 2024-04-15 21:10:14.949788 supamodel-0.5.5/supamodel/trading/tokens.py
--rw-r--r--   0        0        0    14903 2024-04-15 21:10:14.949935 supamodel-0.5.5/supamodel/utils.py
--rw-r--r--   0        0        0     4847 1970-01-01 00:00:00.000000 supamodel-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     3741 2024-04-15 21:10:14.946524 supamodel-0.5.6/README.md
+-rw-r--r--   0        0        0      869 2024-04-28 00:39:47.899464 supamodel-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      265 2024-04-28 00:33:20.687276 supamodel-0.5.6/supamodel/__init__.py
+-rw-r--r--   0        0        0     8349 2024-04-15 21:10:14.947482 supamodel-0.5.6/supamodel/_abc.py
+-rw-r--r--   0        0        0      291 2024-04-16 02:36:19.549095 supamodel-0.5.6/supamodel/_client.py
+-rw-r--r--   0        0        0     8016 2024-04-15 21:10:14.947711 supamodel-0.5.6/supamodel/_core.py
+-rw-r--r--   0        0        0      674 2024-04-15 21:10:14.947815 supamodel-0.5.6/supamodel/_logging.py
+-rw-r--r--   0        0        0      335 2024-04-15 21:10:14.947906 supamodel-0.5.6/supamodel/_types.py
+-rw-r--r--   0        0        0     1488 2024-04-15 21:10:14.948025 supamodel-0.5.6/supamodel/config.py
+-rw-r--r--   0        0        0     2284 2024-04-15 21:10:14.948124 supamodel-0.5.6/supamodel/enums.py
+-rw-r--r--   0        0        0      321 2024-04-15 21:10:14.948205 supamodel-0.5.6/supamodel/errors.py
+-rw-r--r--   0        0        0     1432 2024-04-15 21:10:14.948303 supamodel-0.5.6/supamodel/exceptions.py
+-rw-r--r--   0        0        0     8307 2024-04-15 21:10:14.948494 supamodel-0.5.6/supamodel/supa.py
+-rw-r--r--   0        0        0     4187 2024-04-15 21:10:14.948633 supamodel-0.5.6/supamodel/supa_builder.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:10:14.948743 supamodel-0.5.6/supamodel/trading/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:10:14.948807 supamodel-0.5.6/supamodel/trading/assets.py
+-rw-r--r--   0        0        0     3690 2024-04-15 21:10:14.949133 supamodel-0.5.6/supamodel/trading/clock.py
+-rw-r--r--   0        0        0     3464 2024-04-15 23:57:47.194613 supamodel-0.5.6/supamodel/trading/exchange.py
+-rw-r--r--   0        0        0     1336 2024-04-15 21:10:14.949430 supamodel-0.5.6/supamodel/trading/market_data.py
+-rw-r--r--   0        0        0     2111 2024-04-27 20:47:39.714063 supamodel-0.5.6/supamodel/trading/order_management.py
+-rw-r--r--   0        0        0     1850 2024-04-27 20:48:25.673948 supamodel-0.5.6/supamodel/trading/portfolio.py
+-rw-r--r--   0        0        0    11732 2024-04-15 21:10:14.949788 supamodel-0.5.6/supamodel/trading/tokens.py
+-rw-r--r--   0        0        0    14903 2024-04-15 21:10:14.949935 supamodel-0.5.6/supamodel/utils.py
+-rw-r--r--   0        0        0     4847 1970-01-01 00:00:00.000000 supamodel-0.5.6/PKG-INFO
```

### Comparing `supamodel-0.5.5/README.md` & `supamodel-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.5/pyproject.toml` & `supamodel-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "supamodel"
-version = "0.5.5"
+version = "0.5.6"
 description = "Pydantic Models for Trading Algos and Supabase"
 authors = ["Kevin Hill <kivo360@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<=3.12"
 pendulum = ">=2.0.0,<4.0.0"
```

### Comparing `supamodel-0.5.5/supamodel/_abc.py` & `supamodel-0.5.6/supamodel/_abc.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.5/supamodel/_core.py` & `supamodel-0.5.6/supamodel/_core.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.5/supamodel/_logging.py` & `supamodel-0.5.6/supamodel/_logging.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.5/supamodel/config.py` & `supamodel-0.5.6/supamodel/config.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.5/supamodel/enums.py` & `supamodel-0.5.6/supamodel/enums.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.5/supamodel/exceptions.py` & `supamodel-0.5.6/supamodel/exceptions.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.5/supamodel/supa.py` & `supamodel-0.5.6/supamodel/supa.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.5/supamodel/supa_builder.py` & `supamodel-0.5.6/supamodel/supa_builder.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.5/supamodel/trading/clock.py` & `supamodel-0.5.6/supamodel/trading/clock.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.5/supamodel/trading/exchange.py` & `supamodel-0.5.6/supamodel/trading/exchange.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.5/supamodel/trading/market_data.py` & `supamodel-0.5.6/supamodel/trading/market_data.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.5/supamodel/trading/order_management.py` & `supamodel-0.5.6/supamodel/trading/order_management.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 from datetime import datetime
 from typing import Optional
 from uuid import UUID
 
+from pendulum import DateTime
 from pydantic import Field
 
 from supamodel._abc import BaseModel
 from supamodel.enums import OrderSide, OrderStatus, OrderType
 
 
 class Trade(BaseModel):
-    id: Optional[UUID] = Field(description="Unique identifier of the trade")
+    id: Optional[UUID] = Field(None, description="Unique identifier of the trade")
     position_id: UUID = Field(description="ID of the associated position")
     order_id: UUID = Field(description="ID of the associated order")
     quantity: float = Field(description="Quantity of the asset traded")
     price: float = Field(description="Price at which the trade occurred")
     fee: float = Field(description="Fee charged for the trade")
-    timestamp: datetime = Field(description="Timestamp of when the trade occurred")
+    timestamp: datetime = Field(
+        description="Timestamp of when the trade occurred",
+        default_factory=lambda: DateTime.now("UTC"),
+    )
     created_at: Optional[datetime] = Field(
-        description="Timestamp of when the trade record was created"
+        None, description="Timestamp of when the trade record was created"
     )
 
 
 class Order(BaseModel):
-    id: Optional[UUID] = Field(description="Unique identifier of the order")
+    id: Optional[UUID] = Field(None, description="Unique identifier of the order")
     portfolio_id: UUID = Field(description="ID of the associated portfolio")
     asset_id: UUID = Field(description="ID of the associated asset")
     exchange_id: UUID = Field(description="ID of the associated exchange")
     order_type: OrderType = Field(description="Type of the order (e.g., limit, market)")
     side: OrderSide = Field(description="Side of the order (buy or sell)")
     quantity: float = Field(description="Quantity of the asset to be traded")
     price: Optional[float] = Field(
-        description="Price at which the order should be executed (for limit orders)"
+        description="Price at which the order should be executed (for limit orders)",
+        default=0.0,
     )
     status: OrderStatus = Field(description="Current status of the order")
     created_at: Optional[datetime] = Field(
-        description="Timestamp of when the order was created"
+        description="Timestamp of when the order was created",
+        default_factory=lambda: DateTime.now("UTC"),
     )
     updated_at: Optional[datetime] = Field(
-        description="Timestamp of when the order was last updated"
+        description="Timestamp of when the order was last updated",
+        default_factory=lambda: DateTime.now("UTC"),
     )
```

### Comparing `supamodel-0.5.5/supamodel/trading/portfolio.py` & `supamodel-0.5.6/supamodel/trading/portfolio.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     )
     balance: float = Field(
         default=0.0, description="The total balance of the portfolio"
     )
 
 
 class Position(BaseModel):
-    id: Optional[UUID] = Field(description="Unique identifier of the position")
+    id: Optional[UUID] = Field(None, description="Unique identifier of the position")
     portfolio_id: UUID = Field(description="ID of the associated portfolio")
     asset_id: UUID = Field(description="ID of the associated asset")
     quantity: float = Field(
         description="Quantity of the asset held in the position", alias="amount"
     )
     average_price: float = Field(
         alias="value", description="Average price of the asset in the position"
     )
     created_at: Optional[DateTime] = Field(
-        description="Timestamp of when the position was created"
+        None, description="Timestamp of when the position was created"
     )
     updated_at: Optional[DateTime] = Field(
-        description="Timestamp of when the position was last updated"
+        None, description="Timestamp of when the position was last updated"
     )
```

### Comparing `supamodel-0.5.5/supamodel/trading/tokens.py` & `supamodel-0.5.6/supamodel/trading/tokens.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.5/supamodel/utils.py` & `supamodel-0.5.6/supamodel/utils.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.5.5/PKG-INFO` & `supamodel-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supamodel
-Version: 0.5.5
+Version: 0.5.6
 Summary: Pydantic Models for Trading Algos and Supabase
 Author: Kevin Hill
 Author-email: kivo360@gmail.com
 Requires-Python: >=3.9,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

