# Comparing `tmp/api-omie-0.3.12.tar.gz` & `tmp/api_omie-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api-omie-0.3.12.tar", last modified: Mon Mar 25 03:58:30 2024, max compression
+gzip compressed data, was "api_omie-0.3.8.tar", last modified: Sat Apr 27 23:58:07 2024, max compression
```

## Comparing `api-omie-0.3.12.tar` & `api_omie-0.3.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 03:58:30.462724 api-omie-0.3.12/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-25 03:58:27.000000 api-omie-0.3.12/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-03-25 03:58:30.462724 api-omie-0.3.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-25 03:58:27.000000 api-omie-0.3.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 03:58:30.462724 api-omie-0.3.12/api_omie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-03-25 03:58:30.000000 api-omie-0.3.12/api_omie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-25 03:58:30.000000 api-omie-0.3.12/api_omie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 03:58:30.000000 api-omie-0.3.12/api_omie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-25 03:58:30.000000 api-omie-0.3.12/api_omie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-25 03:58:30.000000 api-omie-0.3.12/api_omie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 03:58:30.462724 api-omie-0.3.12/omieapi/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-25 03:58:27.000000 api-omie-0.3.12/omieapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 03:58:30.462724 api-omie-0.3.12/omieapi/core/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-25 03:58:27.000000 api-omie-0.3.12/omieapi/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-03-25 03:58:27.000000 api-omie-0.3.12/omieapi/core/omiebase.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-25 03:58:27.000000 api-omie-0.3.12/omieapi/omie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 03:58:30.462724 api-omie-0.3.12/omieapi/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-25 03:58:27.000000 api-omie-0.3.12/omieapi/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   116800 2024-03-25 03:58:27.000000 api-omie-0.3.12/omieapi/scripts/cod_automatico.py
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-03-25 03:58:27.000000 api-omie-0.3.12/omieapi/scripts/scrap.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 03:58:30.462724 api-omie-0.3.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-25 03:58:27.000000 api-omie-0.3.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:07.303317 api_omie-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-27 23:58:04.000000 api_omie-0.3.8/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-27 23:58:07.303317 api_omie-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-27 23:58:04.000000 api_omie-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:07.303317 api_omie-0.3.8/api_omie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-27 23:58:07.000000 api_omie-0.3.8/api_omie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-27 23:58:07.000000 api_omie-0.3.8/api_omie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 23:58:07.000000 api_omie-0.3.8/api_omie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-27 23:58:07.000000 api_omie-0.3.8/api_omie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-27 23:58:07.000000 api_omie-0.3.8/api_omie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:07.303317 api_omie-0.3.8/omieapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-27 23:58:04.000000 api_omie-0.3.8/omieapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:07.303317 api_omie-0.3.8/omieapi/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-27 23:58:04.000000 api_omie-0.3.8/omieapi/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-27 23:58:04.000000 api_omie-0.3.8/omieapi/core/omiebase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-27 23:58:04.000000 api_omie-0.3.8/omieapi/omie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 23:58:07.303317 api_omie-0.3.8/omieapi/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 23:58:04.000000 api_omie-0.3.8/omieapi/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116800 2024-04-27 23:58:04.000000 api_omie-0.3.8/omieapi/scripts/cod_automatico.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-27 23:58:04.000000 api_omie-0.3.8/omieapi/scripts/scrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 23:58:07.303317 api_omie-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-27 23:58:04.000000 api_omie-0.3.8/setup.py
```

### Comparing `api-omie-0.3.12/LICENCE` & `api_omie-0.3.8/LICENCE`

 * *Files identical despite different names*

### Comparing `api-omie-0.3.12/PKG-INFO` & `api_omie-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-omie
-Version: 0.3.12
+Version: 0.3.8
 Summary: Ferramenta para api do omie não oficial
 Home-page: https://github.com/MikalROn/ApiOmie-nao-oficial
 Author: Daniel Coêlho
 Author-email: heromon.9010@gmail.com
 License: MIT license
 Project-URL: Demonstrações, https://github.com/MikalROn/ApiOmie-nao-oficial/tree/main/demos
 Keywords: Api omie,omie,api do omie,omieapi
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: api-omie Version: 0.3.12 Summary: Ferramenta para
+Metadata-Version: 2.1 Name: api-omie Version: 0.3.8 Summary: Ferramenta para
 api do omie nÃ£o oficial Home-page: https://github.com/MikalROn/ApiOmie-nao-
 oficial Author: Daniel CoÃªlho Author-email: heromon.9010@gmail.com License:
 MIT license Project-URL: DemonstraÃ§Ãµes, https://github.com/MikalROn/ApiOmie-
 nao-oficial/tree/main/demos Keywords: Api omie,omie,api do omie,omieapi
 Classifier: Development Status :: 3 - Alpha Requires-Python: >=3 Description-
 Content-Type: text/markdown License-File: LICENCE Requires-Dist: requests
 Requires-Dist: beautifulsoup4 Requires-Dist: pandas # Api Omie (NAO OFICIAL)
