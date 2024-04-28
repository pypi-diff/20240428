# Comparing `tmp/ynab_transaction_adjuster-1.1.0.tar.gz` & `tmp/ynab_transaction_adjuster-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynab_transaction_adjuster-1.1.0.tar", max compression
+gzip compressed data, was "ynab_transaction_adjuster-1.2.0.tar", max compression
```

## Comparing `ynab_transaction_adjuster-1.1.0.tar` & `ynab_transaction_adjuster-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35148 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/LICENSE
--rw-r--r--   0        0        0     3566 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/README.md
--rw-r--r--   0        0        0      673 2024-04-26 07:48:01.514400 ynab_transaction_adjuster-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      291 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/__init__.py
--rw-r--r--   0        0        0     5359 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/adjuster.py
--rw-r--r--   0        0        0     2954 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/client.py
--rw-r--r--   0        0        0     1003 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/exceptions.py
--rw-r--r--   0        0        0      357 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/__init__.py
--rw-r--r--   0        0        0      246 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/category.py
--rw-r--r--   0        0        0      621 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/categorygroup.py
--rw-r--r--   0        0        0      263 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/credentials.py
--rw-r--r--   0        0        0     2920 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/modifiedtransaction.py
--rw-r--r--   0        0        0     1718 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/modifier.py
--rw-r--r--   0        0        0     1252 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/modifiersubtransaction.py
--rw-r--r--   0        0        0      586 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/payee.py
--rw-r--r--   0        0        0      594 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/subtransaction.py
--rw-r--r--   0        0        0     3106 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/transaction.py
--rw-r--r--   0        0        0       72 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/repos/__init__.py
--rw-r--r--   0        0        0     1980 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/repos/categoryrepo.py
--rw-r--r--   0        0        0     1771 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/repos/payeerepo.py
--rw-r--r--   0        0        0     2848 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/serializer.py
--rw-r--r--   0        0        0     1283 2024-04-26 07:47:44.514477 ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/signaturechecker.py
--rw-r--r--   0        0        0     4363 1970-01-01 00:00:00.000000 ynab_transaction_adjuster-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3421 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/README.md
+-rw-r--r--   0        0        0      696 2024-04-28 06:43:23.459809 ynab_transaction_adjuster-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      291 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/__init__.py
+-rw-r--r--   0        0        0     6369 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/adjuster.py
+-rw-r--r--   0        0        0     2954 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/client.py
+-rw-r--r--   0        0        0     1003 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/exceptions.py
+-rw-r--r--   0        0        0      357 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/category.py
+-rw-r--r--   0        0        0      621 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/categorygroup.py
+-rw-r--r--   0        0        0      263 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/credentials.py
+-rw-r--r--   0        0        0     2927 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/modifiedtransaction.py
+-rw-r--r--   0        0        0     1718 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/modifier.py
+-rw-r--r--   0        0        0     1252 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/modifiersubtransaction.py
+-rw-r--r--   0        0        0      586 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/payee.py
+-rw-r--r--   0        0        0      594 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/subtransaction.py
+-rw-r--r--   0        0        0     3106 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/transaction.py
+-rw-r--r--   0        0        0       72 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/repos/__init__.py
+-rw-r--r--   0        0        0     1980 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/repos/categoryrepo.py
+-rw-r--r--   0        0        0     1771 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/repos/payeerepo.py
+-rw-r--r--   0        0        0     2848 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/serializer.py
+-rw-r--r--   0        0        0     1283 2024-04-28 06:43:06.019781 ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/signaturechecker.py
+-rw-r--r--   0        0        0     4262 1970-01-01 00:00:00.000000 ynab_transaction_adjuster-1.2.0/PKG-INFO
```

### Comparing `ynab_transaction_adjuster-1.1.0/LICENSE` & `ynab_transaction_adjuster-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.1.0/README.md` & `ynab_transaction_adjuster-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -56,27 +56,25 @@
 
 ### Initialize
 Create a `Credentials` object and initialize Adjuster class with it
 ```py
 from ynabtransactionadjuster import Credentials
 
 my_credentials = Credentials(token='<token>', budget='<budget>', account='<account>')
-my_adjuster = MyAdjuster.from_credentials(credentials=my_credentials)
+my_adjuster = MyAdjuster(my_credentials)
 ```
 
-### Test
-Test the adjuster on records fetched via the `dry_run()` method. It executes the adjustments but doesn't write the 
-results back to YNAB. Instead it returns a list of the changed transactions which can be inspected for the changed 
-properties. It takes an optional parameter `pretty_print` which, if set to `True`, prints modifications in an easy 
-readable string representation to the console.
-
+### Apply
+Apply the filter and adjust function on the fetched transactions from YNAB via the `apply()` method. It 
+returns a filtered list of `ModifiedTransaction` which can be inspected for the changed properties via the 
+`changed_attributes` attribute. Only actually changed transactions are returned. 
 ```py
-mod_transactions = my_adjuster.dry_run()
+modified_transactions = my_adjuster.apply()
 ```
 
