# Comparing `tmp/llm_axe-1.0.0.tar.gz` & `tmp/llm_axe-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_axe-1.0.0.tar", last modified: Mon Apr 22 05:45:08 2024, max compression
+gzip compressed data, was "llm_axe-1.0.1.tar", last modified: Sun Apr 28 06:19:22 2024, max compression
```

## Comparing `llm_axe-1.0.0.tar` & `llm_axe-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 05:45:08.308189 llm_axe-1.0.0/
--rw-rw-rw-   0        0        0      729 2024-04-22 05:45:08.307190 llm_axe-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-22 05:45:08.283188 llm_axe-1.0.0/llm_axe/
--rw-rw-rw-   0        0        0       67 2024-04-22 04:52:11.000000 llm_axe-1.0.0/llm_axe/__init__.py
--rw-rw-rw-   0        0        0    12307 2024-04-22 04:25:13.000000 llm_axe-1.0.0/llm_axe/agents.py
--rw-rw-rw-   0        0        0     4256 2024-04-22 04:58:19.000000 llm_axe-1.0.0/llm_axe/core.py
--rw-rw-rw-   0        0        0      576 2024-04-20 19:13:17.000000 llm_axe-1.0.0/llm_axe/models.py
--rw-rw-rw-   0        0        0     4581 2024-04-22 03:56:37.000000 llm_axe-1.0.0/llm_axe/system_prompts.yaml
-drwxrwxrwx   0        0        0        0 2024-04-22 05:45:08.306187 llm_axe-1.0.0/llm_axe.egg-info/
--rw-rw-rw-   0        0        0      729 2024-04-22 05:45:08.000000 llm_axe-1.0.0/llm_axe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-04-22 05:45:08.000000 llm_axe-1.0.0/llm_axe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 05:45:08.000000 llm_axe-1.0.0/llm_axe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 05:45:08.000000 llm_axe-1.0.0/llm_axe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 05:45:08.308189 llm_axe-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1206 2024-04-22 05:45:02.000000 llm_axe-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 06:19:22.268359 llm_axe-1.0.1/
+-rw-rw-rw-   0        0        0      722 2024-04-28 06:19:22.267360 llm_axe-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-28 06:19:22.255847 llm_axe-1.0.1/llm_axe/
+-rw-rw-rw-   0        0        0       67 2024-04-22 04:52:11.000000 llm_axe-1.0.1/llm_axe/__init__.py
+-rw-rw-rw-   0        0        0    16990 2024-04-28 06:02:15.000000 llm_axe-1.0.1/llm_axe/agents.py
+-rw-rw-rw-   0        0        0     5933 2024-04-28 05:38:57.000000 llm_axe-1.0.1/llm_axe/core.py
+-rw-rw-rw-   0        0        0      551 2024-04-27 04:29:01.000000 llm_axe-1.0.1/llm_axe/models.py
+-rw-rw-rw-   0        0        0     5735 2024-04-28 05:52:53.000000 llm_axe-1.0.1/llm_axe/system_prompts.yaml
+drwxrwxrwx   0        0        0        0 2024-04-28 06:19:22.266359 llm_axe-1.0.1/llm_axe.egg-info/
+-rw-rw-rw-   0        0        0      722 2024-04-28 06:19:22.000000 llm_axe-1.0.1/llm_axe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-04-28 06:19:22.000000 llm_axe-1.0.1/llm_axe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 06:19:22.000000 llm_axe-1.0.1/llm_axe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2024-04-28 06:19:22.000000 llm_axe-1.0.1/llm_axe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-28 06:19:22.000000 llm_axe-1.0.1/llm_axe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 06:19:22.268359 llm_axe-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1403 2024-04-28 06:17:24.000000 llm_axe-1.0.1/setup.py
```

### Comparing `llm_axe-1.0.0/PKG-INFO` & `llm_axe-1.0.1/llm_axe.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: llm_axe
-Version: 1.0.0
-Summary: A toolkit for quickly implementing complex interactions for local LLMs
+Name: llm-axe
+Version: 1.0.1
+Summary: A toolkit for quickly implementing llm powered functionalities.
 Author: Emir Sahin
 Author-email: emirsah122@gmail.com
 License: MIT
 Keywords: python,llm axe,llm toolkit,local llm,local llm internet,function caller llm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `llm_axe-1.0.0/llm_axe/agents.py` & `llm_axe-1.0.1/llm_axe/agents.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,119 @@
 import warnings
 import os
-from llm_axe.core import AgentType, safe_read_json, generate_schema, get_yaml_prompt, internet_search, read_website, read_pdf
+import json
 
+from llm_axe.core import AgentType, safe_read_json, generate_schema, get_yaml_prompt, internet_search, read_website, read_pdf, make_prompt, llm_has_ask
+
+
+class Agent:
+    """
+    Basic agent that can use premade or custom system prompts.
+    """
+    def __init__(self, llm:object, agent_type:AgentType=None, additional_system_instructions:str="", custom_system_prompt:str=None):
+        """
+        Args:
+            llm (object): An LLM object with an ask function.
+            agent_type (AgentType, optional): The type of agent to use. Choose from AgentType enum. Defaults to None.
+            system_prompt (Agent): The name of the system prompt to use from the system_prompts.yaml file. See documentation for list.
+            custom_system_prompt (any, optional): An optional string to override and use as the custom system prompt.
+        """
+        self.llm = llm
+        self.chat_history = []
+        if custom_system_prompt is None:
+            if agent_type is None:
+                raise ValueError("You must provide either a system_prompt or a custom_system_prompt.")
+            else:
+                self.system_prompt = get_yaml_prompt("system_prompts.yaml", agent_type.value)
+        else:
+            self.system_prompt = custom_system_prompt
+        
+        self.system_prompt = make_prompt("system", self.system_prompt.format(additional_instructions=additional_system_instructions))
+
+    def get_prompt(self, question):
+        """
+        Get the prompt for the given question.
+        Args:
+            question (str): The question to get the prompt for.
+        """
+        user_prompt = make_prompt("user", question)
+        prompts = [self.system_prompt, user_prompt]
+        return prompts
+
+    def ask(self, prompt, history:list=None):
+        """
+        Ask a question based on the given prompt.
+        Args:
+            prompt (str): The prompt to use for the question. Will only use system_prompt if prompt is None.
+            history (list, optional): The history of the conversation. Defaults to None.
+        """
+        if llm_has_ask(self.llm) is False:
+            return None
+        
+        prompts = [self.system_prompt]
+        if history is not None:
+            prompts.extend(history)
+
+        if prompt is not None:
+            prompts.append(make_prompt("user", prompt))
+            self.chat_history.extend(prompts[1:])
+    
+        response = self.llm.ask(prompts)
+        self.chat_history.append(make_prompt("assistant", response))
+        return response
+
+
+class DataExtractor():
+    """
+    A DataExtractor agent is used to extract information from given content.
+    """
+    def __init__(self, llm:object=None, reply_as_json:bool=False, additional_system_instructions:str=""):
+        """
+        Initializes a new DataExtractor.
+        Args:
+            llm (object): An object that implements the ask() method.
+            reply_as_json (bool, optional): If True, the response will be in the format of a JSON object. Defaults to False.
+            additional_system_instructions (str, optional): Additional instructions to include in the system prompt. Defaults to "".
+        """
+        yaml_prompt = "DataExtractorJson" if reply_as_json else "DataExtractor"
+        self.system_prompt = get_yaml_prompt("system_prompts.yaml", yaml_prompt)
+        self.system_prompt = make_prompt("system", self.system_prompt.format(additional_instructions=additional_system_instructions))
+        self.llm = llm
+        self.chat_history = []
+
+    def get_prompt(self, info:str, data_points:list=[]):
+        """
+        Get the prompt for the given content.
+        Args:
+            info (str): The content to extract information from.
+            data_points (list, optional): A list of data points to extract. Defaults to None.
+        """
+        prompt = '''
+                Extract information from the following content:
+                {content}
+
+                Extract the following data:
+                {data}
+        '''
+        prompt = prompt.format(content=info, data=", ".join(data_points))
+        return [self.system_prompt, make_prompt("user", prompt)]
+    
+    def ask(self, info:str, data_points:list=[]):
+        """
+        Ask a question based on the given content.
+        Args:
+            info (str): The content to extract information from.
+            data_points (list, optional): A list of data points to extract. Defaults to None.
+        """
+        prompts = self.get_prompt(info, data_points)
+        resp = self.llm.ask(self.get_prompt(info, data_points))
+        self.chat_history.extend(prompts[1:])
+        self.chat_history.append(make_prompt("assistant", resp))
+        return resp
+    
 
 class PdfReader():
     """
     A PdfReader agent is used to answer questions based on information from given PDF files.
     """
 
     def __init__(self, llm:object=None, pdf_files:list=None, additional_system_instructions:str="", custom_system_prompt:str=None):
@@ -13,30 +121,44 @@
         Initializes a new PdfReader.
         Args:
             llm (object): An object that implements the ask() method.
             pdf_files (list): A list of PDF files to read. Each file should be a string representing the path to the PDF file.
             additional_system_instructions (str, optional): Additional instructions to include in the system prompt.
             custom_system_prompt (str, optional): Custom system prompt. Defaults to None.
         """
+        self.chat_history = []
         self.llm = llm
         self.pdf_files = pdf_files
         self.additional_instructions = additional_system_instructions
         self.system_prompt = get_yaml_prompt("system_prompts.yaml", "DocumentReader")
         self.custom_system_prompt = custom_system_prompt
 
 
-    def ask(self, question:str, pdf_files:list=None):
+    def ask(self, question:str, pdf_files:list=None, history:list=None):
         """
         Ask a question based on the given PDF files.
+        Args:
+            question (str): The question to ask.
+            pdf_files (list): A list of PDF files to read. Each file should be a string representing the path to the PDF file.
+            history (list): A list of previous chat messages in openai format.
         """
         if self.llm is None:
             raise ValueError("No LLM object provided.")
-        
-        prompts = self.get_prompt(question, pdf_files)
-        return self.llm.ask(prompts)
+            
+        prompts = []
+        if history is not None:
+            prompts.extend(history)
+
+        question_prompts = self.get_prompt(question, pdf_files)
+        prompts.extend(question_prompts)
+        response = self.llm.ask(prompts)
+
+        self.chat_history.append(question_prompts[1:]) # dont include the system prompt
+        self.chat_history.append(make_prompt("assistant", response))
+        return response
     
     def get_prompt(self, question, pdf_files:list=None):
         """
         Generates the prompt for the LLM.
         args:
             question (str): The question to ask.
             pdf_files (list): A list of PDF files to read. Each file should be a string representing the path to the PDF file. 
@@ -47,18 +169,17 @@
             pdf_text += read_pdf(pdf_file) + "\n\n"
         
         if self.custom_system_prompt is None:
             self.system_prompt = get_yaml_prompt("system_prompts.yaml", "DocumentReader")
         else:
             self.system_prompt = self.custom_system_prompt
 
-        self.system_prompt = {"role":"system", 
-                          "content": self.system_prompt.format(documents=pdf_text, additional_instructions=self.additional_instructions)}
+        self.system_prompt = make_prompt("system", self.system_prompt.format(documents=pdf_text, additional_instructions=self.additional_instructions))
         
-        user_prompt = {"role":"user", "content": question}
+        user_prompt = make_prompt("user", question)
         prompts = [self.system_prompt, user_prompt]
 
         return prompts
     
 
 class FunctionCaller():
     """
@@ -74,33 +195,34 @@
 
         Args:
             llm (object, optional): An LLM object. Must have an ask method. Defaults to None.
             functions (list, optional): A list of functions. Defaults to None.
             additional_system_instructions (str, optional): Instructions in addition to the system prompt. Defaults to "".
             custom_system_prompt (str, optional): A custom system prompt. Will override the default. Defaults to None.
         """
-       
+        self.chat_history = []
         self.llm = llm
         self.functions_dict = {func.__name__: func for func in functions}
         self.additional_instructions = additional_system_instructions
         self.schema = generate_schema(functions)
 
         if custom_system_prompt is None:
             self.system_prompt = get_yaml_prompt("system_prompts.yaml", "FunctionCaller")
         else:
             self.system_prompt = custom_system_prompt
-        self.system_prompt = {"role":"system", 
-                              "content": self.system_prompt.format(schema=self.schema, additional_instructions=additional_system_instructions)}
 
-    def get_function(self, question):
+        self.system_prompt = make_prompt("system", self.system_prompt.format(schema=self.schema, additional_instructions=additional_system_instructions))
+       
+    def get_function(self, question, history:list=None):
         """
         Get the most appropriate function and its parameters based on the provided question.
 
         Parameters:
             question (str): The question to prompt the function caller with.
+            history (list): A list of previous chat messages in openai format.
 
         Returns:
             tuple: A tuple containing the function, its parameters and the prompts used.
                 - function (Callable): The function to be called.
                 - parameters (dict): The parameters for the function.
                 - prompts (list): The prompts that were used to speak to the llm.
 
@@ -109,24 +231,30 @@
         """
 
         if self.llm is None:
             raise ValueError('''You must provide an llm to prompt the function caller!
                                 If you wish to use external llms, use the get_prompt function to get the usable prompt.''')
         
         # check if llm has an ask function
-        if not hasattr(self.llm, "ask"):
-            warnings.warn("llm object must have an ask function! See OllamaChat class in models.py for an example.")
+        if llm_has_ask(self.llm) is False:
             return None
         
-        user_prompt = {"role":"user", "content": question}
-        prompts = [self.system_prompt, user_prompt]
+        prompts = []
+        if history is not None:
+            prompts.extend(history)
+
+        question_prompts = self.get_prompt(question)
+        prompts.extend(question_prompts)
 
         response = self.llm.ask(prompts)
         response_json = safe_read_json(response)
 
+        self.chat_history.extend(question_prompts[1:])
+        self.chat_history.append(make_prompt("assistant", response))
+
         if response_json is None:
             return None
 
         try:
             function_name = response_json["function"]
             parameters = response_json["parameters"]
         except KeyError:
@@ -157,39 +285,41 @@
                 - system_prompt (dict): The system prompt.
                     - role (str): The role of the prompt (system).
                     - content (str): The content of the system prompt.
                 - user_prompt (dict): The user prompt.
                     - role (str): The role of the prompt (user).
                     - content (str): The content of the user prompt.
         """
-        user_prompt = {"role":"user", "content": question}
+        user_prompt = make_prompt("user", question)
         prompts = [self.system_prompt, user_prompt]
         return prompts
 
 
 class OnlineAgent:
     """
     An agent that has internet access. 
     It will use the internet to try and best answer the user prompt
     """
 
-    def __init__(self, llm:object, additional_system_instructions:str="", custom_searcher:callable=None):
+    def __init__(self, llm:object, additional_system_instructions:str="", custom_searcher:callable=None, custom_site_reader:callable=None):
         """
         Args:
             llm (object): An LLM object. Must have an ask method.
             additional_system_instructions (str, optional): Instructions in addition to the system prompt. Defaults to "".
             custom_searcher (function, optional): A custom online searcher function. The searcher function must take a query and return a list of string URLS
+            custom_site_reader (function, optional): A custom online site reader function. The site reader function must take a URL and return a string representation of the site.
         """
         self.llm = llm
+        self.chat_history = []
         self.system_prompt = get_yaml_prompt("system_prompts.yaml", "OnlineSearcher")
-        self.system_prompt = {"role":"system", 
-                              "content": self.system_prompt.format(additional_instructions=additional_system_instructions)}
+        self.system_prompt = make_prompt("system", self.system_prompt.format(additional_instructions=additional_system_instructions))
         self.search_function = custom_searcher if custom_searcher else internet_search
+        self.site_reader_function = custom_site_reader if custom_site_reader else read_website
 
-    def search(self, prompt):
+    def search(self, prompt, history:list=None):
         """
         Searches the internet and answers the prompt based on the search results.
 
         Parameters:
             prompt (str): The prompt or question to answer.
 
         Returns:
@@ -201,85 +331,63 @@
         # The llm will pick the best URL and read it to answer the prompt
     
         query = self.get_search_query(prompt)
         if query is None:
             return None
 
         search_results = self.search_function(query)
-        search_results = " ".join(search_results) #list to a string
+        search_results =  json.dumps(search_results)
+
+        url_picker_prompts = []
+        if history is not None:
+            url_picker_prompts.extend(history)
+
         url_picker_prompt = get_yaml_prompt("system_prompts.yaml", "UrlPicker")
-        url_picker_prompt = {"role":"system", "content": url_picker_prompt.format(question=prompt, urls=search_results)}
-        resp = self.llm.ask([url_picker_prompt])
+        url_picker_prompt = make_prompt("system", url_picker_prompt.format(question=prompt, urls=search_results))
+        url_picker_prompts.append(url_picker_prompt)
+
+        resp = self.llm.ask(url_picker_prompts)
         resp_json = safe_read_json(resp)
-        
+        self.chat_history.extend(url_picker_prompts[1:])
+        self.chat_history.append(make_prompt("assistant", resp))
+
         # Check if the response is a valid url
         url = None
         if resp_json is not None and "url" in resp_json:
             url = resp_json["url"]
         else:
             warnings.warn("LLM did not respond with valid url or json response.")
             return None
             
-        website_text = read_website(url)
+        website_text = self.site_reader_function(url)
         user_prompt = f'''
                     Please read the following information:
                     
                     Information about Website {url}: 
                     {website_text}
 
                     Answer the following question based on the above information: 
                     {prompt}
 
                     Start your answer with "Based on information from the internet, "
                     '''
         
         final_responder = Agent(llm=self.llm, agent_type=AgentType.GENERIC_RESPONDER)
-        return final_responder.ask(user_prompt)
+        response = final_responder.ask(user_prompt, history)
+
+        self.chat_history.append(make_prompt("user", user_prompt))
+        self.chat_history.append(make_prompt("assistant", response))
+        
+        return response
 
     def get_search_query(self, question):
-        user_prompt = {"role":"user", "content": question}
+        user_prompt = make_prompt("user", question)
         prompts = [self.system_prompt, user_prompt]
         response = self.llm.ask(prompts)
         response_json = safe_read_json(response)
-        
+        self.chat_history.extend(prompts[1:])
+        self.chat_history.append(make_prompt("assistant", response))
         if response_json is not None and "search_query" in response_json:
             return response_json["search_query"]
         else:
             return None
-            
-
-class Agent:
-    """
-    Basic agent that can use premade or custom system prompts.
-    """
-    def __init__(self, llm:object, agent_type:AgentType=None, additional_system_instructions:str="", custom_system_prompt:str=None):
-        """
-        Args:
-            llm (object): An LLM object with an ask function.
-            system_prompt (Agent): The name of the system prompt to use from the system_prompts.yaml file. See documentation for list.
-            custom_system_prompt (any, optional): An optional string to override and use as the custom system prompt.
-        """
-        self.llm = llm
-        if custom_system_prompt is None:
-            if agent_type is None:
-                raise ValueError("You must provide either a system_prompt or a custom_system_prompt.")
-            else:
-                self.system_prompt = get_yaml_prompt("system_prompts.yaml", agent_type.value)
-        else:
-            self.system_prompt = custom_system_prompt
-        
-        self.system_prompt = {"role":"system", 
-                              "content": self.system_prompt.format(additional_instructions=additional_system_instructions)}
-
-    def get_prompt(self, question):
-        user_prompt = {"role":"user", "content": question}
-        prompts = [self.system_prompt, user_prompt]
-        return prompts
-
-    def ask(self, prompt):
-        if not hasattr(self.llm, "ask"):
-            warnings.warn("llm object must have an ask function! See OllamaChat class in models.py for an example.")
-            return None
-        prompts = [self.system_prompt, {"role":"user", "content": prompt}]
-        return self.llm.ask(prompts)
-
-
+
```

