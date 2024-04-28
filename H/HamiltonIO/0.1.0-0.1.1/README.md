# Comparing `tmp/hamiltonio-0.1.0.tar.gz` & `tmp/hamiltonio-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hamiltonio-0.1.0.tar", last modified: Fri Apr 19 14:15:49 2024, max compression
+gzip compressed data, was "hamiltonio-0.1.1.tar", last modified: Sun Apr 28 20:25:15 2024, max compression
```

## Comparing `hamiltonio-0.1.0.tar` & `hamiltonio-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:15:49.882298 hamiltonio-0.1.0/
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:15:49.882298 hamiltonio-0.1.0/HamiltonIO/
--rw-r--r--   0 hexu      (1032) phythema   (500)        0 2024-04-08 08:09:06.000000 hamiltonio-0.1.0/HamiltonIO/__init__.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:15:49.882298 hamiltonio-0.1.0/HamiltonIO/abacus/
--rw-r--r--   0 hexu      (1032) phythema   (500)       56 2024-04-19 11:11:36.000000 hamiltonio-0.1.0/HamiltonIO/abacus/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     7267 2024-04-19 11:11:05.000000 hamiltonio-0.1.0/HamiltonIO/abacus/abacus_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8492 2024-04-19 11:11:05.000000 hamiltonio-0.1.0/HamiltonIO/abacus/abacus_wrapper.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1562 2024-04-19 11:11:05.000000 hamiltonio-0.1.0/HamiltonIO/abacus/orbital_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    67888 2024-04-19 11:11:05.000000 hamiltonio-0.1.0/HamiltonIO/abacus/stru_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2024-04-19 11:11:05.000000 hamiltonio-0.1.0/HamiltonIO/abacus/test_read_HRSR.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      785 2024-04-19 11:12:00.000000 hamiltonio-0.1.0/HamiltonIO/abacus/test_read_stru.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2101 2024-04-19 12:55:29.000000 hamiltonio-0.1.0/HamiltonIO/abstractTB.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:15:49.882298 hamiltonio-0.1.0/HamiltonIO/siesta/
--rw-r--r--   0 hexu      (1032) phythema   (500)        0 2024-04-19 11:07:02.000000 hamiltonio-0.1.0/HamiltonIO/siesta/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    14823 2024-04-19 11:06:56.000000 hamiltonio-0.1.0/HamiltonIO/siesta/sisl_wrapper.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:15:49.882298 hamiltonio-0.1.0/HamiltonIO/wannier/
--rw-r--r--   0 hexu      (1032) phythema   (500)       68 2024-04-19 12:53:51.000000 hamiltonio-0.1.0/HamiltonIO/wannier/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    16288 2024-04-19 13:43:25.000000 hamiltonio-0.1.0/HamiltonIO/wannier/myTB.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6709 2024-04-19 12:56:02.000000 hamiltonio-0.1.0/HamiltonIO/wannier/utils.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4616 2024-04-19 12:54:53.000000 hamiltonio-0.1.0/HamiltonIO/wannier/w90_parser.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4610 2024-04-19 12:54:29.000000 hamiltonio-0.1.0/HamiltonIO/wannier/w90_tb_parser.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:15:49.882298 hamiltonio-0.1.0/HamiltonIO/wantibexos/
--rw-r--r--   0 hexu      (1032) phythema   (500)    12752 2024-04-19 11:10:44.000000 hamiltonio-0.1.0/HamiltonIO/wantibexos/H_extract-siesta.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:15:49.882298 hamiltonio-0.1.0/HamiltonIO.egg-info/
--rw-r--r--   0 hexu      (1032) phythema   (500)     1455 2024-04-19 14:15:49.000000 hamiltonio-0.1.0/HamiltonIO.egg-info/PKG-INFO
--rw-r--r--   0 hexu      (1032) phythema   (500)      743 2024-04-19 14:15:49.000000 hamiltonio-0.1.0/HamiltonIO.egg-info/SOURCES.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)        1 2024-04-19 14:15:49.000000 hamiltonio-0.1.0/HamiltonIO.egg-info/dependency_links.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)      157 2024-04-19 14:15:49.000000 hamiltonio-0.1.0/HamiltonIO.egg-info/requires.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)       11 2024-04-19 14:15:49.000000 hamiltonio-0.1.0/HamiltonIO.egg-info/top_level.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)     1294 2024-04-08 08:08:40.000000 hamiltonio-0.1.0/LICENSE
--rw-r--r--   0 hexu      (1032) phythema   (500)     1455 2024-04-19 14:15:49.882298 hamiltonio-0.1.0/PKG-INFO
--rw-r--r--   0 hexu      (1032) phythema   (500)       63 2024-04-08 08:08:40.000000 hamiltonio-0.1.0/README.md
--rw-r--r--   0 hexu      (1032) phythema   (500)     1488 2024-04-19 14:14:50.000000 hamiltonio-0.1.0/pyproject.toml
--rw-r--r--   0 hexu      (1032) phythema   (500)       38 2024-04-19 14:15:49.882298 hamiltonio-0.1.0/setup.cfg
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.526590 hamiltonio-0.1.1/
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.523225 hamiltonio-0.1.1/HamiltonIO/
+-rw-r--r--   0 hexu       (501) staff       (20)       87 2024-04-28 11:37:36.000000 hamiltonio-0.1.1/HamiltonIO/__init__.py
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.524721 hamiltonio-0.1.1/HamiltonIO/abacus/
+-rw-r--r--   0 hexu       (501) staff       (20)       56 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/abacus/__init__.py
+-rw-r--r--   0 hexu       (501) staff       (20)     7267 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/abacus/abacus_api.py
+-rw-r--r--   0 hexu       (501) staff       (20)     8492 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/abacus/abacus_wrapper.py
+-rw-r--r--   0 hexu       (501) staff       (20)     1562 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/abacus/orbital_api.py
+-rw-r--r--   0 hexu       (501) staff       (20)    67888 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/abacus/stru_api.py
+-rw-r--r--   0 hexu       (501) staff       (20)     1254 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/abacus/test_read_HRSR.py
+-rw-r--r--   0 hexu       (501) staff       (20)      785 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/abacus/test_read_stru.py
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.524828 hamiltonio-0.1.1/HamiltonIO/format/
+-rw-r--r--   0 hexu       (501) staff       (20)      325 2024-04-27 12:46:18.000000 hamiltonio-0.1.1/HamiltonIO/format/spmat.py
+-rw-r--r--   0 hexu       (501) staff       (20)     6136 2024-04-28 13:14:07.000000 hamiltonio-0.1.1/HamiltonIO/hamiltonian.py
+-rw-r--r--   0 hexu       (501) staff       (20)      241 2024-04-28 11:03:11.000000 hamiltonio-0.1.1/HamiltonIO/orbital.py
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.525025 hamiltonio-0.1.1/HamiltonIO/siesta/
+-rw-r--r--   0 hexu       (501) staff       (20)      104 2024-04-27 13:50:08.000000 hamiltonio-0.1.1/HamiltonIO/siesta/__init__.py
+-rw-r--r--   0 hexu       (501) staff       (20)    15997 2024-04-28 20:21:16.000000 hamiltonio-0.1.1/HamiltonIO/siesta/sisl_wrapper.py
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.525594 hamiltonio-0.1.1/HamiltonIO/wannier/
+-rw-r--r--   0 hexu       (501) staff       (20)       68 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/wannier/__init__.py
+-rw-r--r--   0 hexu       (501) staff       (20)    16289 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/wannier/myTB.py
+-rw-r--r--   0 hexu       (501) staff       (20)     6709 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/wannier/utils.py
+-rw-r--r--   0 hexu       (501) staff       (20)     4616 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/wannier/w90_parser.py
+-rw-r--r--   0 hexu       (501) staff       (20)     4610 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/HamiltonIO/wannier/w90_tb_parser.py
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.525846 hamiltonio-0.1.1/HamiltonIO/wantibexos/
+-rw-r--r--   0 hexu       (501) staff       (20)    12752 2024-04-27 21:04:30.000000 hamiltonio-0.1.1/HamiltonIO/wantibexos/H_extract-siesta.py
+-rw-r--r--   0 hexu       (501) staff       (20)    23160 2024-04-27 13:15:06.000000 hamiltonio-0.1.1/HamiltonIO/wantibexos/output_wantibexos.py
+drwxr-xr-x   0 hexu       (501) staff       (20)        0 2024-04-28 20:25:15.525996 hamiltonio-0.1.1/HamiltonIO.egg-info/
+-rw-r--r--   0 hexu       (501) staff       (20)     1537 2024-04-28 20:25:15.000000 hamiltonio-0.1.1/HamiltonIO.egg-info/PKG-INFO
+-rw-r--r--   0 hexu       (501) staff       (20)      836 2024-04-28 20:25:15.000000 hamiltonio-0.1.1/HamiltonIO.egg-info/SOURCES.txt
+-rw-r--r--   0 hexu       (501) staff       (20)        1 2024-04-28 20:25:15.000000 hamiltonio-0.1.1/HamiltonIO.egg-info/dependency_links.txt
+-rw-r--r--   0 hexu       (501) staff       (20)      157 2024-04-28 20:25:15.000000 hamiltonio-0.1.1/HamiltonIO.egg-info/requires.txt
+-rw-r--r--   0 hexu       (501) staff       (20)       11 2024-04-28 20:25:15.000000 hamiltonio-0.1.1/HamiltonIO.egg-info/top_level.txt
+-rw-r--r--   0 hexu       (501) staff       (20)     1294 2024-04-27 07:42:37.000000 hamiltonio-0.1.1/LICENSE
+-rw-r--r--   0 hexu       (501) staff       (20)     1537 2024-04-28 20:25:15.526421 hamiltonio-0.1.1/PKG-INFO
+-rw-r--r--   0 hexu       (501) staff       (20)      145 2024-04-28 19:16:43.000000 hamiltonio-0.1.1/README.md
+-rw-r--r--   0 hexu       (501) staff       (20)     1488 2024-04-28 20:22:55.000000 hamiltonio-0.1.1/pyproject.toml
+-rw-r--r--   0 hexu       (501) staff       (20)       38 2024-04-28 20:25:15.526624 hamiltonio-0.1.1/setup.cfg
```

### Comparing `hamiltonio-0.1.0/HamiltonIO/abacus/abacus_api.py` & `hamiltonio-0.1.1/HamiltonIO/abacus/abacus_api.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.0/HamiltonIO/abacus/abacus_wrapper.py` & `hamiltonio-0.1.1/HamiltonIO/abacus/abacus_wrapper.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.0/HamiltonIO/abacus/orbital_api.py` & `hamiltonio-0.1.1/HamiltonIO/abacus/orbital_api.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.0/HamiltonIO/abacus/stru_api.py` & `hamiltonio-0.1.1/HamiltonIO/abacus/stru_api.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.0/HamiltonIO/abacus/test_read_HRSR.py` & `hamiltonio-0.1.1/HamiltonIO/abacus/test_read_HRSR.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.0/HamiltonIO/abacus/test_read_stru.py` & `hamiltonio-0.1.1/HamiltonIO/abacus/test_read_stru.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.0/HamiltonIO/siesta/sisl_wrapper.py` & `hamiltonio-0.1.1/HamiltonIO/siesta/sisl_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,55 @@
 import os
 import numpy as np
 from ase.atoms import Atoms
