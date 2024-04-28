# Comparing `tmp/dropletevapmodel-0.1.tar.gz` & `tmp/dropletevapmodel-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dropletevapmodel-0.1.tar", last modified: Fri Feb 16 21:41:03 2024, max compression
+gzip compressed data, was "dropletevapmodel-0.2.0.tar", last modified: Sun Apr 28 13:08:49 2024, max compression
```

## Comparing `dropletevapmodel-0.1.tar` & `dropletevapmodel-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:41:03.139574 dropletevapmodel-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-16 21:40:57.000000 dropletevapmodel-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-16 21:40:57.000000 dropletevapmodel-0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20960 2024-02-16 21:41:03.139574 dropletevapmodel-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20584 2024-02-16 21:40:57.000000 dropletevapmodel-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-02-16 21:40:57.000000 dropletevapmodel-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-16 21:40:57.000000 dropletevapmodel-0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 21:41:03.139574 dropletevapmodel-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-16 21:40:57.000000 dropletevapmodel-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:41:03.135574 dropletevapmodel-0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:41:03.135574 dropletevapmodel-0.1/src/dropletevapmodel/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-16 21:40:57.000000 dropletevapmodel-0.1/src/dropletevapmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-02-16 21:40:57.000000 dropletevapmodel-0.1/src/dropletevapmodel/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-16 21:40:57.000000 dropletevapmodel-0.1/src/dropletevapmodel/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12506 2024-02-16 21:40:57.000000 dropletevapmodel-0.1/src/dropletevapmodel/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:41:03.139574 dropletevapmodel-0.1/src/dropletevapmodel/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-02-16 21:40:57.000000 dropletevapmodel-0.1/src/dropletevapmodel/models/phy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-02-16 21:40:57.000000 dropletevapmodel-0.1/src/dropletevapmodel/phy_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-16 21:40:57.000000 dropletevapmodel-0.1/src/dropletevapmodel/post_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:41:03.139574 dropletevapmodel-0.1/src/dropletevapmodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20960 2024-02-16 21:41:03.000000 dropletevapmodel-0.1/src/dropletevapmodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-16 21:41:03.000000 dropletevapmodel-0.1/src/dropletevapmodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 21:41:03.000000 dropletevapmodel-0.1/src/dropletevapmodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-16 21:41:03.000000 dropletevapmodel-0.1/src/dropletevapmodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-16 21:41:03.000000 dropletevapmodel-0.1/src/dropletevapmodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 21:41:02.000000 dropletevapmodel-0.1/src/dropletevapmodel.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:41:03.139574 dropletevapmodel-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-02-16 21:40:57.000000 dropletevapmodel-0.1/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:08:49.587447 dropletevapmodel-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 13:08:43.000000 dropletevapmodel-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-28 13:08:43.000000 dropletevapmodel-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23065 2024-04-28 13:08:49.587447 dropletevapmodel-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22688 2024-04-28 13:08:43.000000 dropletevapmodel-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-28 13:08:43.000000 dropletevapmodel-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 13:08:43.000000 dropletevapmodel-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 13:08:49.587447 dropletevapmodel-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-28 13:08:43.000000 dropletevapmodel-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:08:49.583447 dropletevapmodel-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:08:49.583447 dropletevapmodel-0.2.0/src/dropletevapmodel/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-28 13:08:43.000000 dropletevapmodel-0.2.0/src/dropletevapmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-28 13:08:43.000000 dropletevapmodel-0.2.0/src/dropletevapmodel/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-28 13:08:43.000000 dropletevapmodel-0.2.0/src/dropletevapmodel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12506 2024-04-28 13:08:43.000000 dropletevapmodel-0.2.0/src/dropletevapmodel/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:08:49.587447 dropletevapmodel-0.2.0/src/dropletevapmodel/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-28 13:08:43.000000 dropletevapmodel-0.2.0/src/dropletevapmodel/models/phy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-28 13:08:43.000000 dropletevapmodel-0.2.0/src/dropletevapmodel/phy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-28 13:08:43.000000 dropletevapmodel-0.2.0/src/dropletevapmodel/post_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:08:49.587447 dropletevapmodel-0.2.0/src/dropletevapmodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23065 2024-04-28 13:08:49.000000 dropletevapmodel-0.2.0/src/dropletevapmodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-28 13:08:49.000000 dropletevapmodel-0.2.0/src/dropletevapmodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 13:08:49.000000 dropletevapmodel-0.2.0/src/dropletevapmodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-28 13:08:49.000000 dropletevapmodel-0.2.0/src/dropletevapmodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 13:08:49.000000 dropletevapmodel-0.2.0/src/dropletevapmodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 13:08:49.000000 dropletevapmodel-0.2.0/src/dropletevapmodel.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:08:49.587447 dropletevapmodel-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-28 13:08:43.000000 dropletevapmodel-0.2.0/tests/test_model.py
```

### Comparing `dropletevapmodel-0.1/PKG-INFO` & `dropletevapmodel-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: dropletevapmodel
-Version: 0.1
-Summary: Droplet 0D evaporation model
-Author-email: Tommaso Gallingani <t.gallingani@gmail.com>
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pandas
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-Requires-Dist: seaborn
-Requires-Dist: Pyyaml
-Requires-Dist: tqdm
-Requires-Dist: pydantic
-
 # Droplet Evaporation 0D model
 ## How to install
 You can download the latest version of the repository from the GitHub page and then you can install the package with pip:
 
 ```bash
 pip install dropletevapmodel
 ```
@@ -80,21 +65,111 @@
 
 #### Import Necessary Modules
 
 ```python
 import tqdm
 import numpy as np
 from typing import Dict
+from dropletevapmodel import EvapModel, DropletEvapModel
+
+
+```
+#### Prepare your data model
+
+```python
+
+model_config = {
+    'simulation_config': {
+        'modelling': {
+            'timestep': 2e-05, # seconds
+            'max_iteration': 100000.0 # number of iteration
+        },
+        'environment': {
+            'pressure': 101325, # Pa
+            'pressure_atm': 101325, # Pa
+            'kb': 1.380649e-23, # J⋅K−1⋅mol−1
+            'drop_conc': 1000000000.0 # number/cm3
+        },
+        't_zero': {
+            'd_zero': 2.33315e-05, # Droplet diameter at t0 in m
+            't_d_zero': 293, # Droplet temperature at t0 in K
+            't_g_zero': 293, # Gas temperature at t0 in K
+            'water_content_g_zero': 0 # Water content at t0 in ppm
+        },
+        'output': {
+            'csv': True,
+            'plotting': True
+        }
+    }
+}
+
+```
+
+Liquid and gas properties can be added using the available database or loading custom data. Gas information can be added updating the model config dict.
 
