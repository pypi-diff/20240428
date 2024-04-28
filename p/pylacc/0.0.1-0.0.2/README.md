# Comparing `tmp/pylacc-0.0.1.tar.gz` & `tmp/pylacc-0.0.2.tar.gz`

## Comparing `pylacc-0.0.1.tar` & `pylacc-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pylacc-0.0.1/README.md
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 pylacc-0.0.1/tox.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylacc-0.0.1/src/pylacc/__init__.py
--rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 pylacc-0.0.1/src/pylacc/circuit.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 pylacc-0.0.1/tests/test_circuit.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pylacc-0.0.1/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 pylacc-0.0.1/LICENSE
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pylacc-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pylacc-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 pylacc-0.0.2/tox.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylacc-0.0.2/src/pylacc/__init__.py
+-rw-r--r--   0        0        0    11167 2020-02-02 00:00:00.000000 pylacc-0.0.2/src/pylacc/circuit.py
+-rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 pylacc-0.0.2/tests/test_circuit.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pylacc-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 pylacc-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 pylacc-0.0.2/README.md
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pylacc-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pylacc-0.0.2/PKG-INFO
```

### Comparing `pylacc-0.0.1/README.md` & `pylacc-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -72,10 +72,27 @@
 +-S[12V 60Hz](72.1∠-56.3°mA 865mVA)
 +-/(12V 72.1∠-56.3°mA)
 + /-L[100Ω](12V 120∠-90°mA 265mH)
 + /-C[200Ω](12V 60∠90°mA 13.3μF)
 + /-R[300Ω](12V 40mA)
 ```
 
+## Groups
+
+Components can be grouped to prevent further concatenation.
+
+```
+FILTER = (l(1e-3) + c(0.0022e-6)).g
+C = e(10, 107e3) + FILTER + r(100)
+C.solve()
+FILTER
+```
+
+```
++(380∠-87.8°mV 99.9∠2.18°mA)
++-L[1mH](67.2∠92.2°V 99.9∠2.18°mA 672Ω)
++-C[2.2nF](67.6∠-87.8°V 99.9∠2.18°mA 676Ω)
+```
+
 ## TODO
 
 - Support multiple sources
```

### Comparing `pylacc-0.0.1/src/pylacc/circuit.py` & `pylacc-0.0.2/src/pylacc/circuit.py`

 * *Files 12% similar despite different names*

