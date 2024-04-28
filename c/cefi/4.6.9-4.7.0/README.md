# Comparing `tmp/cefi-4.6.9.tar.gz` & `tmp/cefi-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefi-4.6.9.tar", max compression
+gzip compressed data, was "cefi-4.7.0.tar", max compression
```

## Comparing `cefi-4.6.9.tar` & `cefi-4.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-04-27 09:43:41.749979 cefi-4.6.9/LICENSE
--rw-r--r--   0        0        0     2661 2024-04-27 09:43:41.749979 cefi-4.6.9/README.md
--rw-r--r--   0        0        0       87 2024-04-27 09:44:21.287169 cefi-4.6.9/cefi/__init__.py
--rw-r--r--   0        0        0      439 2024-04-27 09:43:41.749979 cefi-4.6.9/cefi/config.py
--rw-r--r--   0        0        0     3617 2024-04-27 09:43:41.749979 cefi-4.6.9/cefi/default_settings.toml
--rw-r--r--   0        0        0      158 2024-04-27 09:43:41.749979 cefi-4.6.9/cefi/handler/__init__.py
--rw-r--r--   0        0        0    11153 2024-04-27 09:43:41.749979 cefi-4.6.9/cefi/handler/capitalcom.py
--rw-r--r--   0        0        0     5517 2024-04-27 09:43:41.749979 cefi-4.6.9/cefi/handler/ccxt.py
--rw-r--r--   0        0        0     9015 2024-04-27 09:43:41.749979 cefi-4.6.9/cefi/handler/client.py
--rw-r--r--   0        0        0     1938 2024-04-27 09:43:41.749979 cefi-4.6.9/cefi/handler/ctrader.py
--rw-r--r--   0        0        0     7006 2024-04-27 09:43:41.749979 cefi-4.6.9/cefi/handler/ib_sync.py
--rw-r--r--   0        0        0     8160 2024-04-27 09:43:41.749979 cefi-4.6.9/cefi/main.py
--rw-r--r--   0        0        0     3780 2024-04-27 09:44:21.287169 cefi-4.6.9/pyproject.toml
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-28 14:49:54.464340 cefi-4.7.0/LICENSE
+-rw-r--r--   0        0        0     2661 2024-04-28 14:49:54.464340 cefi-4.7.0/README.md
+-rw-r--r--   0        0        0       87 2024-04-28 14:50:33.680206 cefi-4.7.0/cefi/__init__.py
+-rw-r--r--   0        0        0      439 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/config.py
+-rw-r--r--   0        0        0     3617 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/default_settings.toml
+-rw-r--r--   0        0        0      158 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/handler/__init__.py
+-rw-r--r--   0        0        0    13356 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/handler/capitalcom.py
+-rw-r--r--   0        0        0     5517 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/handler/ccxt.py
+-rw-r--r--   0        0        0     9225 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/handler/client.py
+-rw-r--r--   0        0        0     1938 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/handler/ctrader.py
+-rw-r--r--   0        0        0     7006 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/handler/ib_sync.py
+-rw-r--r--   0        0        0     8586 2024-04-28 14:49:54.464340 cefi-4.7.0/cefi/main.py
+-rw-r--r--   0        0        0     3782 2024-04-28 14:50:33.680206 cefi-4.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.7.0/PKG-INFO
```

### Comparing `cefi-4.6.9/LICENSE` & `cefi-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cefi-4.6.9/README.md` & `cefi-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cefi-4.6.9/cefi/default_settings.toml` & `cefi-4.7.0/cefi/default_settings.toml`

 * *Files identical despite different names*

### Comparing `cefi-4.6.9/cefi/handler/capitalcom.py` & `cefi-4.7.0/cefi/handler/capitalcom.py`

 * *Files 11% similar despite different names*

```diff
@@ -346,7 +346,64 @@
                 "datetime": order_check.get("date", ""),
             }
             return await self.get_trade_confirmation(trade, instrument, action)
 
         except Exception as e:
             logger.error("{} Error {}", self.name, e)
             return f"Error executing {self.name}: {e}"