-from ._utils import setup_logger
-from .models.phy_model import DropletEvapModel
-from .phy_utils import layer_temp, sat_pressure_g, vap_pressure_g, eval_omega, eval_diff_coeff, eval_vap_heat, eval_viscosity, eval_m_viscosity, eval_cp, eval_k, eval_phi
+```python
+
+model_config.update(
+  {
+    'gas_propeties': 
+      {
+      'mm_g': 39.948,  # g/mol
+      'sigma_g': 3.542,  # Angstrom
+      'eps_fact': 93.3,  # K
+      'r': 8.314,  # J/(mol*K)
+      'speed_g': 32.0,  # m/s
+      'viscosity_a': 6.1e-08,  # m^2/s
+      'viscosity_b': 3.33e-06,  # K
+      'cp_a': 20.786,  # J/mol
+      'cp_b': 2.83e-07,  # J/(mol*K)
+      'cp_c': -1.46e-07,  # J/(mol*K^2)
+      'cp_d': 1.09e-08,  # J/(mol*K^3)
+      'cp_e': -3.66e-09,  # J/(mol*K^4)
+      'k_a': -2.91e-05,  # W/(m*K)
+      'k_b': 0.068089,  # W/(m*K^2)
+      'k_c': -0.15  # W/(m*K^3)
+    }
+  }
+)
+
+```
+
+In the same way, liquid information can be added
+
+```python
+
+model_config.update(
+  {
+    'fluid_properties': 
+      {
+      'rho_d': 1000000.0,  # kg/m^3
+      'boiling_t': 373.0,  # K
+      'cp_l': 4.186,  # J/(g*K)
+      'mm_d': 18.0,  # g/mol
+      'sigma_d': 2.641,  # N/m
+      'eps_fact': 809.1,  # K
+      'speed_d': 32.0,  # m/s
+      'viscosity_a': 4.7e-08,  # m^2/s
+      'viscosity_b': 3.53e-06,  # K
+      'cp_a': 30.092,  # J/mol
+      'cp_b': 6.832514,  # J/(mol*K)
+      'cp_c': 6.793435,  # J/(mol*K^2)
+      'cp_d': -2.53448,  # J/(mol*K^3)
+      'cp_e': 0.082139,  # J/(mol*K^4)
+      'k_a': 7.75e-05,  # W/(m*K)
+      'k_b': 0.02255,  # W/(m*K^2)
+      'k_c': 4.815  # W/(m*K^3)
+  }
+
+  }
+)
 
 ```
 