```diff
@@ -182,26 +182,28 @@
                 V = law(**P)
                 if V is None:
                     continue
                 if not isclose(self[K], V):
                     errors.append('{} -> {}: {} != {}'.format(D, K, self[K], V))
         if errors:
             raise AssertionError('\n'.join(errors))
+
+    def __call__(self, *props):
+        self.solve()
+        return Filter(self.__str__(props))
         
     @property
     def p(self):
-        self.solve()
-        return Filter(self.__str__(Q=('PT', 'PR', 'PA')))
+        return self('PT', 'PR', 'PA')
         
     @property
     def z(self):
-        self.solve()
-        return Filter(self.__str__(Q=('Z',)))
+        return self('Z')
 
-    def __str__(self, indent='', Q=None):
+    def __str__(self, Q=None, indent=''):
         G = tuple(self.given)
         if Q is None:
             Q = self.show + tuple(p for p in self.optional if self[p] is not None)
         Q = tuple(q for q in Q if q not in G)
         V = ''
         GN = [norm(p, self[p], self.AC, True) for p in G]
         GN = [p for p in GN if p]
@@ -214,25 +216,19 @@
         return self.name + V
     
     def __repr__(self):
         self.solve()
         return str(self)
 
 Component.law(Z=('E', 'I'))(lambda E, I: E / I)
-Component.law(Z=('PA', 'E'))(lambda PA, E: E * E / PA)
-Component.law(Z=('PA', 'I'))(lambda PA, I: PA / (I * I))
 Component.law(PA=('E', 'I'))(lambda E, I: E * I)
 Component.law(PA=('E', 'Z'))(lambda E, Z: E * E / Z)
 Component.law(PA=('I', 'Z'))(lambda I, Z: I * I * Z)
 Component.law(E=('I', 'Z'))(lambda I, Z: I * Z)
-Component.law(E=('PA', 'I'))(lambda PA, I: PA / I)
-# Component.law(E=('PA', 'Z'))(lambda PA, Z: sqrt(PA * Z)) # TODO: Reactive signs are lost in sqrt
 Component.law(I=('E', 'Z'))(lambda E, Z: E / Z)
-Component.law(I=('PA', 'E'))(lambda PA, E: PA / E)
-Component.law(I=('PA', 'Z'))(lambda PA, Z: sqrt(PA / Z))
 
 Component.law(PT=('E', 'Z'))(lambda E, Z: E * E / Z.real if not isclose(Z.real, 0) else None)
 Component.law(PR=('E', 'Z'))(lambda E, Z: 1j * E * E / Z.imag if not isclose(Z.imag, 0) else None)
 
 Component.law(R=('Z',))(lambda Z: Z.real)
 Component.law(XC=('Z',))(lambda Z: -Z.imag if Z.imag < 0 and not isclose(Z.imag, 0) else None)
 Component.law(XL=('Z',))(lambda Z: Z.imag if Z.imag > 0 and not isclose(Z.imag, 0) else None)
@@ -282,30 +278,32 @@
             extra['e'] = e
         if f is not None:
             extra['f'] = f
         super().__init__(**{k: v for k, v in tuple(extra.items()) + tuple(kwargs.items())})
 
 class Circuit(Component):
     show = ('E', 'I')
+    lock = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(**kwargs)
         self.nodes = list(args)
 
-    def __call__(self, *nodes):
-        self.nodes.extend(nodes)
-        return self
-
     @property
     def loads(self):
         return [L for L in self.nodes if not isinstance(L, Source)]
 
     @property
     def sources(self):
         return [S for S in self.nodes if isinstance(S, Source)]
+
+    @property
+    def g(self):
+        self.lock = True
+        return self
     
     def constant(self, prop, G=None):
         if G is None:
             G = self.nodes
         change = False
         if not given(self[prop]):
             for c in G:
@@ -346,18 +344,18 @@
         return change
 
     def verify(self):
         super().verify()
         for c in self.nodes:
             c.verify()
 
-    def __str__(self, indent='', Q=None):
+    def __str__(self, Q=None, indent=''):
         indent = indent.replace(DELIM[0], DELIM[1]) + self.name + DELIM[0]
-        return super().__str__(indent, Q) + ''.join(
-            '\n' + indent + c.__str__(indent, Q)
+        return super().__str__(Q, indent) + ''.join(
+            '\n' + indent + c.__str__(Q, indent)
             for c in self.nodes
         )
 
 class Series(Circuit):
     name = '+'
     def _solve(self):
         change = super()._solve()
@@ -368,14 +366,16 @@
         change |= self.constant('F')
         change |= self.linear('Z')
         change |= self.linear('E')
         change |= self.linear('PA')
         return change
     
     def __add__(self, other):
+        if self.lock:
+            return super().__add__(other)
         self.nodes.append(other)
         return self
 
 class Parallel(Circuit):
     name = '/'
     def _solve(self):
         change = super()._solve()
@@ -385,14 +385,16 @@
         change |= self.constant('F')
         change |= self.linear('I')
         change |= self.linear('PA')
         change |= self.linear('Y')
         return change
 
     def __truediv__(self, other):
+        if self.lock:
+            return super().__truediv__(other)
         self.nodes.append(other)
         return self
 
 e = lambda v=None, f=None, **k: Source(e=v, f=f, **k)
 i = lambda v=None, f=None, **k: Source(i=v, f=f, **k)
 r = lambda v=None, **k: Load(r=v, **k)
 xc = lambda v=None, **k: Load(xc=v, **k)
```