+
+    async def modify_position(self, order_params):
+        """
+        Modify parameters such as SL / TP of a position that is opened
+        No capability to modify amount to reduce
+
+        Args:
+            order_params (dict):
+                action(str)
+                instrument(str)
+                quantity(int)
+                stop_price(int)
+                stop_distance(int)
+                stop_amount(int)
+                take_profit_price(int)
+                take_profit_distance(int)
+                take_profit_amount(int)
+
+        Returns:
+            trade_confirmation(dict)
+
+        """
+        try:
+            order = self.client.update_the_position(
+                dealid=order_params["id"],
+                gsl=order_params.get("trailing_stop_enabled", False),
+                tsl=order_params.get("trailing_stop_enabled", False),
+                stop_level=order_params.get("stop_price"),
+                stop_distance=order_params.get("stop_distance"),
+                stop_amount=order_params.get("stop_amount"),
+                profit_level=order_params.get("take_profit_price"),
+                profit_distance=order_params.get("take_profit_distance"),
+                profit_amount=order_params.get("take_profit_amount"),
+            )
+
+            if "errorCode" in order:
+                logger.error(f"Error modifying order: {order['errorCode']}")
+                return str(order["errorCode"])
+
+            logger.debug("Order: {}", order)
+            deal_reference = order["dealReference"]
+            order_check = self.client.position_order_confirmation(
+                deal_reference=deal_reference
+            )
+
+            trade = {
+                "amount": order_check.get("size", 0),
+                "price": order_check.get("level", 0),
+                "id": order_check.get("dealId", ""),
+                "datetime": order_check.get("date", ""),
+            }
+            return await self.get_trade_confirmation(
+                trade, order_params.get("instrument"), order_params.get("action")
+            )
+        except Exception as e:
+            logger.error("{} Error {}", self.name, e)
+            return f"Error executing {self.name}: {e}"
```

### Comparing `cefi-4.6.9/cefi/handler/ccxt.py` & `cefi-4.7.0/cefi/handler/ccxt.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.9/cefi/handler/client.py` & `cefi-4.7.0/cefi/handler/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,7 +295,19 @@
             trade_confirmation += f"🔴 {round(0 or trade['stopLossPrice'], 4)}\n"
             trade_confirmation += f"ℹ️ {trade['id']}\n"
             trade_confirmation += f"🗓️ {trade['datetime']}"
             if trade_confirmation:
                 return f"{trade_confirmation}"
         except Exception as e:
             logger.error("Error {}", e)
+
+    async def modify_position(self, order_params):
+        """
+        Modify opened position
+
+        Args:
+            order_params (dict)
+
+        Returns:
+            trade_confirmation(dict)
+
+        """
```

### Comparing `cefi-4.6.9/cefi/handler/ctrader.py` & `cefi-4.7.0/cefi/handler/ctrader.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.9/cefi/handler/ib_sync.py` & `cefi-4.7.0/cefi/handler/ib_sync.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.9/cefi/main.py` & `cefi-4.7.0/cefi/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -262,7 +262,25 @@
         """
         _order = ["🧾 Order\n"]
         for client in self.clients:
             _order.append(
                 f"{client.name}:\n{await client.execute_order(order_params)}\n"
             )
         return "\n".join(_order)
+
+    async def modify_position(self, order_params):
+        """
+        Modify order
+
+        Args:
+            order_params (dict)
+
+        Returns:
+            trade_confirmation(dict)
+
+        """
+        _order = ["🧾 Order\n"]
+        for client in self.clients:
+            _order.append(
+                f"{client.name}:\n{await client.modify_position(order_params)}\n"
+            )
+        return "\n".join(_order)
```

### Comparing `cefi-4.6.9/pyproject.toml` & `cefi-4.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "cefi"
-version = "4.6.9"
+version = "4.7.0"
 description = "A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["cex, cefi, crypto, exchange, broker"]
 packages = [
     {include = "cefi"}
@@ -168,27 +168,29 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^5.0.0"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
 
 
 
 
 
 
+
```

### Comparing `cefi-4.6.9/PKG-INFO` & `cefi-4.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefi
-Version: 4.6.9
+Version: 4.7.0
 Summary: A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT
 Keywords: cex, cefi, crypto, exchange, broker
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cefi Version: 4.6.9 Summary: A python library, to
+Metadata-Version: 2.1 Name: cefi Version: 4.7.0 Summary: A python library, to
 interact with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT Keywords: cex, cefi, crypto, exchange, broker Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: capitalcom-python
```