+
 #### Load your DropletEvapModel instance
 
 ```python
 model_config = {...}  # Your data
 model_instance = DropletEvapModel(**model_config)
 
 evap_model = EvapModel(model=model_instance)
@@ -121,27 +196,27 @@
 
 
 
 ## Technical backgroud
 
 The 0-D model used for the simulation of a single droplet evaporation was developed according to a diffusion model based on mass and energy balance well reported in literature [[1]](#1) [[2]](#2), following the classical evaporation model (CEM) proposed by Spalding [[3]](#3) and Godsave [[4]](#4). This model was further improved following Abramzon-Sirignano approach [[5]](#5) [[6]](#6), that enabled a better account for advective mass and energy transport. A detailed description of the governing equations and limitations of this model was recently reviewed by Pinheiro et al. [[7]](#7). Mass and energy balances can be described according to following equations, respectively:
 
-$\frac{{d m_d}}{{dt}} = -\dot{m}_d$
+$\frac{{d m_d}}{{dt}} = -\dot{m}_d \quad (1)$
 
-$m_d \cdot c_{p_l} \frac{{dT_d}}{{dt}} = -Q_s$
+$m_d \cdot c_{p_l} \frac{{dT_d}}{{dt}} = -Q_s \quad (2)$
 
-where $m_d$ is the droplet mass, $\dot{m}_d$ is the mass evaporation rate, $`c_{p_l}`$ is the specific heat capacity of the liquid droplet, $T_d$ is the droplet temperature, and $Q_s$ is the net power transferred from the environment which contributes to droplet temperature increase.
+where $m_d$ is the droplet mass, $\dot{m}_d$ is the mass evaporation rate, ${c_p}_l$ is the specific heat capacity of the liquid droplet, $T_d$ is the droplet temperature, and $Q_s$ is the net power transferred from the environment which contributes to droplet temperature increase.
 
 Balance can be rewritten as a function of droplet diameter $D_d$, under the hypothesis of a spherical and homogeneous droplet:
 
 $\frac{{dD_d}}{{dt}} = -\frac{{2 \dot{m}_d}}{{\pi \rho_l D_d^2}} \quad (3)$
 
 According to the CEM model, widely discussed and applied in different fields of research to study droplet evaporation, based on mass and energy balance evaporation flow rate can be described according to the following equation:
 
-$`\dot{m}_d = \pi D_d D_{vm} \rho_m Sh_m \ln(1 + B_M) \quad (4)`$
+$\dot{m}_d = {\pi} D_d D_v \rho_m Sh_m \ln{(1 + B_M)} \quad (4)$
 
 where $D_v$ is the vapor diffusion coefficient, $\rho$ is the density, $Sh$ is the Sherwood number, and $B_M$ is the Spalding mass transfer number. It’s worth mentioning that all the physical properties were calculated in the region of gas-vapor film, considering the presence of both gas and water vapor species. Moreover, as described below, the temperature effect on the value of physical properties was included.
 
 <img src="docs/source/_static/schema_droplet.jpg" alt="Schematic droplet evaporation" width="400"/>
 
 
 The Spalding mass transfer number can be calculated using Equation (5):
@@ -176,29 +251,29 @@
 
 $Pr_m = \frac{{\mu_m c_{p_m}}}{{k_m}} \quad (12)$
 
 The correction factor $G$ can be expressed as a function of a non-dimensional evaporation parameter $\beta$:
 
 $G = \frac{\beta}{{e^\beta - 1}} \quad (13)$
 
-$`\beta = -\frac{\dot{m}_d c_{p_m}}{2\pi k_m D_d} \quad (14)`$
+$\beta = -\frac{\dot{m}_d {c_p}_m}{2\pi k_m D_d} \quad (14)$
 
 As detailed in several publications by Abramzon and Sirignano [[5]](#5) [[6]](#6), a more realistic approach can be used taking more precisely into account mass and energy transport. In this perspective, modification to the CEM model was carried out using two different correction factors ($F_M$ and $F_T$), based on the film theory considering the effect of Stefan’s flows at the liquid-gas interface.
 
 $F_M = \left(1 + B_M\right)^{0.7} \frac{\ln(1 + B_M)}{B_M} \quad (15)$
 
 $F_T = \left(1 + B_T\right)^{0.7} \frac{\ln(1 + B_T)}{B_T} \quad (16)$
 
 Where $B_T$ is the Spalding thermal energy transfer number calculated according to the following equations:
 
 $B_T = \left(1 + B_M\right)^\phi \quad (17)$
 
 $\phi = \frac{c_{p_v}/c_{p_g} \cdot Sh/Nu \cdot 1/\text{Le}_m} \quad (18)$
 
-$`\text{Le}_m = \frac{{k_m}}{{c_{p_m} D_{vm} \rho_m}} \quad (19)`$
+$\text{Le}_m = \frac{{k_m}}{{{c_p}_m D_v \rho_m}} \quad (19)$
 
 where $\text{Le}$ is Lewis number. The corrected value of $G$, $Sh^*$ and $Nu^*$ numbers that should be employed in Abramzon-Sirignano model are reported in the following equations:
 
 $Sh^* = 2 + \frac{{Sh_0 - 2}}{{F_M}} \quad (20)$
 
 $Nu^* = 2 + \frac{{Nu_0 - 2}}{{F_T}} \quad (21)$
 
@@ -210,29 +285,29 @@
 
 In the droplet proximity, gas-vapor properties can be described according to the film theory. A brief schematic representation of the droplet-gas environment and the “film region” is reported in Figure 4.3, where $T$ is the temperature and $Y$ is the vapor mass fraction. As reported by Hubbard et al. [[10]](#10) and Yuen and Chen [[11]](#11), temperature and other physical properties can be approximated using an averaging procedure (Equation (23)), where the weighting coefficient ($\alpha$) is 1/3 [[7]](#7).
 
 $T_m = T_s + \alpha (T_g - T_s) \quad (23)$
 
 Vapor diffusion coefficient ($D_{vm}, \, \text{cm}^2/\text{s}$) were calculated following the approach reported by Cussler [[12]](#12) and proposed by Chapman and Enskog:
 
-$`D_{vm} = \frac{{1.86 \times 10^{-3} T_m^{3/2} \left(\frac{1}{M_{Ar}} + \frac{1}{M_v}\right)}}{{p \times \sigma_{12} \times \Omega}} \quad (24)`$
+$D_{vm} = \frac{{1.86 \times 10^{-3} T_m^{3/2} \left(\frac{1}{M_{Ar}} + \frac{1}{M_v}\right)}}{{p \times \sigma_{12} \times \Omega}} \quad (24)$
 
 where $p$ is the process pressure in atm, $\sigma_{12}$ is the collisional diameter in Å, while $\Omega$ is a dimensionless factor that can be described according Lennard–Jones 12-6 potential. The temperature dependence of all these factors was taken into account by fitting the data reported in [[12]](#12) (Table 5.1-2, 5.1-3) for different temperature values.
 
 The fitting of experimental data on liquid enthalpy of vaporization ($L_v$) was used to calculate its dependence with respect to the droplet temperature ($T_d$). While gas density was calculated using the hypothesis of an ideal gas, dynamic viscosity ($\mu_m$) and gas thermal conductivity ($k_m$) at the film interface were obtained applying Wilke equation and Chapman-Enskog model [[13]](#13) to pure gas values obtained from NIST database [[14]](#14). Likewise, the specific heat capacity ($C_{pm}$) of gas mixture was calculated through an average weighted on the value of the single gas component obtained from NIST database [[15]](#15) [[16]](#16).
 
 ## Variation of Environment Vapor Content
 
 As a consequence of the droplet evaporation, the water vapor content of the environment increases during droplet shrinking. Since the model was developed to study droplet evaporation in a close-not infinite environment (because of the plasma source relatively low volume dimension with respect to droplet diameter), an increase of vapor content affects the driving force of liquid evaporation (mass concentration gradients) and should be considered.
 
 In this perspective, droplet concentration can be obtained using scanning mobility particle sizer (SMPS) data under the hypothesis of one droplet-one particle conversion, as widely discussed in literature [[17]](#17) [[18]](#18) [[19]](#19). Under the assumption that droplets are equally distributed in the space, each droplet can be considered at the center of a control volume whose dimension is the reciprocal of particle concentration. Following this hypothesis, the hypothetical control volume in which each droplet is contained is much larger than the droplet volume: for a droplet density of $10^5 \, \text{cm}^3$, each droplet is enclosed in a control volume of $10^6 \, \mu \text{m}^3$. If the particle size distribution is small enough (1-5 μm or below), the relative contribution of the droplet volume to the available gas volume can be neglected (for a 5 μm droplet, the ratio between liquid volume and control volume is 0.01 %).
 
 Under the hypothesis, the gas mass for each volume unit ($mass_{Ar}$) can be calculated using the gas ideal law. For each time step of the simulation ($\Delta t$), water content ($\text{ppm}_i$) was updated considering the initial vapor concentration ($\text{ppm}_0$) and the mass evaporated from the droplet ($m_d$), as reported in Equation (25).
 
-$`\text{ppm}_1 = \frac{{\text{ppm}_0 \cdot mass_{Ar} + m_d \cdot 10^6 \cdot \Delta t}}{{mass_{Ar}}} \quad \text{for } i=1 \ldots n  \quad (25) `$
+$\text{ppm}_1 = \frac{{\text{ppm}_0 \cdot mass_Ar + m_d \cdot 10^6 \cdot \Delta t}}{{mass_Ar}} \quad \text{for } i=1 \ldots n  \quad (25)$
 
 ## Assumptions and Limitation of the Simulative Model
 
 
 It's important to note that the model presented here is characterized by certain assumptions and limitations. According to the literature, these factors may marginally affect the obtained results. However, since the model's output will be compared to experimental results, it's essential to highlight the main hypotheses on which the model is based.
 
 ## Gas Temperature Assumption
```

