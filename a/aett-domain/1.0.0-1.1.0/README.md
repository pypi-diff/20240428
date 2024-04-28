# Comparing `tmp/aett_domain-1.0.0.tar.gz` & `tmp/aett_domain-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett_domain-1.0.0.tar", last modified: Fri Apr 26 16:18:52 2024, max compression
+gzip compressed data, was "aett_domain-1.1.0.tar", last modified: Sun Apr 28 12:39:56 2024, max compression
```

## Comparing `aett_domain-1.0.0.tar` & `aett_domain-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:52.621385 aett_domain-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-26 16:18:47.000000 aett_domain-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 16:18:47.000000 aett_domain-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-26 16:18:52.621385 aett_domain-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-26 16:18:47.000000 aett_domain-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-26 16:18:47.000000 aett_domain-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:18:52.621385 aett_domain-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:52.617385 aett_domain-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:52.617385 aett_domain-1.0.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:52.617385 aett_domain-1.0.0/src/aett/domain/
--rw-r--r--   0 runner    (1001) docker     (127)    16637 2024-04-26 16:18:47.000000 aett_domain-1.0.0/src/aett/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:18:52.621385 aett_domain-1.0.0/src/aett_domain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-26 16:18:52.000000 aett_domain-1.0.0/src/aett_domain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-26 16:18:52.000000 aett_domain-1.0.0/src/aett_domain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:18:52.000000 aett_domain-1.0.0/src/aett_domain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 16:18:52.000000 aett_domain-1.0.0/src/aett_domain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 16:18:52.000000 aett_domain-1.0.0/src/aett_domain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:39:56.357047 aett_domain-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-28 12:39:50.000000 aett_domain-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 12:39:50.000000 aett_domain-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-28 12:39:56.353047 aett_domain-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-28 12:39:50.000000 aett_domain-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-28 12:39:50.000000 aett_domain-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:39:56.357047 aett_domain-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:39:56.353047 aett_domain-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:39:56.353047 aett_domain-1.1.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:39:56.353047 aett_domain-1.1.0/src/aett/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-04-28 12:39:50.000000 aett_domain-1.1.0/src/aett/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:39:56.353047 aett_domain-1.1.0/src/aett_domain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-28 12:39:56.000000 aett_domain-1.1.0/src/aett_domain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-28 12:39:56.000000 aett_domain-1.1.0/src/aett_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:39:56.000000 aett_domain-1.1.0/src/aett_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-28 12:39:56.000000 aett_domain-1.1.0/src/aett_domain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-28 12:39:56.000000 aett_domain-1.1.0/src/aett_domain.egg-info/top_level.txt
```

### Comparing `aett_domain-1.0.0/LICENSE` & `aett_domain-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett_domain-1.0.0/PKG-INFO` & `aett_domain-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-domain
-Version: 1.0.0
+Version: 1.1.0
 Summary: Domain modeling types aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: multipledispatch>=1.0.0
-Requires-Dist: aett-eventstore>=1.0.0
+Requires-Dist: aett-eventstore>=1.1.0
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

### Comparing `aett_domain-1.0.0/README.md` & `aett_domain-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aett_domain-1.0.0/pyproject.toml` & `aett_domain-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.domain"]
 
 [project]
 name = "aett-domain"