-from TB2J.utils import symbol_number
 from collections import defaultdict
 from scipy.linalg import eigh
-from TB2J.myTB import AbstractTB
+from TB2J.utils import symbol_number
+from HamiltonIO.hamiltonian import Hamiltonian
 from TB2J.mathutils import Lowdin
+try:
+    import sisl
+except Exception as e:
+    print(e)
+    print("Sisl is not installed, please install it by 'pip install sisl'")
+
 
 
-class SislWrapper(AbstractTB):
-    def __init__(self, sisl_hamiltonian, geom=None, spin=None):
-        self.is_siesta = False
+class SislWrapper(Hamiltonian):
+    def __init__(self, fdf_fname=None, sisl_hamiltonian=None, geom=None, spin=None):
+        self._name = "SIESTA"
         self.is_orthogonal = False
-        self.ham = sisl_hamiltonian
+        if fdf_fname is not None:
+            fdf = sisl.get_sile(fdf_fname)
+            self.ham = fdf.read_hamiltonian()
+            self.geom = self.ham._geometry
+        elif sisl_hamiltonian is not None:
+            self.ham = sisl_hamiltonian
+        else:
+            raise ValueError("Either fdf_fname or sisl_hamiltonian should be provided")
         # k2Rfactor : H(k) = \int_R H(R) * e^(k2Rfactor * k.R)
         self.R2kfactor = 2.0j * np.pi  #
         if spin == "up":
             spin = 0
         elif spin == "down":
             spin = 1