### Comparing `dropletevapmodel-0.1/README.md` & `dropletevapmodel-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: dropletevapmodel
+Version: 0.2.0
+Summary: Droplet 0D evaporation model
+Author-email: Tommaso Gallingani <t.gallingani@gmail.com>
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: Pyyaml
+Requires-Dist: tqdm
+Requires-Dist: pydantic
+
 # Droplet Evaporation 0D model
 ## How to install
 You can download the latest version of the repository from the GitHub page and then you can install the package with pip:
 
 ```bash
 pip install dropletevapmodel
 ```
@@ -65,21 +80,111 @@
 
 #### Import Necessary Modules
 
 ```python
 import tqdm
 import numpy as np
 from typing import Dict
+from dropletevapmodel import EvapModel, DropletEvapModel
+
+
+```
+#### Prepare your data model
+
+```python
+
+model_config = {
+    'simulation_config': {
+        'modelling': {
+            'timestep': 2e-05, # seconds
+            'max_iteration': 100000.0 # number of iteration
+        },
+        'environment': {
+            'pressure': 101325, # Pa
+            'pressure_atm': 101325, # Pa
+            'kb': 1.380649e-23, # J⋅K−1⋅mol−1
+            'drop_conc': 1000000000.0 # number/cm3
+        },
+        't_zero': {
+            'd_zero': 2.33315e-05, # Droplet diameter at t0 in m
+            't_d_zero': 293, # Droplet temperature at t0 in K
+            't_g_zero': 293, # Gas temperature at t0 in K
+            'water_content_g_zero': 0 # Water content at t0 in ppm
+        },
+        'output': {
+            'csv': True,
+            'plotting': True
+        }
+    }
+}
+
+```
+
+Liquid and gas properties can be added using the available database or loading custom data. Gas information can be added updating the model config dict.
 
-from ._utils import setup_logger
-from .models.phy_model import DropletEvapModel
-from .phy_utils import layer_temp, sat_pressure_g, vap_pressure_g, eval_omega, eval_diff_coeff, eval_vap_heat, eval_viscosity, eval_m_viscosity, eval_cp, eval_k, eval_phi
+```python
+
+model_config.update(
+  {
+    'gas_propeties': 
+      {
+      'mm_g': 39.948,  # g/mol
+      'sigma_g': 3.542,  # Angstrom
+      'eps_fact': 93.3,  # K
+      'r': 8.314,  # J/(mol*K)
+      'speed_g': 32.0,  # m/s
+      'viscosity_a': 6.1e-08,  # m^2/s
+      'viscosity_b': 3.33e-06,  # K
+      'cp_a': 20.786,  # J/mol
+      'cp_b': 2.83e-07,  # J/(mol*K)
+      'cp_c': -1.46e-07,  # J/(mol*K^2)
+      'cp_d': 1.09e-08,  # J/(mol*K^3)
+      'cp_e': -3.66e-09,  # J/(mol*K^4)
+      'k_a': -2.91e-05,  # W/(m*K)
+      'k_b': 0.068089,  # W/(m*K^2)
+      'k_c': -0.15  # W/(m*K^3)
+    }
+  }
+)
+
+```
+
+In the same way, liquid information can be added
+
+```python
+
+model_config.update(
+  {
+    'fluid_properties': 
+      {
+      'rho_d': 1000000.0,  # kg/m^3
+      'boiling_t': 373.0,  # K
+      'cp_l': 4.186,  # J/(g*K)
+      'mm_d': 18.0,  # g/mol
+      'sigma_d': 2.641,  # N/m
+      'eps_fact': 809.1,  # K
+      'speed_d': 32.0,  # m/s
+      'viscosity_a': 4.7e-08,  # m^2/s
+      'viscosity_b': 3.53e-06,  # K
+      'cp_a': 30.092,  # J/mol
+      'cp_b': 6.832514,  # J/(mol*K)
+      'cp_c': 6.793435,  # J/(mol*K^2)
+      'cp_d': -2.53448,  # J/(mol*K^3)
+      'cp_e': 0.082139,  # J/(mol*K^4)
+      'k_a': 7.75e-05,  # W/(m*K)
+      'k_b': 0.02255,  # W/(m*K^2)
+      'k_c': 4.815  # W/(m*K^3)
+  }
+
+  }
+)
 
 ```
 