```

### Comparing `api-omie-0.3.12/README.md` & `api_omie-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `api-omie-0.3.12/api_omie.egg-info/PKG-INFO` & `api_omie-0.3.8/api_omie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-omie
-Version: 0.3.12
+Version: 0.3.8
 Summary: Ferramenta para api do omie não oficial
 Home-page: https://github.com/MikalROn/ApiOmie-nao-oficial
 Author: Daniel Coêlho
 Author-email: heromon.9010@gmail.com
 License: MIT license
 Project-URL: Demonstrações, https://github.com/MikalROn/ApiOmie-nao-oficial/tree/main/demos
 Keywords: Api omie,omie,api do omie,omieapi
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: api-omie Version: 0.3.12 Summary: Ferramenta para
+Metadata-Version: 2.1 Name: api-omie Version: 0.3.8 Summary: Ferramenta para
 api do omie nÃ£o oficial Home-page: https://github.com/MikalROn/ApiOmie-nao-
 oficial Author: Daniel CoÃªlho Author-email: heromon.9010@gmail.com License:
 MIT license Project-URL: DemonstraÃ§Ãµes, https://github.com/MikalROn/ApiOmie-
 nao-oficial/tree/main/demos Keywords: Api omie,omie,api do omie,omieapi
 Classifier: Development Status :: 3 - Alpha Requires-Python: >=3 Description-
 Content-Type: text/markdown License-File: LICENCE Requires-Dist: requests
 Requires-Dist: beautifulsoup4 Requires-Dist: pandas # Api Omie (NAO OFICIAL)
```

### Comparing `api-omie-0.3.12/omieapi/core/omiebase.py` & `api_omie-0.3.8/omieapi/core/omiebase.py`

 * *Files identical despite different names*

### Comparing `api-omie-0.3.12/omieapi/omie.py` & `api_omie-0.3.8/omieapi/omie.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,13 +5,13 @@
         """
         :param omie_app_key:              Chave api da omie
         :param omie_app_secret:           APi Secret da omie
         """
         
 
 CREDENCIAIS_PARA_HOMOLOGACAO_E_TESTE =  (
-        OMIE_APP_KEY  := "38333295000",
-        OMIE_APP_SECRET := "fed2163e2e8dccb53ff914ce9e2f1258"
+        OMIE_APP_KEY  := "1560731700",
+        OMIE_APP_SECRET := "226dcf372489bb45ceede61bfd98f0f1"
 )
 
 OmieHomologacao: Omie = Omie(*CREDENCIAIS_PARA_HOMOLOGACAO_E_TESTE) 
 OmieHomologacaoSession: Omie = Omie(*CREDENCIAIS_PARA_HOMOLOGACAO_E_TESTE, session=True)
