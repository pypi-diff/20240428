# Comparing `tmp/blinker-1.8.0.tar.gz` & `tmp/blinker-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blinker-1.8.0.tar", last modified: Sat Apr 27 17:47:47 2024, max compression
+gzip compressed data, was "blinker-1.8.1.tar", last modified: Sun Apr 28 20:04:27 2024, max compression
```

## Comparing `blinker-1.8.0.tar` & `blinker-1.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     4339 2024-04-27 17:47:47.000000 blinker-1.8.0/CHANGES.rst
--rw-r--r--   0        0        0     1054 2024-04-27 17:47:47.000000 blinker-1.8.0/LICENSE.txt
--rw-r--r--   0        0        0     1021 2024-04-27 17:47:47.000000 blinker-1.8.0/README.md
--rw-r--r--   0        0        0     3627 2024-04-27 17:47:47.000000 blinker-1.8.0/docs/_static/blinker-named.png
--rw-r--r--   0        0        0     1437 2024-04-27 17:47:47.000000 blinker-1.8.0/docs/conf.py
--rw-r--r--   0        0        0     9905 2024-04-27 17:47:47.000000 blinker-1.8.0/docs/index.rst
--rw-r--r--   0        0        0     1695 2024-04-27 17:47:47.000000 blinker-1.8.0/pyproject.toml
--rw-r--r--   0        0        0        6 2024-04-27 17:47:47.000000 blinker-1.8.0/requirements/build.in
--rw-r--r--   0        0        0      227 2024-04-27 17:47:47.000000 blinker-1.8.0/requirements/build.txt
--rw-r--r--   0        0        0       54 2024-04-27 17:47:47.000000 blinker-1.8.0/requirements/dev.in
--rw-r--r--   0        0        0     3010 2024-04-27 17:47:47.000000 blinker-1.8.0/requirements/dev.txt
--rw-r--r--   0        0        0       55 2024-04-27 17:47:47.000000 blinker-1.8.0/requirements/docs.in
--rw-r--r--   0        0        0     1141 2024-04-27 17:47:47.000000 blinker-1.8.0/requirements/docs.txt
--rw-r--r--   0        0        0       22 2024-04-27 17:47:47.000000 blinker-1.8.0/requirements/tests.in
--rw-r--r--   0        0        0      331 2024-04-27 17:47:47.000000 blinker-1.8.0/requirements/tests.txt
--rw-r--r--   0        0        0       20 2024-04-27 17:47:47.000000 blinker-1.8.0/requirements/typing.in
--rw-r--r--   0        0        0      536 2024-04-27 17:47:47.000000 blinker-1.8.0/requirements/typing.txt
--rw-r--r--   0        0        0     1577 2024-04-27 17:47:47.000000 blinker-1.8.0/src/blinker/__init__.py
--rw-r--r--   0        0        0     1164 2024-04-27 17:47:47.000000 blinker-1.8.0/src/blinker/_utilities.py
--rw-r--r--   0        0        0    20498 2024-04-27 17:47:47.000000 blinker-1.8.0/src/blinker/base.py
--rw-r--r--   0        0        0        0 2024-04-27 17:47:47.000000 blinker-1.8.0/src/blinker/py.typed
--rw-r--r--   0        0        0     1237 2024-04-27 17:47:47.000000 blinker-1.8.0/tests/test_context.py
--rw-r--r--   0        0        0    11795 2024-04-27 17:47:47.000000 blinker-1.8.0/tests/test_signals.py
--rw-r--r--   0        0        0      503 2024-04-27 17:47:47.000000 blinker-1.8.0/tests/test_symbol.py
--rw-r--r--   0        0        0     1044 2024-04-27 17:47:47.000000 blinker-1.8.0/tox.ini
--rw-r--r--   0        0        0     1633 1970-01-01 00:00:00.000000 blinker-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     4803 2024-04-28 20:04:27.000000 blinker-1.8.1/CHANGES.rst
+-rw-r--r--   0        0        0     1054 2024-04-28 20:04:27.000000 blinker-1.8.1/LICENSE.txt
+-rw-r--r--   0        0        0     1021 2024-04-28 20:04:27.000000 blinker-1.8.1/README.md
+-rw-r--r--   0        0        0     3627 2024-04-28 20:04:27.000000 blinker-1.8.1/docs/_static/blinker-named.png
+-rw-r--r--   0        0        0     1410 2024-04-28 20:04:27.000000 blinker-1.8.1/docs/conf.py
+-rw-r--r--   0        0        0    10352 2024-04-28 20:04:27.000000 blinker-1.8.1/docs/index.rst
+-rw-r--r--   0        0        0     1695 2024-04-28 20:04:27.000000 blinker-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0        6 2024-04-28 20:04:27.000000 blinker-1.8.1/requirements/build.in
+-rw-r--r--   0        0        0      227 2024-04-28 20:04:27.000000 blinker-1.8.1/requirements/build.txt
+-rw-r--r--   0        0        0       54 2024-04-28 20:04:27.000000 blinker-1.8.1/requirements/dev.in
+-rw-r--r--   0        0        0     3010 2024-04-28 20:04:27.000000 blinker-1.8.1/requirements/dev.txt
+-rw-r--r--   0        0        0       55 2024-04-28 20:04:27.000000 blinker-1.8.1/requirements/docs.in
+-rw-r--r--   0        0        0     1141 2024-04-28 20:04:27.000000 blinker-1.8.1/requirements/docs.txt
+-rw-r--r--   0        0        0       22 2024-04-28 20:04:27.000000 blinker-1.8.1/requirements/tests.in
+-rw-r--r--   0        0        0      331 2024-04-28 20:04:27.000000 blinker-1.8.1/requirements/tests.txt
+-rw-r--r--   0        0        0       20 2024-04-28 20:04:27.000000 blinker-1.8.1/requirements/typing.in
+-rw-r--r--   0        0        0      536 2024-04-28 20:04:27.000000 blinker-1.8.1/requirements/typing.txt
+-rw-r--r--   0        0        0     1577 2024-04-28 20:04:27.000000 blinker-1.8.1/src/blinker/__init__.py
+-rw-r--r--   0        0        0     1675 2024-04-28 20:04:27.000000 blinker-1.8.1/src/blinker/_utilities.py
+-rw-r--r--   0        0        0    22698 2024-04-28 20:04:27.000000 blinker-1.8.1/src/blinker/base.py
+-rw-r--r--   0        0        0        0 2024-04-28 20:04:27.000000 blinker-1.8.1/src/blinker/py.typed
+-rw-r--r--   0        0        0     1237 2024-04-28 20:04:27.000000 blinker-1.8.1/tests/test_context.py
+-rw-r--r--   0        0        0    11890 2024-04-28 20:04:27.000000 blinker-1.8.1/tests/test_signals.py
+-rw-r--r--   0        0        0      503 2024-04-28 20:04:27.000000 blinker-1.8.1/tests/test_symbol.py
+-rw-r--r--   0        0        0     1095 2024-04-28 20:04:27.000000 blinker-1.8.1/tox.ini
+-rw-r--r--   0        0        0     1633 1970-01-01 00:00:00.000000 blinker-1.8.1/PKG-INFO
```

### Comparing `blinker-1.8.0/CHANGES.rst` & `blinker-1.8.1/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Version 1.8.1
+-------------
+
+Released 2024-04-28
+
+-   Restore identity handling for ``str`` and ``int`` senders. :pr:`148`
+-   Fix deprecated ``blinker.base.WeakNamespace`` import. :pr:`149`
+-   Fix deprecated ``blinker.base.receiver_connected import``. :pr:`153`
+-   Use types from ``collections.abc`` instead of ``typing``. :pr:`150`
+-   Fully specify exported types as reported by pyright. :pr:`152`
+
+
 Version 1.8.0
 -------------
 
 Released 2024-04-27
 
 -   Deprecate the ``__version__`` attribute. Use feature detection, or
     ``importlib.metadata.version("blinker")``, instead. :issue:`128`