+
 #### Load your DropletEvapModel instance
 
 ```python
 model_config = {...}  # Your data
 model_instance = DropletEvapModel(**model_config)
 
 evap_model = EvapModel(model=model_instance)
@@ -106,27 +211,27 @@
 
 
 
 ## Technical backgroud
 
 The 0-D model used for the simulation of a single droplet evaporation was developed according to a diffusion model based on mass and energy balance well reported in literature [[1]](#1) [[2]](#2), following the classical evaporation model (CEM) proposed by Spalding [[3]](#3) and Godsave [[4]](#4). This model was further improved following Abramzon-Sirignano approach [[5]](#5) [[6]](#6), that enabled a better account for advective mass and energy transport. A detailed description of the governing equations and limitations of this model was recently reviewed by Pinheiro et al. [[7]](#7). Mass and energy balances can be described according to following equations, respectively:
 
-$\frac{{d m_d}}{{dt}} = -\dot{m}_d$
+$\frac{{d m_d}}{{dt}} = -\dot{m}_d \quad (1)$
 
-$m_d \cdot c_{p_l} \frac{{dT_d}}{{dt}} = -Q_s$
+$m_d \cdot c_{p_l} \frac{{dT_d}}{{dt}} = -Q_s \quad (2)$
 
-where $m_d$ is the droplet mass, $\dot{m}_d$ is the mass evaporation rate, $`c_{p_l}`$ is the specific heat capacity of the liquid droplet, $T_d$ is the droplet temperature, and $Q_s$ is the net power transferred from the environment which contributes to droplet temperature increase.
+where $m_d$ is the droplet mass, $\dot{m}_d$ is the mass evaporation rate, ${c_p}_l$ is the specific heat capacity of the liquid droplet, $T_d$ is the droplet temperature, and $Q_s$ is the net power transferred from the environment which contributes to droplet temperature increase.
 
 Balance can be rewritten as a function of droplet diameter $D_d$, under the hypothesis of a spherical and homogeneous droplet:
 
 $\frac{{dD_d}}{{dt}} = -\frac{{2 \dot{m}_d}}{{\pi \rho_l D_d^2}} \quad (3)$
 
 According to the CEM model, widely discussed and applied in different fields of research to study droplet evaporation, based on mass and energy balance evaporation flow rate can be described according to the following equation:
 
-$`\dot{m}_d = \pi D_d D_{vm} \rho_m Sh_m \ln(1 + B_M) \quad (4)`$
+$\dot{m}_d = {\pi} D_d D_v \rho_m Sh_m \ln{(1 + B_M)} \quad (4)$
 
 where $D_v$ is the vapor diffusion coefficient, $\rho$ is the density, $Sh$ is the Sherwood number, and $B_M$ is the Spalding mass transfer number. It’s worth mentioning that all the physical properties were calculated in the region of gas-vapor film, considering the presence of both gas and water vapor species. Moreover, as described below, the temperature effect on the value of physical properties was included.
 
 <img src="docs/source/_static/schema_droplet.jpg" alt="Schematic droplet evaporation" width="400"/>
 
 
 The Spalding mass transfer number can be calculated using Equation (5):
@@ -161,29 +266,29 @@
 
 $Pr_m = \frac{{\mu_m c_{p_m}}}{{k_m}} \quad (12)$
 
 The correction factor $G$ can be expressed as a function of a non-dimensional evaporation parameter $\beta$:
 
 $G = \frac{\beta}{{e^\beta - 1}} \quad (13)$
 
-$`\beta = -\frac{\dot{m}_d c_{p_m}}{2\pi k_m D_d} \quad (14)`$
+$\beta = -\frac{\dot{m}_d {c_p}_m}{2\pi k_m D_d} \quad (14)$
 
 As detailed in several publications by Abramzon and Sirignano [[5]](#5) [[6]](#6), a more realistic approach can be used taking more precisely into account mass and energy transport. In this perspective, modification to the CEM model was carried out using two different correction factors ($F_M$ and $F_T$), based on the film theory considering the effect of Stefan’s flows at the liquid-gas interface.
 
 $F_M = \left(1 + B_M\right)^{0.7} \frac{\ln(1 + B_M)}{B_M} \quad (15)$
 
 $F_T = \left(1 + B_T\right)^{0.7} \frac{\ln(1 + B_T)}{B_T} \quad (16)$
 
 Where $B_T$ is the Spalding thermal energy transfer number calculated according to the following equations:
 
 $B_T = \left(1 + B_M\right)^\phi \quad (17)$
 
 $\phi = \frac{c_{p_v}/c_{p_g} \cdot Sh/Nu \cdot 1/\text{Le}_m} \quad (18)$
 
-$`\text{Le}_m = \frac{{k_m}}{{c_{p_m} D_{vm} \rho_m}} \quad (19)`$
+$\text{Le}_m = \frac{{k_m}}{{{c_p}_m D_v \rho_m}} \quad (19)$
 
 where $\text{Le}$ is Lewis number. The corrected value of $G$, $Sh^*$ and $Nu^*$ numbers that should be employed in Abramzon-Sirignano model are reported in the following equations:
 
 $Sh^* = 2 + \frac{{Sh_0 - 2}}{{F_M}} \quad (20)$
 
 $Nu^* = 2 + \frac{{Nu_0 - 2}}{{F_T}} \quad (21)$
 
@@ -195,29 +300,29 @@
 
 In the droplet proximity, gas-vapor properties can be described according to the film theory. A brief schematic representation of the droplet-gas environment and the “film region” is reported in Figure 4.3, where $T$ is the temperature and $Y$ is the vapor mass fraction. As reported by Hubbard et al. [[10]](#10) and Yuen and Chen [[11]](#11), temperature and other physical properties can be approximated using an averaging procedure (Equation (23)), where the weighting coefficient ($\alpha$) is 1/3 [[7]](#7).
 
 $T_m = T_s + \alpha (T_g - T_s) \quad (23)$
 
 Vapor diffusion coefficient ($D_{vm}, \, \text{cm}^2/\text{s}$) were calculated following the approach reported by Cussler [[12]](#12) and proposed by Chapman and Enskog:
 
-$`D_{vm} = \frac{{1.86 \times 10^{-3} T_m^{3/2} \left(\frac{1}{M_{Ar}} + \frac{1}{M_v}\right)}}{{p \times \sigma_{12} \times \Omega}} \quad (24)`$
+$D_{vm} = \frac{{1.86 \times 10^{-3} T_m^{3/2} \left(\frac{1}{M_{Ar}} + \frac{1}{M_v}\right)}}{{p \times \sigma_{12} \times \Omega}} \quad (24)$
 
 where $p$ is the process pressure in atm, $\sigma_{12}$ is the collisional diameter in Å, while $\Omega$ is a dimensionless factor that can be described according Lennard–Jones 12-6 potential. The temperature dependence of all these factors was taken into account by fitting the data reported in [[12]](#12) (Table 5.1-2, 5.1-3) for different temperature values.
 
 The fitting of experimental data on liquid enthalpy of vaporization ($L_v$) was used to calculate its dependence with respect to the droplet temperature ($T_d$). While gas density was calculated using the hypothesis of an ideal gas, dynamic viscosity ($\mu_m$) and gas thermal conductivity ($k_m$) at the film interface were obtained applying Wilke equation and Chapman-Enskog model [[13]](#13) to pure gas values obtained from NIST database [[14]](#14). Likewise, the specific heat capacity ($C_{pm}$) of gas mixture was calculated through an average weighted on the value of the single gas component obtained from NIST database [[15]](#15) [[16]](#16).
 
 ## Variation of Environment Vapor Content
 
 As a consequence of the droplet evaporation, the water vapor content of the environment increases during droplet shrinking. Since the model was developed to study droplet evaporation in a close-not infinite environment (because of the plasma source relatively low volume dimension with respect to droplet diameter), an increase of vapor content affects the driving force of liquid evaporation (mass concentration gradients) and should be considered.
 
 In this perspective, droplet concentration can be obtained using scanning mobility particle sizer (SMPS) data under the hypothesis of one droplet-one particle conversion, as widely discussed in literature [[17]](#17) [[18]](#18) [[19]](#19). Under the assumption that droplets are equally distributed in the space, each droplet can be considered at the center of a control volume whose dimension is the reciprocal of particle concentration. Following this hypothesis, the hypothetical control volume in which each droplet is contained is much larger than the droplet volume: for a droplet density of $10^5 \, \text{cm}^3$, each droplet is enclosed in a control volume of $10^6 \, \mu \text{m}^3$. If the particle size distribution is small enough (1-5 μm or below), the relative contribution of the droplet volume to the available gas volume can be neglected (for a 5 μm droplet, the ratio between liquid volume and control volume is 0.01 %).
 
 Under the hypothesis, the gas mass for each volume unit ($mass_{Ar}$) can be calculated using the gas ideal law. For each time step of the simulation ($\Delta t$), water content ($\text{ppm}_i$) was updated considering the initial vapor concentration ($\text{ppm}_0$) and the mass evaporated from the droplet ($m_d$), as reported in Equation (25).
 
-$`\text{ppm}_1 = \frac{{\text{ppm}_0 \cdot mass_{Ar} + m_d \cdot 10^6 \cdot \Delta t}}{{mass_{Ar}}} \quad \text{for } i=1 \ldots n  \quad (25) `$
+$\text{ppm}_1 = \frac{{\text{ppm}_0 \cdot mass_Ar + m_d \cdot 10^6 \cdot \Delta t}}{{mass_Ar}} \quad \text{for } i=1 \ldots n  \quad (25)$
 
 ## Assumptions and Limitation of the Simulative Model
 
 
 It's important to note that the model presented here is characterized by certain assumptions and limitations. According to the literature, these factors may marginally affect the obtained results. However, since the model's output will be compared to experimental results, it's essential to highlight the main hypotheses on which the model is based.
 
 ## Gas Temperature Assumption
@@ -290,8 +395,8 @@
 <a id="18">[18]</a>
 Chen T M and Chein H M 2017 Generation and Evaluation of Mono
 
 <a id="19">[19]</a>
 Hinds W C 1999 Aerosol technology: properties, behavior, and measurement of airborne particles (John Wiley & Sons)
 
 <a id="20">[20]</a>
-Gallingani T 2020 (Alma Mater Studiorum)
+Gallingani T 2020 (Alma Mater Studiorum)
```