### Comparing `pylacc-0.0.1/tests/test_circuit.py` & `pylacc-0.0.2/tests/test_circuit.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from itertools import combinations, permutations
 import pytest
 
 from pylacc.circuit import Series, Parallel, Load, Source, Component
 from pylacc.circuit import e, r, xc, xl, c, l
 
 
-C1 = {'E': 12, 'I': 4, 'Z': 3, 'PA': 48}
+C1 = {'E': 12, 'I': 4, 'Z': 3}
 
 class TestComponent:
     def test_unknown(self):
         C = Component()
         assert repr(C) == '?(Z=? E=? I=?)'
         C.verify()
 
@@ -26,67 +26,67 @@
         with pytest.raises(AssertionError):
             C.verify()
 
 class TestSeries:
     @pytest.mark.parametrize('T', permutations(C1.items(), 2))
     def test_split_solve(self, T):
         L = Load(**dict(T[1:]))
-        C = Series(**dict(T[:1]))(L)
+        C = Series(L, **dict(T[:1]))
         C.solve()
         for k, v in C1.items():
             assert C[k] == v
             assert L[k] == v
         C.verify()
 
     @pytest.mark.parametrize('T', [dict([p]) for p in C1.items() if p[0] != 'E'])
     def test_voltage_source(self, T):
         S = Source(12)
         L = Load(**T)
-        C = Series()(S, L)
+        C = Series(S, L)
         C.solve()
         for k, v in C1.items():
             assert C[k] == v
             assert S[k] == v
             assert L[k] == v
         C.verify()
 
     @pytest.mark.parametrize('T', [dict([p]) for p in C1.items() if p[0] != 'I'])
     def test_current_source(self, T):
         S = Source(I=4)
         L = Load(**T)
-        C = Series()(S, L)
+        C = Series(S, L)
         C.solve()
         for k, v in C1.items():
             assert C[k] == v
             assert S[k] == v
             assert L[k] == v
         C.verify()
 
     def test_loads(self):
-        C = Series(E=12)(Load(Z=1), Load(Z=2))
+        C = Series(Load(Z=1), Load(Z=2), E=12)
         assert repr(C) == '''\
 +[12V](4A)
 +-R[1Ω](4V 4A)
 +-R[2Ω](8V 4A)\
 '''
         C.verify()
 
 class TestParallel:
     @pytest.mark.parametrize('T', permutations(C1.items(), 2))
     def test_split_solve(self, T):
         L = Load(**dict(T[1:]))
-        C = Parallel(**dict(T[:1]))(L)
+        C = Parallel(L, **dict(T[:1]))
         C.solve()
         for k, v in C1.items():
             assert C[k] == v
             assert L[k] == v
         C.verify()
 
     def test_loads(self):
-        C = Parallel(E=12)(Load(Z=6), Load(Z=6))
+        C = Parallel(Load(Z=6), Load(Z=6), E=12)
         assert repr(C) == '''\
 /[12V](4A)
 /-R[6Ω](12V 2A)
 /-R[6Ω](12V 2A)\
 '''
         C.verify()
 