-### Run
-If you are satisfied with the functionality you can execute the adjuster with the `run()` method. This will run the 
-adjustments and will update the changed transactions in YNAB. The method returns an integer with the number of 
-successfully updated records.
+### Update
+The modified transactions can be upated in YNAB passing them to the `update()` function. The method returns an integer 
+with the number of successfully updated records.
 ```py
-count_of_updated_transactions = my_adjuster.run()
+modified_transactions = my_adjuster.apply()
+count_of_updated_transactions = my_adjuster.update(modified_transactions)
 ```
```

### Comparing `ynab_transaction_adjuster-1.1.0/pyproject.toml` & `ynab_transaction_adjuster-1.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ynab-transaction-adjuster"
-version = "1.1.0"
+version = "1.2.0"
 description = "Library to adjust transactions in YNAB based on custom patterns"
 authors = ["Daniel Basta <ynab@basta.info>"]
 readme = "README.md"
 license = 'MIT'
 packages = [{include = 'ynabtransactionadjuster'}]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -12,15 +12,16 @@
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = '^3.8'
 requests = '^2.28.0'
 pydantic = '^2.7.0'
-pytest = "^8.1.1"
+deprecated = "^1.2.14"
+pytest = "^8.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/adjuster.py` & `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/adjuster.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,54 @@
+
 from abc import abstractmethod, ABCMeta
-from dataclasses import dataclass
 from typing import List
+from deprecated import deprecated
 
 from ynabtransactionadjuster.models import ModifiedTransaction
 from ynabtransactionadjuster.models.credentials import Credentials
 from ynabtransactionadjuster.client import Client
 from ynabtransactionadjuster.models import Transaction
 from ynabtransactionadjuster.models import Modifier
 from ynabtransactionadjuster.repos import CategoryRepo
 from ynabtransactionadjuster.repos import PayeeRepo
 from ynabtransactionadjuster.serializer import Serializer
 from ynabtransactionadjuster.signaturechecker import SignatureChecker
 
 
-@dataclass
 class Adjuster(metaclass=ABCMeta):
 	"""Abstract class which modifies transactions according to concrete implementation. You need to create your own
 	child class and implement the `filter()`and `adjust()` method in it according to your needs. It has attributes
 	which allow you to lookup categories and payees from your budget.
 
 	:ivar categories: Collection of current categories in YNAB budget
 	:ivar payees: Collection of current payees in YNAB budget
-	:ivar transactions: Transactions from YNAB Account
+	:ivar transactions: All current non deleted transactions from YNAB Account
 	:ivar credentials: Credentials for YNAB API
 	"""
-	credentials: Credentials
-	categories: CategoryRepo
-	payees: PayeeRepo
-	transactions: List[Transaction]
-
-	@classmethod
-	def from_credentials(cls, credentials: Credentials):
-		"""Instantiate a Adjuster class from a Credentials object
-
-		:param credentials: Credentials to use for YNAB API
-		"""
-		client = Client.from_credentials(credentials=credentials)
-		categories = CategoryRepo(client.fetch_categories())
-		payees = PayeeRepo(client.fetch_payees())
-		transactions = client.fetch_transactions()
-		return cls(categories=categories, payees=payees, transactions=transactions, credentials=credentials)
+	def __init__(self, credentials: Credentials):
+		self.credentials = credentials
+		self._client = Client.from_credentials(self.credentials)
+		self._categories = None
+		self._payees = None
+
+	@property
+	def categories(self) -> CategoryRepo:
+		if not self._categories:
+			self._categories = CategoryRepo(self._client.fetch_categories())
+		return self._categories
+
+	@property
+	def payees(self) -> PayeeRepo:
+		if not self._payees:
+			self._payees = PayeeRepo(self._client.fetch_payees())
+		return self._payees
+
+	@property
+	def transactions(self) -> List[Transaction]:
+		return self._client.fetch_transactions()
 
 	@abstractmethod
 	def filter(self, transactions: List[Transaction]) -> List[Transaction]:
 		"""Function which implements filtering for the list of transactions from YNAB account. It receives a list of
 		the original transactions which can be filtered. Must return the filtered list or just the list if no filtering
 		is intended.
 
@@ -59,57 +64,84 @@
 		:param transaction: Original transaction
 		:param modifier: Transaction modifier prefilled with values from original transaction. All attributes can be
 		changed and will modify the transaction
 		:returns: Method needs to return the transaction modifier after modification
 		"""
 		pass
 