### Comparing `dropletevapmodel-0.1/pyproject.toml` & `dropletevapmodel-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dropletevapmodel"
-version = "0.1"
+version = "0.2.0"
 authors = [
     { name = "Tommaso Gallingani", email = "t.gallingani@gmail.com" }
 ]
 description = "Droplet 0D evaporation model"
 readme = "README.md"
 # requires-python = ">=3.7"
```

### Comparing `dropletevapmodel-0.1/src/dropletevapmodel/_utils.py` & `dropletevapmodel-0.2.0/src/dropletevapmodel/_utils.py`

 * *Files identical despite different names*

### Comparing `dropletevapmodel-0.1/src/dropletevapmodel/model.py` & `dropletevapmodel-0.2.0/src/dropletevapmodel/model.py`

 * *Files identical despite different names*

### Comparing `dropletevapmodel-0.1/src/dropletevapmodel/models/phy_model.py` & `dropletevapmodel-0.2.0/src/dropletevapmodel/models/phy_model.py`

 * *Files identical despite different names*

### Comparing `dropletevapmodel-0.1/src/dropletevapmodel/phy_utils.py` & `dropletevapmodel-0.2.0/src/dropletevapmodel/phy_utils.py`

 * *Files identical despite different names*

### Comparing `dropletevapmodel-0.1/src/dropletevapmodel/post_process.py` & `dropletevapmodel-0.2.0/src/dropletevapmodel/post_process.py`

 * *Files identical despite different names*

### Comparing `dropletevapmodel-0.1/src/dropletevapmodel.egg-info/PKG-INFO` & `dropletevapmodel-0.2.0/src/dropletevapmodel.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropletevapmodel
-Version: 0.1
+Version: 0.2.0
 Summary: Droplet 0D evaporation model
 Author-email: Tommaso Gallingani <t.gallingani@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: matplotlib
@@ -80,20 +80,110 @@
 
 #### Import Necessary Modules
 
 ```python
 import tqdm
 import numpy as np
 from typing import Dict
+from dropletevapmodel import EvapModel, DropletEvapModel
 
-from ._utils import setup_logger
-from .models.phy_model import DropletEvapModel
-from .phy_utils import layer_temp, sat_pressure_g, vap_pressure_g, eval_omega, eval_diff_coeff, eval_vap_heat, eval_viscosity, eval_m_viscosity, eval_cp, eval_k, eval_phi
 
 ```