```

### Comparing `api-omie-0.3.12/omieapi/scripts/cod_automatico.py` & `api_omie-0.3.8/omieapi/scripts/cod_automatico.py`

 * *Files identical despite different names*

### Comparing `api-omie-0.3.12/omieapi/scripts/scrap.py` & `api_omie-0.3.8/omieapi/scripts/scrap.py`

 * *Files 14% similar despite different names*

```diff
@@ -144,68 +144,114 @@
                     endpoint= '{valor['endpoint']}',
                     param = kargs
                 )
             '''
     with open('cod_automatico.py', 'w', encoding='utf-8') as w:
         w.write(codigo)
 
-
-def gerar_codigo(metodos) -> None:
-    gerar_codigo_automatico(metodos)
-
-def gerar_codigo_tipos_automatico_em_python(lista_tipos: list):
-    codigo = 'from dataclasses import dataclass \n\n' \
-             '# Aviso -> antes de usar confira se não a oq vc precisa já feito no codigo principal,\n' \
-             '# o codigo autogerdo pode conter erros não detectados ainda\n\n'
-    for tipo in lista_tipos:
-        codigo += f'''@dataclass\nclass {tipo["nome"]}:\n    """{tipo["descricao"]}"""\n'''
-    
-        for parametro in tipo['parametros']:
-            codigo += f'    {parametro["nome_parametro"]} #{parametro["tipo_parametro"]}\n'
-        
-    with open('tipos_complexos.py', 'w', encoding='utf-8') as w:
-        w.write(codigo)
-
-
 def pega_todos_tipos_complexos(urls: list[str]) -> list:
-    
+
     remove_numero = lambda x: ''.join([i for i in x if not i.isdigit()])
-    
+
     lista_tipos: list = []
-    
+
     for url in urls:
         for item in retorna_tipos_complexos(url):
             parametros = []
             try:
                 nome = item.h3.text
                 descricao = item.p.text
 
                 for parametro in item.table.find_all("tr"):
-                    
+
                     nome_parametro = parametro.find("td", {"class": "parameter-name"})
                     tipo = parametro.find("td", {"class": "parameter-type"})
                     descricao_parametro = parametro.find("td", {"class": "parameter-docs"})
                     parametros.append(
                         {
                             "nome_parametro": nome_parametro.text if nome_parametro else "",
                             "tipo_parametro": remove_numero(tipo.text) if tipo else "None",
                             "descricao_parametro": descricao_parametro.text if descricao_parametro else ""
                         }
                     )
-                    
+
                 lista_tipos.append(
                     {
                         "nome": nome,
                         "descricao": descricao,
                         "parametros": parametros
                     }
                 )
 
             except Exception as error:
                 print(error)
     print("Fim acabou")
     print(lista_tipos)
     return lista_tipos
 
+
+def gerar_codigo_automatico_java(dicionario: dict):
+
+    def lower_first_letter(string) -> str:
+        if len(string) > 0:
+            return string[0].lower() + string[1:]
+        else:
+            return string
+    def sanitiza_metodo_java(metodo: str) -> str:
+        lista_palavras = re.sub(r"([A-Z])", r" \1", metodo).split()
+        nome_final = ''.join(lista_palavras)
+        return lower_first_letter(nome_final)
+
+    def tratar_json(data: dict):
+        return json.dumps(data, indent=16).replace("}", '').replace("{", '')
+
+
+    codigo = 'package org; \n\n' \
+             'import org.json.JSONObject;\n' \
+             'import java.io.IOException;\n' \
+             'import java.net.URISyntaxException;\n\n' \
+             'public class OmieAuto extends OmieObject{\n' \
+             '    public OmieAuto(String appKey, String appSecreet) {\n' \
+             '    super(appKey, appSecreet);\n' \
+             '}\n'
+    for metodo, valor in dicionario.items():
+
+        lista_atributos = [x[0] for x in valor["exemplo_de_uso"].items()]
+        param = dict(zip(lista_atributos, lista_atributos))
+        codigo += \
+            f'''\n    public JSONObject {sanitiza_metodo_java(metodo)}(JSONArray parametros) throws URISyntaxException, IOException, InterruptedException{"{"} 
+                    //{valor['descricao']} 
+    
+                    return this.chamarApi(
+                        "{valor['endpoint']}",
+                        "{metodo}",
+                        parametros
+                    );
+            {"}"}
+                '''
+    codigo += "\n}"
+    with open('java/apiomie/src/main/java/org/OmieAuto.java', 'w', encoding='utf-8') as w:
+        w.write(codigo)
+
+def gerar_codigo(metodos) -> None:
+    gerar_codigo_automatico(metodos)
+
+def gerar_codigo_java(metodos) -> None:
+    gerar_codigo_automatico_java(metodos)
+
+def gerar_codigo_tipos_automatico_em_python(lista_tipos: list):
+    codigo = 'from dataclasses import dataclass \n\n' \
+             '# Aviso -> antes de usar confira se não a oq vc precisa já feito no codigo principal,\n' \
+             '# o codigo autogerdo pode conter erros não detectados ainda\n\n'
+    for tipo in lista_tipos:
+        codigo += f'''@dataclass\nclass {tipo["nome"]}:\n    """{tipo["descricao"]}"""\n'''
+
+        for parametro in tipo['parametros']:
+            codigo += f'    {parametro["nome_parametro"]} #{parametro["tipo_parametro"]}\n'
+
+    with open('tipos_complexos.py', 'w', encoding='utf-8') as w:
+        w.write(codigo)
+
 if __name__ == '__main__':
     #gerar_codigo(metodos())
-    gerar_codigo_tipos_automatico_em_python(tipos())
+    gerar_codigo_automatico_java(metodos())
+    #gerar_codigo_tipos_automatico_em_python(tipos())
```

### Comparing `api-omie-0.3.12/setup.py` & `api_omie-0.3.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION =  '0.3.12'
+VERSION =  '0.3.8'
 
 
 with open('README.md', 'rt', encoding='latin-1') as arq:
       readme = arq.read()
 
 keywords = ['Api omie', 'omie', 'api do omie', 'omieapi']
 
@@ -17,14 +17,14 @@
       long_description_content_type='text/markdown',
       author_email='heromon.9010@gmail.com',
       keywords=keywords,
       classifiers=[
             "Development Status :: 3 - Alpha"
       ],
       description='Ferramenta para api do omie não oficial',
-      packages=find_packages(exclude=('scrap.py')),
+      packages=find_packages(exclude=('scrap.py', 'java/*', 'php/*')),
       install_requires=['requests', 'beautifulsoup4', 'pandas'],
       python_requires='>=3',
       project_urls={
             'Demonstrações': 'https://github.com/MikalROn/ApiOmie-nao-oficial/tree/main/demos',
       }
 )
```