-	def dry_run(self, pretty_print: bool = False) -> List[ModifiedTransaction]:
-		"""Tests the adjuster. It will fetch transactions from the YNAB account, filter & adjust them as per
-		implementation of the two methods. This function doesn't update records in YNAB but returns the modified
-		transactions so that they can be inspected.
-
-		:param pretty_print: if set to True will print modified transactions as strings in console
+	def apply(self) -> List[ModifiedTransaction]:
+		"""Function which applies filter & adjust function on transactions as per implementation of the two methods.
 
-		:return: List of modified transactions
+		:return: Filtered list of modified transactions (only transactions with actual changes are returned)
 		:raises SignatureError: if signature of implemented adjuster functions is not compatible
 		:raises AdjustError: if there is any error during the adjust process
-		:raises HTTPError: if there is any error with the YNAB API (e.g. wrong credentials)
 		"""
 		self._check_signatures()
 		filtered_transactions = self.filter(self.transactions)
 		s = Serializer(transactions=filtered_transactions, adjust_func=self.adjust, categories=self.categories)
 		modified_transactions = s.run()
-		if pretty_print:
-			print('\n'.join(map(str, modified_transactions)))
 		return modified_transactions
 
-	def run(self) -> int:
-		"""Run the adjuster. It will fetch transactions from the YNAB account, filter & adjust them as per
-		implementation of the two methods and push the updated transactions back to YNAB
+	def update(self, modified_transactions: List[ModifiedTransaction]) -> int:
+		"""Updates the modified transactions in YNAB
 
+		:param modified_transactions: List of modified transactions to be updated in YNAB
 		:return: count of adjusted transactions which have been updated in YNAB
-		:raises SignatureError: if signature of implemented adjuster functions is not compatible
-		:raises AdjustError: if there is any error during the adjust process
 		:raises HTTPError: if there is any error with the YNAB API (e.g. wrong credentials)
 		"""
-		self._check_signatures()
-		filtered_transactions = self.filter(self.transactions)
-		s = Serializer(transactions=filtered_transactions, adjust_func=self.adjust, categories=self.categories)
-		modified_transactions = s.run()
 		if modified_transactions:
-			client = Client.from_credentials(credentials=self.credentials)
-			updated = client.update_transactions(modified_transactions)
+			updated = self._client.update_transactions(modified_transactions)
 			return updated
 		return 0
 
 	def _check_signatures(self):
 		SignatureChecker(func=self.filter, parent_func=Adjuster.filter).check()
 		SignatureChecker(func=self.adjust, parent_func=Adjuster.adjust).check()
 
 	def fetch_transaction(self, transaction_id: str) -> Transaction:
 		"""Fetches an individual transaction from the YNAB account
 
 		:param transaction_id: Transaction ID of the transaction to be fetched
 		"""
-		client = Client.from_credentials(credentials=self.credentials)
-		return client.fetch_transaction(transaction_id=transaction_id)
+		return self._client.fetch_transaction(transaction_id=transaction_id)
+
+	@classmethod
+	@deprecated(version='1.2.0', reason='Use the standard constructor method MyAdjuster(credentials) instead.')
+	def from_credentials(cls, credentials: Credentials):
+		"""**Deprecated** Use the standard constructor method `MyAdjuster(credentials)` instead.
+
+		Classmethod which creates a new Adjuster instance from credentials
+
+		:param credentials: Credentials for YNAB APIx
+		"""
+		return cls(credentials)
+
+	@deprecated(version='1.2.0', reason='Use apply() function instead.')
+	def dry_run(self, pretty_print: bool = False) -> List[ModifiedTransaction]:
+		"""	**Deprecated** Use `apply()` function instead
+
+		Tests the filter & adjust methods of the adjuster.This function doesn't update records in YNAB.
+
+		:param pretty_print: if set to True will print modified transactions as strings in console
+
+		:return: List of modified transactions
+		:raises SignatureError: if signature of implemented adjuster functions is not compatible
+		:raises AdjustError: if there is any error during the adjust process
+		"""
+		modified_transactions = self.apply()
+		if pretty_print:
+			print('\n'.join(map(str, modified_transactions)))
+		return modified_transactions
+
+	@deprecated(version='1.2.0', reason='Use apply() and updated() function instead.')
+	def run(self) -> int:
+		"""**Deprecated** Use `apply()` and `update()` functions instead.
+
+		Run the adjuster. It will apply the filter & adjust methods and update the modified transactions in YNAB
+
+		:return: count of adjusted transactions which have been updated in YNAB
+		:raises SignatureError: if signature of implemented adjuster functions is not compatible
+		:raises AdjustError: if there is any error during the adjust process
+		:raises HTTPError: if there is any error with the YNAB API (e.g. wrong credentials)
+		"""
+		modified_transactions = self.apply()
+		return self.update(modified_transactions)
```

### Comparing `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/client.py` & `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/client.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/exceptions.py` & `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/exceptions.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/categorygroup.py` & `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/categorygroup.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/modifiedtransaction.py` & `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/modifiedtransaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 	modifier: Modifier
 
 	def is_changed(self) -> bool:
 		"""Helper function to determine if transaction has been altered as compared to original one
 
 		:returns: True if values from original transaction have been altered, False otherwise
 		"""