### Comparing `llm_axe-1.0.0/llm_axe/core.py` & `llm_axe-1.0.1/llm_axe/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,14 +16,25 @@
     See documentation for explanation of Agents
     """
     PLANNER = "Planner"
     SUMMARIZER = "Summarizer"
     GENERIC_RESPONDER = "GenericResponder"
 
 
+def llm_has_ask(llm):
+    if not hasattr(llm, "ask"):
+            warnings.warn("llm object must have an ask function! See OllamaChat class in models.py for an example.")
+            return False
+    return True
+
+
+def make_prompt(role:str, content:str):
+    return {"role": role, "content": content}
+
+
 def read_pdf(file):
     """
     Reads a pdf file and returns the complete text content.
     Args:
         file (str): The path to the pdf file.
     """
     reader = PdfReader(file)
@@ -119,24 +130,58 @@
 def internet_search(query):
     """
     Searches the internet for a query.
     Returns top 10 results.
     Args:
         query (str): The query to search for.
     """
-    return list(search(query, tld="co.in", num=10, stop=10, pause=2))
+    urls = list(search(query, tld="co.in", num=5, stop=10, pause=2))
+    urls_detailed = []
+
+    for url in urls:
+        urls_detailed.append(fetch_url_info(url))
+
+    return urls_detailed
 
 def read_website(url):
     """
     Reads the body of the website at the given url.
     Args:
         url (str): The url of the website to read.
     """
-    response = requests.get(url)
+    headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3'}
+    response = requests.get(url, headers=headers)
     if response.status_code == 200:
         soup = BeautifulSoup(response.text, 'html.parser')
         body = soup.body        
         body_text = body.get_text(strip=True)
         return body_text        
     else:
         warnings.warn("Failed to retrieve the website")
-        return None
+        return None
+    
+
+def fetch_url_info(url):
+    """
+    Fetches the description and title of the website at the given url.
+    Args:
+        url (str): The url of the website to read.
+    
+    Returns:
+        dict: A dictionary containing the url, title and description of the website.
+    """
+    headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3'}
+    try:
+        response = requests.get(url, headers=headers)
+        if response.status_code == 200:
+            soup = BeautifulSoup(response.text, 'html.parser')
+            title = soup.find('title').text if soup.find('title') else 'No title found'
+            meta_desc = soup.find('meta', attrs={'name': 'description'})
+            description = meta_desc['content'] if meta_desc else 'No description found'
+            return {"url": url, 'title': title, 'description': description}
+        else:
+            return None
+    except Exception as e:
+        return None
+
+
+# TODO:: Add custom html reader option
```

### Comparing `llm_axe-1.0.0/llm_axe/models.py` & `llm_axe-1.0.1/llm_axe/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,13 +5,13 @@
 
         if model is None:
             raise ValueError('''You must provide a model to use OllamaChat. 
                                 example: OllamaChat(model='llama3:instruct')''')
 
         self._host = host
         self._model = model
-        self._ollama = Client(host='http://localhost:11434')
+        self._ollama = Client(host)
 
 
     def ask(self, prompts:list):
         return self._ollama.chat(model=self._model, messages=prompts)["message"]["content"]
```

### Comparing `llm_axe-1.0.0/llm_axe/system_prompts.yaml` & `llm_axe-1.0.1/llm_axe/system_prompts.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -96,28 +96,60 @@
         }}
 
         URLS:
         {urls}
     
 GenericResponder:
     prompt: |
-        You are a helpful assistant.
-        You must answer the user's question using the context given. You must not provide any additional information.
+        You are a helpful chat assistant.
+        You must respond to the user's prompt using your chat history or context. You must not provide any additional information.
         You cannot lie.
 
 
 DocumentReader:
     prompt: |
         You are a helpful assistant.
         You must answer the user's question using ONLY the information from the documents. 
         You must not provide any additional information.
-        You CANNOT lie. You CANNOT make up things. You CANNOT user external references or sources.
+        You CANNOT lie. You CANNOT make up things. You CANNOT use external references or sources.
 
         You must reference which document that your answer came from. If you cannot provide a reference, then your answer is INCORRECT.
 
         {additional_instructions}
 
         Documents:
 
         {documents}
 
+DataExtractor:
+    prompt: |
+        You are a helpful assistant.
+        Your only job is to extract data from the user provided information.
+        You must not provide any additional information or say anything else.
+
+        You must respond in this format:
+            Data1: value1
+            Data2: value2
+            Data3: value3
+
+        You must not make up any data. You must only extract the specified data.
+        Only extract the SPECIFIC data that was requested.
+
+        {additional_instructions}
 
+DataExtractorJson:
+    prompt: |
+        You are a helpful assistant.
+        Your only job is to extract data from the user provided information.
+        You must not provide any additional information or say anything else.
+
+        You must respond in this exact JSON format:
+            {{
+                "Data1": "value1",
+                "Data2": "value2",
+                "Data3": "value3"
+            }}
+
+        You must not make up any data. You must only extract the specified data.
+        Only extract the SPECIFIC data that was requested.
+
+        {additional_instructions}
```

### Comparing `llm_axe-1.0.0/llm_axe.egg-info/PKG-INFO` & `llm_axe-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: llm-axe
-Version: 1.0.0
-Summary: A toolkit for quickly implementing complex interactions for local LLMs
+Name: llm_axe
+Version: 1.0.1
+Summary: A toolkit for quickly implementing llm powered functionalities.
 Author: Emir Sahin
 Author-email: emirsah122@gmail.com
 License: MIT
 Keywords: python,llm axe,llm toolkit,local llm,local llm internet,function caller llm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `llm_axe-1.0.0/setup.py` & `llm_axe-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0' 
-DESCRIPTION = 'A toolkit for quickly implementing complex interactions for local LLMs'
+VERSION = '1.0.1' 
+DESCRIPTION = 'A toolkit for quickly implementing llm powered functionalities.'
 LONG_DESCRIPTION = 'llm_axe allows you to quickly implement complex interactions for local LLMs, such as function callers, online agents, pre-made generic agents, and more.'
 
 # Setting up
 setup(
         name="llm_axe", 
         version=VERSION,
         author="Emir Sahin",
         author_email="emirsah122@gmail.com",
         license="MIT",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=[], # add any additional packages that 
+        install_requires=[
+            'beautifulsoup4>=4.12.3',
+            'docstring_parser>=0.16',
+            'google>=3.0.0',
+            'ollama>=0.1.9',
+            'pypdf>=4.2.0',
+            'PyYAML>=6.0.1',
+            'requests>=2.31.0'
+        ], 
          package_data={
         '': ['*.yaml'],
         },
         
         keywords=['python', 'llm axe', 'llm toolkit', 'local llm', 'local llm internet', 'function caller llm'],
         classifiers= [
             "Development Status :: 3 - Alpha",
```