-version = "1.0.0"
+version = "1.1.0"
 description = "Domain modeling types aett event store"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "ddd", "domain"]
 dependencies = [
     'multipledispatch >= 1.0.0',
-    'aett-eventstore>=1.0.0'
+    'aett-eventstore>=1.1.0'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
 
 [project.urls]
```

### Comparing `aett_domain-1.0.0/src/aett/domain/__init__.py` & `aett_domain-1.1.0/src/aett/domain/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import uuid
 
 from aett.eventstore import *
 
 T = typing.TypeVar('T', bound=Memento)
 
 
@@ -10,26 +11,28 @@
     An aggregate is a cluster of domain objects that can be treated as a single unit. The aggregate base class requires
     implementors to provide a method to apply a snapshot and to get a memento.
 
     In addition to this, the aggregate base class provides a method to raise events, but the concrete application
     of the event relies on multiple dispatch to call the correct apply method in the subclass.
     """
 
-    def __init__(self, stream_id: str, commit_sequence: int):
+    def __init__(self, stream_id: str, commit_sequence: int, memento: Memento[T] = None):
         """
         Initialize the aggregate
 
         param stream_id: The id of the stream
         param commit_sequence: The commit sequence number which the aggregate was built from
         """
         self.uncommitted: typing.List[EventMessage] = []
         self._id = stream_id
         self._version = 0
         self._commit_sequence = commit_sequence
-        self.uncommitted.clear()
+        if memento is not None:
+            self._version = memento.version
+            self.apply_memento(memento)
 
     @property
     def id(self) -> str:
         """
         Gets the id of the aggregate
         """
         return self._id
@@ -89,14 +92,15 @@
     """
     A saga is a long-running process that coordinates multiple services to achieve a goal.
     The saga base class requires implementors to provide a method to apply events during state transition.
 
     In addition to this, the aggregate base class provides a method to raise events, but the concrete application
     of the event relies on multiple dispatch to call the correct apply method in the subclass.
     """
+
     def __init__(self, saga_id: str, commit_sequence: int):
         """
         Initialize the saga
 
         param saga_id: The id of the saga
         param commit_sequence: The commit sequence number which the saga was built from
         """
@@ -186,14 +190,21 @@
         pass
 
     @abstractmethod
     def save(self, aggregate: T, headers: Dict[str, str] = None) -> None:
         """
         Save the aggregate to the repository.
 
+        The call to save should be wrapped in a try-except block as concurrent modifications can cause a conflict with
+        events committed from a different source. A ConflictingCommitException will be thrown by the storage layer if
+        an attempt is made to save an aggregate with a version that is lower than the current version in the store and
+        the uncommitted events conflict with the committed events.A NonConflictingCommitException will be thrown if the
+        uncommitted events do not conflict with the committed events. In this case it should be safe to retry the
+        operation.
+
         :param aggregate: The aggregate to save.
         :param headers: The headers to assign to the commit.
         """
         pass
 
     @abstractmethod
     def snapshot(self, cls: typing.Type[TAggregate], stream_id: str, version: int, headers: Dict[str, str]) -> None:
@@ -241,164 +252,188 @@
         """
         Save the saga to the repository.
         """
         pass
 
 
 class DefaultAggregateRepository(AggregateRepository):
+    def __init__(self, tenant_id: str, store: ICommitEvents, snapshot_store: IAccessSnapshots,
+                 logger: logging.Logger = None):
+        """
+        Initialize the default aggregate repository.
 
-    def get(self, cls: typing.Type[AggregateRepository.TAggregate], stream_id: str, max_version: int = 2 ** 32) -> AggregateRepository.TAggregate:
-        memento_type = inspect.signature(cls.apply_memento).parameters['memento'].annotation
+        param tenant_id: The tenant id of the repository instance
+        param store: The event store to use
+        param snapshot_store: The snapshot store to use
+        """
+        self._tenant_id = tenant_id
+        self._store = store
+        self._snapshot_store = snapshot_store
+        self._logger = logger if logger is not None else logging.getLogger(DefaultAggregateRepository.__name__)
+
+    def get(self, cls: typing.Type[AggregateRepository.TAggregate], stream_id: str, max_version: int = 2 ** 32) -> \
+            AggregateRepository.TAggregate:
+        self._logger.info(f'Getting aggregate {cls.__name__} with id {stream_id} at version {max_version}')
         snapshot = self._snapshot_store.get(tenant_id=self._tenant_id, stream_id=stream_id, max_revision=max_version)
         min_version = 0
+        commit_sequence = 0
         if snapshot is not None:
-            min_version = snapshot.stream_revision
+            min_version = snapshot.stream_revision + 1
+            commit_sequence = snapshot.commit_sequence
         commits = list(self._store.get(tenant_id=self._tenant_id,
                                        stream_id=stream_id,
                                        min_revision=min_version,
                                        max_revision=max_version))
-        commit_sequence = commits[-1].commit_sequence if len(commits) > 0 else 0
-        aggregate = cls(stream_id, commit_sequence)
-        if snapshot is not None:
-            aggregate.apply_memento(memento_type(**jsonpickle.decode(snapshot.payload)))
+        if len(commits) > 0:
+            commit_sequence = commits[-1].commit_sequence
+        memento_type = inspect.signature(cls.apply_memento).parameters['memento'].annotation
+        aggregate = cls(stream_id, commit_sequence,
+                        memento_type(**jsonpickle.decode(snapshot.payload)) if snapshot is not None else None)
         for commit in commits:
             for event in commit.events:
                 aggregate.raise_event(event.body)
         aggregate.uncommitted.clear()
         return aggregate
 
     def get_to(self, cls: typing.Type[AggregateRepository.TAggregate], stream_id: str,
                max_time: datetime = datetime.datetime.max) -> AggregateRepository.TAggregate:
+        self._logger.info(
+            f'Getting aggregate {cls.__name__} with id {stream_id} at time point {max_time:%Y%m%d-%H%M%S%z}')
         commits = list(self._store.get_to(tenant_id=self._tenant_id,
                                           stream_id=stream_id,
                                           max_time=max_time))
         commit_sequence = commits[-1].commit_sequence if len(commits) > 0 else 0
-        aggregate = cls(stream_id, commit_sequence)
+        aggregate = cls(stream_id, commit_sequence, None)
         for commit in commits:
             for event in commit.events:
                 aggregate.raise_event(event.body)
         aggregate.uncommitted.clear()
         return aggregate
 
     def save(self, aggregate: AggregateRepository.TAggregate, headers: Dict[str, str] = None) -> None:
+        self._logger.info(f'Saving aggregate {aggregate.id} at version {aggregate.version}')
         if headers is None:
             headers = {}
         if len(aggregate.uncommitted) == 0:
             return
-        start_version = aggregate.version - len(aggregate.uncommitted)
-        persisted = list(self._store.get(self._tenant_id, aggregate.id, start_version))
-        persisted.sort(key=lambda c: c.stream_revision)
-        if len(persisted) == 0 and start_version != 0:
-            raise ValueError('Invalid version')
-        if len(persisted) > 0 and persisted[-1].stream_revision != start_version:
-            raise ValueError('Invalid version')
         commit = Commit(tenant_id=self._tenant_id,
                         stream_id=aggregate.id,
                         stream_revision=aggregate.version,
                         commit_id=uuid.uuid4(),
                         commit_sequence=aggregate.commit_sequence + 1,
                         commit_stamp=datetime.datetime.now(datetime.UTC),
                         headers=dict(headers),
                         events=list(aggregate.uncommitted),
                         checkpoint_token=0)
         self._store.commit(commit)
+        self._logger.info(f'Saved aggregate {aggregate.id}')
         aggregate.uncommitted.clear()
 
     def snapshot(self, cls: typing.Type[AggregateRepository.TAggregate], stream_id: str, version: int = MAX_INT,
                  headers: Dict[str, str] = None) -> None:
+        self._logger.info(f'Snapshotting aggregate {cls.__name__} with id {stream_id} at version {version}')
         agg = self.get(cls, stream_id, version)
         self._snapshot_aggregate(agg, headers)
 
     def snapshot_at(self, cls: typing.Type[AggregateRepository.TAggregate], stream_id: str, cut_off: datetime.datetime,
                     headers: Dict[str, str] = None) -> None:
+        self._logger.info(
+            f'Snapshotting aggregate {cls.__name__} with id {stream_id} at time point {cut_off:%Y%m%d-%H%M%S%z}')
         agg = self.get_to(cls, stream_id, cut_off)
         self._snapshot_aggregate(agg, headers)
 
     def _snapshot_aggregate(self, aggregate: Aggregate, headers: Dict[str, str] = None) -> None:
         memento = aggregate.get_memento()
-        snapshot = Snapshot(tenant_id=self._tenant_id, stream_id=aggregate.id,
-                            payload=jsonpickle.encode(memento.payload, unpicklable=False),
-                            stream_revision=memento.version, headers={})
+        snapshot = Snapshot(tenant_id=self._tenant_id,
+                            stream_id=aggregate.id,
+                            commit_sequence=aggregate.commit_sequence,
+                            payload=jsonpickle.encode(memento, unpicklable=False),
+                            stream_revision=memento.version,
+                            headers=headers or {})
         self._snapshot_store.add(snapshot=snapshot, headers=headers)
 
-    def __init__(self, tenant_id: str, store: ICommitEvents, snapshot_store: IAccessSnapshots):
-        """
-        Initialize the default aggregate repository.
-
-        param tenant_id: The tenant id of the repository instance
-        param store: The event store to use
-        param snapshot_store: The snapshot store to use
-        """
-        self._tenant_id = tenant_id
-        self._store = store
-        self._snapshot_store = snapshot_store
-
 
 class DefaultSagaRepository(SagaRepository):
 
-    def __init__(self, tenant_id: str, store: ICommitEvents):
+    def __init__(self, tenant_id: str, store: ICommitEvents, logger: logging.Logger = None):
         """
         Initialize the default saga repository.
 
         param tenant_id: The tenant id of the repository instance
         param store: The event store to use
         """
         self._tenant_id = tenant_id
         self._store = store
+        self._logger = logger if logger is not None else logging.getLogger(DefaultSagaRepository.__name__)
 
     def get(self, cls: typing.Type[SagaRepository.TSaga], stream_id: str) -> SagaRepository.TSaga:
+        self._logger.info(f'Getting saga {cls.__name__} with id {stream_id}')
         commits = list(self._store.get(self._tenant_id, stream_id))
         commit_sequence = commits[-1].commit_sequence if len(commits) > 0 else 0
         saga = cls(stream_id, commit_sequence)
         for commit in commits:
             for event in commit.events:
                 saga.transition(event.body)
         saga.uncommitted.clear()
         return saga
 
     def save(self, saga: Saga) -> None:
+        self._logger.info(f'Saving saga {saga.id} at version {saga.version}')
         commit = Commit(tenant_id=self._tenant_id,
                         stream_id=saga.id,
                         stream_revision=saga.version,
                         commit_id=uuid.uuid4(),
                         commit_sequence=saga.commit_sequence + 1,
                         commit_stamp=datetime.datetime.now(datetime.UTC),
                         headers=dict(saga.headers),
                         events=list(saga.uncommitted),
                         checkpoint_token=0)
         self._store.commit(commit=commit)
+        self._logger.info(f'Saved saga {saga.id}')
         saga.uncommitted.clear()
         saga.headers.clear()
 
 
 TUncommitted = typing.TypeVar('TUncommitted', bound=BaseEvent)
 TCommitted = typing.TypeVar('TCommitted', bound=BaseEvent)
 
 
 class ConflictDelegate(ABC, typing.Generic[TUncommitted, TCommitted]):
     """
     A conflict delegate is a class that can detect conflicts between two events.
     """
+
     @abstractmethod
     def detect(self, uncommitted: TUncommitted, committed: TCommitted) -> bool:
         """
-        Detects if the uncommitted event conflicts with the committed event.
+        Detects if the uncommitted event conflicts with the committed event. The delegate should return True if an event
+        is incompatible with a previously persisted event.
+
+        If the delegate returns False then it is assumed that the later event is compatible with the previously
+        persisted.
         """
         pass
 
 
 class ConflictDetector:
-    def __init__(self, delegates: typing.List[ConflictDelegate] = None):
+    @staticmethod
+    def empty() -> 'ConflictDetector':
+        return ConflictDetector()
+
+    def __init__(self, delegates: typing.List[ConflictDelegate] = None, logger: logging.Logger = None):
         """
         Initialize the conflict detector with the specified delegates.
 
         param delegates: The delegates to use for conflict detection
+        param logger: The optional logger to use for logging.
         """
         self.delegates: typing.Dict[
             typing.Type, typing.Dict[typing.Type, typing.Callable[[BaseEvent, BaseEvent], bool]]] = {}
+        self._logger = logger if logger is not None and delegates is not None else logging.getLogger(
+            ConflictDetector.__name__)
         if delegates is not None:
             for delegate in delegates:
                 args = inspect.getfullargspec(delegate.detect)
                 uncommitted_type = args.annotations[args.args[1]]
                 committed_type = args.annotations[args.args[2]]
                 if uncommitted_type not in self.delegates:
                     self.delegates[uncommitted_type] = {}
@@ -415,33 +450,42 @@
         """
         if len(self.delegates) == 0:
             return False
         for uncommitted in uncommitted_events:
             for committed in committed_events:
                 if type(uncommitted) in self.delegates and type(committed) in self.delegates[type(uncommitted)]:
                     if self.delegates[type(uncommitted)][type(committed)](uncommitted, committed):
+                        if isinstance(uncommitted, DomainEvent):
+                            self._logger.warning(
+                                f'Detected conflict between uncommitted event {type(uncommitted).__name__} from {uncommitted.source} with version {uncommitted.version}')
+                        else:
+                            self._logger.warning(
+                                f'Detected conflict between uncommitted event {type(uncommitted).__name__} from {uncommitted.source} with timestamp {uncommitted.timestamp:%Y%m%d-%H%M%S%z}')
                         return True
         return False
 
 
 class DuplicateCommitException(Exception):
     """
     Exception raised when a duplicate commit is detected.
     """
+
     def __init__(self, message: str):
         super().__init__(message)
 
 
 class ConflictingCommitException(Exception):
     """
     Exception raised when a conflicting commit is detected.
     """
+
     def __init__(self, message: str):
         super().__init__(message)
 
 
 class NonConflictingCommitException(Exception):
     """
     Exception raised when a non-conflicting commit is detected.
     """
+
     def __init__(self, message: str):
         super().__init__(message)
```

### Comparing `aett_domain-1.0.0/src/aett_domain.egg-info/PKG-INFO` & `aett_domain-1.1.0/src/aett_domain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-domain
-Version: 1.0.0
+Version: 1.1.0
 Summary: Domain modeling types aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: multipledispatch>=1.0.0
-Requires-Dist: aett-eventstore>=1.0.0
+Requires-Dist: aett-eventstore>=1.1.0
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