@@ -127,15 +127,15 @@
 +-S[12V](1.5Ω)
 +-/(1.5Ω)
 + /-R[3Ω]
 + /-R[3Ω]\
 '''
         C.verify()
 
-C2 = {'E': 120, 'I': 20 - 20j, 'Z': 3 + 3j, 'PA': 2400-2400j}
+C2 = {'E': 120, 'I': 20 - 20j, 'Z': 3 + 3j}
 
 class TestAlernatingCurrent:
     @pytest.mark.parametrize(('D'), [-1, 1])
     def test_no_frequency(self, D):
         C = e(120, z=100 + 100j * D)
         assert repr(C) == f'S[120V 141∠{D * 45}°Ω](849∠{-D * 45}°mA 102VA)'
         C.verify()
@@ -170,7 +170,112 @@
         assert 'S[120V](60A 7.2kVA 30Hz)' in repr(C)
         C.verify()
 
     def test_reverse_ind_frequency(self):
         C = e(120) + r(2) + l(2.654e-3, xl=2) + xc(2)
         assert 'S[120V](60A 7.2kVA 120Hz)' in repr(C)
         C.verify()
+
+class TestFilter:
+    @pytest.mark.parametrize('n', range(-4, 5))
+    def test_rc_low_pass(self, n):
+        fc = 339e3
+        f = fc * 2 ** n
+        CAP = c(0.0047e-6)
+        C = e(10, f) + r(100) + CAP
+        C.solve()
+        if f <= fc:
+            assert abs(CAP.E) >= 7.06
+        else:
+            assert abs(CAP.E) < 7.06
+        C.verify()
+
+    @pytest.mark.parametrize('n', range(-4, 5))
+    def test_rc_high_pass(self, n):
+        fc = 339e3
+        f = fc * 2 ** n
+        R = r(100)
+        C = e(10, f) + c(0.0047e-6) + R
+        C.solve()
+        if f < fc:
+            assert abs(R.E) < 7.06
+        else:
+            assert abs(R.E) >= 7.06
+        C.verify()
+
+    @pytest.mark.parametrize('n', range(-4, 5))
+    def test_rl_low_pass(self, n):
+        fc = 74.5e3
+        f = fc * 2 ** n
+        R = r(2.2e3)
+        C = e(10, f) + l(4.7e-3) + R
+        C.solve()
+        if f <= fc:
+            assert abs(R.E) >= 7.06
+        else:
+            assert abs(R.E) < 7.06
+        C.verify()
+
+    @pytest.mark.parametrize('n', range(-4, 5))
+    def test_rl_high_pass(self, n):
+        fc = 74.5e3
+        f = fc * 2 ** n
+        IND = l(4.7e-3)
+        C = e(10, f) + r(2.2e3) + IND
+        C.solve()
+        if f < fc:
+            assert abs(IND.E) < 7.06
+        else:
+            assert abs(IND.E) >= 7.06
+        C.verify()
+
+    @pytest.mark.parametrize('n', range(-4, 5))
+    def test_series_band_pass(self, n):
+        fc = 107e3
+        f = fc * 2 ** n
+        R = r(100)
+        C = e(10, f) + l(1e-3) + c(0.0022e-6) + R
+        C.solve()
+        if f == fc:
+            assert abs(R.E) > 9.9
+        else:
+            assert abs(R.E) < 7.07
+        C.verify()
+
+    @pytest.mark.parametrize('n', range(-4, 5))
+    def test_parallel_band_pass(self, n):
+        fc = 107e3
+        f = fc * 2 ** n
+        TANK = (l(1e-3) / c(0.0022e-6)).g
+        C = e(10, f) + r(100) + TANK
+        C.solve()
+        if f == fc:
+            assert abs(TANK.E) > 9.9
+        else:
+            assert abs(TANK.E) < 9.9
+        C.verify()
+
+    @pytest.mark.parametrize('n', range(-4, 5))
+    def test_series_band_stop(self, n):
+        fc = 107e3
+        f = fc * 2 ** n
+        SINK = (l(1e-3) + c(0.0022e-6)).g
+        C = e(10, f) + r(100) + SINK
+        C.solve()
+        if f == fc:
+            assert abs(SINK.E) < 0.4
+        else:
+            assert abs(SINK.E) > 9
+        C.verify()
+
+    @pytest.mark.parametrize('n', range(-4, 5))
+    def test_parallel_band_stop(self, n):
+        fc = 107e3
+        f = fc * 2 ** n
+        R = r(100)
+        C = e(10, f) + (l(1e-3) / c(0.0022e-6)) + R
+        C.solve()
+        if f == fc:
+            assert abs(R.E) < 0.1
+        else:
+            assert abs(R.E) > 2
+        C.verify()
```

### Comparing `pylacc-0.0.1/LICENSE` & `pylacc-0.0.2/LICENSE`

 * *Files identical despite different names*