-        if spin not in [None, 0, 1, "merge", "fakemerge"]:
+        if spin not in [None, 0, 1, "merge" ]:
             raise ValueError("spin should be None/0/1, but is %s" % spin)
+
         self.spin = spin
+        if not self.ham.spin.is_colinear:
+            self.spin = None
+
         self.orbs = []
         self.orb_dict = defaultdict(lambda: [])
         if geom is None:
             g = self.ham._geometry
         else:
             g = geom
-        _atoms = geom._atoms
+        _atoms = self.geom._atoms
         atomic_numbers = []
         self.positions = g.xyz
         self.cell = np.array(g.sc.cell)
         for ia, a in enumerate(_atoms):
             atomic_numbers.append(a.Z % 200)
         self.atoms = Atoms(
             numbers=atomic_numbers, cell=self.cell, positions=self.positions
@@ -45,34 +62,132 @@
                     orb_names = [f"{symnum}|{x.name()}|up" for x in a.orbital]
                 except:
                     orb_names = [f"{symnum}|{x.name()}|up" for x in a.orbitals]
                 self.orbs += orb_names
                 self.orb_dict[ia] += orb_names
             self.norb = len(self.orbs)
             self.nbasis = self.norb
+        elif self.ham.spin.is_colinear and self.spin is None:
+            raise ValueError("spin should be 0/1 for collinear spin, but is %s" % self.spin)
         elif (
             self.ham.spin.is_spinorbit
             or self.ham.spin.is_noncolinear
             or self.spin == "merge"
-            or self.spin == "fakemerge"
         ):
             for ia, a in enumerate(_atoms):
                 symnum = sdict[ia]
                 orb_names = []
                 for x in a.orbitals:
                     for spin in {"up", "down"}:
                         orb_names.append(f"{symnum}|{x.name()}|{spin}")
                 self.orbs += orb_names
                 self.orb_dict[ia] += orb_names
             self.norb = len(self.orbs) // 2
             self.nbasis = len(self.orbs)
-        else:
-            raise ValueError("The hamiltonian should be either spin-orbit or colinear")
+        else:   # non-polarized, spin=None
+            for ia, a in enumerate(_atoms):
+               symnum = sdict[ia]
+               orb_names = []
+               for x in a.orbitals:
+                   orb_names.append(f"{symnum}|{x.name()}")
+               self.orbs += orb_names
+               self.orb_dict[ia] += orb_names
+            self.norb = len(self.orbs) 
+            self.nbasis = len(self.orbs)
+        
         self._name = "SIESTA"
 
+        self.Rlist = self.geom.sc_off
+
+    @property
+    def Rlist(self):
+        return self._Rlist
+
+    @Rlist.setter
+    def Rlist(self, Rlist):
+        self._Rlist = Rlist
+        self._Rdict = {}
+        self._nR = len(self._Rlist)
+        for i, R in enumerate(self.Rlist):
+            self._Rdict[tuple(R)] = i
+
+    @property
+    def nR(self):
+        return self._nR
+
+    def get_Ridx(self, R):
+        """
+        Get the index of R in the Rlist 
+        """
+        return self._Rdict[tuple(R)]
+
+    def _get_HR_all_nonpolarized(self,dense=True):
+        """
+        Get the Hamiltonian matrix in real space
+        """
+        mat=self.ham._csr.todense()
+        return mat.reshape((self.norb,self.nR, self.norb, 2))[:,:, :, 0].transpose((1, 0, 2))
+
+    def _get_HR_all_colinear(self, dense=True, ispin=None):
+        """
+        Get the Hamiltonian matrix in real space
+        """
+        #mat = self.ham._csr.todense()
+        norb, norb_sc, ndspin = self.ham._csr.shape
+        ndspin = ndspin
+        #HRs = np.zeros((2, self.nR, self.norb, self.norb), dtype=float)
+
+        #if False:
+        #    for ispin in range(2):
+        #        for iR in range(self.nR):
+        #            for iorb in range(self.norb):
+        #                for jorb in range(self.norb):
+        #                    HRs[ispin, iR, iorb, jorb] = self.ham[iorb, jorb, ispin, iR]
+
+        dmat=self.ham._csr.todense()
+        mat=dmat.reshape((self.norb,   self.nR, self.norb, 3))
+        HRs = mat.transpose((3, 1, 0, 2))[:2, :, :, :]
+        if ispin is not None:
+            return HRs[ispin]
+        else:
+            return HRs
+
+    def get_SR_all(self, dense=True):
+        smat = np.asarray(self.ham.tocsr(self.ham.S_idx).todense())
+        smat = np.reshape(smat, (self.norb, self.nR, self.norb)).transpose((1, 0, 2))
+        return smat
+
+    def _get_HR_all_SOC(self, dense=True):
+        """
+        Get the Hamiltonian matrix in real space
+        """
+        mat = self.ham._csr.todense()
+        norb, norb_sc, ndspin = mat.shape
+        nbasis = norb*2
+        mat=mat.reshape((norb, self.nR, norb, ndspin)).transpose((1, 0, 2, 3))
+        HRs = np.zeros((self.nR, self.norb*2, self.norb*2),dtype=complex)
+        # up-up:
+        HRs[:, ::2, ::2] = mat[:, :, :, 0] + 1j*mat[:, :, :, 4]
+        # up-down:
+        HRs[:, ::2, 1::2] = mat[:, :, :, 2] + 1j*mat[:, :, :, 3]
+        # down-up:
+        HRs[:, 1::2, ::2] = mat[:, :, :, 6] + 1j*mat[:, :, :, 7]
+        # down-down:
+        HRs[:, 1::2, 1::2] = mat[:, :, :, 1] + 1j*mat[:, :, :, 5]
+        return HRs
+
+    def get_HR_all(self, dense=True):
+        if self.ham.spin.is_colinear:
+            return self._get_HR_all_colinear(dense=dense)
+        elif self.ham.spin.is_spinorbit or self.ham.spin.is_noncolinear:
+            return self._get_HR_all_SOC(dense=dense)
+        else:
+            return self._get_HR_all_nonpolarized(dense=dense)
+    
+
     def view_info(self):
         print(self.orb_dict)
         print(self.atoms)
 
     def solve(self, k, convention=2):
         if convention == 1:
             gauge = "r"
@@ -89,24 +204,14 @@
             evals1, evecs1 = self.ham.eigh(k=k, spin=1, eigvals_only=False, gauge=gauge)
             evals = np.zeros(self.nbasis, dtype=float)
             evecs = np.zeros((self.nbasis, self.nbasis), dtype=complex)
             evals[::2] = evals0
             evals[1::2] = evals1
             evecs[::2, ::2] = evecs0
             evecs[1::2, 1::2] = evecs1
-
-        elif self.spin == "fakemerge":
-            evals0, evecs0 = self.ham.eigh(k=k, eigvals_only=False, gauge=gauge)
-            evals1, evecs1 = self.ham.eigh(k=k, eigvals_only=False, gauge=gauge)
-            evals = np.zeros(self.nbasis, dtype=float)
-            evecs = np.zeros((self.nbasis, self.nbasis), dtype=complex)
-            evals[::2] = evals0
-            evals[1::2] = evals1
-            evecs[::2, ::2] = evecs0
-            evecs[1::2, 1::2] = evecs1
         return evals, evecs
 
     def Hk(self, k, convention=2):
         if convention == 1:
             gauge = "r"
         elif convention == 2:
             gauge = "R"
@@ -114,18 +219,14 @@
             H = self.ham.Hk(k, gauge=gauge, format="dense")
         elif self.spin in [0, 1]:
             H = self.ham.Hk(k, spin=self.spin, gauge=gauge, format="dense")
         elif self.spin == "merge":
             H = np.zeros((self.nbasis, self.nbasis), dtype="complex")
             H[::2, ::2] = self.ham.Hk(k, spin=0, gauge=gauge, format="dense")
             H[1::2, 1::2] = self.ham.Hk(k, spin=1, gauge=gauge, format="dense")
-        elif self.spin == "fakemerge":
-            H = np.zeros((self.nbasis, self.nbasis), dtype="complex")
-            H[::2, ::2] = self.ham.Hk(k, gauge=gauge, format="dense")
-            H[1::2, 1::2] = self.ham.Hk(k, gauge=gauge, format="dense")
         return H
 
     def eigen(self, k, convention=2):
         return self.solve(k)
 
     def gen_ham(self, k, convention=2):
         return self.Hk(k, convention=convention)
@@ -136,15 +237,15 @@
         elif convention == 2:
             pass
         S0 = self.ham.Sk(k, gauge="R", format="dense")
         if self.spin is None:
             S = S0
         elif self.spin in [0, 1]:
             S = S0
-        elif self.spin == "merge" or self.spin == "fakemerge":
+        elif self.spin == "merge":
             S = np.zeros((self.nbasis, self.nbasis), dtype="complex")
             S[::2, ::2] = S0
             S[1::2, 1::2] = S0
         return S
 
     def solve_all(self, kpts, orth=False):
         evals = []
@@ -216,42 +317,14 @@
     def _prepare_cache(self, path="./TB2J_results/cache"):
         if not os.path.exists(path):
             os.makedirs(path)
         else:
             os.remove(path)
         self.cache_path = path
 
-    # def get_HSE_cached(self, kpt, convention=2):
-    #     kpt = tuple(kpt)
-    #     kname = f"{kpt[0]:9.5f}_{kpt[1]:9.5f}_{kpt[2]:9.5f}"
-    #     if kname in self.cache_dict:
-    #         path = self.cache_dict[kname]
-    #         Hk = np.memmap(os.path.join(path, 'H.dat'),
-    #                        dtype='complex',
-    #                        mode='r',
-    #                        shape=(self.nbasis, self.nbasis))
-    #         Sk = np.memmap(os.path.join(path, 'H.dat'),
-    #                        dtype='complex',
-    #                        mode='r',
-    #                        shape=(self.nbasis, self.nbasis))
-    #         evalue = np.memmap(os.path.join(path, 'evalue.dat'),
-    #                            dtype='float',
-    #                            mode='r',
-    #                            shape=(self.nbasis))
-    #         evec = np.memmap(os.path.join(path, 'evec.dat'),
-    #                          dtype='complex',
-    #                          mode='r',
-    #                          shape=(self.nbasis, self.nbasis))
-    #     else:
-    #         Hk, Sk, evalue, evec = self.get_HSE(kpt, convention=convention)
-    #         path = os.path.join(self.cache_path, )
-    #         self.cache_dict[tuple(kpt)] = path
-    #         fpH = np.memmap(os.path.join(path, 'H.dat'))
-    #     return Hk, Sk, evalue, evec
-
     def get_HSE(self, kpt, convention=2):
         Hk = self.Hk(kpt, convention=convention)
         Sk = self.Sk(kpt, convention=convention)
         evalue, evec = self.solve(kpt, convention=convention)
         return Hk, Sk, evalue, evec
 
     def get_fermi_level(self):
@@ -360,26 +433,7 @@
                 + "\n".join([str(k) for k in kpts])
             )
         if not np.all(np.isclose(self.wfsx_kpts[sort_idx], kpts)):
             # raise ValueError(       wfsx_kpts = np.asarray(wfsx_kpts)
             pass
 
 
