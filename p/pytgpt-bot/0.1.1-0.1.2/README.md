# Comparing `tmp/pytgpt_bot-0.1.1.tar.gz` & `tmp/pytgpt_bot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytgpt_bot-0.1.1.tar", last modified: Fri Apr 26 22:02:38 2024, max compression
+gzip compressed data, was "pytgpt_bot-0.1.2.tar", last modified: Sun Apr 28 00:53:26 2024, max compression
```

## Comparing `pytgpt_bot-0.1.1.tar` & `pytgpt_bot-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:02:38.716123 pytgpt_bot-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-26 22:02:20.000000 pytgpt_bot-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 22:02:38.716123 pytgpt_bot-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-04-26 22:02:20.000000 pytgpt_bot-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:02:38.712123 pytgpt_bot-0.1.1/pytgpt_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-26 22:02:20.000000 pytgpt_bot-0.1.1/pytgpt_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 22:02:20.000000 pytgpt_bot-0.1.1/pytgpt_bot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-26 22:02:20.000000 pytgpt_bot-0.1.1/pytgpt_bot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-26 22:02:20.000000 pytgpt_bot-0.1.1/pytgpt_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-26 22:02:20.000000 pytgpt_bot-0.1.1/pytgpt_bot/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    20108 2024-04-26 22:02:20.000000 pytgpt_bot-0.1.1/pytgpt_bot/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-26 22:02:20.000000 pytgpt_bot-0.1.1/pytgpt_bot/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-26 22:02:20.000000 pytgpt_bot-0.1.1/pytgpt_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:02:38.716123 pytgpt_bot-0.1.1/pytgpt_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-26 22:02:38.000000 pytgpt_bot-0.1.1/pytgpt_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-26 22:02:38.000000 pytgpt_bot-0.1.1/pytgpt_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 22:02:38.000000 pytgpt_bot-0.1.1/pytgpt_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 22:02:38.000000 pytgpt_bot-0.1.1/pytgpt_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-26 22:02:38.000000 pytgpt_bot-0.1.1/pytgpt_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 22:02:38.000000 pytgpt_bot-0.1.1/pytgpt_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 22:02:38.716123 pytgpt_bot-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-26 22:02:20.000000 pytgpt_bot-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:53:26.067393 pytgpt_bot-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-28 00:53:26.067393 pytgpt_bot-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:53:26.067393 pytgpt_bot-0.1.2/pytgpt_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21893 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:53:26.067393 pytgpt_bot-0.1.2/pytgpt_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-28 00:53:26.000000 pytgpt_bot-0.1.2/pytgpt_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-28 00:53:26.000000 pytgpt_bot-0.1.2/pytgpt_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 00:53:26.000000 pytgpt_bot-0.1.2/pytgpt_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 00:53:26.000000 pytgpt_bot-0.1.2/pytgpt_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-28 00:53:26.000000 pytgpt_bot-0.1.2/pytgpt_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 00:53:26.000000 pytgpt_bot-0.1.2/pytgpt_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 00:53:26.067393 pytgpt_bot-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/setup.py
```

### Comparing `pytgpt_bot-0.1.1/LICENSE` & `pytgpt_bot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.1/PKG-INFO` & `pytgpt_bot-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.1.1
-Summary: Telegram bot for chatting, text-to-image and text-to-voice conversions
+Version: 0.1.2
+Summary: Telegram bot for chatting, text-to-image and text-to-speech conversions
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/pytgpt-bot
@@ -86,30 +86,23 @@
 
 Alternatively, using CLI:
 
    `$ pytgpt-bot run <Your Telegram Token>`
 
 ## Features
 
-### Commands
-
-
-### Usage Information
-
-This section provides detailed instructions on how to use the various commands available in the bot.
-
 - **/start**: Displays the help information, offering a comprehensive list of available commands and their functionalities. This command is essential for users to quickly understand how to interact with the bot.
 
 - **/chat**: Initiate a natural language conversation with the AI. This command allows users to engage in interactive dialogues, ask questions, or make requests.
 
 - **/image**: Generates images from textual descriptions using the default provider. This feature enables users to visualize ideas or concepts through images.
 
 - **/prodia**: Generates images from textual descriptions using the Prodia provider. This command offers a unique style or interpretation of the text descriptions compared to the default method.
 
-- **/audio**: Converts text to speech, providing users with the ability to listen to descriptions, instructions, or any text content read out by the AI.
+- **/speak**: Converts text to speech, providing users with the ability to listen to descriptions, instructions, or any text content read out by the AI.
 
 - **/intro**: Sets a new text for the chat intro. This command allows users to customize the chat introductory prompt which serves as a guide in the human-AI engagement.
 
 - **/voice**: Sets a new voice for speech synthesis. This command enables users to choose from different voices for the AI to use when generating audio from text.
 
 - **/provider**: Sets a new chat provider. This command allows users to switch between different providers for various functionalities, such as `phind`, `llama2`, `koboldai` etc.
 
@@ -119,18 +112,19 @@
 
 - **/check**: Offers an overview of the bot's current configuration, including any custom settings applied by the user.
 
 - **/reset**: Resets the chat history and starts a new conversation thread. This command is useful for users who wish to start fresh or clear their chat history for privacy reasons.
 
 - **/myid**: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for various purposes, such as setting up bot admin.
 
-- `any other text`: An alias for `/chat`, allowing users to continue with chatting.
+- **/suspend**: Pauses the bot's service temporarily. This command is useful for channel administrators who need to temporarily halt the bot's operations without deleting its data or settings. It's a way to manage the bot's availability based on operational needs.
 
+- **/resume**: Resumes the bot's service after it has been suspended. This command allows administrators to quickly bring the bot back online after a pause, ensuring that users can continue interacting with the bot without interruption.
 
-### Administrative Commands
+- `any other text`: An alias for `/chat`, allowing users to continue with chatting.
 
 
 ### Administrative Commands
 
 - `/clear`: Clears all chats. This command is used to remove all chat data from the bot's database. It's a powerful command that should be used with caution, as it will delete all chat history.
 
 - `/total`: Shows the total number of chats available. This command provides an overview of the current chat data stored in the bot's database, helping administrators understand the volume of interactions the bot has had.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.1 Summary: Telegram bot for
-chatting, text-to-image and text-to-voice conversions Home-page: https://
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.2 Summary: Telegram bot for
+chatting, text-to-image and text-to-speech conversions Home-page: https://
 github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
 pytgpt-bot/releases Project-URL: Documentation, https://github.com/Simatwa/