@@ -20,58 +32,63 @@
 Version 1.7.0
 -------------
 
 Released 2023-11-01
 
 -   Fixed messages printed to standard error about unraisable exceptions during
     signal cleanup, typically during interpreter shutdown. :pr:`123`
--   Allow the Signal set_class to be customised, to allow calling of receivers
-    in registration order. :pr:`116`.
+-   Allow the Signal ``set_class`` to be customised, to allow calling of
+    receivers in registration order. :pr:`116`.
 -   Drop Python 3.7 and support Python 3.12. :pr:`126`
 
+
 Version 1.6.3
 -------------
 
 Released 2023-09-23
 
--   Fix `SyncWrapperType` and `AsyncWrapperType` :pr:`108`
--   Fixed issue where ``signal.connected_to`` would not disconnect the
-    receiver if an instance of ``BaseException`` was raised. :pr:`114`
+-   Fix ``SyncWrapperType`` and ``AsyncWrapperType`` :pr:`108`
+-   Fixed issue where ``connected_to`` would not disconnect the receiver if an
+    instance of ``BaseException`` was raised. :pr:`114`
+
 
 Version 1.6.2
 -------------
 
 Released 2023-04-12
 
--   Type annotations are not evaluated at runtime. typing-extensions is not a runtime
-    dependency. :pr:`94`
+-   Type annotations are not evaluated at runtime. typing-extensions is not a
+    runtime dependency. :pr:`94`
+
 
 Version 1.6.1
 -------------
 
 Released 2023-04-09
 
