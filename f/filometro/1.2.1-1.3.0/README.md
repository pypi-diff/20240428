# Comparing `tmp/filometro-1.2.1.tar.gz` & `tmp/filometro-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filometro-1.2.1.tar", last modified: Sun Jul 16 21:53:49 2023, max compression
+gzip compressed data, was "filometro-1.3.0.tar", last modified: Sun Apr 28 19:53:15 2024, max compression
```

## Comparing `filometro-1.2.1.tar` & `filometro-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-16 21:53:49.127969 filometro-1.2.1/
--rw-r--r--   0 matheus   (1000) matheus   (1000)     1071 2022-03-17 02:44:05.000000 filometro-1.2.1/LICENSE
--rw-r--r--   0 matheus   (1000) matheus   (1000)    11182 2023-07-16 21:53:49.117969 filometro-1.2.1/PKG-INFO
--rw-r--r--   0 matheus   (1000) matheus   (1000)     9691 2022-12-23 01:57:30.000000 filometro-1.2.1/README.md
-drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-16 21:53:49.117969 filometro-1.2.1/filometro/
--rw-r--r--   0 matheus   (1000) matheus   (1000)      571 2023-07-16 21:51:10.000000 filometro-1.2.1/filometro/__init__.py
--rw-r--r--   0 matheus   (1000) matheus   (1000)     3064 2023-07-14 19:28:15.000000 filometro-1.2.1/filometro/dataclasses.py
--rw-r--r--   0 matheus   (1000) matheus   (1000)     2383 2023-07-16 21:51:10.000000 filometro-1.2.1/filometro/deolhonafila.py
--rw-r--r--   0 matheus   (1000) matheus   (1000)     4161 2022-12-23 01:57:30.000000 filometro-1.2.1/filometro/enums.py
--rw-r--r--   0 matheus   (1000) matheus   (1000)      212 2023-07-16 21:51:10.000000 filometro-1.2.1/filometro/exceptions.py
--rw-r--r--   0 matheus   (1000) matheus   (1000)     4299 2023-07-16 21:51:10.000000 filometro-1.2.1/filometro/filometro.py
-drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-16 21:53:49.117969 filometro-1.2.1/filometro.egg-info/
--rw-r--r--   0 matheus   (1000) matheus   (1000)    11182 2023-07-16 21:53:48.000000 filometro-1.2.1/filometro.egg-info/PKG-INFO
--rw-r--r--   0 matheus   (1000) matheus   (1000)      361 2023-07-16 21:53:49.000000 filometro-1.2.1/filometro.egg-info/SOURCES.txt
--rw-r--r--   0 matheus   (1000) matheus   (1000)        1 2023-07-16 21:53:48.000000 filometro-1.2.1/filometro.egg-info/dependency_links.txt
--rw-r--r--   0 matheus   (1000) matheus   (1000)        1 2022-03-29 22:27:15.000000 filometro-1.2.1/filometro.egg-info/not-zip-safe
--rw-r--r--   0 matheus   (1000) matheus   (1000)       17 2023-07-16 21:53:48.000000 filometro-1.2.1/filometro.egg-info/requires.txt
--rw-r--r--   0 matheus   (1000) matheus   (1000)       10 2023-07-16 21:53:49.000000 filometro-1.2.1/filometro.egg-info/top_level.txt
--rw-r--r--   0 matheus   (1000) matheus   (1000)       38 2023-07-16 21:53:49.127969 filometro-1.2.1/setup.cfg
--rw-r--r--   0 matheus   (1000) matheus   (1000)     3136 2022-10-21 23:35:36.000000 filometro-1.2.1/setup.py
+drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2024-04-28 19:53:15.936220 filometro-1.3.0/
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     1071 2022-03-17 02:44:05.000000 filometro-1.3.0/LICENSE
+-rw-r--r--   0 matheus   (1000) matheus   (1000)    11308 2024-04-28 19:53:15.936220 filometro-1.3.0/PKG-INFO
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     9805 2024-04-28 19:52:54.000000 filometro-1.3.0/README.md
+drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2024-04-28 19:53:15.926220 filometro-1.3.0/filometro/
+-rw-r--r--   0 matheus   (1000) matheus   (1000)      571 2024-04-28 19:52:54.000000 filometro-1.3.0/filometro/__init__.py
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     3100 2024-04-28 19:52:54.000000 filometro-1.3.0/filometro/dataclasses.py
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     2383 2023-07-16 21:51:10.000000 filometro-1.3.0/filometro/deolhonafila.py
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     4183 2024-04-28 19:52:54.000000 filometro-1.3.0/filometro/enums.py
+-rw-r--r--   0 matheus   (1000) matheus   (1000)      212 2023-07-16 21:51:10.000000 filometro-1.3.0/filometro/exceptions.py
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     4330 2024-04-28 19:52:54.000000 filometro-1.3.0/filometro/filometro.py
+drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2024-04-28 19:53:15.936220 filometro-1.3.0/filometro.egg-info/
+-rw-r--r--   0 matheus   (1000) matheus   (1000)    11308 2024-04-28 19:53:15.000000 filometro-1.3.0/filometro.egg-info/PKG-INFO
+-rw-r--r--   0 matheus   (1000) matheus   (1000)      412 2024-04-28 19:53:15.000000 filometro-1.3.0/filometro.egg-info/SOURCES.txt
+-rw-r--r--   0 matheus   (1000) matheus   (1000)        1 2024-04-28 19:53:15.000000 filometro-1.3.0/filometro.egg-info/dependency_links.txt
+-rw-r--r--   0 matheus   (1000) matheus   (1000)        1 2022-03-29 22:27:15.000000 filometro-1.3.0/filometro.egg-info/not-zip-safe
+-rw-r--r--   0 matheus   (1000) matheus   (1000)       17 2024-04-28 19:53:15.000000 filometro-1.3.0/filometro.egg-info/requires.txt
+-rw-r--r--   0 matheus   (1000) matheus   (1000)       10 2024-04-28 19:53:15.000000 filometro-1.3.0/filometro.egg-info/top_level.txt
+-rw-r--r--   0 matheus   (1000) matheus   (1000)       38 2024-04-28 19:53:15.936220 filometro-1.3.0/setup.cfg
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     3136 2022-10-21 23:35:36.000000 filometro-1.3.0/setup.py
+drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2024-04-28 19:53:15.936220 filometro-1.3.0/tests/
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     2221 2023-07-16 21:51:10.000000 filometro-1.3.0/tests/test_deolhonafila.py
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     7068 2024-04-28 19:52:54.000000 filometro-1.3.0/tests/test_filometro.py
```

### Comparing `filometro-1.2.1/LICENSE` & `filometro-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `filometro-1.2.1/PKG-INFO` & `filometro-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: filometro
-Version: 1.2.1
+Version: 1.3.0
 Summary: Obtenha os dados dos postos de vacinação da covid-19 em São Paulo
 Home-page: https://github.com/matheusfelipeog/filometro
 Author: Matheus Felipe
 Author-email: matheusfelipeog@protonmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/matheusfelipeog/filometro/issues
 Project-URL: Documentation, https://github.com/matheusfelipeog/filometro/tree/master#documentação
 Project-URL: Source Code, https://github.com/matheusfelipeog/filometro
 Keywords: filometro,de-olho-na-fila,data,sao-paulo,covid-19,vacina,vacinasampa,python,wrapper,coronavirus
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -24,14 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.27.1
 
 
 <h1 align="center">
     <img src="https://raw.githubusercontent.com/matheusfelipeog/filometro/master/.github/assets/images/logo.png" alt="Logo filometro" width="100px" />
     <br />Filometro
 </h1>
 
@@ -189,14 +189,15 @@
 >>> posto.pfizer                # '0' ou '1' caso pfizer não esteja ou esteja disponível.
 >>> posto.pfizer_baby           # '0' ou '1' caso pfizer baby não esteja ou esteja disponível.
 >>> posto.pfizer_bivalente      # '0' ou '1' caso pfizer bivalente não esteja ou esteja disponível.
 >>> posto.pfizer_pediatrica     # '0' ou '1' caso pfizer pediátrica não esteja ou esteja disponível.
 >>> posto.janssen               # '0' ou '1' caso janssen não esteja ou esteja disponível.
 >>> posto.influenza             # '0' ou '1' caso influenza não esteja ou esteja disponível.
 >>> posto.intercambialidade     # '0' ou '1' caso intercambialidade não esteja ou esteja disponível.
+>>> posto.dengue                # '0' ou '1' caso dengue não esteja ou esteja disponível.
 >>> posto.situation             # A última atualização da situação da fila.
 >>> posto.modality              # A modalidade da unidade.
 >>> posto.last_update           # Data e hora da última atualização no formato AAAA-MM-DD HH:MM:SS.MS.
 ```
 
 ### Métodos da classe Filometro
 