@@ -36,27 +36,25 @@
 [Python>=3.10](https://python.org) ## Installation 1. From Source Clone repo
 and install. ```bash git clone https://github.com/Simatwa/pytgpt-bot.git cd
 pytgpt-bot pip install . ``` 2. From Pypi *(recommended)* ```sh pip install
 pytgpt-bot ``` ## Usage Before getting started, ensure you've your Telegram bot
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
 file as per the needs and then rename it `.env` before firing up the bot
-`python3 run.py`. Alternatively, using CLI: `$ pytgpt-bot run ` ## Features ###
-Commands ### Usage Information This section provides detailed instructions on
-how to use the various commands available in the bot. - **/start**: Displays
-the help information, offering a comprehensive list of available commands and
-their functionalities. This command is essential for users to quickly
-understand how to interact with the bot. - **/chat**: Initiate a natural
-language conversation with the AI. This command allows users to engage in
-interactive dialogues, ask questions, or make requests. - **/image**: Generates
-images from textual descriptions using the default provider. This feature
-enables users to visualize ideas or concepts through images. - **/prodia**:
-Generates images from textual descriptions using the Prodia provider. This
-command offers a unique style or interpretation of the text descriptions
-compared to the default method. - **/audio**: Converts text to speech,
+`python3 run.py`. Alternatively, using CLI: `$ pytgpt-bot run ` ## Features -
+**/start**: Displays the help information, offering a comprehensive list of
+available commands and their functionalities. This command is essential for
+users to quickly understand how to interact with the bot. - **/chat**: Initiate
+a natural language conversation with the AI. This command allows users to
+engage in interactive dialogues, ask questions, or make requests. - **/image**:
+Generates images from textual descriptions using the default provider. This
+feature enables users to visualize ideas or concepts through images. - **/
+prodia**: Generates images from textual descriptions using the Prodia provider.
+This command offers a unique style or interpretation of the text descriptions
+compared to the default method. - **/speak**: Converts text to speech,
 providing users with the ability to listen to descriptions, instructions, or
 any text content read out by the AI. - **/intro**: Sets a new text for the chat
 intro. This command allows users to customize the chat introductory prompt
 which serves as a guide in the human-AI engagement. - **/voice**: Sets a new
 voice for speech synthesis. This command enables users to choose from different
 voices for the AI to use when generating audio from text. - **/provider**: Sets
 a new chat provider. This command allows users to switch between different
@@ -67,31 +65,37 @@
 interactions or finding specific information from previous conversations. - **/
 check**: Offers an overview of the bot's current configuration, including any
 custom settings applied by the user. - **/reset**: Resets the chat history and
 starts a new conversation thread. This command is useful for users who wish to
 start fresh or clear their chat history for privacy reasons. - **/myid**:
 Echoes the user's Telegram ID. This command is useful for users who need to
 know their Telegram ID for various purposes, such as setting up bot admin. -
-`any other text`: An alias for `/chat`, allowing users to continue with
-chatting. ### Administrative Commands ### Administrative Commands - `/clear`:
-Clears all chats. This command is used to remove all chat data from the bot's
-database. It's a powerful command that should be used with caution, as it will
-delete all chat history. - `/total`: Shows the total number of chats available.
-This command provides an overview of the current chat data stored in the bot's
-database, helping administrators understand the volume of interactions the bot
-has had. - `/drop`: Clears the entire chat table and bot logs. Similar to `/
-clear`, this command removes all data from the chat table in the database. It's
-a more drastic measure than `/clear`, as it completely wipes out all chat data
-and current contents of log file. - `/sql`: Allows running SQL statements
-against the database. This command provides a way for administrators to
-directly interact with the bot's database using SQL queries. It's a powerful
-tool for managing and analyzing the bot's data but should be used with caution
-to avoid unintended data loss or corruption. - `/logs`: Checks the logs. This
-command is used to access the bot's logs, which can provide insights into the
-bot's activity, errors, and user interactions. It's a valuable tool for
-monitoring and troubleshooting the bot's performance. ## Support and Feedback
-If you have any questions, feedback, or suggestions for `pytgpt`, please feel
-free to reach out. Your input is valuable in helping us improve and expand the
-bot's capabilities. ## License `pytgpt-bot` is open-source and available under
-the [MIT License](LICENSE). Feel free to use, modify, and distribute the code
-as you see fit. --- Thank you for using `pytgpt-bot`. Enjoy your AI-powered
-interactions!
+**/suspend**: Pauses the bot's service temporarily. This command is useful for
+channel administrators who need to temporarily halt the bot's operations
+without deleting its data or settings. It's a way to manage the bot's
+availability based on operational needs. - **/resume**: Resumes the bot's
+service after it has been suspended. This command allows administrators to
+quickly bring the bot back online after a pause, ensuring that users can
+continue interacting with the bot without interruption. - `any other text`: An
+alias for `/chat`, allowing users to continue with chatting. ### Administrative
+Commands - `/clear`: Clears all chats. This command is used to remove all chat
+data from the bot's database. It's a powerful command that should be used with
+caution, as it will delete all chat history. - `/total`: Shows the total number
+of chats available. This command provides an overview of the current chat data
+stored in the bot's database, helping administrators understand the volume of
+interactions the bot has had. - `/drop`: Clears the entire chat table and bot
+logs. Similar to `/clear`, this command removes all data from the chat table in
+the database. It's a more drastic measure than `/clear`, as it completely wipes
+out all chat data and current contents of log file. - `/sql`: Allows running
+SQL statements against the database. This command provides a way for
+administrators to directly interact with the bot's database using SQL queries.
+It's a powerful tool for managing and analyzing the bot's data but should be
+used with caution to avoid unintended data loss or corruption. - `/logs`:
+Checks the logs. This command is used to access the bot's logs, which can
+provide insights into the bot's activity, errors, and user interactions. It's a
+valuable tool for monitoring and troubleshooting the bot's performance. ##
+Support and Feedback If you have any questions, feedback, or suggestions for
+`pytgpt`, please feel free to reach out. Your input is valuable in helping us
+improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
+source and available under the [MIT License](LICENSE). Feel free to use,
+modify, and distribute the code as you see fit. --- Thank you for using
+`pytgpt-bot`. Enjoy your AI-powered interactions!
```

### Comparing `pytgpt_bot-0.1.1/README.md` & `pytgpt_bot-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,30 +47,23 @@
 
 Alternatively, using CLI:
 
    `$ pytgpt-bot run <Your Telegram Token>`
 
 ## Features
 
-### Commands
-
-
-### Usage Information
-
-This section provides detailed instructions on how to use the various commands available in the bot.
-
 - **/start**: Displays the help information, offering a comprehensive list of available commands and their functionalities. This command is essential for users to quickly understand how to interact with the bot.
 
 - **/chat**: Initiate a natural language conversation with the AI. This command allows users to engage in interactive dialogues, ask questions, or make requests.
 
 - **/image**: Generates images from textual descriptions using the default provider. This feature enables users to visualize ideas or concepts through images.
 
 - **/prodia**: Generates images from textual descriptions using the Prodia provider. This command offers a unique style or interpretation of the text descriptions compared to the default method.
 
-- **/audio**: Converts text to speech, providing users with the ability to listen to descriptions, instructions, or any text content read out by the AI.
+- **/speak**: Converts text to speech, providing users with the ability to listen to descriptions, instructions, or any text content read out by the AI.
 
 - **/intro**: Sets a new text for the chat intro. This command allows users to customize the chat introductory prompt which serves as a guide in the human-AI engagement.
 
 - **/voice**: Sets a new voice for speech synthesis. This command enables users to choose from different voices for the AI to use when generating audio from text.
 
 - **/provider**: Sets a new chat provider. This command allows users to switch between different providers for various functionalities, such as `phind`, `llama2`, `koboldai` etc.
 
@@ -80,18 +73,19 @@
 
 - **/check**: Offers an overview of the bot's current configuration, including any custom settings applied by the user.
 
 - **/reset**: Resets the chat history and starts a new conversation thread. This command is useful for users who wish to start fresh or clear their chat history for privacy reasons.
 
 - **/myid**: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for various purposes, such as setting up bot admin.
 
-- `any other text`: An alias for `/chat`, allowing users to continue with chatting.
+- **/suspend**: Pauses the bot's service temporarily. This command is useful for channel administrators who need to temporarily halt the bot's operations without deleting its data or settings. It's a way to manage the bot's availability based on operational needs.
 
+- **/resume**: Resumes the bot's service after it has been suspended. This command allows administrators to quickly bring the bot back online after a pause, ensuring that users can continue interacting with the bot without interruption.
 
-### Administrative Commands
+- `any other text`: An alias for `/chat`, allowing users to continue with chatting.
 
 
 ### Administrative Commands
 
 - `/clear`: Clears all chats. This command is used to remove all chat data from the bot's database. It's a powerful command that should be used with caution, as it will delete all chat history.
 
 - `/total`: Shows the total number of chats available. This command provides an overview of the current chat data stored in the bot's database, helping administrators understand the volume of interactions the bot has had.
```

#### html2text {}

```diff
@@ -11,27 +11,25 @@
 [Python>=3.10](https://python.org) ## Installation 1. From Source Clone repo
 and install. ```bash git clone https://github.com/Simatwa/pytgpt-bot.git cd
 pytgpt-bot pip install . ``` 2. From Pypi *(recommended)* ```sh pip install
 pytgpt-bot ``` ## Usage Before getting started, ensure you've your Telegram bot
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
 file as per the needs and then rename it `.env` before firing up the bot
-`python3 run.py`. Alternatively, using CLI: `$ pytgpt-bot run ` ## Features ###
-Commands ### Usage Information This section provides detailed instructions on
-how to use the various commands available in the bot. - **/start**: Displays
-the help information, offering a comprehensive list of available commands and
-their functionalities. This command is essential for users to quickly
-understand how to interact with the bot. - **/chat**: Initiate a natural
-language conversation with the AI. This command allows users to engage in
-interactive dialogues, ask questions, or make requests. - **/image**: Generates
-images from textual descriptions using the default provider. This feature
-enables users to visualize ideas or concepts through images. - **/prodia**:
-Generates images from textual descriptions using the Prodia provider. This
-command offers a unique style or interpretation of the text descriptions
-compared to the default method. - **/audio**: Converts text to speech,
+`python3 run.py`. Alternatively, using CLI: `$ pytgpt-bot run ` ## Features -
+**/start**: Displays the help information, offering a comprehensive list of
+available commands and their functionalities. This command is essential for
+users to quickly understand how to interact with the bot. - **/chat**: Initiate
+a natural language conversation with the AI. This command allows users to
+engage in interactive dialogues, ask questions, or make requests. - **/image**:
+Generates images from textual descriptions using the default provider. This
+feature enables users to visualize ideas or concepts through images. - **/
+prodia**: Generates images from textual descriptions using the Prodia provider.
+This command offers a unique style or interpretation of the text descriptions
+compared to the default method. - **/speak**: Converts text to speech,
 providing users with the ability to listen to descriptions, instructions, or
 any text content read out by the AI. - **/intro**: Sets a new text for the chat
 intro. This command allows users to customize the chat introductory prompt
 which serves as a guide in the human-AI engagement. - **/voice**: Sets a new
 voice for speech synthesis. This command enables users to choose from different
 voices for the AI to use when generating audio from text. - **/provider**: Sets
 a new chat provider. This command allows users to switch between different
@@ -42,31 +40,37 @@
 interactions or finding specific information from previous conversations. - **/
 check**: Offers an overview of the bot's current configuration, including any
 custom settings applied by the user. - **/reset**: Resets the chat history and
 starts a new conversation thread. This command is useful for users who wish to
 start fresh or clear their chat history for privacy reasons. - **/myid**:
 Echoes the user's Telegram ID. This command is useful for users who need to
 know their Telegram ID for various purposes, such as setting up bot admin. -
-`any other text`: An alias for `/chat`, allowing users to continue with
-chatting. ### Administrative Commands ### Administrative Commands - `/clear`:
-Clears all chats. This command is used to remove all chat data from the bot's
-database. It's a powerful command that should be used with caution, as it will
-delete all chat history. - `/total`: Shows the total number of chats available.
-This command provides an overview of the current chat data stored in the bot's
-database, helping administrators understand the volume of interactions the bot
-has had. - `/drop`: Clears the entire chat table and bot logs. Similar to `/
-clear`, this command removes all data from the chat table in the database. It's
-a more drastic measure than `/clear`, as it completely wipes out all chat data
-and current contents of log file. - `/sql`: Allows running SQL statements
-against the database. This command provides a way for administrators to
-directly interact with the bot's database using SQL queries. It's a powerful
-tool for managing and analyzing the bot's data but should be used with caution
-to avoid unintended data loss or corruption. - `/logs`: Checks the logs. This
-command is used to access the bot's logs, which can provide insights into the
-bot's activity, errors, and user interactions. It's a valuable tool for
-monitoring and troubleshooting the bot's performance. ## Support and Feedback
-If you have any questions, feedback, or suggestions for `pytgpt`, please feel
-free to reach out. Your input is valuable in helping us improve and expand the
-bot's capabilities. ## License `pytgpt-bot` is open-source and available under
-the [MIT License](LICENSE). Feel free to use, modify, and distribute the code
-as you see fit. --- Thank you for using `pytgpt-bot`. Enjoy your AI-powered
-interactions!
+**/suspend**: Pauses the bot's service temporarily. This command is useful for
+channel administrators who need to temporarily halt the bot's operations
+without deleting its data or settings. It's a way to manage the bot's
+availability based on operational needs. - **/resume**: Resumes the bot's
+service after it has been suspended. This command allows administrators to
+quickly bring the bot back online after a pause, ensuring that users can
+continue interacting with the bot without interruption. - `any other text`: An
+alias for `/chat`, allowing users to continue with chatting. ### Administrative
+Commands - `/clear`: Clears all chats. This command is used to remove all chat
+data from the bot's database. It's a powerful command that should be used with
+caution, as it will delete all chat history. - `/total`: Shows the total number
+of chats available. This command provides an overview of the current chat data
+stored in the bot's database, helping administrators understand the volume of
+interactions the bot has had. - `/drop`: Clears the entire chat table and bot
+logs. Similar to `/clear`, this command removes all data from the chat table in
+the database. It's a more drastic measure than `/clear`, as it completely wipes
+out all chat data and current contents of log file. - `/sql`: Allows running
+SQL statements against the database. This command provides a way for
+administrators to directly interact with the bot's database using SQL queries.
+It's a powerful tool for managing and analyzing the bot's data but should be
+used with caution to avoid unintended data loss or corruption. - `/logs`:
+Checks the logs. This command is used to access the bot's logs, which can
+provide insights into the bot's activity, errors, and user interactions. It's a
+valuable tool for monitoring and troubleshooting the bot's performance. ##
+Support and Feedback If you have any questions, feedback, or suggestions for
+`pytgpt`, please feel free to reach out. Your input is valuable in helping us
+improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
+source and available under the [MIT License](LICENSE). Feel free to use,
+modify, and distribute the code as you see fit. --- Thank you for using
+`pytgpt-bot`. Enjoy your AI-powered interactions!
```

### Comparing `pytgpt_bot-0.1.1/pytgpt_bot/cli.py` & `pytgpt_bot-0.1.2/pytgpt_bot/cli.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.1/pytgpt_bot/config.py` & `pytgpt_bot-0.1.2/pytgpt_bot/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from dotenv import load_dotenv
 from os import environ
 from pytgpt.utils import Audio
-from .utils import provider_keys
+from pytgpt_bot.utils import provider_keys
 
 load_dotenv()
 
 assert environ.get("token"), "Export bot's token to the environment 😠"
 
 bot_token: str = environ.get("token")
 database: str = environ.get("database")
 provider: str = environ.get("provider", "auto")
-admin_id: int = int(environ.get("admin-id", 1234567))
+admin_id: str = environ.get("admin-id", "")
 max_tokens: int = int(environ.get("max-tokens", 600))
 timeout: int = int(environ.get("timeout", 30))
 loglevel: int = int(environ.get("loglevel", 20))
 logfile = environ.get("logfile", "")
 voice: str = environ.get("voice", "Brian")
 
 assert (
     provider in provider_keys
 ), f"Provider '{provider}' is not one of {', '.join(provider_keys)}"
 
 
 assert (
     voice in Audio.all_voices
 ), f"Voice '{voice}' is not one of {', '.join(Audio.all_voices)}"
+
+admin_ids: list = admin_id.replace(" ", "").split(",")
```

### Comparing `pytgpt_bot-0.1.1/pytgpt_bot/db.py` & `pytgpt_bot-0.1.2/pytgpt_bot/db.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,34 @@
-from .models import Chat
-from .models import session
-from .config import admin_id
-from telebot.types import Message
+from pytgpt_bot.models import Chat
+from pytgpt_bot.models import session
+from pytgpt_bot.config import admin_id
+from telebot.types import Message, CallbackQuery
 
 
 class User:
     """User dummy model"""
 
-    def __init__(self, message: Message = None, user_id: int = None):
+    def __init__(self, message: Message | CallbackQuery = None, user_id: int = None):
         """Constructor
 
         Args:
             message (telebot.types.Message): Message object. Defaults to None.
             user_id (int): User id. Defaults to None
         """
         assert message or user_id, "Message or User id is required."
-        id = user_id or message.from_user.id
+
+        if user_id:
+            id = user_id
+
+        elif message.chat.type == "private":
+            id = message.from_user.id
+
+        else:
+            id = message.chat.id
+
         chat = session.query(Chat).filter_by(id=id).first()
         if chat:
             # chat exist
             self.chat = chat
         else:
             self.chat = Chat(id=id)
             session.add(self.chat)
```

### Comparing `pytgpt_bot-0.1.1/pytgpt_bot/main.py` & `pytgpt_bot-0.1.2/pytgpt_bot/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 import telebot
 import json
 import logging
+import telebot.util as telebot_util
 import pytgpt.imager as image_generator
 from pytgpt.utils import Audio as audio_generator
 from pytgpt.utils import Conversation
 from pytgpt.utils import AwesomePrompts
 from functools import wraps
 from sqlalchemy import text
 
-from . import __version__, __repo__
+from pytgpt_bot import __version__, __repo__
 
-from .config import (
+from pytgpt_bot.config import (
     bot_token,
     max_tokens,
     timeout,
     loglevel,
     logfile,
-    admin_id,
+    admin_ids,
     provider,
 )
-from .db import User
-from .utils import provider_keys
-from .utils import provider_map
-from .utils import get_random_emoji
-from .models import session, Chat, create_all, drop_all
+from pytgpt_bot.db import User
+from pytgpt_bot.utils import (
+    provider_keys,
+    get_random_emoji,
+    provider_map,
+    make_delete_markup,
+)
+from pytgpt_bot.models import session, Chat, create_all, drop_all
+from pytgpt_bot.filters import (
+    IsActiveFilter,
+    IsBotOwnerFilter,
+    IsAdminFilter,
+    IsBotTaggedFilter,
+    IsChatCommandFilter,
+)
 
 chosen_provider: str = provider_map.get(provider)
 
 log_params = dict(
     format="%(asctime)s : %(levelname)s - %(message)s",
     datefmt="%d-%b-%Y %H:%M:%S",
     level=loglevel,
@@ -42,40 +53,42 @@
 logging.basicConfig(**log_params)
 
 bot = telebot.TeleBot(bot_token, disable_web_page_preview=True)
 
 bot.remove_webhook()
 
 logging.info(
-    f"Bot started sucessfully {get_random_emoji('happy')}. Admin ID - [{admin_id}]"
+    f"Bot started sucessfully {get_random_emoji('happy')}. Admin IDs - [{', '.join(admin_ids)}]"
 )
 
 usage_info = (
     "Welcome to [PYTGPT-BOT](https://github.com/Simatwa/pytgpt-bot) ✨.\n"
-    "For chatting, text-to-image and text-to-voice conversions.\n\n"
+    "For chatting, text-to-image and text-to-speech conversions.\n\n"
     "Usage commands:\n"
     "1. /start : Show this help info 📚\n"
     "2. /chat : Chat with AI 🤖\n"
     "3. /image : Generate image from text 🖼️ (default)\n"
     "4. /prodia : Generate image from text 🎨 (Prodia)\n"
-    "5. /audio : Generate audio from text 🎧\n"
+    "5. /speak : Generate speech from text 🎧\n"
     "6. /intro : Set new text for chat intro 📝\n"
     "7. /voice : Set new voice for speech synthesis 🎙️\n"
     "8. /provider : Set new chat provider 🌐\n"
     "9. /awesome : Set awesome prompt as intro 💥\n"
     "10. /history : Check chat history 🕰️\n"
     "11. /check : Check current settings ⚙️\n"
     "12. /reset : Start new chat thread 🔄\n"
     "13. /myid : Echo your Telegram ID 🆔\n"
+    "14. /suspend : Pause service for a while 🚫\n"
+    "15. /resume : Resume paused sevice 🚀\n"
     "default : Chat with AI.\n\n"
     f"For instances {get_random_emoji('love')}:\n"
     "\t\t\t/chat Hello there.\n"
     "\t\t\t/image Peaceful desert scene\n"
     "\t\t\t/prodia Clear cool shore view\n"
-    "\t\t\t/audio I am better than you.\n\n"
+    "\t\t\t/speak I am better than you.\n\n"
     f"[🌟 Star me on Github]({__repo__}) pytgpt-bot v{__version__}"
 )
 
 admin_commands = (
     "\n\nAdmin Commands\n"
     "/clear : Clear all chats 🧹\n"
     "/total : Total chats available 📊\n"
@@ -95,65 +108,46 @@
     """
 
     def main(func):
 
         @wraps(func)
         def decorator(message: telebot.types.Message):
             try:
-                logging.info(
-                    f"Serving user [{message.from_user.id}] ({message.from_user.full_name}) - Function [{func.__name__}]"
-                )
-                if admin and not User(message).is_admin:
-                    return bot.reply_to(
-                        message,
-                        f"{get_random_emoji('angry')} Action restricted to admins only❗️",
-                        reply_markup=make_delete_markup(message),
+                if message.chat.type == "private":
+                    logging.info(
+                        f"Serving user [{message.from_user.id}] ({message.from_user.full_name}) - Function [{func.__name__}]"
                     )
-
-                if message.text and message.text.startswith("/") and not preserve:
-                    message.text = " ".join(message.text.split(" ")[1:])
+                else:
+                    logging.info(f"Serving Group  - Function [{func.__name__}]")
+                if not preserve:
+                    message.text = telebot_util.extract_arguments(message.text)
 
                 if text and not message.text:
                     return bot.reply_to(
                         message,
                         f"{get_random_emoji()} Text is required❗️❗️.",
                         reply_markup=make_delete_markup(message),
                     )
 
                 return func(message)
             except Exception as e:
+                logging.exception(e)
                 logging.error(f"Error on function - {func.__name__} - {e}")
                 logging.debug(str(e))
                 bot.reply_to(
                     message,
                     text=f"{get_random_emoji('angry')} An error occured and I could't complete that request ❗️❗️❗️",
                     reply_markup=make_delete_markup(message),
                 )
 
         return decorator
 
     return main
 
 
-def make_delete_markup(
-    message: telebot.types.Message,
-) -> telebot.types.InlineKeyboardMarkup:
-    """Creates delete markup
-
-    Args:
-        message (telebot.types.Message):
-    """
-    markup = telebot.types.InlineKeyboardMarkup(row_width=1)
-    callback_button = telebot.types.InlineKeyboardButton(
-        text="🗑️", callback_data=f"delete:{message.chat.id}:{message.id}"
-    )
-    markup.add(callback_button)
-    return markup
-
-
 def send_and_add_delete_button(
     message: telebot.types.Message,
     text: str,
     as_reply: bool = False,
     parse_mode="Markdown",
 ):
     """Add send text and add delete inlineKeyboard item
@@ -187,53 +181,48 @@
 
     Args:
         message (telebot.types.Message): Message object.
         text (str): Text to be sent.
         add_delete (bool). Add delete button. Defaults to False.
         parse_mode (str): __. Defaults to Markdown.
     """
-    max_length = 4096
     take_action = send_and_add_delete_button if add_delete else bot.send_message
-    if len(text) <= max_length:
-        # bot.send_message(message.chat.id, text)
+    for part in telebot_util.smart_split(text):
         take_action(
-            message if add_delete else message.chat.id, text, parse_mode=parse_mode
+            message if add_delete else message.chat.id, part, parse_mode=parse_mode
         )
-    else:
-        parts = [text[i : i + max_length] for i in range(0, len(text), max_length)]
-        for part in parts:
-            take_action(
-                message if add_delete else message.chat.id, part, parse_mode=parse_mode
-            )
 
 
-@bot.message_handler(commands=["help", "start"])
+@bot.message_handler(commands=["help", "start"], is_chat_active=True)
+@bot.channel_post_handler(commands=["help", "start"], is_chat_active=True)
 @handler_formatter()
 def home(message: telebot.types.Message):
     """Show help"""
-
+    # print(message)
     return bot.send_message(
         message.chat.id,
         text=(usage_info + admin_commands if User(message).is_admin else usage_info),
         reply_markup=make_delete_markup(message),
         parse_mode="Markdown",
     )
 
 
-@bot.message_handler(commands=["myid"])
+@bot.message_handler(commands=["myid"], is_chat_admin=True)
+@bot.channel_post_handler(commands=["myid"], is_chat_admin=True)
 @handler_formatter()
 def echo_user_id(message: telebot.types.Message):
     return bot.reply_to(
         message,
         f"Greetings {message.from_user.first_name} {get_random_emoji('love')}. Your Telegram ID is {message.from_user.id}.",
         reply_markup=make_delete_markup(message),
     )
 
 
-@bot.message_handler(commands=["intro"])
+@bot.message_handler(commands=["intro"], is_chat_admin=True)
+@bot.channel_post_handler(commands=["intro"], is_chat_admin=True)
 @handler_formatter(text=True)
 def set_chat_intro(message: telebot.types.Message):
     """Set new value for chat intro"""
     intro = awesome_prompts_dict.get(message.text, message.text)
     if not len(intro) > 10:
         return bot.reply_to(
             message,
@@ -243,15 +232,16 @@
     user = User(message)
     user.chat.intro = intro
     return bot.reply_to(
         message, "New intro set successfully.", reply_markup=make_delete_markup(message)
     )
 
 
-@bot.message_handler(commands=["voice"])
+@bot.message_handler(commands=["voice"], is_chat_admin=True)
+@bot.channel_post_handler(commands=["voice"], is_chat_admin=True)
 @handler_formatter(text=False)
 def set_new_speech_voice(message: telebot.types.Message):
     """Set new voice for speech synthesis"""
     user_id: str = message.from_user.id
     markup = telebot.types.InlineKeyboardMarkup(row_width=4)
     make_item = lambda voice: telebot.types.InlineKeyboardButton(
         voice, callback_data=f"{voice}:{user_id}"
@@ -280,15 +270,16 @@
         message.chat.id,
         f"{get_random_emoji('happy')} New voice set : `{voice}`",
         reply_markup=markup,
         parse_mode="Markdown",
     )
 
 
-@bot.message_handler(commands=["provider"])
+@bot.message_handler(commands=["provider"], is_chat_admin=True)
+@bot.channel_post_handler(commands=["provider"], is_chat_admin=True)
 @handler_formatter(text=False)
 def set_new_text_provider(message: telebot.types.Message):
     """Set new text provider"""
     user_id: str = message.from_user.id
     markup = telebot.types.InlineKeyboardMarkup(row_width=2)
     make_item = lambda provider: telebot.types.InlineKeyboardButton(
         provider, callback_data=f"{provider}:{user_id}"
@@ -315,15 +306,16 @@
         message.chat.id,
         f"New text provider set {get_random_emoji('love')}: `{provider}`",
         reply_markup=markup,
         parse_mode="Markdown",
     )
 
 
-@bot.message_handler(commands=["awesome"])
+@bot.message_handler(commands=["awesome"], is_chat_admin=True, is_chat_active=True)
+@bot.channel_post_handler(commands=["awesome"], is_chat_admin=True, is_chat_active=True)
 @handler_formatter(text=False)
 def set_awesome_prompt_as_chat_intro(message: telebot.types.Message):
     """Set awesome prompt as intro"""
     user_id: str = message.from_user.id
     markup = telebot.types.InlineKeyboardMarkup(row_width=4)
     make_item = lambda awesome: telebot.types.InlineKeyboardButton(
         awesome, callback_data=f"{awesome}:{user_id}"
@@ -352,46 +344,50 @@
         call.message.chat.id,
         f"""New awesome-intro set:\n```{user.chat.intro}\n```.""",
         reply_markup=make_delete_markup(call.message),
         parse_mode="Markdown",
     )
 
 
-@bot.message_handler(commands=["check"])
+@bot.message_handler(commands=["check"], is_chat_admin=True)
+@bot.channel_post_handler(commands=["check"], is_chat_admin=True)
 @handler_formatter()
 def check_current_settings(message: telebot.types.Message):
     """Check current user settings"""
     chat = User(message).chat
     current_user_settings = (
+        f"Is Active :  `{chat.is_active}`\n"
         f"Chat Length : `{len(chat.history)}`\n"
         f"Speech Voice : `{chat.voice}`\n"
         f"Chat Provider : `{chat.provider}`\n"
         f"Chat Intro : `{chat.intro}`"
     )
     return bot.reply_to(
         message,
         current_user_settings,
         reply_markup=make_delete_markup(message),
         parse_mode="Markdown",
     )
 
 
-@bot.message_handler(commands=["history"])
+@bot.message_handler(commands=["history"], is_chat_admin=True, is_chat_active=True)
+@bot.channel_post_handler(commands=["history"], is_chat_admin=True, is_chat_active=True)
 @handler_formatter()
 def check_chat_history(message: telebot.types.Message):
     user = User(message)
     return send_long_text(
         message,
         user.chat.history or f"{get_random_emoji()} Your chat history is empty ❗️",
         add_delete=True,
         parse_mode="Markdown",
     )
 
 
-@bot.message_handler(commands=["image", "img"])
+@bot.message_handler(commands=["image", "img"], is_chat_active=True)
+@bot.channel_post_handler(commands=["image", "img"], is_chat_active=True)
 @handler_formatter(text=True)
 def text_to_image_default(message: telebot.types.Message):
     """Generate image using `image`"""
     bot.send_chat_action(message.chat.id, "upload_photo", timeout=timeout)
     generator_obj = image_generator.Imager(
         timeout=timeout,
     )
@@ -401,29 +397,31 @@
             message.text,
         )[0],
         caption=message.text,
         reply_markup=make_delete_markup(message),
     )
 
 
-@bot.message_handler(commands=["prodia", "prod"])
+@bot.message_handler(commands=["prodia", "prod"], is_chat_active=True)
+@bot.channel_post_handler(commands=["prodia", "prod"], is_chat_active=True)
 @handler_formatter(text=True)
 def text_to_image_prodia(message: telebot.types.Message):
     """Generate image using `prodia`"""
     bot.send_chat_action(message.chat.id, "upload_photo", timeout=timeout)
     generator_obj = image_generator.Prodia(timeout=timeout)
     return bot.send_photo(
         message.chat.id,
         photo=generator_obj.generate(message.text)[0],
         caption=message.text,
         reply_markup=make_delete_markup(message),
     )
 
 
-@bot.message_handler(commands=["audio", "aud"])
+@bot.message_handler(commands=["speak", "spe"], is_chat_active=True)
+@bot.channel_post_handler(commands=["speak", "spe"], is_chat_active=True)
 @handler_formatter(text=True)
 def text_to_audio(message: telebot.types.Message):
     """Convert text to audio"""
     bot.send_chat_action(message.chat.id, "upload_audio", timeout=timeout)
     voice = User(message).chat.voice
     audio_chunk = audio_generator.text_to_audio(
         message=message.text,
@@ -432,62 +430,85 @@
     )
     return bot.send_audio(
         message.chat.id,
         audio=audio_chunk,
         caption=message.text,
         reply_markup=make_delete_markup(message),
         performer=voice,
-        title="Text-to-Audio",
+        title="Text-to-Speech",
     )
 
 
-@bot.message_handler(commands=["reset"])
+@bot.message_handler(commands=["reset"], is_chat_admin=True, is_chat_active=True)
+@bot.channel_post_handler(commands=["reset"], is_chat_admin=True, is_chat_active=True)
 @handler_formatter()
 def reset_chat(message: telebot.types.Message):
     """Reset current chat thread"""
     user = User(message)
     user.delete()
     return bot.reply_to(
         message,
         f"New chat instance created. {get_random_emoji('happy')}",
         reply_markup=make_delete_markup(message),
     )
 
 
-@bot.message_handler(commands=["clear", "clear_chats"])
+@bot.message_handler(commands=["suspend"], is_chat_admin=True, is_chat_active=True)
+@bot.channel_post_handler(commands=["suspend"], is_chat_admin=True, is_chat_active=True)
+@handler_formatter()
+def change_chat_status_to_inactive(message: telebot.types.Message):
+    chats = User(message).chat
+    chats.is_active = False
+    return bot.reply_to(
+        message, text=f"Service Suspended 🚫.", reply_markup=make_delete_markup(message)
+    )
+
+
+@bot.message_handler(commands=["resume"], is_chat_admin=True)
+@bot.channel_post_handler(commands=["resume"], is_chat_admin=True)
+@handler_formatter()
+def change_chat_status_to_active(message: telebot.types.Message):
+    chat = User(message).chat
+    chat.is_active = True
+    return bot.reply_to(
+        message, text=f"Service Resumed 🚀.", reply_markup=make_delete_markup(message)
+    )
+
+
+@bot.message_handler(commands=["clear", "clear_chats"], is_bot_owner=True)
 @handler_formatter(admin=True)
 def clear_chats(message: telebot.types.Message):
     """Delete all chat entries"""
     session.query(Chat).delete()
     logging.warning(
         f"Clearing Chats - [{message.from_user.full_name}] ({message.from_user.id}, {message.from_user.username})"
     )
     return bot.reply_to(
         message,
         f"{get_random_emoji('love')} Chats cleared successfully.",
         reply_markup=make_delete_markup(message),
     )
 
 
-@bot.message_handler(commands=["total", "total_chats"])
+@bot.message_handler(commands=["total", "total_chats"], is_bot_owner=True)
 @handler_formatter(admin=True)
 def total_chats_query(message: telebot.types.Message):
     """Query total chats"""
     total_chats = session.query(Chat).count()
     logging.warning(
         f"Total Chats query - [{message.from_user.full_name}] ({message.from_user.id}, {message.from_user.username})"
     )
     return bot.reply_to(
         message,
         f"Total Chats {total_chats}",
         reply_markup=make_delete_markup(message),
     )
 
 
-@bot.message_handler(commands=["drop", "drop_chats"])
+@bot.message_handler(commands=["drop", "drop_chats"], is_bot_owner=True)
 @handler_formatter(admin=True)
 def total_chats_table_and_logs(message: telebot.types.Message):
     """Drop chat table and create new"""
     if logfile:
         with open(logfile, "w") as fh:
             fh.write(
                 f"ADMIN CLEARED LOGS & DROPPED CHAT TABLE [{message.from_user.id}] - ({message.from_user.full_name})\n"
@@ -500,15 +521,15 @@
     return bot.reply_to(
         message,
         f"{get_random_emoji('love')} Chat table and bot logs dropped and new one created.",
         reply_markup=make_delete_markup(message),
     )
 
 
-@bot.message_handler(commands=["sql"])
+@bot.message_handler(commands=["sql"], is_bot_owner=True)
 @handler_formatter(admin=True, text=True)
 def run_sql_statement(message: telebot.types.Message):
     """Run sql statements against database"""
     logging.warning(
         f"Running SQL statements - [{message.from_user.full_name}] ({message.from_user.id}, {message.from_user.username})"
     )
     try:
@@ -533,41 +554,36 @@
         return send_long_text(
             message,
             response,
             add_delete=True,
         )
 
 
-@bot.message_handler(commands=["logs"])
+@bot.message_handler(commands=["logs"], is_bot_owner=True)
 @handler_formatter(admin=True)
 def check_current_settings(message: telebot.types.Message):
     """View bot logs"""
     if not logfile:
         return bot.reply_to(
             message,
             f"{get_random_emoji()} Logfile not specified ❗️",
             reply_markup=make_delete_markup(message),
         )
     with open(logfile, encoding="utf-8") as fh:
         contents: str = fh.read()
     return send_long_text(message, contents, add_delete=True, parse_mode=None)
 
 
-def is_action_for_chat(message: telebot.types.Message) -> bool:
-    splitted_text = message.text.split(" ")
-    if splitted_text[0].startswith("/"):
-        if splitted_text[0] == "/chat":
-            return True
-        else:
-            return False
-    return True
-
-
-@bot.message_handler(content_types=["text"], func=is_action_for_chat)
-@handler_formatter(text=True)
+@bot.message_handler(content_types=["text"], is_chat_active=True, is_chat_command=True)
+@bot.channel_post_handler(
+    content_types=["text"],
+    is_chat_active=True,
+    commands=["chat"],
+)
+@handler_formatter()
 def text_chat(message: telebot.types.Message):
     """Text generation"""
     user = User(message)
     conversation = Conversation(max_tokens=max_tokens)
     conversation.chat_history = user.chat.history
     user_provider = provider_map.get(user.chat.provider)
     conversation_prompt = conversation.gen_complete_prompt(
@@ -580,15 +596,16 @@
     conversation.update_chat_history(
         prompt=message.text, response=ai_response, force=True
     )
     user.chat.history = conversation.chat_history
     send_long_text(message, ai_response)
 
 
-@bot.message_handler(func=lambda val: True)
+@bot.message_handler(is_chat_active=True)
+@bot.channel_post_handler(is_chat_active=True, is_bot_tagged=True)
 def any_other_action(message):
     return bot.reply_to(
         message,
         usage_info,
         reply_markup=make_delete_markup(message),
         parse_mode="Markdown",
     )
@@ -604,7 +621,14 @@
         bot.delete_message(trigger_chat_id, trigger_message_id)
     except:
         pass
     try:
         bot.delete_message(call.message.chat.id, call.message.id)
     except:
         pass
+
+
+bot.add_custom_filter(IsBotOwnerFilter())
+bot.add_custom_filter(IsAdminFilter(bot))
+bot.add_custom_filter(IsActiveFilter())
+bot.add_custom_filter(IsBotTaggedFilter(bot.get_me()))
+bot.add_custom_filter(IsChatCommandFilter())
```

### Comparing `pytgpt_bot-0.1.1/pytgpt_bot/models.py` & `pytgpt_bot-0.1.2/pytgpt_bot/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.orm import declarative_base
-from sqlalchemy import Column, Integer, Text, String
+from sqlalchemy import Column, Integer, Text, String, Boolean
 from pytgpt.utils import Conversation
-from .config import database as database_str
-from .config import provider as default_provider
-from .config import voice
+from pytgpt_bot.config import database as database_str
+from pytgpt_bot.config import provider as default_provider
+from pytgpt_bot.config import voice
 
 if not database_str:
     from .utils import path_to_default_db
 
     database_str: str = f"sqlite:///{path_to_default_db.as_posix()}"
 
 engine = create_engine(database_str)
@@ -26,14 +26,15 @@
 class Chat(Base):
     __tablename__ = "chats"
     id = Column(Integer, primary_key=True)
     intro = Column(Text, default=Conversation.intro, nullable=False)
     provider = Column(String(20), default=default_provider, nullable=False)
     history = Column(Text, default="")
     voice = Column(String(30), default=voice, nullable=False)
+    is_active = Column(Boolean, default=True, nullable=False)
 
 
 def create_all():
     """Create tables from models"""
     Base.metadata.create_all(engine)
```

### Comparing `pytgpt_bot-0.1.1/pytgpt_bot/utils.py` & `pytgpt_bot-0.1.2/pytgpt_bot/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pytgpt.phind import PHIND
 from pytgpt.llama2 import LLAMA2
 from pytgpt.blackboxai import BLACKBOXAI
 from pytgpt.perplexity import PERPLEXITY
 from pytgpt.yepchat import YEPCHAT
 from pytgpt.auto import AUTO
 from random import choice
+import telebot
 
 provider_map: dict[str, object] = {
     "opengpt": OPENGPT,
     "koboldai": KOBOLDAI,
     "phind": PHIND,
     "llama2": LLAMA2,
     "blackboxai": BLACKBOXAI,
@@ -79,7 +80,23 @@
 
     Returns:
         str: emoji
     """
     if not mood:
         mood = choice(emoji_keys)
     return choice(emojis[mood])
+
+
+def make_delete_markup(
+    message: telebot.types.Message,
+) -> telebot.types.InlineKeyboardMarkup:
+    """Creates delete markup
+
+    Args:
+        message (telebot.types.Message):
+    """
+    markup = telebot.types.InlineKeyboardMarkup(row_width=1)
+    callback_button = telebot.types.InlineKeyboardButton(
+        text="🗑️", callback_data=f"delete:{message.chat.id}:{message.id}"
+    )
+    markup.add(callback_button)
+    return markup
```

### Comparing `pytgpt_bot-0.1.1/pytgpt_bot.egg-info/PKG-INFO` & `pytgpt_bot-0.1.2/pytgpt_bot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.1.1
-Summary: Telegram bot for chatting, text-to-image and text-to-voice conversions
+Version: 0.1.2
+Summary: Telegram bot for chatting, text-to-image and text-to-speech conversions
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/pytgpt-bot
@@ -86,30 +86,23 @@
 
 Alternatively, using CLI:
 
    `$ pytgpt-bot run <Your Telegram Token>`
 
 ## Features
 
-### Commands
-
-
-### Usage Information
-
-This section provides detailed instructions on how to use the various commands available in the bot.
-
 - **/start**: Displays the help information, offering a comprehensive list of available commands and their functionalities. This command is essential for users to quickly understand how to interact with the bot.
 
 - **/chat**: Initiate a natural language conversation with the AI. This command allows users to engage in interactive dialogues, ask questions, or make requests.
 
 - **/image**: Generates images from textual descriptions using the default provider. This feature enables users to visualize ideas or concepts through images.
 
 - **/prodia**: Generates images from textual descriptions using the Prodia provider. This command offers a unique style or interpretation of the text descriptions compared to the default method.
 
-- **/audio**: Converts text to speech, providing users with the ability to listen to descriptions, instructions, or any text content read out by the AI.
+- **/speak**: Converts text to speech, providing users with the ability to listen to descriptions, instructions, or any text content read out by the AI.
 
 - **/intro**: Sets a new text for the chat intro. This command allows users to customize the chat introductory prompt which serves as a guide in the human-AI engagement.
 
 - **/voice**: Sets a new voice for speech synthesis. This command enables users to choose from different voices for the AI to use when generating audio from text.
 
 - **/provider**: Sets a new chat provider. This command allows users to switch between different providers for various functionalities, such as `phind`, `llama2`, `koboldai` etc.
 
@@ -119,18 +112,19 @@
 
 - **/check**: Offers an overview of the bot's current configuration, including any custom settings applied by the user.
 
 - **/reset**: Resets the chat history and starts a new conversation thread. This command is useful for users who wish to start fresh or clear their chat history for privacy reasons.
 
 - **/myid**: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for various purposes, such as setting up bot admin.
 
-- `any other text`: An alias for `/chat`, allowing users to continue with chatting.
+- **/suspend**: Pauses the bot's service temporarily. This command is useful for channel administrators who need to temporarily halt the bot's operations without deleting its data or settings. It's a way to manage the bot's availability based on operational needs.
 
+- **/resume**: Resumes the bot's service after it has been suspended. This command allows administrators to quickly bring the bot back online after a pause, ensuring that users can continue interacting with the bot without interruption.
 
-### Administrative Commands
+- `any other text`: An alias for `/chat`, allowing users to continue with chatting.
 
 
 ### Administrative Commands
 
 - `/clear`: Clears all chats. This command is used to remove all chat data from the bot's database. It's a powerful command that should be used with caution, as it will delete all chat history.
 
 - `/total`: Shows the total number of chats available. This command provides an overview of the current chat data stored in the bot's database, helping administrators understand the volume of interactions the bot has had.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.1 Summary: Telegram bot for
-chatting, text-to-image and text-to-voice conversions Home-page: https://
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.2 Summary: Telegram bot for
+chatting, text-to-image and text-to-speech conversions Home-page: https://
 github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
 pytgpt-bot/releases Project-URL: Documentation, https://github.com/Simatwa/
@@ -36,27 +36,25 @@
 [Python>=3.10](https://python.org) ## Installation 1. From Source Clone repo
 and install. ```bash git clone https://github.com/Simatwa/pytgpt-bot.git cd
 pytgpt-bot pip install . ``` 2. From Pypi *(recommended)* ```sh pip install
 pytgpt-bot ``` ## Usage Before getting started, ensure you've your Telegram bot
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
 file as per the needs and then rename it `.env` before firing up the bot
-`python3 run.py`. Alternatively, using CLI: `$ pytgpt-bot run ` ## Features ###
-Commands ### Usage Information This section provides detailed instructions on
-how to use the various commands available in the bot. - **/start**: Displays
-the help information, offering a comprehensive list of available commands and
-their functionalities. This command is essential for users to quickly
-understand how to interact with the bot. - **/chat**: Initiate a natural
-language conversation with the AI. This command allows users to engage in
-interactive dialogues, ask questions, or make requests. - **/image**: Generates
-images from textual descriptions using the default provider. This feature
-enables users to visualize ideas or concepts through images. - **/prodia**:
-Generates images from textual descriptions using the Prodia provider. This
-command offers a unique style or interpretation of the text descriptions
-compared to the default method. - **/audio**: Converts text to speech,
+`python3 run.py`. Alternatively, using CLI: `$ pytgpt-bot run ` ## Features -
+**/start**: Displays the help information, offering a comprehensive list of
+available commands and their functionalities. This command is essential for
+users to quickly understand how to interact with the bot. - **/chat**: Initiate
+a natural language conversation with the AI. This command allows users to
+engage in interactive dialogues, ask questions, or make requests. - **/image**:
+Generates images from textual descriptions using the default provider. This
+feature enables users to visualize ideas or concepts through images. - **/
+prodia**: Generates images from textual descriptions using the Prodia provider.
+This command offers a unique style or interpretation of the text descriptions
+compared to the default method. - **/speak**: Converts text to speech,
 providing users with the ability to listen to descriptions, instructions, or
 any text content read out by the AI. - **/intro**: Sets a new text for the chat
 intro. This command allows users to customize the chat introductory prompt
 which serves as a guide in the human-AI engagement. - **/voice**: Sets a new
 voice for speech synthesis. This command enables users to choose from different
 voices for the AI to use when generating audio from text. - **/provider**: Sets
 a new chat provider. This command allows users to switch between different
@@ -67,31 +65,37 @@
 interactions or finding specific information from previous conversations. - **/
 check**: Offers an overview of the bot's current configuration, including any
 custom settings applied by the user. - **/reset**: Resets the chat history and
 starts a new conversation thread. This command is useful for users who wish to
 start fresh or clear their chat history for privacy reasons. - **/myid**:
 Echoes the user's Telegram ID. This command is useful for users who need to
 know their Telegram ID for various purposes, such as setting up bot admin. -
-`any other text`: An alias for `/chat`, allowing users to continue with
-chatting. ### Administrative Commands ### Administrative Commands - `/clear`:
-Clears all chats. This command is used to remove all chat data from the bot's
-database. It's a powerful command that should be used with caution, as it will
-delete all chat history. - `/total`: Shows the total number of chats available.
-This command provides an overview of the current chat data stored in the bot's
-database, helping administrators understand the volume of interactions the bot
-has had. - `/drop`: Clears the entire chat table and bot logs. Similar to `/
-clear`, this command removes all data from the chat table in the database. It's
-a more drastic measure than `/clear`, as it completely wipes out all chat data
-and current contents of log file. - `/sql`: Allows running SQL statements
-against the database. This command provides a way for administrators to
-directly interact with the bot's database using SQL queries. It's a powerful
-tool for managing and analyzing the bot's data but should be used with caution
-to avoid unintended data loss or corruption. - `/logs`: Checks the logs. This
-command is used to access the bot's logs, which can provide insights into the
-bot's activity, errors, and user interactions. It's a valuable tool for
-monitoring and troubleshooting the bot's performance. ## Support and Feedback
-If you have any questions, feedback, or suggestions for `pytgpt`, please feel
-free to reach out. Your input is valuable in helping us improve and expand the
-bot's capabilities. ## License `pytgpt-bot` is open-source and available under
-the [MIT License](LICENSE). Feel free to use, modify, and distribute the code
-as you see fit. --- Thank you for using `pytgpt-bot`. Enjoy your AI-powered
-interactions!
+**/suspend**: Pauses the bot's service temporarily. This command is useful for
+channel administrators who need to temporarily halt the bot's operations
+without deleting its data or settings. It's a way to manage the bot's
+availability based on operational needs. - **/resume**: Resumes the bot's
+service after it has been suspended. This command allows administrators to
+quickly bring the bot back online after a pause, ensuring that users can
+continue interacting with the bot without interruption. - `any other text`: An
+alias for `/chat`, allowing users to continue with chatting. ### Administrative
+Commands - `/clear`: Clears all chats. This command is used to remove all chat
+data from the bot's database. It's a powerful command that should be used with
+caution, as it will delete all chat history. - `/total`: Shows the total number
+of chats available. This command provides an overview of the current chat data
+stored in the bot's database, helping administrators understand the volume of
+interactions the bot has had. - `/drop`: Clears the entire chat table and bot
+logs. Similar to `/clear`, this command removes all data from the chat table in
+the database. It's a more drastic measure than `/clear`, as it completely wipes
+out all chat data and current contents of log file. - `/sql`: Allows running
+SQL statements against the database. This command provides a way for
+administrators to directly interact with the bot's database using SQL queries.
+It's a powerful tool for managing and analyzing the bot's data but should be
+used with caution to avoid unintended data loss or corruption. - `/logs`:
+Checks the logs. This command is used to access the bot's logs, which can
+provide insights into the bot's activity, errors, and user interactions. It's a
+valuable tool for monitoring and troubleshooting the bot's performance. ##
+Support and Feedback If you have any questions, feedback, or suggestions for
+`pytgpt`, please feel free to reach out. Your input is valuable in helping us
+improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
+source and available under the [MIT License](LICENSE). Feel free to use,
+modify, and distribute the code as you see fit. --- Thank you for using
+`pytgpt-bot`. Enjoy your AI-powered interactions!
```

### Comparing `pytgpt_bot-0.1.1/setup.py` & `pytgpt_bot-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     full_path: Path = ROOT_PATH / path
     return full_path.read_text(encoding="utf-8")
 
 
 setup(
     name="pytgpt-bot",
     packages=["pytgpt_bot"],
-    version="0.1.1",
+    version="0.1.2",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
-    description="Telegram bot for chatting, text-to-image and text-to-voice conversions",
+    description="Telegram bot for chatting, text-to-image and text-to-speech conversions",
     url="https://github.com/Simatwa/pytgpt-bot",
     project_urls={
         "Bug Report": "https://github.com/Simatwa/pytgpt-bot/issues/new",
         "Homepage": "https://github.com/Simatwa/pytgpt-bot",
         "Source Code": "https://github.com/Simatwa/pytgpt-bot",
         "Issue Tracker": "https://github.com/Simatwa/pytgpt-bot/issues",
         "Download": "https://github.com/Simatwa/pytgpt-bot/releases",
```