--   Ensure that py.typed is present in the distributions (to enable other
-    projects to use blinker's typing).
--   Require typing-extensions > 4.2 to ensure it includes
-    ParamSpec. :issue:`90`
+-   Ensure that ``py.typed`` is present in the distributions (to enable other
+    projects to use Blinker's typing).
+-   Require typing-extensions > 4.2 to ensure it includes ``ParamSpec``.
+    :issue:`90`
+
 
 Version 1.6
 -----------
 
 Released 2023-04-02
 
--   Add a muted context manager to temporarily turn off a
-    signal. :pr:`84`
--   Allow int senders (alongside existing string senders). :pr:`83`
--   Add a send_async method to the Signal to allow signals to send to
-    coroutine receivers. :pr:`76`
--   Update and modernise the project structure to match that used by the
-    pallets projects. :pr:`77`
--   Add an intial set of type hints for the project.
+-   Add a ``muted`` context manager to temporarily turn off a signal. :pr:`84`
+-   ``int`` instances with the same value will be treated as the same sender,
+    the same as ``str`` instances. :pr:`83`
+-   Add a ``send_async`` method to allow signals to send to coroutine receivers.
+    :pr:`76`
+-   Update and modernise the project structure to match that used by the Pallets
+    projects. :pr:`77`
+-   Add an initial set of type hints for the project.
+
 
 Version 1.5
 -----------
 
 Released 2022-07-17
 
 -   Support Python >= 3.7 and PyPy. Python 2, Python < 3.7, and Jython
```

### Comparing `blinker-1.8.0/LICENSE.txt` & `blinker-1.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blinker-1.8.0/README.md` & `blinker-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `blinker-1.8.0/docs/_static/blinker-named.png` & `blinker-1.8.1/docs/_static/blinker-named.png`

 * *Files identical despite different names*

### Comparing `blinker-1.8.0/docs/conf.py` & `blinker-1.8.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 default_role = "code"
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.extlinks",
     "sphinxcontrib.log_cabinet",
     "pallets_sphinx_themes",
 ]
-autoclass_content = "both"
 autodoc_member_order = "groupwise"
 autodoc_typehints = "description"
 autodoc_preserve_defaults = True
 extlinks = {
     "issue": ("https://github.com/pallets-eco/blinker/issues/%s", "#%s"),
     "pr": ("https://github.com/pallets-eco/blinker/pull/%s", "#%s"),
 }
```

### Comparing `blinker-1.8.0/docs/index.rst` & `blinker-1.8.1/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 Blinker Documentation
 =====================
 
 .. image:: _static/blinker-named.png
     :align: center
 
+.. currentmodule:: blinker
+
 Blinker provides fast & simple object-to-object and broadcast
 signaling for Python objects.
 
 The core of Blinker is quite small but provides powerful features:
 
  - a global registry of named signals
  - anonymous signals
@@ -353,35 +355,46 @@
 API Documentation
 -----------------
 
 All public API members can (and should) be imported from ``blinker``::
 
   from blinker import ANY, signal
 
-.. currentmodule:: blinker.base
-
 Basic Signals
 +++++++++++++
 
-.. autodata:: blinker.base.ANY
+.. data:: ANY
+
+    Symbol for "any sender".
 
 .. autoclass:: Signal
    :members:
-   :undoc-members:
 
 Named Signals
 +++++++++++++
 
-.. autofunction:: signal
+.. function:: signal(name, doc=None)
 
-.. autodata:: default_namespace
+    Return a :class:`NamedSignal` in :data:`default_namespace` for the given
+    name, creating it if required. Repeated calls with the same name return the
+    same signal.
+
+    :param name: The name of the signal.
+    :type name: str
+    :param doc: The docstring of the signal.
+    :type doc: str | None
+    :rtype: NamedSignal
+
+.. data:: default_namespace
+
+    A default :class:`Namespace` for creating named signals. :func:`signal`
+    creates a :class:`NamedSignal` in this namespace.
 
 .. autoclass:: NamedSignal
    :show-inheritance:
-   :members:
 
 .. autoclass:: Namespace
    :show-inheritance:
    :members: signal
 
 
 Changes
```

### Comparing `blinker-1.8.0/pyproject.toml` & `blinker-1.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "blinker"
-version = "1.8.0"
+version = "1.8.1"
 description = "Fast, simple object-to-object and broadcast signaling"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 authors = [{ name = "Jason Kirtland" }]
 maintainers = [{ name = "Pallets Ecosystem", email = "contact@palletsprojects.com" }]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `blinker-1.8.0/requirements/dev.txt` & `blinker-1.8.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `blinker-1.8.0/requirements/docs.txt` & `blinker-1.8.1/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `blinker-1.8.0/requirements/typing.txt` & `blinker-1.8.1/requirements/typing.txt`

 * *Files identical despite different names*

### Comparing `blinker-1.8.0/src/blinker/__init__.py` & `blinker-1.8.1/src/blinker/__init__.py`

 * *Files identical despite different names*

### Comparing `blinker-1.8.0/src/blinker/base.py` & `blinker-1.8.1/src/blinker/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,131 +1,126 @@
-"""Signals and events.
-
-A small implementation of signals, inspired by a snippet of Django signal
-API client code seen in a blog post.  Signals are first-class objects and
-each manages its own receivers and message emission.
-
-The :func:`signal` function provides singleton behavior for named signals.
-"""
-
 from __future__ import annotations
 
+import collections.abc as c
 import typing as t
 import warnings
 import weakref
 from collections import defaultdict
+from contextlib import AbstractContextManager
 from contextlib import contextmanager
 from functools import cached_property
 from inspect import iscoroutinefunction
 from weakref import WeakValueDictionary
 
 from ._utilities import make_id
 from ._utilities import make_ref
 from ._utilities import Symbol
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
 
-    F = t.TypeVar("F", bound=t.Callable[..., t.Any])
+    F = t.TypeVar("F", bound=c.Callable[..., t.Any])
     T = t.TypeVar("T")
     P = te.ParamSpec("P")
 
     class PAsyncWrapper(t.Protocol):
-        def __call__(self, f: t.Callable[P, t.Awaitable[T]]) -> t.Callable[P, T]: ...
+        def __call__(self, f: c.Callable[P, c.Awaitable[T]]) -> c.Callable[P, T]: ...
 
     class PSyncWrapper(t.Protocol):
-        def __call__(self, f: t.Callable[P, T]) -> t.Callable[P, t.Awaitable[T]]: ...
+        def __call__(self, f: c.Callable[P, T]) -> c.Callable[P, c.Awaitable[T]]: ...
 
 
 ANY = Symbol("ANY")
-"""Token for "any sender"."""
+"""Symbol for "any sender"."""
+
 ANY_ID = 0
 
 
 class Signal:
-    """A notification emitter."""
+    """A notification emitter.
+
+    :param doc: The docstring for the signal.
+    """
 
-    #: An :obj:`ANY` convenience synonym, allows ``Signal.ANY``
-    #: without an additional import.
     ANY = ANY
+    """An alias for the :data:`~blinker.ANY` sender symbol."""
 
     set_class: type[set[t.Any]] = set
+    """The set class to use for tracking connected receivers and senders.
+    Python's ``set`` is unordered. If receivers must be dispatched in the order
+    they were connected, an ordered set implementation can be used.
+
+    .. versionadded:: 1.7
+    """
 
     @cached_property
     def receiver_connected(self) -> Signal:
-        """Emitted after each :meth:`connect`.
+        """Emitted at the end of each :meth:`connect` call.
 
         The signal sender is the signal instance, and the :meth:`connect`
-        arguments are passed through: *receiver*, *sender*, and *weak*.
+        arguments are passed through: ``receiver``, ``sender``, and ``weak``.
 
         .. versionadded:: 1.2
         """
         return Signal(doc="Emitted after a receiver connects.")
 
     @cached_property
     def receiver_disconnected(self) -> Signal:
-        """Emitted after :meth:`disconnect`.
+        """Emitted at the end of each :meth:`disconnect` call.
 
         The sender is the signal instance, and the :meth:`disconnect` arguments
-        are passed through: *receiver* and *sender*.
-
-        Note, this signal is emitted **only** when :meth:`disconnect` is
-        called explicitly.
+        are passed through: ``receiver`` and ``sender``.
 
-        The disconnect signal can not be emitted by an automatic disconnect
-        (due to a weakly referenced receiver or sender going out of scope),
-        as the receiver and/or sender instances are no longer available for
-        use at the time this signal would be emitted.
+        This signal is emitted **only** when :meth:`disconnect` is called
+        explicitly. This signal cannot be emitted by an automatic disconnect
+        when a weakly referenced receiver or sender goes out of scope, as the
+        instance is no longer be available to be used as the sender for this
+        signal.
 
         An alternative approach is available by subscribing to
         :attr:`receiver_connected` and setting up a custom weakref cleanup
         callback on weak receivers and senders.
 
         .. versionadded:: 1.2
         """
         return Signal(doc="Emitted after a receiver disconnects.")
 
     def __init__(self, doc: str | None = None) -> None:
-        """
-        :param doc: Set the instance's ``__doc__`` attribute for documentation.
-        """
         if doc:
             self.__doc__ = doc
 
-        #: A mapping of connected receivers.
-        #:
-        #: The values of this mapping are not meaningful outside of the
-        #: internal :class:`Signal` implementation, however the boolean value
-        #: of the mapping is useful as an extremely efficient check to see if
-        #: any receivers are connected to the signal.
         self.receivers: dict[
-            t.Any, weakref.ref[t.Callable[..., t.Any]] | t.Callable[..., t.Any]
+            t.Any, weakref.ref[c.Callable[..., t.Any]] | c.Callable[..., t.Any]
         ] = {}
+        """The map of connected receivers. Useful to quickly check if any
+        receivers are connected to the signal: ``if s.receivers:``. The
+        structure and data is not part of the public API, but checking its
+        boolean value is.
+        """
+
         self.is_muted: bool = False
         self._by_receiver: dict[t.Any, set[t.Any]] = defaultdict(self.set_class)
         self._by_sender: dict[t.Any, set[t.Any]] = defaultdict(self.set_class)
         self._weak_senders: dict[t.Any, weakref.ref[t.Any]] = {}
 
     def connect(self, receiver: F, sender: t.Any = ANY, weak: bool = True) -> F:
-        """Connect *receiver* to signal events sent by *sender*.
+        """Connect ``receiver`` to be called when the signal is sent by
+        ``sender``.
 
-        :param receiver: A callable.  Will be invoked by :meth:`send` with
-          `sender=` as a single positional argument and any ``kwargs`` that
-          were provided to a call to :meth:`send`.
-
-        :param sender: Any object or :obj:`ANY`, defaults to ``ANY``.
-          Restricts notifications delivered to *receiver* to only those
-          :meth:`send` emissions sent by *sender*.  If ``ANY``, the receiver
-          will always be notified.  A *receiver* may be connected to
-          multiple *sender* values on the same Signal through multiple calls
-          to :meth:`connect`.
-
-        :param weak: If true, the Signal will hold a weakref to *receiver*
-          and automatically disconnect when *receiver* goes out of scope or
-          is garbage collected.  Defaults to True.
+        :param receiver: The callable to call when :meth:`send` is called with
+            the given ``sender``, passing ``sender`` as a positional argument
+            along with any extra keyword arguments.
+        :param sender: Any object or :data:`ANY`. ``receiver`` will only be
+            called when :meth:`send` is called with this sender. If ``ANY``, the
+            receiver will be called for any sender. A receiver may be connected
+            to multiple senders by calling :meth:`connect` multiple times.
+        :param weak: Track the receiver with a :mod:`weakref`. The receiver will
+            be automatically disconnected when it is garbage collected. When
+            connecting a receiver defined within a function, set to ``False``,
+            otherwise it will be disconnected when the function scope ends.
         """
         receiver_id = make_id(receiver)
         sender_id = ANY_ID if sender is ANY else make_id(sender)
 
         if weak:
             self.receivers[receiver_id] = make_ref(
                 receiver, self._make_cleanup_receiver(receiver_id)
@@ -162,95 +157,86 @@
                 )
             except TypeError:
                 self.disconnect(receiver, sender)
                 raise
 
         return receiver
 
-    def connect_via(self, sender: t.Any, weak: bool = False) -> t.Callable[[F], F]:
-        """Connect the decorated function as a receiver for *sender*.
-
-        :param sender: Any object or :obj:`ANY`.  The decorated function
-          will only receive :meth:`send` emissions sent by *sender*.  If
-          ``ANY``, the receiver will always be notified.  A function may be
-          decorated multiple times with differing *sender* values.
-
-        :param weak: If true, the Signal will hold a weakref to the
-          decorated function and automatically disconnect when *receiver*
-          goes out of scope or is garbage collected.  Unlike
-          :meth:`connect`, this defaults to False.
-
-        The decorated function will be invoked by :meth:`send` with
-          `sender=` as a single positional argument and any ``kwargs`` that
-          were provided to the call to :meth:`send`.
-
+    def connect_via(self, sender: t.Any, weak: bool = False) -> c.Callable[[F], F]:
+        """Connect the decorated function to be called when the signal is sent
+        by ``sender``.
+
+        The decorated function will be called when :meth:`send` is called with
+        the given ``sender``, passing ``sender`` as a positional argument along
+        with any extra keyword arguments.
+
+        :param sender: Any object or :data:`ANY`. ``receiver`` will only be
+            called when :meth:`send` is called with this sender. If ``ANY``, the
+            receiver will be called for any sender. A receiver may be connected
+            to multiple senders by calling :meth:`connect` multiple times.
+        :param weak: Track the receiver with a :mod:`weakref`. The receiver will
+            be automatically disconnected when it is garbage collected. When
+            connecting a receiver defined within a function, set to ``False``,
+            otherwise it will be disconnected when the function scope ends.=
 
         .. versionadded:: 1.1
         """
 
         def decorator(fn: F) -> F:
             self.connect(fn, sender, weak)
             return fn
 
         return decorator
 
     @contextmanager
     def connected_to(
-        self, receiver: t.Callable[..., t.Any], sender: t.Any = ANY
-    ) -> t.Generator[None, None, None]:
-        """Execute a block with the signal temporarily connected to *receiver*.
-
-        :param receiver: a receiver callable
-        :param sender: optional, a sender to filter on
-
-        This is a context manager for use in the ``with`` statement.  It can
-        be useful in unit tests.  *receiver* is connected to the signal for
-        the duration of the ``with`` block, and will be disconnected
-        automatically when exiting the block:
-
-        .. code-block:: python
-
-          with on_ready.connected_to(receiver):
-             # do stuff
-             on_ready.send(123)
+        self, receiver: c.Callable[..., t.Any], sender: t.Any = ANY
+    ) -> c.Generator[None, None, None]:
+        """A context manager that temporarily connects ``receiver`` to the
+        signal while a ``with`` block executes. When the block exits, the
+        receiver is disconnected. Useful for tests.
+
+        :param receiver: The callable to call when :meth:`send` is called with
+            the given ``sender``, passing ``sender`` as a positional argument
+            along with any extra keyword arguments.
+        :param sender: Any object or :data:`ANY`. ``receiver`` will only be
+            called when :meth:`send` is called with this sender. If ``ANY``, the
+            receiver will be called for any sender.
 
         .. versionadded:: 1.1
-
         """
         self.connect(receiver, sender=sender, weak=False)
 
         try:
             yield None
         finally:
             self.disconnect(receiver)
 
     @contextmanager
-    def muted(self) -> t.Generator[None, None, None]:
-        """Context manager for temporarily disabling signal.
-        Useful for test purposes.
+    def muted(self) -> c.Generator[None, None, None]:
+        """A context manager that temporarily disables the signal. No receivers
+        will be called if the signal is sent, until the ``with`` block exits.
+        Useful for tests.
         """
         self.is_muted = True
 
         try:
             yield None
         finally:
             self.is_muted = False
 
     def temporarily_connected_to(
-        self, receiver: t.Callable[..., t.Any], sender: t.Any = ANY
-    ) -> t.ContextManager[None]:
-        """An alias for :meth:`connected_to`.
-
-        :param receiver: a receiver callable
-        :param sender: optional, a sender to filter on
-
-        .. versionadded:: 0.9
+        self, receiver: c.Callable[..., t.Any], sender: t.Any = ANY
+    ) -> AbstractContextManager[None]:
+        """Deprecated alias for :meth:`connected_to`.
 
         .. deprecated:: 1.1
             Renamed to ``connected_to``. Will be removed in Blinker 1.9.
+
+        .. versionadded:: 0.9
         """
         warnings.warn(
             "'temporarily_connected_to' is renamed to 'connected_to'. The old name is"
             " deprecated and will be removed in Blinker 1.9.",
             DeprecationWarning,
             stacklevel=2,
         )
@@ -259,26 +245,36 @@
     def send(
         self,
         sender: t.Any | None = None,
         /,
         *,
         _async_wrapper: PAsyncWrapper | None = None,
         **kwargs: t.Any,
-    ) -> list[tuple[t.Callable[..., t.Any], t.Any]]:
-        """Emit this signal on behalf of *sender*, passing on ``kwargs``.
+    ) -> list[tuple[c.Callable[..., t.Any], t.Any]]:
+        """Call all receivers that are connected to the given ``sender``
+        or :data:`ANY`. Each receiver is called with ``sender`` as a positional
+        argument along with any extra keyword arguments. Return a list of
+        ``(receiver, return value)`` tuples.
+
+        The order receivers are called is undefined, but can be influenced by
+        setting :attr:`set_class`.
+
+        If a receiver raises an exception, that exception will propagate up.
+        This makes debugging straightforward, with an assumption that correctly
+        implemented receivers will not raise.
+
+        :param sender: Call receivers connected to this sender, in addition to
+            those connected to :data:`ANY`.
+        :param _async_wrapper: Will be called on any receivers that are async
+            coroutines to turn them into sync callables. For example, could run
+            the receiver with an event loop.
+        :param kwargs: Extra keyword arguments to pass to each receiver.
 
-        Returns a list of 2-tuples, pairing receivers with their return
-        value. The ordering of receiver notification is undefined.
-
-        :param sender: Any object or ``None``.  If omitted, synonymous
-          with ``None``.  Only accepts one positional argument.
-        :param _async_wrapper: A callable that should wrap a coroutine
-          receiver and run it when called synchronously.
-
-        :param kwargs: Data to be sent to receivers.
+        .. versionchanged:: 1.7
+            Added the ``_async_wrapper`` argument.
         """
         if self.is_muted:
             return []
 
         results = []
 
         for receiver in self.receivers_for(sender):