-# def test():
-#    fdf = sisl.get_sile('/home/hexu/projects/learn_siesta/SMO_Wannier/siesta.fdf')
-#    H = fdf.read_hamiltonian(order='nc',dim=2)
-#    print(H._spin._is_polarized)
-#    print(H.__dict__.keys())
-#    print(H._geometry.__dict__.keys())
-#    print(H._geometry.xyz)
-#    print(H._geometry.sc)
-#    H._geometry.sc.cell
-#    orb=H._geometry._atoms[0].orbital[0]
-#    print(orb.name())
-#    s=SislWrapper(H)
-#    s.view_info()
-#
-# import sisl
-# fdf = sisl.get_sile('/home/hexu/projects/learn_siesta/SMO_Wannier/siesta.fdf')
-# H = fdf.read_hamiltonian(order='nc',dim=2)
-# if __name__=='__main__':
-#    test()
```

### Comparing `hamiltonio-0.1.0/HamiltonIO/wannier/myTB.py` & `hamiltonio-0.1.1/HamiltonIO/wannier/myTB.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,14 +157,15 @@
             nm = m
         nm.set_atoms(atoms)
         return nm
 
     @staticmethod
     def load_banddownfolder(path, prefix, atoms=None, nls=True, groupby="spin"):
         from banddownfolder.scdm.lwf import LWF