@@ -268,14 +269,15 @@
 >>> Immunizing.PFIZER_BABY
 >>> Immunizing.PFIZER_BIVALENTE
 >>> Immunizing.PFIZER_PEDIATRICA
 >>> Immunizing.CORONAVAC
 >>> Immunizing.CORONAVAC_PEDIATRICA
 >>> Immunizing.JANSSEN
 >>> Immunizing.INFLUENZA
+>>> Immunizing.DENGUE
 ```
 
 
 ## Contribuições
 
 Toda contribuição é super bem-vinda!
 
@@ -289,9 +291,7 @@
 
 Obrigado pelo interesse em colaborar de alguma forma com o projeto ❤
 
 
 ## Licença
 
 **Filometro** utiliza a *licença MIT* em todo seu código, confira suas condições em [MIT License](https://github.com/matheusfelipeog/filometro/blob/master/LICENSE).
-
-
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: filometro Version: 1.2.1 Summary: Obtenha os dados
+Metadata-Version: 2.1 Name: filometro Version: 1.3.0 Summary: Obtenha os dados
 dos postos de vacinaÃ§Ã£o da covid-19 em SÃ£o Paulo Home-page: https://
 github.com/matheusfelipeog/filometro Author: Matheus Felipe Author-email:
 matheusfelipeog@protonmail.com License: MIT License Project-URL: Bug Tracker,
 https://github.com/matheusfelipeog/filometro/issues Project-URL: Documentation,
 https://github.com/matheusfelipeog/filometro/tree/master#documentaÃ§Ã£o
 Project-URL: Source Code, https://github.com/matheusfelipeog/filometro
 Keywords: filometro,de-olho-na-fila,data,sao-paulo,covid-
-19,vacina,vacinasampa,python,wrapper,coronavirus Platform: UNKNOWN Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Information Technology Classifier:
-License :: OSI Approved :: MIT License Classifier: Natural Language ::
-Portuguese (Brazilian) Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Topic :: Software Development :: Libraries Classifier:
-Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
->=3.7 Description-Content-Type: text/markdown License-File: LICENSE
+19,vacina,vacinasampa,python,wrapper,coronavirus Classifier: Development Status
+:: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology Classifier: License ::
+OSI Approved :: MIT License Classifier: Natural Language :: Portuguese
+(Brazilian) Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python ::
+3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Requires-Python: >=3.7
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+requests>=2.27.1
                             ************ [[LLooggoo ffiilloommeettrroo]]
                                FFiilloommeettrroo ************
                                    Metadata
                      _[_P_y_P_I_]_[_L_i_c_e_n_s_e_ _M_I_T_]_[_T_o_t_a_l_ _D_o_w_n_l_o_a_d_s_]
                                     Status
                         _[_P_y_P_I_ _-_ _S_t_a_t_u_s_]_[_T_e_s_t_s_ _-_ _S_t_a_t_u_s_]
 ## Index - [O que Ã©?](#o-que-Ã©) - [InstalaÃ§Ã£o](#instalaÃ§Ã£o) - [Demo]
@@ -85,14 +86,15 @@
 esteja disponÃ­vel. >>> posto.pfizer_baby # '0' ou '1' caso pfizer baby nÃ£o
 esteja ou esteja disponÃ­vel. >>> posto.pfizer_bivalente # '0' ou '1' caso
 pfizer bivalente nÃ£o esteja ou esteja disponÃ­vel. >>> posto.pfizer_pediatrica
 # '0' ou '1' caso pfizer pediÃ¡trica nÃ£o esteja ou esteja disponÃ­vel. >>>
 posto.janssen # '0' ou '1' caso janssen nÃ£o esteja ou esteja disponÃ­vel. >>>
 posto.influenza # '0' ou '1' caso influenza nÃ£o esteja ou esteja disponÃ­vel.
 >>> posto.intercambialidade # '0' ou '1' caso intercambialidade nÃ£o esteja ou
+esteja disponÃ­vel. >>> posto.dengue # '0' ou '1' caso dengue nÃ£o esteja ou
 esteja disponÃ­vel. >>> posto.situation # A Ãºltima atualizaÃ§Ã£o da situaÃ§Ã£o
 da fila. >>> posto.modality # A modalidade da unidade. >>> posto.last_update #
 Data e hora da Ãºltima atualizaÃ§Ã£o no formato AAAA-MM-DD HH:MM:SS.MS. ``` ###
 MÃ©todos da classe Filometro ```python >>> filometro.reload() # Atualizar dados
 em memÃ³ria. >>> filometro.all_postos() # Obter todos os postos. >>>
 filometro.all_postos_open() # Obter todos os postos abertos. >>>
 filometro.all_postos_closed() # Obter todos os postos fechados. >>>
@@ -117,18 +119,19 @@
 Situation.NAO_FUNCIONANDO >>> Situation.SEM_FILA >>> Situation.FILA_PEQUENA >>>
 Situation.FILA_MEDIA >>> Situation.FILA_GRANDE ``` `Immunizing` - Representa os
 imunizantes disponÃ­veis nos postos no Estado de SÃ£o Paulo: ```python >>>
 Immunizing.ASTRAZENECA >>> Immunizing.INTERCAMBIALIDADE >>> Immunizing.PFIZER
 >>> Immunizing.PFIZER_BABY >>> Immunizing.PFIZER_BIVALENTE >>>
 Immunizing.PFIZER_PEDIATRICA >>> Immunizing.CORONAVAC >>>
 Immunizing.CORONAVAC_PEDIATRICA >>> Immunizing.JANSSEN >>> Immunizing.INFLUENZA
-``` ## ContribuiÃ§Ãµes Toda contribuiÃ§Ã£o Ã© super bem-vinda! Abaixo mostro
-com o que vocÃª pode contribuir: - Encontrou algum bug, quer propor uma nova
-funcionalidade ou conversar sobre o projeto? [Abra uma Issue](https://
-github.com/matheusfelipeog/filometro/issues) e descreva seu caso. - Existe uma
-issue aberta e vocÃª quer resolve-la, quer implementar uma nova funcionalidade
-ou melhorar a documentaÃ§Ã£o? FaÃ§a suas adiÃ§Ãµes e me envie um *Pull Request*
-- Gostou do projeto, mas nÃ£o quer ou ainda nÃ£o consegue contribuir com ele?
-Considere deixar uma estrela â­ para o **Filometro** Obrigado pelo interesse
-em colaborar de alguma forma com o projeto â¤ ## LicenÃ§a **Filometro**
-utiliza a *licenÃ§a MIT* em todo seu cÃ³digo, confira suas condiÃ§Ãµes em [MIT
-License](https://github.com/matheusfelipeog/filometro/blob/master/LICENSE).
+>>> Immunizing.DENGUE ``` ## ContribuiÃ§Ãµes Toda contribuiÃ§Ã£o Ã© super bem-
+vinda! Abaixo mostro com o que vocÃª pode contribuir: - Encontrou algum bug,
+quer propor uma nova funcionalidade ou conversar sobre o projeto? [Abra uma
+Issue](https://github.com/matheusfelipeog/filometro/issues) e descreva seu
+caso. - Existe uma issue aberta e vocÃª quer resolve-la, quer implementar uma
+nova funcionalidade ou melhorar a documentaÃ§Ã£o? FaÃ§a suas adiÃ§Ãµes e me
+envie um *Pull Request* - Gostou do projeto, mas nÃ£o quer ou ainda nÃ£o
+consegue contribuir com ele? Considere deixar uma estrela â­ para o
+**Filometro** Obrigado pelo interesse em colaborar de alguma forma com o
+projeto â¤ ## LicenÃ§a **Filometro** utiliza a *licenÃ§a MIT* em todo seu
+cÃ³digo, confira suas condiÃ§Ãµes em [MIT License](https://github.com/
+matheusfelipeog/filometro/blob/master/LICENSE).
```

### Comparing `filometro-1.2.1/README.md` & `filometro-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,15 @@
 >>> posto.pfizer                # '0' ou '1' caso pfizer não esteja ou esteja disponível.
 >>> posto.pfizer_baby           # '0' ou '1' caso pfizer baby não esteja ou esteja disponível.
 >>> posto.pfizer_bivalente      # '0' ou '1' caso pfizer bivalente não esteja ou esteja disponível.
 >>> posto.pfizer_pediatrica     # '0' ou '1' caso pfizer pediátrica não esteja ou esteja disponível.
 >>> posto.janssen               # '0' ou '1' caso janssen não esteja ou esteja disponível.
 >>> posto.influenza             # '0' ou '1' caso influenza não esteja ou esteja disponível.
 >>> posto.intercambialidade     # '0' ou '1' caso intercambialidade não esteja ou esteja disponível.
+>>> posto.dengue                # '0' ou '1' caso dengue não esteja ou esteja disponível.
 >>> posto.situation             # A última atualização da situação da fila.
 >>> posto.modality              # A modalidade da unidade.
 >>> posto.last_update           # Data e hora da última atualização no formato AAAA-MM-DD HH:MM:SS.MS.
 ```
 
 ### Métodos da classe Filometro
 
@@ -236,14 +237,15 @@
 >>> Immunizing.PFIZER_BABY
 >>> Immunizing.PFIZER_BIVALENTE
 >>> Immunizing.PFIZER_PEDIATRICA
 >>> Immunizing.CORONAVAC
 >>> Immunizing.CORONAVAC_PEDIATRICA
 >>> Immunizing.JANSSEN
 >>> Immunizing.INFLUENZA
+>>> Immunizing.DENGUE
 ```
 
 
 ## Contribuições
 
 Toda contribuição é super bem-vinda!
```

#### html2text {}

```diff
@@ -65,14 +65,15 @@
 esteja disponÃ­vel. >>> posto.pfizer_baby # '0' ou '1' caso pfizer baby nÃ£o
 esteja ou esteja disponÃ­vel. >>> posto.pfizer_bivalente # '0' ou '1' caso
 pfizer bivalente nÃ£o esteja ou esteja disponÃ­vel. >>> posto.pfizer_pediatrica
 # '0' ou '1' caso pfizer pediÃ¡trica nÃ£o esteja ou esteja disponÃ­vel. >>>
 posto.janssen # '0' ou '1' caso janssen nÃ£o esteja ou esteja disponÃ­vel. >>>
 posto.influenza # '0' ou '1' caso influenza nÃ£o esteja ou esteja disponÃ­vel.
 >>> posto.intercambialidade # '0' ou '1' caso intercambialidade nÃ£o esteja ou
+esteja disponÃ­vel. >>> posto.dengue # '0' ou '1' caso dengue nÃ£o esteja ou
 esteja disponÃ­vel. >>> posto.situation # A Ãºltima atualizaÃ§Ã£o da situaÃ§Ã£o
 da fila. >>> posto.modality # A modalidade da unidade. >>> posto.last_update #
 Data e hora da Ãºltima atualizaÃ§Ã£o no formato AAAA-MM-DD HH:MM:SS.MS. ``` ###
 MÃ©todos da classe Filometro ```python >>> filometro.reload() # Atualizar dados
 em memÃ³ria. >>> filometro.all_postos() # Obter todos os postos. >>>
 filometro.all_postos_open() # Obter todos os postos abertos. >>>
 filometro.all_postos_closed() # Obter todos os postos fechados. >>>
@@ -97,18 +98,19 @@
 Situation.NAO_FUNCIONANDO >>> Situation.SEM_FILA >>> Situation.FILA_PEQUENA >>>
 Situation.FILA_MEDIA >>> Situation.FILA_GRANDE ``` `Immunizing` - Representa os
 imunizantes disponÃ­veis nos postos no Estado de SÃ£o Paulo: ```python >>>
 Immunizing.ASTRAZENECA >>> Immunizing.INTERCAMBIALIDADE >>> Immunizing.PFIZER
 >>> Immunizing.PFIZER_BABY >>> Immunizing.PFIZER_BIVALENTE >>>
 Immunizing.PFIZER_PEDIATRICA >>> Immunizing.CORONAVAC >>>
 Immunizing.CORONAVAC_PEDIATRICA >>> Immunizing.JANSSEN >>> Immunizing.INFLUENZA
-``` ## ContribuiÃ§Ãµes Toda contribuiÃ§Ã£o Ã© super bem-vinda! Abaixo mostro
-com o que vocÃª pode contribuir: - Encontrou algum bug, quer propor uma nova
-funcionalidade ou conversar sobre o projeto? [Abra uma Issue](https://
-github.com/matheusfelipeog/filometro/issues) e descreva seu caso. - Existe uma
-issue aberta e vocÃª quer resolve-la, quer implementar uma nova funcionalidade
-ou melhorar a documentaÃ§Ã£o? FaÃ§a suas adiÃ§Ãµes e me envie um *Pull Request*
-- Gostou do projeto, mas nÃ£o quer ou ainda nÃ£o consegue contribuir com ele?
-Considere deixar uma estrela â­ para o **Filometro** Obrigado pelo interesse
-em colaborar de alguma forma com o projeto â¤ ## LicenÃ§a **Filometro**
-utiliza a *licenÃ§a MIT* em todo seu cÃ³digo, confira suas condiÃ§Ãµes em [MIT
-License](https://github.com/matheusfelipeog/filometro/blob/master/LICENSE).
+>>> Immunizing.DENGUE ``` ## ContribuiÃ§Ãµes Toda contribuiÃ§Ã£o Ã© super bem-
+vinda! Abaixo mostro com o que vocÃª pode contribuir: - Encontrou algum bug,
+quer propor uma nova funcionalidade ou conversar sobre o projeto? [Abra uma
+Issue](https://github.com/matheusfelipeog/filometro/issues) e descreva seu
+caso. - Existe uma issue aberta e vocÃª quer resolve-la, quer implementar uma
+nova funcionalidade ou melhorar a documentaÃ§Ã£o? FaÃ§a suas adiÃ§Ãµes e me
+envie um *Pull Request* - Gostou do projeto, mas nÃ£o quer ou ainda nÃ£o
+consegue contribuir com ele? Considere deixar uma estrela â­ para o
+**Filometro** Obrigado pelo interesse em colaborar de alguma forma com o
+projeto â¤ ## LicenÃ§a **Filometro** utiliza a *licenÃ§a MIT* em todo seu
+cÃ³digo, confira suas condiÃ§Ãµes em [MIT License](https://github.com/
+matheusfelipeog/filometro/blob/master/LICENSE).
```

### Comparing `filometro-1.2.1/filometro/__init__.py` & `filometro-1.3.0/filometro/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'Zone',
     'Modality',
     'Situation',
     'Immunizing',
     'District',
     'Filometro'
 ]
-__version__ = '1.2.1'
+__version__ = '1.3.0'
 __author__ = 'Matheus Felipe'
 
 from filometro.enums import Zone
 from filometro.enums import Modality
 from filometro.enums import Situation
 from filometro.enums import Immunizing
 from filometro.enums import District
```

### Comparing `filometro-1.2.1/filometro/dataclasses.py` & `filometro-1.3.0/filometro/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     pfizer: str = field(repr=False)
     pfizer_baby: str = field(repr=False)
     pfizer_bivalente: str = field(repr=False)
     pfizer_pediatrica: str = field(repr=False)
     janssen: str = field(repr=False)
     influenza: str = field(repr=False)
     intercambialidade: str = field(repr=False)
+    dengue: str = field(repr=False)
     situation: str = field(repr=False)           # status_fila
     modality: str = field(repr=False)            # tipo_posto
     last_update: str                             # data_hora
     _index_situation: str = field(repr=False)    # indice_fila
     _id_district: str = field(repr=False)        # id_distrito
     _id_zone: str = field(repr=False)            # id_crs
     _id_tb_unidades: str = field(repr=False)
```

### Comparing `filometro-1.2.1/filometro/deolhonafila.py` & `filometro-1.3.0/filometro/deolhonafila.py`

 * *Files identical despite different names*

### Comparing `filometro-1.2.1/filometro/enums.py` & `filometro-1.3.0/filometro/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     PFIZER_BABY = 'pfizer_baby'
     PFIZER_BIVALENTE = 'pfizer_bivalente'
     PFIZER_PEDIATRICA = 'pfizer_pediatrica'
     CORONAVAC = 'coronavac'
     CORONAVAC_PEDIATRICA = 'coronavac_pediatrica'
     JANSSEN = 'janssen'
     INFLUENZA = 'influenza'
+    DENGUE = 'dengue'
 
 
 class District(Enum):
     """Fornece todos os distritos onde há um ou mais postos."""
 
     AGUA_RASA = 'Água Rasa'
     ALTO_DE_PINHEIROS = 'Alto de Pinheiros'
```

### Comparing `filometro-1.2.1/filometro/filometro.py` & `filometro-1.3.0/filometro/filometro.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         pfizer=data['pfizer'],
         pfizer_baby=data['pfizer_baby'],
         pfizer_bivalente=data['pfizer_bivalente'],
         pfizer_pediatrica=data['pfizer_ped'],
         janssen=data['janssen'],
         influenza=data['influenza'],
         intercambialidade=data['intercambialidade'],
+        dengue=data['dengue'],
         situation=data['status_fila'],
         modality=data['tipo_posto'],
         last_update=data['data_hora'],
         _index_situation=data['indice_fila'],
         _id_district=data['id_distrito'],
         _id_zone=data['id_crs'],
         _id_tb_unidades=data['id_tb_unidades'],
```

### Comparing `filometro-1.2.1/filometro.egg-info/PKG-INFO` & `filometro-1.3.0/filometro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: filometro
-Version: 1.2.1
+Version: 1.3.0
 Summary: Obtenha os dados dos postos de vacinação da covid-19 em São Paulo
 Home-page: https://github.com/matheusfelipeog/filometro
 Author: Matheus Felipe
 Author-email: matheusfelipeog@protonmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/matheusfelipeog/filometro/issues
 Project-URL: Documentation, https://github.com/matheusfelipeog/filometro/tree/master#documentação
 Project-URL: Source Code, https://github.com/matheusfelipeog/filometro
 Keywords: filometro,de-olho-na-fila,data,sao-paulo,covid-19,vacina,vacinasampa,python,wrapper,coronavirus
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -24,14 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.27.1
 
 
 <h1 align="center">
     <img src="https://raw.githubusercontent.com/matheusfelipeog/filometro/master/.github/assets/images/logo.png" alt="Logo filometro" width="100px" />
     <br />Filometro
 </h1>
 
@@ -189,14 +189,15 @@
 >>> posto.pfizer                # '0' ou '1' caso pfizer não esteja ou esteja disponível.
 >>> posto.pfizer_baby           # '0' ou '1' caso pfizer baby não esteja ou esteja disponível.
 >>> posto.pfizer_bivalente      # '0' ou '1' caso pfizer bivalente não esteja ou esteja disponível.
 >>> posto.pfizer_pediatrica     # '0' ou '1' caso pfizer pediátrica não esteja ou esteja disponível.
 >>> posto.janssen               # '0' ou '1' caso janssen não esteja ou esteja disponível.
 >>> posto.influenza             # '0' ou '1' caso influenza não esteja ou esteja disponível.
 >>> posto.intercambialidade     # '0' ou '1' caso intercambialidade não esteja ou esteja disponível.
+>>> posto.dengue                # '0' ou '1' caso dengue não esteja ou esteja disponível.
 >>> posto.situation             # A última atualização da situação da fila.
 >>> posto.modality              # A modalidade da unidade.
 >>> posto.last_update           # Data e hora da última atualização no formato AAAA-MM-DD HH:MM:SS.MS.
 ```
 
 ### Métodos da classe Filometro
 
@@ -268,14 +269,15 @@
 >>> Immunizing.PFIZER_BABY
 >>> Immunizing.PFIZER_BIVALENTE
 >>> Immunizing.PFIZER_PEDIATRICA
 >>> Immunizing.CORONAVAC
 >>> Immunizing.CORONAVAC_PEDIATRICA
 >>> Immunizing.JANSSEN
 >>> Immunizing.INFLUENZA
+>>> Immunizing.DENGUE
 ```
 
 
 ## Contribuições
 
 Toda contribuição é super bem-vinda!
 
@@ -289,9 +291,7 @@
 
 Obrigado pelo interesse em colaborar de alguma forma com o projeto ❤
 
 
 ## Licença
 
 **Filometro** utiliza a *licença MIT* em todo seu código, confira suas condições em [MIT License](https://github.com/matheusfelipeog/filometro/blob/master/LICENSE).
-
-
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: filometro Version: 1.2.1 Summary: Obtenha os dados
+Metadata-Version: 2.1 Name: filometro Version: 1.3.0 Summary: Obtenha os dados
 dos postos de vacinaÃ§Ã£o da covid-19 em SÃ£o Paulo Home-page: https://
 github.com/matheusfelipeog/filometro Author: Matheus Felipe Author-email:
 matheusfelipeog@protonmail.com License: MIT License Project-URL: Bug Tracker,
 https://github.com/matheusfelipeog/filometro/issues Project-URL: Documentation,
 https://github.com/matheusfelipeog/filometro/tree/master#documentaÃ§Ã£o
 Project-URL: Source Code, https://github.com/matheusfelipeog/filometro
 Keywords: filometro,de-olho-na-fila,data,sao-paulo,covid-
-19,vacina,vacinasampa,python,wrapper,coronavirus Platform: UNKNOWN Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Information Technology Classifier:
-License :: OSI Approved :: MIT License Classifier: Natural Language ::
-Portuguese (Brazilian) Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Topic :: Software Development :: Libraries Classifier:
-Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
->=3.7 Description-Content-Type: text/markdown License-File: LICENSE
+19,vacina,vacinasampa,python,wrapper,coronavirus Classifier: Development Status
+:: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology Classifier: License ::
+OSI Approved :: MIT License Classifier: Natural Language :: Portuguese
+(Brazilian) Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python ::
+3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Requires-Python: >=3.7
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+requests>=2.27.1
                             ************ [[LLooggoo ffiilloommeettrroo]]
                                FFiilloommeettrroo ************
                                    Metadata
                      _[_P_y_P_I_]_[_L_i_c_e_n_s_e_ _M_I_T_]_[_T_o_t_a_l_ _D_o_w_n_l_o_a_d_s_]
                                     Status
                         _[_P_y_P_I_ _-_ _S_t_a_t_u_s_]_[_T_e_s_t_s_ _-_ _S_t_a_t_u_s_]
 ## Index - [O que Ã©?](#o-que-Ã©) - [InstalaÃ§Ã£o](#instalaÃ§Ã£o) - [Demo]
@@ -85,14 +86,15 @@
 esteja disponÃ­vel. >>> posto.pfizer_baby # '0' ou '1' caso pfizer baby nÃ£o
 esteja ou esteja disponÃ­vel. >>> posto.pfizer_bivalente # '0' ou '1' caso
 pfizer bivalente nÃ£o esteja ou esteja disponÃ­vel. >>> posto.pfizer_pediatrica
 # '0' ou '1' caso pfizer pediÃ¡trica nÃ£o esteja ou esteja disponÃ­vel. >>>
 posto.janssen # '0' ou '1' caso janssen nÃ£o esteja ou esteja disponÃ­vel. >>>
 posto.influenza # '0' ou '1' caso influenza nÃ£o esteja ou esteja disponÃ­vel.
 >>> posto.intercambialidade # '0' ou '1' caso intercambialidade nÃ£o esteja ou
+esteja disponÃ­vel. >>> posto.dengue # '0' ou '1' caso dengue nÃ£o esteja ou
 esteja disponÃ­vel. >>> posto.situation # A Ãºltima atualizaÃ§Ã£o da situaÃ§Ã£o
 da fila. >>> posto.modality # A modalidade da unidade. >>> posto.last_update #
 Data e hora da Ãºltima atualizaÃ§Ã£o no formato AAAA-MM-DD HH:MM:SS.MS. ``` ###
 MÃ©todos da classe Filometro ```python >>> filometro.reload() # Atualizar dados
 em memÃ³ria. >>> filometro.all_postos() # Obter todos os postos. >>>
 filometro.all_postos_open() # Obter todos os postos abertos. >>>
 filometro.all_postos_closed() # Obter todos os postos fechados. >>>
@@ -117,18 +119,19 @@
 Situation.NAO_FUNCIONANDO >>> Situation.SEM_FILA >>> Situation.FILA_PEQUENA >>>
 Situation.FILA_MEDIA >>> Situation.FILA_GRANDE ``` `Immunizing` - Representa os
 imunizantes disponÃ­veis nos postos no Estado de SÃ£o Paulo: ```python >>>
 Immunizing.ASTRAZENECA >>> Immunizing.INTERCAMBIALIDADE >>> Immunizing.PFIZER
 >>> Immunizing.PFIZER_BABY >>> Immunizing.PFIZER_BIVALENTE >>>
 Immunizing.PFIZER_PEDIATRICA >>> Immunizing.CORONAVAC >>>
 Immunizing.CORONAVAC_PEDIATRICA >>> Immunizing.JANSSEN >>> Immunizing.INFLUENZA
-``` ## ContribuiÃ§Ãµes Toda contribuiÃ§Ã£o Ã© super bem-vinda! Abaixo mostro
-com o que vocÃª pode contribuir: - Encontrou algum bug, quer propor uma nova
-funcionalidade ou conversar sobre o projeto? [Abra uma Issue](https://
-github.com/matheusfelipeog/filometro/issues) e descreva seu caso. - Existe uma
-issue aberta e vocÃª quer resolve-la, quer implementar uma nova funcionalidade
-ou melhorar a documentaÃ§Ã£o? FaÃ§a suas adiÃ§Ãµes e me envie um *Pull Request*
-- Gostou do projeto, mas nÃ£o quer ou ainda nÃ£o consegue contribuir com ele?
-Considere deixar uma estrela â­ para o **Filometro** Obrigado pelo interesse
-em colaborar de alguma forma com o projeto â¤ ## LicenÃ§a **Filometro**
-utiliza a *licenÃ§a MIT* em todo seu cÃ³digo, confira suas condiÃ§Ãµes em [MIT
-License](https://github.com/matheusfelipeog/filometro/blob/master/LICENSE).
+>>> Immunizing.DENGUE ``` ## ContribuiÃ§Ãµes Toda contribuiÃ§Ã£o Ã© super bem-
+vinda! Abaixo mostro com o que vocÃª pode contribuir: - Encontrou algum bug,
+quer propor uma nova funcionalidade ou conversar sobre o projeto? [Abra uma
+Issue](https://github.com/matheusfelipeog/filometro/issues) e descreva seu
+caso. - Existe uma issue aberta e vocÃª quer resolve-la, quer implementar uma
+nova funcionalidade ou melhorar a documentaÃ§Ã£o? FaÃ§a suas adiÃ§Ãµes e me
+envie um *Pull Request* - Gostou do projeto, mas nÃ£o quer ou ainda nÃ£o
+consegue contribuir com ele? Considere deixar uma estrela â­ para o
+**Filometro** Obrigado pelo interesse em colaborar de alguma forma com o
+projeto â¤ ## LicenÃ§a **Filometro** utiliza a *licenÃ§a MIT* em todo seu
+cÃ³digo, confira suas condiÃ§Ãµes em [MIT License](https://github.com/
+matheusfelipeog/filometro/blob/master/LICENSE).
```

### Comparing `filometro-1.2.1/setup.py` & `filometro-1.3.0/setup.py`

 * *Files identical despite different names*