@@ -297,26 +293,35 @@
     async def send_async(
         self,
         sender: t.Any | None = None,
         /,
         *,
         _sync_wrapper: PSyncWrapper | None = None,
         **kwargs: t.Any,
-    ) -> list[tuple[t.Callable[..., t.Any], t.Any]]:
-        """Emit this signal on behalf of *sender*, passing on ``kwargs``.
-
-        Returns a list of 2-tuples, pairing receivers with their return
-        value. The ordering of receiver notification is undefined.
+    ) -> list[tuple[c.Callable[..., t.Any], t.Any]]:
+        """Await all receivers that are connected to the given ``sender``
+        or :data:`ANY`. Each receiver is called with ``sender`` as a positional
+        argument along with any extra keyword arguments. Return a list of
+        ``(receiver, return value)`` tuples.
+
+        The order receivers are called is undefined, but can be influenced by
+        setting :attr:`set_class`.
+
+        If a receiver raises an exception, that exception will propagate up.
+        This makes debugging straightforward, with an assumption that correctly
+        implemented receivers will not raise.
+
+        :param sender: Call receivers connected to this sender, in addition to
+            those connected to :data:`ANY`.
+        :param _sync_wrapper: Will be called on any receivers that are sync
+            callables to turn them into async coroutines. For example,
+            could call the receiver in a thread.
+        :param kwargs: Extra keyword arguments to pass to each receiver.
 