+
         lwf = LWF.load_nc(fname=os.path.join(path, f"{prefix}.nc"))
         nbasis = lwf.nwann
         nspin = 1
         positions = lwf.wann_centers
         ndim = lwf.ndim
         H_mnR = defaultdict(lambda: np.zeros((nbasis, nbasis), dtype=complex))
```

### Comparing `hamiltonio-0.1.0/HamiltonIO/wannier/utils.py` & `hamiltonio-0.1.1/HamiltonIO/wannier/utils.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.0/HamiltonIO/wannier/w90_parser.py` & `hamiltonio-0.1.1/HamiltonIO/wannier/w90_parser.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.0/HamiltonIO/wannier/w90_tb_parser.py` & `hamiltonio-0.1.1/HamiltonIO/wannier/w90_tb_parser.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.0/HamiltonIO/wantibexos/H_extract-siesta.py` & `hamiltonio-0.1.1/HamiltonIO/wantibexos/H_extract-siesta.py`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.0/HamiltonIO.egg-info/PKG-INFO` & `hamiltonio-0.1.1/HamiltonIO.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HamiltonIO
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for reading/writting Hamiltonian with localized basis set.
 Author-email: Xu He <mailhexu@gmail.com>
 License: BSD-2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
@@ -32,7 +32,17 @@
 Requires-Dist: pytest>=6.2.0; extra == "dev"
 Requires-Dist: black>=21.6b0; extra == "dev"
 Requires-Dist: pre-commit>=2.13.0; extra == "dev"
 Requires-Dist: sphinx>=4.1.2; extra == "dev"
 
 # HamiltonIO
 A library of IO of Hamiltonian files of DFT codes
+
+## Installation
+```bash
+pip install hamiltonIO
+```
+
+## Usage
+
+See the examples.
+
```