+#### Prepare your data model
+
+```python
+
+model_config = {
+    'simulation_config': {
+        'modelling': {
+            'timestep': 2e-05, # seconds
+            'max_iteration': 100000.0 # number of iteration
+        },
+        'environment': {
+            'pressure': 101325, # Pa
+            'pressure_atm': 101325, # Pa
+            'kb': 1.380649e-23, # J⋅K−1⋅mol−1
+            'drop_conc': 1000000000.0 # number/cm3
+        },
+        't_zero': {
+            'd_zero': 2.33315e-05, # Droplet diameter at t0 in m
+            't_d_zero': 293, # Droplet temperature at t0 in K
+            't_g_zero': 293, # Gas temperature at t0 in K
+            'water_content_g_zero': 0 # Water content at t0 in ppm
+        },
+        'output': {
+            'csv': True,
+            'plotting': True
+        }
+    }
+}
+
+```
+
+Liquid and gas properties can be added using the available database or loading custom data. Gas information can be added updating the model config dict.
+
+```python
+
+model_config.update(
+  {
+    'gas_propeties': 
+      {
+      'mm_g': 39.948,  # g/mol
+      'sigma_g': 3.542,  # Angstrom
+      'eps_fact': 93.3,  # K
+      'r': 8.314,  # J/(mol*K)
+      'speed_g': 32.0,  # m/s
+      'viscosity_a': 6.1e-08,  # m^2/s
+      'viscosity_b': 3.33e-06,  # K
+      'cp_a': 20.786,  # J/mol
+      'cp_b': 2.83e-07,  # J/(mol*K)
+      'cp_c': -1.46e-07,  # J/(mol*K^2)
+      'cp_d': 1.09e-08,  # J/(mol*K^3)
+      'cp_e': -3.66e-09,  # J/(mol*K^4)
+      'k_a': -2.91e-05,  # W/(m*K)
+      'k_b': 0.068089,  # W/(m*K^2)
+      'k_c': -0.15  # W/(m*K^3)
+    }
+  }
+)
+
+```
+
+In the same way, liquid information can be added
+
+```python
+
+model_config.update(
+  {
+    'fluid_properties': 
+      {
+      'rho_d': 1000000.0,  # kg/m^3
+      'boiling_t': 373.0,  # K
+      'cp_l': 4.186,  # J/(g*K)
+      'mm_d': 18.0,  # g/mol
+      'sigma_d': 2.641,  # N/m
+      'eps_fact': 809.1,  # K
+      'speed_d': 32.0,  # m/s
+      'viscosity_a': 4.7e-08,  # m^2/s
+      'viscosity_b': 3.53e-06,  # K
+      'cp_a': 30.092,  # J/mol
+      'cp_b': 6.832514,  # J/(mol*K)
+      'cp_c': 6.793435,  # J/(mol*K^2)
+      'cp_d': -2.53448,  # J/(mol*K^3)
+      'cp_e': 0.082139,  # J/(mol*K^4)
+      'k_a': 7.75e-05,  # W/(m*K)
+      'k_b': 0.02255,  # W/(m*K^2)
+      'k_c': 4.815  # W/(m*K^3)
+  }
+
+  }
+)
+
+```
+
 
 #### Load your DropletEvapModel instance
 
 ```python
 model_config = {...}  # Your data
 model_instance = DropletEvapModel(**model_config)
 
@@ -121,27 +211,27 @@
 
 
 
 ## Technical backgroud
 
 The 0-D model used for the simulation of a single droplet evaporation was developed according to a diffusion model based on mass and energy balance well reported in literature [[1]](#1) [[2]](#2), following the classical evaporation model (CEM) proposed by Spalding [[3]](#3) and Godsave [[4]](#4). This model was further improved following Abramzon-Sirignano approach [[5]](#5) [[6]](#6), that enabled a better account for advective mass and energy transport. A detailed description of the governing equations and limitations of this model was recently reviewed by Pinheiro et al. [[7]](#7). Mass and energy balances can be described according to following equations, respectively:
 
-$\frac{{d m_d}}{{dt}} = -\dot{m}_d$
+$\frac{{d m_d}}{{dt}} = -\dot{m}_d \quad (1)$
 
-$m_d \cdot c_{p_l} \frac{{dT_d}}{{dt}} = -Q_s$
+$m_d \cdot c_{p_l} \frac{{dT_d}}{{dt}} = -Q_s \quad (2)$
 
-where $m_d$ is the droplet mass, $\dot{m}_d$ is the mass evaporation rate, $`c_{p_l}`$ is the specific heat capacity of the liquid droplet, $T_d$ is the droplet temperature, and $Q_s$ is the net power transferred from the environment which contributes to droplet temperature increase.
+where $m_d$ is the droplet mass, $\dot{m}_d$ is the mass evaporation rate, ${c_p}_l$ is the specific heat capacity of the liquid droplet, $T_d$ is the droplet temperature, and $Q_s$ is the net power transferred from the environment which contributes to droplet temperature increase.
 
 Balance can be rewritten as a function of droplet diameter $D_d$, under the hypothesis of a spherical and homogeneous droplet:
 
 $\frac{{dD_d}}{{dt}} = -\frac{{2 \dot{m}_d}}{{\pi \rho_l D_d^2}} \quad (3)$
 
 According to the CEM model, widely discussed and applied in different fields of research to study droplet evaporation, based on mass and energy balance evaporation flow rate can be described according to the following equation:
 
-$`\dot{m}_d = \pi D_d D_{vm} \rho_m Sh_m \ln(1 + B_M) \quad (4)`$
+$\dot{m}_d = {\pi} D_d D_v \rho_m Sh_m \ln{(1 + B_M)} \quad (4)$
 
 where $D_v$ is the vapor diffusion coefficient, $\rho$ is the density, $Sh$ is the Sherwood number, and $B_M$ is the Spalding mass transfer number. It’s worth mentioning that all the physical properties were calculated in the region of gas-vapor film, considering the presence of both gas and water vapor species. Moreover, as described below, the temperature effect on the value of physical properties was included.
 
 <img src="docs/source/_static/schema_droplet.jpg" alt="Schematic droplet evaporation" width="400"/>
 
 
 The Spalding mass transfer number can be calculated using Equation (5):
@@ -176,29 +266,29 @@
 
 $Pr_m = \frac{{\mu_m c_{p_m}}}{{k_m}} \quad (12)$
 
 The correction factor $G$ can be expressed as a function of a non-dimensional evaporation parameter $\beta$:
 
 $G = \frac{\beta}{{e^\beta - 1}} \quad (13)$
 
-$`\beta = -\frac{\dot{m}_d c_{p_m}}{2\pi k_m D_d} \quad (14)`$
+$\beta = -\frac{\dot{m}_d {c_p}_m}{2\pi k_m D_d} \quad (14)$
 
 As detailed in several publications by Abramzon and Sirignano [[5]](#5) [[6]](#6), a more realistic approach can be used taking more precisely into account mass and energy transport. In this perspective, modification to the CEM model was carried out using two different correction factors ($F_M$ and $F_T$), based on the film theory considering the effect of Stefan’s flows at the liquid-gas interface.
 
 $F_M = \left(1 + B_M\right)^{0.7} \frac{\ln(1 + B_M)}{B_M} \quad (15)$
 
 $F_T = \left(1 + B_T\right)^{0.7} \frac{\ln(1 + B_T)}{B_T} \quad (16)$
 
 Where $B_T$ is the Spalding thermal energy transfer number calculated according to the following equations:
 
 $B_T = \left(1 + B_M\right)^\phi \quad (17)$
 
 $\phi = \frac{c_{p_v}/c_{p_g} \cdot Sh/Nu \cdot 1/\text{Le}_m} \quad (18)$
 
-$`\text{Le}_m = \frac{{k_m}}{{c_{p_m} D_{vm} \rho_m}} \quad (19)`$
+$\text{Le}_m = \frac{{k_m}}{{{c_p}_m D_v \rho_m}} \quad (19)$
 
 where $\text{Le}$ is Lewis number. The corrected value of $G$, $Sh^*$ and $Nu^*$ numbers that should be employed in Abramzon-Sirignano model are reported in the following equations:
 
 $Sh^* = 2 + \frac{{Sh_0 - 2}}{{F_M}} \quad (20)$
 
 $Nu^* = 2 + \frac{{Nu_0 - 2}}{{F_T}} \quad (21)$
 
@@ -210,29 +300,29 @@
 
 In the droplet proximity, gas-vapor properties can be described according to the film theory. A brief schematic representation of the droplet-gas environment and the “film region” is reported in Figure 4.3, where $T$ is the temperature and $Y$ is the vapor mass fraction. As reported by Hubbard et al. [[10]](#10) and Yuen and Chen [[11]](#11), temperature and other physical properties can be approximated using an averaging procedure (Equation (23)), where the weighting coefficient ($\alpha$) is 1/3 [[7]](#7).
 
 $T_m = T_s + \alpha (T_g - T_s) \quad (23)$
 
 Vapor diffusion coefficient ($D_{vm}, \, \text{cm}^2/\text{s}$) were calculated following the approach reported by Cussler [[12]](#12) and proposed by Chapman and Enskog:
 
-$`D_{vm} = \frac{{1.86 \times 10^{-3} T_m^{3/2} \left(\frac{1}{M_{Ar}} + \frac{1}{M_v}\right)}}{{p \times \sigma_{12} \times \Omega}} \quad (24)`$
+$D_{vm} = \frac{{1.86 \times 10^{-3} T_m^{3/2} \left(\frac{1}{M_{Ar}} + \frac{1}{M_v}\right)}}{{p \times \sigma_{12} \times \Omega}} \quad (24)$
 
 where $p$ is the process pressure in atm, $\sigma_{12}$ is the collisional diameter in Å, while $\Omega$ is a dimensionless factor that can be described according Lennard–Jones 12-6 potential. The temperature dependence of all these factors was taken into account by fitting the data reported in [[12]](#12) (Table 5.1-2, 5.1-3) for different temperature values.
 
 The fitting of experimental data on liquid enthalpy of vaporization ($L_v$) was used to calculate its dependence with respect to the droplet temperature ($T_d$). While gas density was calculated using the hypothesis of an ideal gas, dynamic viscosity ($\mu_m$) and gas thermal conductivity ($k_m$) at the film interface were obtained applying Wilke equation and Chapman-Enskog model [[13]](#13) to pure gas values obtained from NIST database [[14]](#14). Likewise, the specific heat capacity ($C_{pm}$) of gas mixture was calculated through an average weighted on the value of the single gas component obtained from NIST database [[15]](#15) [[16]](#16).
 
 ## Variation of Environment Vapor Content
 
 As a consequence of the droplet evaporation, the water vapor content of the environment increases during droplet shrinking. Since the model was developed to study droplet evaporation in a close-not infinite environment (because of the plasma source relatively low volume dimension with respect to droplet diameter), an increase of vapor content affects the driving force of liquid evaporation (mass concentration gradients) and should be considered.
 
 In this perspective, droplet concentration can be obtained using scanning mobility particle sizer (SMPS) data under the hypothesis of one droplet-one particle conversion, as widely discussed in literature [[17]](#17) [[18]](#18) [[19]](#19). Under the assumption that droplets are equally distributed in the space, each droplet can be considered at the center of a control volume whose dimension is the reciprocal of particle concentration. Following this hypothesis, the hypothetical control volume in which each droplet is contained is much larger than the droplet volume: for a droplet density of $10^5 \, \text{cm}^3$, each droplet is enclosed in a control volume of $10^6 \, \mu \text{m}^3$. If the particle size distribution is small enough (1-5 μm or below), the relative contribution of the droplet volume to the available gas volume can be neglected (for a 5 μm droplet, the ratio between liquid volume and control volume is 0.01 %).
 
 Under the hypothesis, the gas mass for each volume unit ($mass_{Ar}$) can be calculated using the gas ideal law. For each time step of the simulation ($\Delta t$), water content ($\text{ppm}_i$) was updated considering the initial vapor concentration ($\text{ppm}_0$) and the mass evaporated from the droplet ($m_d$), as reported in Equation (25).
 
-$`\text{ppm}_1 = \frac{{\text{ppm}_0 \cdot mass_{Ar} + m_d \cdot 10^6 \cdot \Delta t}}{{mass_{Ar}}} \quad \text{for } i=1 \ldots n  \quad (25) `$
+$\text{ppm}_1 = \frac{{\text{ppm}_0 \cdot mass_Ar + m_d \cdot 10^6 \cdot \Delta t}}{{mass_Ar}} \quad \text{for } i=1 \ldots n  \quad (25)$
 
 ## Assumptions and Limitation of the Simulative Model
 
 
 It's important to note that the model presented here is characterized by certain assumptions and limitations. According to the literature, these factors may marginally affect the obtained results. However, since the model's output will be compared to experimental results, it's essential to highlight the main hypotheses on which the model is based.
 
 ## Gas Temperature Assumption
```

### Comparing `dropletevapmodel-0.1/src/dropletevapmodel.egg-info/SOURCES.txt` & `dropletevapmodel-0.2.0/src/dropletevapmodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