-        :param sender: Any object or ``None``.  If omitted, synonymous
-          with ``None``. Only accepts one positional argument.
-        :param _sync_wrapper: A callable that should wrap a synchronous
-          receiver and run it when awaited.
-
-        :param kwargs: Data to be sent to receivers.
+        .. versionadded:: 1.7
         """
         if self.is_muted:
             return []
 
         results = []
 
         for receiver in self.receivers_for(sender):
@@ -329,36 +334,44 @@
                 result = await receiver(sender, **kwargs)
 
             results.append((receiver, result))
 
         return results
 
     def has_receivers_for(self, sender: t.Any) -> bool:
-        """True if there is probably a receiver for *sender*.
-
-        Performs an optimistic check only.  Does not guarantee that all
-        weakly referenced receivers are still alive.  See
-        :meth:`receivers_for` for a stronger search.
+        """Check if there is at least one receiver that will be called with the
+        given ``sender``. A receiver connected to :data:`ANY` will always be
+        called, regardless of sender. Does not check if weakly referenced
+        receivers are still live. See :meth:`receivers_for` for a stronger
+        search.
 
+        :param sender: Check for receivers connected to this sender, in addition
+            to those connected to :data:`ANY`.
         """
         if not self.receivers:
             return False
 
         if self._by_sender[ANY_ID]:
             return True
 
         if sender is ANY:
             return False
 
         return make_id(sender) in self._by_sender
 
     def receivers_for(
         self, sender: t.Any
-    ) -> t.Generator[t.Callable[..., t.Any], None, None]:
-        """Iterate all live receivers listening for *sender*."""
+    ) -> c.Generator[c.Callable[..., t.Any], None, None]:
+        """Yield each receiver to be called for ``sender``, in addition to those
+        to be called for :data:`ANY`. Weakly referenced receivers that are not
+        live will be disconnected and skipped.
+
+        :param sender: Yield receivers connected to this sender, in addition
+            to those connected to :data:`ANY`.
+        """
         # TODO: test receivers_for(ANY)
         if not self.receivers:
             return
 
         sender_id = make_id(sender)
 
         if sender_id in self._by_sender:
@@ -379,24 +392,23 @@
                     self._disconnect(receiver_id, ANY_ID)
                     continue
 
                 yield strong
             else:
                 yield receiver
 
-    def disconnect(self, receiver: t.Callable[..., t.Any], sender: t.Any = ANY) -> None:
-        """Disconnect *receiver* from this signal's events.
-
-        :param receiver: a previously :meth:`connected<connect>` callable
-
-        :param sender: a specific sender to disconnect from, or :obj:`ANY`
-          to disconnect from all senders.  Defaults to ``ANY``.
-
+    def disconnect(self, receiver: c.Callable[..., t.Any], sender: t.Any = ANY) -> None:
+        """Disconnect ``receiver`` from being called when the signal is sent by
+        ``sender``.
+
+        :param receiver: A connected receiver callable.
+        :param sender: Disconnect from only this sender. By default, disconnect
+            from all senders.
         """
-        sender_id: t.Hashable
+        sender_id: c.Hashable
 
         if sender is ANY:
             sender_id = ANY_ID
         else:
             sender_id = make_id(sender)
 
         receiver_id = make_id(receiver)
@@ -404,77 +416,81 @@
 
         if (
             "receiver_disconnected" in self.__dict__
             and self.receiver_disconnected.receivers
         ):
             self.receiver_disconnected.send(self, receiver=receiver, sender=sender)
 
-    def _disconnect(self, receiver_id: t.Hashable, sender_id: t.Hashable) -> None:
+    def _disconnect(self, receiver_id: c.Hashable, sender_id: c.Hashable) -> None:
         if sender_id == ANY_ID:
             if self._by_receiver.pop(receiver_id, None) is not None:
                 for bucket in self._by_sender.values():
                     bucket.discard(receiver_id)
 
             self.receivers.pop(receiver_id, None)
         else:
             self._by_sender[sender_id].discard(receiver_id)
             self._by_receiver[receiver_id].discard(sender_id)
 
     def _make_cleanup_receiver(
-        self, receiver_id: t.Hashable
-    ) -> t.Callable[[weakref.ref[t.Callable[..., t.Any]]], None]:
-        """Disconnect a receiver from all senders."""
+        self, receiver_id: c.Hashable
+    ) -> c.Callable[[weakref.ref[c.Callable[..., t.Any]]], None]:
+        """Create a callback function to disconnect a weakly referenced
+        receiver when it is garbage collected.
+        """
 
-        def cleanup(ref: weakref.ref[t.Callable[..., t.Any]]) -> None:
+        def cleanup(ref: weakref.ref[c.Callable[..., t.Any]]) -> None:
             self._disconnect(receiver_id, ANY_ID)
 
         return cleanup
 
     def _make_cleanup_sender(
-        self, sender_id: t.Hashable
-    ) -> t.Callable[[weakref.ref[t.Any]], None]:
-        """Disconnect all receivers from a sender."""
+        self, sender_id: c.Hashable
+    ) -> c.Callable[[weakref.ref[t.Any]], None]:
+        """Create a callback function to disconnect all receivers for a weakly
+        referenced sender when it is garbage collected.
+        """
         assert sender_id != ANY_ID
 
         def cleanup(ref: weakref.ref[t.Any]) -> None:
             self._weak_senders.pop(sender_id, None)
 
             for receiver_id in self._by_sender.pop(sender_id, ()):
                 self._by_receiver[receiver_id].discard(sender_id)
 
         return cleanup
 
     def _cleanup_bookkeeping(self) -> None:
         """Prune unused sender/receiver bookkeeping. Not threadsafe.
 