### Comparing `hamiltonio-0.1.0/HamiltonIO.egg-info/SOURCES.txt` & `hamiltonio-0.1.1/HamiltonIO.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 LICENSE
 README.md
 pyproject.toml
 HamiltonIO/__init__.py
-HamiltonIO/abstractTB.py
+HamiltonIO/hamiltonian.py
+HamiltonIO/orbital.py
 HamiltonIO.egg-info/PKG-INFO
 HamiltonIO.egg-info/SOURCES.txt
 HamiltonIO.egg-info/dependency_links.txt
 HamiltonIO.egg-info/requires.txt
 HamiltonIO.egg-info/top_level.txt
 HamiltonIO/abacus/__init__.py
 HamiltonIO/abacus/abacus_api.py
 HamiltonIO/abacus/abacus_wrapper.py
 HamiltonIO/abacus/orbital_api.py
 HamiltonIO/abacus/stru_api.py
 HamiltonIO/abacus/test_read_HRSR.py
 HamiltonIO/abacus/test_read_stru.py
+HamiltonIO/format/spmat.py
 HamiltonIO/siesta/__init__.py
 HamiltonIO/siesta/sisl_wrapper.py
 HamiltonIO/wannier/__init__.py
 HamiltonIO/wannier/myTB.py
 HamiltonIO/wannier/utils.py
 HamiltonIO/wannier/w90_parser.py
 HamiltonIO/wannier/w90_tb_parser.py