-		if self.changed_attributes():
+		if self.changed_attributes:
 			return True
 		return False
 
 	def __str__(self) -> str:
-		return f"{self.transaction} | {self.changed_attributes()}"
+		return f"{self.transaction} | {self.changed_attributes}"
 
 	def as_dict(self) -> dict:
 		"""Returns a dictionary representation of the transaction which is used for the update call to YNAB"""
 		t_dict = dict(id=self.transaction.id,
 					  payee_name=self.modifier.payee.name,
 					  payee_id=self.modifier.payee.id,
 					  date=datetime.strftime(self.modifier.transaction_date, '%Y-%m-%d'),
@@ -37,14 +37,15 @@
 		if self.modifier.flag_color:
 			t_dict['flag_color'] = self.modifier.flag_color
 		if self.modifier.memo:
 			t_dict['memo'] = self.modifier.memo
 
 		return t_dict
 
+	@property
 	def changed_attributes(self) -> dict:
 		"""Returns a dictionary representation of the modified values and the original transaction"""
 		changed_attributes = dict()
 
 		for a in ('payee', 'category', 'flag_color', 'memo', 'approved', 'cleared'):
 			if self._attribute_changed(a):
 				changed_attributes[a] = self._create_changed_dict(a)
```

### Comparing `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/modifier.py` & `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/modifier.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/modifiersubtransaction.py` & `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/modifiersubtransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/payee.py` & `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/payee.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/subtransaction.py` & `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/subtransaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/models/transaction.py` & `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/models/transaction.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/repos/categoryrepo.py` & `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/repos/categoryrepo.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/repos/payeerepo.py` & `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/repos/payeerepo.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/serializer.py` & `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/serializer.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.1.0/ynabtransactionadjuster/signaturechecker.py` & `ynab_transaction_adjuster-1.2.0/ynabtransactionadjuster/signaturechecker.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-1.1.0/PKG-INFO` & `ynab_transaction_adjuster-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: ynab-transaction-adjuster
-Version: 1.1.0
+Version: 1.2.0
 Summary: Library to adjust transactions in YNAB based on custom patterns
 License: MIT
 Author: Daniel Basta
 Author-email: ynab@basta.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: deprecated (>=1.2.14,<2.0.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
-Requires-Dist: pytest (>=8.1.1,<9.0.0)
+Requires-Dist: pytest (>=8.2.0,<9.0.0)
 Requires-Dist: requests (>=2.28.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # ynab-transaction-adjuster
 
 [![GitHub Release](https://img.shields.io/github/release/dnbasta/ynab-transaction-adjuster?style=flat)]() 
 [![Maintained](https://img.shields.io/maintenance/yes/2100)]()
@@ -77,28 +78,26 @@
 
 ### Initialize
 Create a `Credentials` object and initialize Adjuster class with it
 ```py
 from ynabtransactionadjuster import Credentials
 
 my_credentials = Credentials(token='<token>', budget='<budget>', account='<account>')
-my_adjuster = MyAdjuster.from_credentials(credentials=my_credentials)
+my_adjuster = MyAdjuster(my_credentials)
 ```
 
-### Test
-Test the adjuster on records fetched via the `dry_run()` method. It executes the adjustments but doesn't write the 
-results back to YNAB. Instead it returns a list of the changed transactions which can be inspected for the changed 
-properties. It takes an optional parameter `pretty_print` which, if set to `True`, prints modifications in an easy 
-readable string representation to the console.
-
+### Apply
+Apply the filter and adjust function on the fetched transactions from YNAB via the `apply()` method. It 
+returns a filtered list of `ModifiedTransaction` which can be inspected for the changed properties via the 
+`changed_attributes` attribute. Only actually changed transactions are returned. 
 ```py
-mod_transactions = my_adjuster.dry_run()
+modified_transactions = my_adjuster.apply()
 ```
 
-### Run
-If you are satisfied with the functionality you can execute the adjuster with the `run()` method. This will run the 
-adjustments and will update the changed transactions in YNAB. The method returns an integer with the number of 
-successfully updated records.
+### Update
+The modified transactions can be upated in YNAB passing them to the `update()` function. The method returns an integer 
+with the number of successfully updated records.
 ```py
-count_of_updated_transactions = my_adjuster.run()
+modified_transactions = my_adjuster.apply()
+count_of_updated_transactions = my_adjuster.update(modified_transactions)
 ```
```