-        Connecting & disconnecting leave behind a small amount of bookkeeping
-        for the receiver and sender values. Typical workloads using Blinker,
-        for example in most web apps, Flask, CLI scripts, etc., are not
-        adversely affected by this bookkeeping.
-
-        With a long-running Python process performing dynamic signal routing
-        with high volume- e.g. connecting to function closures, "senders" are
-        all unique object instances, and doing all of this over and over- you
-        may see memory usage will grow due to extraneous bookkeeping. (An empty
-        set() for each stale sender/receiver pair.)
+        Connecting & disconnecting leaves behind a small amount of bookkeeping
+        data. Typical workloads using Blinker, for example in most web apps,
+        Flask, CLI scripts, etc., are not adversely affected by this
+        bookkeeping.
+
+        With a long-running process performing dynamic signal routing with high
+        volume, e.g. connecting to function closures, senders are all unique
+        object instances. Doing all of this over and over may cause memory usage
+        to grow due to extraneous bookkeeping. (An empty ``set`` for each stale
+        sender/receiver pair.)
 
         This method will prune that bookkeeping away, with the caveat that such
         pruning is not threadsafe. The risk is that cleanup of a fully
         disconnected receiver/sender pair occurs while another thread is
         connecting that same pair. If you are in the highly dynamic, unique
-        receiver/sender situation that has lead you to this method, that
-        failure mode is perhaps not a big deal for you.
+        receiver/sender situation that has lead you to this method, that failure
+        mode is perhaps not a big deal for you.
         """
         for mapping in (self._by_sender, self._by_receiver):
             for ident, bucket in list(mapping.items()):
                 if not bucket:
                     mapping.pop(ident, None)
 
     def _clear_state(self) -> None:
-        """Throw away all signal state.  Useful for unit tests."""
+        """Disconnect all receivers and senders. Useful for tests."""
         self._weak_senders.clear()
         self.receivers.clear()
         self._by_sender.clear()
         self._by_receiver.clear()
 
 
 _receiver_connected = Signal(
@@ -491,101 +507,120 @@
     :attr:`~Signal.receiver_disconnected` signals with a slightly simplified
     call signature. This global signal will be removed in Blinker 1.9.
 """
 )
 
 
 class NamedSignal(Signal):
-    """A named generic notification emitter."""
+    """A named generic notification emitter. The name is not used by the signal
+    itself, but matches the key in the :class:`Namespace` that it belongs to.
+
+    :param name: The name of the signal within the namespace.
+    :param doc: The docstring for the signal.
+    """
 
     def __init__(self, name: str, doc: str | None = None) -> None:
         super().__init__(doc)
 
         #: The name of this signal.
         self.name: str = name
 
     def __repr__(self) -> str:
         base = super().__repr__()
         return f"{base[:-1]}; {self.name!r}>"  # noqa: E702
 
 
-class Namespace(dict):  # type: ignore[type-arg]
-    """A mapping of signal names to signals."""
+if t.TYPE_CHECKING:
+
+    class PNamespaceSignal(t.Protocol):
+        def __call__(self, name: str, doc: str | None = None) -> NamedSignal: ...
+
+    # Python < 3.9
+    _NamespaceBase = dict[str, NamedSignal]  # type: ignore[misc]
+else:
+    _NamespaceBase = dict
+
+
+class Namespace(_NamespaceBase):
+    """A dict mapping names to signals."""
 
     def signal(self, name: str, doc: str | None = None) -> NamedSignal:
-        """Return the :class:`NamedSignal` *name*, creating it if required.
+        """Return the :class:`NamedSignal` for the given ``name``, creating it
+        if required. Repeated calls with the same name return the same signal.
 
-        Repeated calls to this function will return the same signal object.
+        :param name: The name of the signal.
+        :param doc: The docstring of the signal.
         """
-        try:
-            return self[name]  # type: ignore[no-any-return]
-        except KeyError:
-            result = self.setdefault(name, NamedSignal(name, doc))
-            return result  # type: ignore[no-any-return]
+        if name not in self:
+            self[name] = NamedSignal(name, doc)
 
+        return self[name]
 
-class _WeakNamespace(WeakValueDictionary):  # type: ignore[type-arg]
-    """A weak mapping of signal names to signals.
 
-    Automatically cleans up unused Signals when the last reference goes out
-    of scope.  This namespace implementation exists for a measure of legacy
-    compatibility with Blinker <= 1.2, and may be dropped in the future.
+class _WeakNamespace(WeakValueDictionary):  # type: ignore[type-arg]
+    """A weak mapping of names to signals.
 
-    .. versionadded:: 1.3
+    Automatically cleans up unused signals when the last reference goes out
+    of scope. This namespace implementation provides similar behavior to Blinker
+    <= 1.2.
 
     .. deprecated:: 1.3
         Will be removed in Blinker 1.9.
+
+    .. versionadded:: 1.3
     """
 
     def __init__(self) -> None:
         warnings.warn(
             "'WeakNamespace' is deprecated and will be removed in Blinker 1.9."
             " Use 'Namespace' instead.",
             DeprecationWarning,
             stacklevel=2,
         )
         super().__init__()
 
     def signal(self, name: str, doc: str | None = None) -> NamedSignal:
-        """Return the :class:`NamedSignal` *name*, creating it if required.
-
-        Repeated calls to this function will return the same signal object.
+        """Return the :class:`NamedSignal` for the given ``name``, creating it
+        if required. Repeated calls with the same name return the same signal.
 
+        :param name: The name of the signal.
+        :param doc: The docstring of the signal.
         """
-        try:
-            return self[name]  # type: ignore[no-any-return]
-        except KeyError:
-            result = self.setdefault(name, NamedSignal(name, doc))
-            return result  # type: ignore[no-any-return]
+        if name not in self:
+            self[name] = NamedSignal(name, doc)
+
+        return self[name]  # type: ignore[no-any-return]
 
 
-default_namespace = Namespace()
-"""A default namespace for creating named signals. :func:`signal` creates a
-:class:`NamedSignal` in this namespace.
+default_namespace: Namespace = Namespace()
+"""A default :class:`Namespace` for creating named signals. :func:`signal`
+creates a :class:`NamedSignal` in this namespace.
 """
 
-signal = default_namespace.signal
-"""Create a :class:`NamedSignal` in :data:`default_namespace`. Repeated calls
-with the same name will return the same signal.
+signal: PNamespaceSignal = default_namespace.signal
+"""Return a :class:`NamedSignal` in :data:`default_namespace` with the given
+``name``, creating it if required. Repeated calls with the same name return the
+same signal.
 """
 
 
 def __getattr__(name: str) -> t.Any:
-    if name == "reciever_connected":
+    if name == "receiver_connected":
         warnings.warn(
-            "The global 'reciever_connected' signal is deprecated and will be"
+            "The global 'receiver_connected' signal is deprecated and will be"
             " removed in Blinker 1.9. Use 'Signal.receiver_connected' and"
-            " 'Signal.reciever_disconnected' instead.",
+            " 'Signal.receiver_disconnected' instead.",
             DeprecationWarning,
             stacklevel=2,
         )
         return _receiver_connected
 
     if name == "WeakNamespace":
         warnings.warn(
             "'WeakNamespace' is deprecated and will be removed in Blinker 1.9."
             " Use 'Namespace' instead.",
             DeprecationWarning,
             stacklevel=2,
         )
+        return _WeakNamespace
 
     raise AttributeError(name)
```

### Comparing `blinker-1.8.0/tests/test_context.py` & `blinker-1.8.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `blinker-1.8.0/tests/test_signals.py` & `blinker-1.8.1/tests/test_signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import collections.abc as c
 import gc
 import sys
 import typing as t
 
 import pytest
 
 import blinker
@@ -14,15 +15,15 @@
     if sys.implementation.name == "pypy":
         gc.collect()
 
 
 class Sentinel(list):  # type: ignore[type-arg]
     """A signal receipt accumulator."""
 
-    def make_receiver(self, key: t.Any) -> t.Callable[..., t.Any]:
+    def make_receiver(self, key: t.Any) -> c.Callable[..., t.Any]:
         """Return a generic signal receiver function logging as *key*
 
         When connected to a signal, appends (key, sender, kw) to the Sentinel.
 
         """
 
         def receiver(*sentby: t.Any, **kw: t.Any) -> None:
@@ -261,15 +262,15 @@
 
     async def received_async(sender: t.Any) -> None:
         sentinel.append(sender)
 
     def received(sender: t.Any) -> None:
         sentinel.append(sender)
 
-    def wrapper(func: t.Callable[..., t.Any]) -> t.Callable[..., None]:
+    def wrapper(func: c.Callable[..., t.Any]) -> c.Callable[..., None]:
         async def inner(*args: t.Any, **kwargs: t.Any) -> None:
             func(*args, **kwargs)
 
         return inner  # type: ignore[return-value]
 
     sig = blinker.Signal()
     sig.connect(received)
@@ -481,19 +482,19 @@
 
 def values_are_empty_sets_(dictionary: dict[t.Any, t.Any]) -> None:
     for val in dictionary.values():
         assert val == set()
 
 
 def test_int_sender() -> None:
-    sentinel = []
+    count = 0
 
     def received(sender: t.Any) -> None:
-        sentinel.append(sender)
+        nonlocal count
+        count += 1
 
     sig = blinker.Signal()
-
     sig.connect(received, sender=123456789)
-    sig.send(123456789)
-    assert len(sentinel) == 1
-    sig.send(123456789 + 0)  # Forces a new id with CPython
-    assert len(sentinel) == 2
+    sig.send(123456789)  # Python compiler uses same instance for same literal value.
+    assert count == 1
+    sig.send(int("123456789"))  # Force different instance with same value.
+    assert count == 2
```

### Comparing `blinker-1.8.0/tox.ini` & `blinker-1.8.1/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 commands = pre-commit run --all-files
 
 [testenv:typing]
 deps = -r requirements/typing.txt
 commands =
     mypy
     pyright
+    pyright --verifytypes blinker --ignoreexternal
 
 [testenv:docs]
 deps = -r requirements/docs.txt
 commands = sphinx-build -E -W -b dirhtml docs docs/_build/dirhtml
 
 [testenv:update-pre_commit]
 labels = update
```

### Comparing `blinker-1.8.0/PKG-INFO` & `blinker-1.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blinker
-Version: 1.8.0
+Version: 1.8.1
 Summary: Fast, simple object-to-object and broadcast signaling
 Author: Jason Kirtland
 Maintainer-email: Pallets Ecosystem <contact@palletsprojects.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