-HamiltonIO/wantibexos/H_extract-siesta.py
+HamiltonIO/wantibexos/H_extract-siesta.py
+HamiltonIO/wantibexos/output_wantibexos.py
```

### Comparing `hamiltonio-0.1.0/LICENSE` & `hamiltonio-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hamiltonio-0.1.0/PKG-INFO` & `hamiltonio-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HamiltonIO
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for reading/writting Hamiltonian with localized basis set.
 Author-email: Xu He <mailhexu@gmail.com>
 License: BSD-2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
@@ -32,7 +32,17 @@
 Requires-Dist: pytest>=6.2.0; extra == "dev"
 Requires-Dist: black>=21.6b0; extra == "dev"
 Requires-Dist: pre-commit>=2.13.0; extra == "dev"
 Requires-Dist: sphinx>=4.1.2; extra == "dev"
 
 # HamiltonIO
 A library of IO of Hamiltonian files of DFT codes
+
+## Installation
+```bash
+pip install hamiltonIO
+```
+
+## Usage
+
+See the examples.
+
```

### Comparing `hamiltonio-0.1.0/pyproject.toml` & `hamiltonio-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HamiltonIO"
-version = "0.1.0"
+version = "0.1.1"
 description = "A library for reading/writting Hamiltonian with localized basis set."
 authors = [
     {name = "Xu He", email = "mailhexu@gmail.com"},
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 license = {text = "BSD-2"}
```

