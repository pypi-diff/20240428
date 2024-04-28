# Comparing `tmp/pytgpt_bot-0.1.2.tar.gz` & `tmp/pytgpt_bot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytgpt_bot-0.1.2.tar", last modified: Sun Apr 28 00:53:26 2024, max compression
+gzip compressed data, was "pytgpt_bot-0.1.3.tar", last modified: Sun Apr 28 15:22:37 2024, max compression
```

## Comparing `pytgpt_bot-0.1.2.tar` & `pytgpt_bot-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:53:26.067393 pytgpt_bot-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-28 00:53:26.067393 pytgpt_bot-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:53:26.067393 pytgpt_bot-0.1.2/pytgpt_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    21893 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/pytgpt_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 00:53:26.067393 pytgpt_bot-0.1.2/pytgpt_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-28 00:53:26.000000 pytgpt_bot-0.1.2/pytgpt_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-28 00:53:26.000000 pytgpt_bot-0.1.2/pytgpt_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 00:53:26.000000 pytgpt_bot-0.1.2/pytgpt_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 00:53:26.000000 pytgpt_bot-0.1.2/pytgpt_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-28 00:53:26.000000 pytgpt_bot-0.1.2/pytgpt_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 00:53:26.000000 pytgpt_bot-0.1.2/pytgpt_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 00:53:26.067393 pytgpt_bot-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-28 00:53:07.000000 pytgpt_bot-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:22:37.193545 pytgpt_bot-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-28 15:22:37.193545 pytgpt_bot-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:22:37.189545 pytgpt_bot-0.1.3/pytgpt_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25018 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/pytgpt_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:22:37.193545 pytgpt_bot-0.1.3/pytgpt_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-28 15:22:37.000000 pytgpt_bot-0.1.3/pytgpt_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-28 15:22:37.000000 pytgpt_bot-0.1.3/pytgpt_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:22:37.000000 pytgpt_bot-0.1.3/pytgpt_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 15:22:37.000000 pytgpt_bot-0.1.3/pytgpt_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-28 15:22:37.000000 pytgpt_bot-0.1.3/pytgpt_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 15:22:37.000000 pytgpt_bot-0.1.3/pytgpt_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:22:37.193545 pytgpt_bot-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-28 15:22:20.000000 pytgpt_bot-0.1.3/setup.py
```

### Comparing `pytgpt_bot-0.1.2/LICENSE` & `pytgpt_bot-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.2/PKG-INFO` & `pytgpt_bot-0.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.1.2
+Version: 0.1.3
 Summary: Telegram bot for chatting, text-to-image and text-to-speech conversions
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/pytgpt-bot
 Project-URL: Source Code, https://github.com/Simatwa/pytgpt-bot
 Project-URL: Issue Tracker, https://github.com/Simatwa/pytgpt-bot/issues
 Project-URL: Download, https://github.com/Simatwa/pytgpt-bot/releases
 Project-URL: Documentation, https://github.com/Simatwa/pytgpt-bot/blob/main/README.md
-Keywords: ai,tgpt,pytgpt,chatbot,telegrambot,pytelegrambot,chatbot,text-to-audio,text-to-image
+Keywords: ai,tgpt,pytgpt,chatbot,telegrambot,pytelegrambot,chatbot,text-to-speech,text-to-image
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: Free For Home Use
 Classifier: Intended Audience :: Customer Service
 Classifier: Programming Language :: Python
@@ -86,58 +86,89 @@
 
 Alternatively, using CLI:
 
    `$ pytgpt-bot run <Your Telegram Token>`
 
 ## Features
 
-- **/start**: Displays the help information, offering a comprehensive list of available commands and their functionalities. This command is essential for users to quickly understand how to interact with the bot.
+### Access Commands
 
-- **/chat**: Initiate a natural language conversation with the AI. This command allows users to engage in interactive dialogues, ask questions, or make requests.
+- **/start**: This command shows you how to use the bot. It's like a guidebook for all the commands and what they do.
 
-- **/image**: Generates images from textual descriptions using the default provider. This feature enables users to visualize ideas or concepts through images.
+- **/chat**: Use this to talk to the AI. You can ask questions, make requests, or just chat about anything.
 
-- **/prodia**: Generates images from textual descriptions using the Prodia provider. This command offers a unique style or interpretation of the text descriptions compared to the default method.
+- **/image**: Want to see what something looks like? Type a description, and this command will create an image for you.
 
-- **/speak**: Converts text to speech, providing users with the ability to listen to descriptions, instructions, or any text content read out by the AI.
+- **/prodia**: Similar to `/image`, but it gives you a different style of image.
 
-- **/intro**: Sets a new text for the chat intro. This command allows users to customize the chat introductory prompt which serves as a guide in the human-AI engagement.
+- **/speak**: If you prefer listening to text instead of reading it, use this command to have the AI read out text for you.
 
-- **/voice**: Sets a new voice for speech synthesis. This command enables users to choose from different voices for the AI to use when generating audio from text.
+- **/intro**: Sets a new text for the chat intro.
 
-- **/provider**: Sets a new chat provider. This command allows users to switch between different providers for various functionalities, such as `phind`, `llama2`, `koboldai` etc.
+- **/voice**: Choose how the AI's voice sounds when it reads out text.
 
-- **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of them.
+- **/provider**: Switch between different AI providers for various features.
 
-- **/history**: Provides users with the ability to view the history of their chats with the bot. This command is useful for reviewing past interactions or finding specific information from previous conversations.
+- **/awesome**: Browse through a selection of cool chat intros.
 
-- **/check**: Offers an overview of the bot's current configuration, including any custom settings applied by the user.
+- **/history**: See past conversations with the bot.
 
-- **/reset**: Resets the chat history and starts a new conversation thread. This command is useful for users who wish to start fresh or clear their chat history for privacy reasons.
+- **/check**: See what settings are currently active for your bot.
 
-- **/myid**: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for various purposes, such as setting up bot admin.
+- **/reset**: Start a new conversation from scratch.
 
-- **/suspend**: Pauses the bot's service temporarily. This command is useful for channel administrators who need to temporarily halt the bot's operations without deleting its data or settings. It's a way to manage the bot's availability based on operational needs.
+- **/myid**: Find out your Telegram ID.
 
-- **/resume**: Resumes the bot's service after it has been suspended. This command allows administrators to quickly bring the bot back online after a pause, ensuring that users can continue interacting with the bot without interruption.
+- **/suspend**: Temporarily stop the bot from responding.
+
+- **/resume**: Restart the bot after it's been suspended.
+
+- **Any other text**: Just type anything to continue chatting.
+
+### Administrative Commands
+
+- **/clear**: Remove all chat data from the bot's database. Be careful with this one!
+
+- **/total**: See how many chats the bot has had.
+
+- **/drop**: Delete everything from the chat table and bot logs. This is more extreme than `/clear`.
+
+- **/sql**: Run SQL queries on the bot's database. Use this with caution!
+
+- **/logs**: Check the bot's logs for activity, errors, and user interactions.
 
 - `any other text`: An alias for `/chat`, allowing users to continue with chatting.
 
+> [!TIP]
+> For a better understanding of these commands, try interacting with a running bot from [@pytgpt_bot](https://t.me/pytgpt_bot). This can give you a practical idea of how the bot works and how to use it effectively.
 
 ### Administrative Commands
 
-- `/clear`: Clears all chats. This command is used to remove all chat data from the bot's database. It's a powerful command that should be used with caution, as it will delete all chat history.
+To make the administrative commands more understandable, let's simplify the descriptions and provide a bit more context for each command. This should help administrators manage the bot more effectively.
+
+### Simplified Administrative Commands
+
+- **/clear**: Use this command to remove all chat data from the bot's database. It's a powerful tool, so use it carefully to avoid losing important data.
+
+- **/total**: This command shows you the total number of chats the bot has handled. It's a quick way to see how much interaction the bot has had.
+
+- **/drop**: If you need to completely wipe out all chat data and logs, use this command. It's more extreme than `/clear` and should be used with caution to avoid losing all data.
+
+- **/sql**: Want to directly interact with the bot's database? This command lets you run SQL queries. It's a powerful feature for managing and analyzing data, but be cautious to avoid mistakes.
 
-- `/total`: Shows the total number of chats available. This command provides an overview of the current chat data stored in the bot's database, helping administrators understand the volume of interactions the bot has had.
+- **/logs**: This command gives you access to the bot's logs. It's useful for monitoring the bot's activity, spotting errors, and understanding user interactions.
 
-- `/drop`: Clears the entire chat table and bot logs. Similar to `/clear`, this command removes all data from the chat table in the database. It's a more drastic measure than `/clear`, as it completely wipes out all chat data and current contents of log file.
+> [!IMPORTANT]
+> Administrative commands are restricted to the users whose Telegram IDs are specified in the [.env](https://github.com/Simatwa/pytgpt-bot/blob/308f6079d153a429c445649896840fdc7cbfac11/env#L12) file.
 
-- `/sql`: Allows running SQL statements against the database. This command provides a way for administrators to directly interact with the bot's database using SQL queries. It's a powerful tool for managing and analyzing the bot's data but should be used with caution to avoid unintended data loss or corruption.
+## Further Tips
 
-- `/logs`: Checks the logs. This command is used to access the bot's logs, which can provide insights into the bot's activity, errors, and user interactions. It's a valuable tool for monitoring and troubleshooting the bot's performance.
+- The bot features inline query for text generation. The query must end with *three ellipsis* `...`. Remember to enable the mode from [@BotFather](https://t.me/pytgpt_bot). `/setinline`
+- You can as well add the bot to a Telegram channel. Grant it read and delete permissions. The access commands will still work out. `@bot_username <text>` will trigger **text generation**.
+- Channel Admin will control the bot access using the `/suspend` and `/resume` commands. *(Experimental).*
 
 ## Support and Feedback
 
 If you have any questions, feedback, or suggestions for `pytgpt`, please feel free to reach out. Your input is valuable in helping us improve and expand the bot's capabilities.
 
 ## License
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.2 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.3 Summary: Telegram bot for
 chatting, text-to-image and text-to-speech conversions Home-page: https://
 github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
 pytgpt-bot/releases Project-URL: Documentation, https://github.com/Simatwa/
 pytgpt-bot/blob/main/README.md Keywords:
-ai,tgpt,pytgpt,chatbot,telegrambot,pytelegrambot,chatbot,text-to-audio,text-to-
-image Classifier: License :: OSI Approved :: MIT License Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Developers Classifier:
-Natural Language :: English Classifier: License :: Free For Home Use
-Classifier: Intended Audience :: Customer Service Classifier: Programming
+ai,tgpt,pytgpt,chatbot,telegrambot,pytelegrambot,chatbot,text-to-speech,text-
+to-image Classifier: License :: OSI Approved :: MIT License Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English Classifier: License :: Free For Home
+Use Classifier: Intended Audience :: Customer Service Classifier: Programming
 Language :: Python Classifier: Topic :: Software Development :: Libraries ::
 Python Modules Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
@@ -36,66 +36,63 @@
 [Python>=3.10](https://python.org) ## Installation 1. From Source Clone repo
 and install. ```bash git clone https://github.com/Simatwa/pytgpt-bot.git cd
 pytgpt-bot pip install . ``` 2. From Pypi *(recommended)* ```sh pip install
 pytgpt-bot ``` ## Usage Before getting started, ensure you've your Telegram bot
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
 file as per the needs and then rename it `.env` before firing up the bot
-`python3 run.py`. Alternatively, using CLI: `$ pytgpt-bot run ` ## Features -
-**/start**: Displays the help information, offering a comprehensive list of
-available commands and their functionalities. This command is essential for
-users to quickly understand how to interact with the bot. - **/chat**: Initiate
-a natural language conversation with the AI. This command allows users to
-engage in interactive dialogues, ask questions, or make requests. - **/image**:
-Generates images from textual descriptions using the default provider. This
-feature enables users to visualize ideas or concepts through images. - **/
-prodia**: Generates images from textual descriptions using the Prodia provider.
-This command offers a unique style or interpretation of the text descriptions
-compared to the default method. - **/speak**: Converts text to speech,
-providing users with the ability to listen to descriptions, instructions, or
-any text content read out by the AI. - **/intro**: Sets a new text for the chat
-intro. This command allows users to customize the chat introductory prompt
-which serves as a guide in the human-AI engagement. - **/voice**: Sets a new
-voice for speech synthesis. This command enables users to choose from different
-voices for the AI to use when generating audio from text. - **/provider**: Sets
-a new chat provider. This command allows users to switch between different
-providers for various functionalities, such as `phind`, `llama2`, `koboldai`
-etc. - **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of
-them. - **/history**: Provides users with the ability to view the history of
-their chats with the bot. This command is useful for reviewing past
-interactions or finding specific information from previous conversations. - **/
-check**: Offers an overview of the bot's current configuration, including any
-custom settings applied by the user. - **/reset**: Resets the chat history and
-starts a new conversation thread. This command is useful for users who wish to
-start fresh or clear their chat history for privacy reasons. - **/myid**:
-Echoes the user's Telegram ID. This command is useful for users who need to
-know their Telegram ID for various purposes, such as setting up bot admin. -
-**/suspend**: Pauses the bot's service temporarily. This command is useful for
-channel administrators who need to temporarily halt the bot's operations
-without deleting its data or settings. It's a way to manage the bot's
-availability based on operational needs. - **/resume**: Resumes the bot's
-service after it has been suspended. This command allows administrators to
-quickly bring the bot back online after a pause, ensuring that users can
-continue interacting with the bot without interruption. - `any other text`: An
-alias for `/chat`, allowing users to continue with chatting. ### Administrative
-Commands - `/clear`: Clears all chats. This command is used to remove all chat
-data from the bot's database. It's a powerful command that should be used with
-caution, as it will delete all chat history. - `/total`: Shows the total number
-of chats available. This command provides an overview of the current chat data
-stored in the bot's database, helping administrators understand the volume of
-interactions the bot has had. - `/drop`: Clears the entire chat table and bot
-logs. Similar to `/clear`, this command removes all data from the chat table in
-the database. It's a more drastic measure than `/clear`, as it completely wipes
-out all chat data and current contents of log file. - `/sql`: Allows running
-SQL statements against the database. This command provides a way for
-administrators to directly interact with the bot's database using SQL queries.
-It's a powerful tool for managing and analyzing the bot's data but should be
-used with caution to avoid unintended data loss or corruption. - `/logs`:
-Checks the logs. This command is used to access the bot's logs, which can
-provide insights into the bot's activity, errors, and user interactions. It's a
-valuable tool for monitoring and troubleshooting the bot's performance. ##
-Support and Feedback If you have any questions, feedback, or suggestions for
+`python3 run.py`. Alternatively, using CLI: `$ pytgpt-bot run ` ## Features ###
+Access Commands - **/start**: This command shows you how to use the bot. It's
+like a guidebook for all the commands and what they do. - **/chat**: Use this
+to talk to the AI. You can ask questions, make requests, or just chat about
+anything. - **/image**: Want to see what something looks like? Type a
+description, and this command will create an image for you. - **/prodia**:
+Similar to `/image`, but it gives you a different style of image. - **/speak**:
+If you prefer listening to text instead of reading it, use this command to have
+the AI read out text for you. - **/intro**: Sets a new text for the chat intro.
+- **/voice**: Choose how the AI's voice sounds when it reads out text. - **/
+provider**: Switch between different AI providers for various features. - **/
+awesome**: Browse through a selection of cool chat intros. - **/history**: See
+past conversations with the bot. - **/check**: See what settings are currently
+active for your bot. - **/reset**: Start a new conversation from scratch. - **/
+myid**: Find out your Telegram ID. - **/suspend**: Temporarily stop the bot
+from responding. - **/resume**: Restart the bot after it's been suspended. -
+**Any other text**: Just type anything to continue chatting. ### Administrative
+Commands - **/clear**: Remove all chat data from the bot's database. Be careful
+with this one! - **/total**: See how many chats the bot has had. - **/drop**:
+Delete everything from the chat table and bot logs. This is more extreme than
+`/clear`. - **/sql**: Run SQL queries on the bot's database. Use this with
+caution! - **/logs**: Check the bot's logs for activity, errors, and user
+interactions. - `any other text`: An alias for `/chat`, allowing users to
+continue with chatting. > [!TIP] > For a better understanding of these
+commands, try interacting with a running bot from [@pytgpt_bot](https://t.me/
+pytgpt_bot). This can give you a practical idea of how the bot works and how to
+use it effectively. ### Administrative Commands To make the administrative
+commands more understandable, let's simplify the descriptions and provide a bit
+more context for each command. This should help administrators manage the bot
+more effectively. ### Simplified Administrative Commands - **/clear**: Use this
+command to remove all chat data from the bot's database. It's a powerful tool,
+so use it carefully to avoid losing important data. - **/total**: This command
+shows you the total number of chats the bot has handled. It's a quick way to
+see how much interaction the bot has had. - **/drop**: If you need to
+completely wipe out all chat data and logs, use this command. It's more extreme
+than `/clear` and should be used with caution to avoid losing all data. - **/
+sql**: Want to directly interact with the bot's database? This command lets you
+run SQL queries. It's a powerful feature for managing and analyzing data, but
+be cautious to avoid mistakes. - **/logs**: This command gives you access to
+the bot's logs. It's useful for monitoring the bot's activity, spotting errors,
+and understanding user interactions. > [!IMPORTANT] > Administrative commands
+are restricted to the users whose Telegram IDs are specified in the [.env]
+(https://github.com/Simatwa/pytgpt-bot/blob/
+308f6079d153a429c445649896840fdc7cbfac11/env#L12) file. ## Further Tips - The
+bot features inline query for text generation. The query must end with *three
+ellipsis* `...`. Remember to enable the mode from [@BotFather](https://t.me/
+pytgpt_bot). `/setinline` - You can as well add the bot to a Telegram channel.
+Grant it read and delete permissions. The access commands will still work out.
+`@bot_username ` will trigger **text generation**. - Channel Admin will control
+the bot access using the `/suspend` and `/resume` commands. *(Experimental).*
+## Support and Feedback If you have any questions, feedback, or suggestions for
 `pytgpt`, please feel free to reach out. Your input is valuable in helping us
 improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
 source and available under the [MIT License](LICENSE). Feel free to use,
 modify, and distribute the code as you see fit. --- Thank you for using
 `pytgpt-bot`. Enjoy your AI-powered interactions!
```

### Comparing `pytgpt_bot-0.1.2/README.md` & `pytgpt_bot-0.1.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -47,58 +47,89 @@
 
 Alternatively, using CLI:
 
    `$ pytgpt-bot run <Your Telegram Token>`
 
 ## Features
 
-- **/start**: Displays the help information, offering a comprehensive list of available commands and their functionalities. This command is essential for users to quickly understand how to interact with the bot.
+### Access Commands
 
-- **/chat**: Initiate a natural language conversation with the AI. This command allows users to engage in interactive dialogues, ask questions, or make requests.
+- **/start**: This command shows you how to use the bot. It's like a guidebook for all the commands and what they do.
 
-- **/image**: Generates images from textual descriptions using the default provider. This feature enables users to visualize ideas or concepts through images.
+- **/chat**: Use this to talk to the AI. You can ask questions, make requests, or just chat about anything.
 
-- **/prodia**: Generates images from textual descriptions using the Prodia provider. This command offers a unique style or interpretation of the text descriptions compared to the default method.
+- **/image**: Want to see what something looks like? Type a description, and this command will create an image for you.
 
-- **/speak**: Converts text to speech, providing users with the ability to listen to descriptions, instructions, or any text content read out by the AI.
+- **/prodia**: Similar to `/image`, but it gives you a different style of image.
 
-- **/intro**: Sets a new text for the chat intro. This command allows users to customize the chat introductory prompt which serves as a guide in the human-AI engagement.
+- **/speak**: If you prefer listening to text instead of reading it, use this command to have the AI read out text for you.
 
-- **/voice**: Sets a new voice for speech synthesis. This command enables users to choose from different voices for the AI to use when generating audio from text.
+- **/intro**: Sets a new text for the chat intro.
 
-- **/provider**: Sets a new chat provider. This command allows users to switch between different providers for various functionalities, such as `phind`, `llama2`, `koboldai` etc.
+- **/voice**: Choose how the AI's voice sounds when it reads out text.
 
-- **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of them.
+- **/provider**: Switch between different AI providers for various features.
 
-- **/history**: Provides users with the ability to view the history of their chats with the bot. This command is useful for reviewing past interactions or finding specific information from previous conversations.
+- **/awesome**: Browse through a selection of cool chat intros.
 
-- **/check**: Offers an overview of the bot's current configuration, including any custom settings applied by the user.
+- **/history**: See past conversations with the bot.
 
-- **/reset**: Resets the chat history and starts a new conversation thread. This command is useful for users who wish to start fresh or clear their chat history for privacy reasons.
+- **/check**: See what settings are currently active for your bot.
 
-- **/myid**: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for various purposes, such as setting up bot admin.
+- **/reset**: Start a new conversation from scratch.
 
-- **/suspend**: Pauses the bot's service temporarily. This command is useful for channel administrators who need to temporarily halt the bot's operations without deleting its data or settings. It's a way to manage the bot's availability based on operational needs.
+- **/myid**: Find out your Telegram ID.
 
-- **/resume**: Resumes the bot's service after it has been suspended. This command allows administrators to quickly bring the bot back online after a pause, ensuring that users can continue interacting with the bot without interruption.
+- **/suspend**: Temporarily stop the bot from responding.
+
+- **/resume**: Restart the bot after it's been suspended.
+
+- **Any other text**: Just type anything to continue chatting.
+
+### Administrative Commands
+
+- **/clear**: Remove all chat data from the bot's database. Be careful with this one!
+
+- **/total**: See how many chats the bot has had.
+
+- **/drop**: Delete everything from the chat table and bot logs. This is more extreme than `/clear`.
+
+- **/sql**: Run SQL queries on the bot's database. Use this with caution!
+
+- **/logs**: Check the bot's logs for activity, errors, and user interactions.
 
 - `any other text`: An alias for `/chat`, allowing users to continue with chatting.
 
+> [!TIP]
+> For a better understanding of these commands, try interacting with a running bot from [@pytgpt_bot](https://t.me/pytgpt_bot). This can give you a practical idea of how the bot works and how to use it effectively.
 
 ### Administrative Commands
 
-- `/clear`: Clears all chats. This command is used to remove all chat data from the bot's database. It's a powerful command that should be used with caution, as it will delete all chat history.
+To make the administrative commands more understandable, let's simplify the descriptions and provide a bit more context for each command. This should help administrators manage the bot more effectively.
+
+### Simplified Administrative Commands
+
+- **/clear**: Use this command to remove all chat data from the bot's database. It's a powerful tool, so use it carefully to avoid losing important data.
+
+- **/total**: This command shows you the total number of chats the bot has handled. It's a quick way to see how much interaction the bot has had.
+
+- **/drop**: If you need to completely wipe out all chat data and logs, use this command. It's more extreme than `/clear` and should be used with caution to avoid losing all data.
+
+- **/sql**: Want to directly interact with the bot's database? This command lets you run SQL queries. It's a powerful feature for managing and analyzing data, but be cautious to avoid mistakes.
 
-- `/total`: Shows the total number of chats available. This command provides an overview of the current chat data stored in the bot's database, helping administrators understand the volume of interactions the bot has had.
+- **/logs**: This command gives you access to the bot's logs. It's useful for monitoring the bot's activity, spotting errors, and understanding user interactions.
 
-- `/drop`: Clears the entire chat table and bot logs. Similar to `/clear`, this command removes all data from the chat table in the database. It's a more drastic measure than `/clear`, as it completely wipes out all chat data and current contents of log file.
+> [!IMPORTANT]
+> Administrative commands are restricted to the users whose Telegram IDs are specified in the [.env](https://github.com/Simatwa/pytgpt-bot/blob/308f6079d153a429c445649896840fdc7cbfac11/env#L12) file.
 
-- `/sql`: Allows running SQL statements against the database. This command provides a way for administrators to directly interact with the bot's database using SQL queries. It's a powerful tool for managing and analyzing the bot's data but should be used with caution to avoid unintended data loss or corruption.
+## Further Tips
 
-- `/logs`: Checks the logs. This command is used to access the bot's logs, which can provide insights into the bot's activity, errors, and user interactions. It's a valuable tool for monitoring and troubleshooting the bot's performance.
+- The bot features inline query for text generation. The query must end with *three ellipsis* `...`. Remember to enable the mode from [@BotFather](https://t.me/pytgpt_bot). `/setinline`
+- You can as well add the bot to a Telegram channel. Grant it read and delete permissions. The access commands will still work out. `@bot_username <text>` will trigger **text generation**.
+- Channel Admin will control the bot access using the `/suspend` and `/resume` commands. *(Experimental).*
 
 ## Support and Feedback
 
 If you have any questions, feedback, or suggestions for `pytgpt`, please feel free to reach out. Your input is valuable in helping us improve and expand the bot's capabilities.
 
 ## License
```

#### html2text {}

```diff
@@ -11,66 +11,63 @@
 [Python>=3.10](https://python.org) ## Installation 1. From Source Clone repo
 and install. ```bash git clone https://github.com/Simatwa/pytgpt-bot.git cd
 pytgpt-bot pip install . ``` 2. From Pypi *(recommended)* ```sh pip install
 pytgpt-bot ``` ## Usage Before getting started, ensure you've your Telegram bot
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
 file as per the needs and then rename it `.env` before firing up the bot
-`python3 run.py`. Alternatively, using CLI: `$ pytgpt-bot run ` ## Features -
-**/start**: Displays the help information, offering a comprehensive list of
-available commands and their functionalities. This command is essential for
-users to quickly understand how to interact with the bot. - **/chat**: Initiate
-a natural language conversation with the AI. This command allows users to
-engage in interactive dialogues, ask questions, or make requests. - **/image**:
-Generates images from textual descriptions using the default provider. This
-feature enables users to visualize ideas or concepts through images. - **/
-prodia**: Generates images from textual descriptions using the Prodia provider.
-This command offers a unique style or interpretation of the text descriptions
-compared to the default method. - **/speak**: Converts text to speech,
-providing users with the ability to listen to descriptions, instructions, or
-any text content read out by the AI. - **/intro**: Sets a new text for the chat
-intro. This command allows users to customize the chat introductory prompt
-which serves as a guide in the human-AI engagement. - **/voice**: Sets a new
-voice for speech synthesis. This command enables users to choose from different
-voices for the AI to use when generating audio from text. - **/provider**: Sets
-a new chat provider. This command allows users to switch between different
-providers for various functionalities, such as `phind`, `llama2`, `koboldai`
-etc. - **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of
-them. - **/history**: Provides users with the ability to view the history of
-their chats with the bot. This command is useful for reviewing past
-interactions or finding specific information from previous conversations. - **/
-check**: Offers an overview of the bot's current configuration, including any
-custom settings applied by the user. - **/reset**: Resets the chat history and
-starts a new conversation thread. This command is useful for users who wish to
-start fresh or clear their chat history for privacy reasons. - **/myid**:
-Echoes the user's Telegram ID. This command is useful for users who need to
-know their Telegram ID for various purposes, such as setting up bot admin. -
-**/suspend**: Pauses the bot's service temporarily. This command is useful for
-channel administrators who need to temporarily halt the bot's operations
-without deleting its data or settings. It's a way to manage the bot's
-availability based on operational needs. - **/resume**: Resumes the bot's
-service after it has been suspended. This command allows administrators to
-quickly bring the bot back online after a pause, ensuring that users can
-continue interacting with the bot without interruption. - `any other text`: An
-alias for `/chat`, allowing users to continue with chatting. ### Administrative
-Commands - `/clear`: Clears all chats. This command is used to remove all chat
-data from the bot's database. It's a powerful command that should be used with
-caution, as it will delete all chat history. - `/total`: Shows the total number
-of chats available. This command provides an overview of the current chat data
-stored in the bot's database, helping administrators understand the volume of
-interactions the bot has had. - `/drop`: Clears the entire chat table and bot
-logs. Similar to `/clear`, this command removes all data from the chat table in
-the database. It's a more drastic measure than `/clear`, as it completely wipes
-out all chat data and current contents of log file. - `/sql`: Allows running
-SQL statements against the database. This command provides a way for
-administrators to directly interact with the bot's database using SQL queries.
-It's a powerful tool for managing and analyzing the bot's data but should be
-used with caution to avoid unintended data loss or corruption. - `/logs`:
-Checks the logs. This command is used to access the bot's logs, which can
-provide insights into the bot's activity, errors, and user interactions. It's a
-valuable tool for monitoring and troubleshooting the bot's performance. ##
-Support and Feedback If you have any questions, feedback, or suggestions for
+`python3 run.py`. Alternatively, using CLI: `$ pytgpt-bot run ` ## Features ###
+Access Commands - **/start**: This command shows you how to use the bot. It's
+like a guidebook for all the commands and what they do. - **/chat**: Use this
+to talk to the AI. You can ask questions, make requests, or just chat about
+anything. - **/image**: Want to see what something looks like? Type a
+description, and this command will create an image for you. - **/prodia**:
+Similar to `/image`, but it gives you a different style of image. - **/speak**:
+If you prefer listening to text instead of reading it, use this command to have
+the AI read out text for you. - **/intro**: Sets a new text for the chat intro.
+- **/voice**: Choose how the AI's voice sounds when it reads out text. - **/
+provider**: Switch between different AI providers for various features. - **/
+awesome**: Browse through a selection of cool chat intros. - **/history**: See
+past conversations with the bot. - **/check**: See what settings are currently
+active for your bot. - **/reset**: Start a new conversation from scratch. - **/
+myid**: Find out your Telegram ID. - **/suspend**: Temporarily stop the bot
+from responding. - **/resume**: Restart the bot after it's been suspended. -
+**Any other text**: Just type anything to continue chatting. ### Administrative
+Commands - **/clear**: Remove all chat data from the bot's database. Be careful
+with this one! - **/total**: See how many chats the bot has had. - **/drop**:
+Delete everything from the chat table and bot logs. This is more extreme than
+`/clear`. - **/sql**: Run SQL queries on the bot's database. Use this with
+caution! - **/logs**: Check the bot's logs for activity, errors, and user
+interactions. - `any other text`: An alias for `/chat`, allowing users to
+continue with chatting. > [!TIP] > For a better understanding of these
+commands, try interacting with a running bot from [@pytgpt_bot](https://t.me/
+pytgpt_bot). This can give you a practical idea of how the bot works and how to
+use it effectively. ### Administrative Commands To make the administrative
+commands more understandable, let's simplify the descriptions and provide a bit
+more context for each command. This should help administrators manage the bot
+more effectively. ### Simplified Administrative Commands - **/clear**: Use this
+command to remove all chat data from the bot's database. It's a powerful tool,
+so use it carefully to avoid losing important data. - **/total**: This command
+shows you the total number of chats the bot has handled. It's a quick way to
+see how much interaction the bot has had. - **/drop**: If you need to
+completely wipe out all chat data and logs, use this command. It's more extreme
+than `/clear` and should be used with caution to avoid losing all data. - **/
+sql**: Want to directly interact with the bot's database? This command lets you
+run SQL queries. It's a powerful feature for managing and analyzing data, but
+be cautious to avoid mistakes. - **/logs**: This command gives you access to
+the bot's logs. It's useful for monitoring the bot's activity, spotting errors,
+and understanding user interactions. > [!IMPORTANT] > Administrative commands
+are restricted to the users whose Telegram IDs are specified in the [.env]
+(https://github.com/Simatwa/pytgpt-bot/blob/
+308f6079d153a429c445649896840fdc7cbfac11/env#L12) file. ## Further Tips - The
+bot features inline query for text generation. The query must end with *three
+ellipsis* `...`. Remember to enable the mode from [@BotFather](https://t.me/
+pytgpt_bot). `/setinline` - You can as well add the bot to a Telegram channel.
+Grant it read and delete permissions. The access commands will still work out.
+`@bot_username ` will trigger **text generation**. - Channel Admin will control
+the bot access using the `/suspend` and `/resume` commands. *(Experimental).*
+## Support and Feedback If you have any questions, feedback, or suggestions for
 `pytgpt`, please feel free to reach out. Your input is valuable in helping us
 improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
 source and available under the [MIT License](LICENSE). Feel free to use,
 modify, and distribute the code as you see fit. --- Thank you for using
 `pytgpt-bot`. Enjoy your AI-powered interactions!
```

### Comparing `pytgpt_bot-0.1.2/pytgpt_bot/cli.py` & `pytgpt_bot-0.1.3/pytgpt_bot/cli.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.2/pytgpt_bot/config.py` & `pytgpt_bot-0.1.3/pytgpt_bot/config.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.2/pytgpt_bot/db.py` & `pytgpt_bot-0.1.3/pytgpt_bot/db.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.2/pytgpt_bot/filters.py` & `pytgpt_bot-0.1.3/pytgpt_bot/filters.py`

 * *Files identical despite different names*

### Comparing `pytgpt_bot-0.1.2/pytgpt_bot/main.py` & `pytgpt_bot-0.1.3/pytgpt_bot/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 )
 from pytgpt_bot.db import User
 from pytgpt_bot.utils import (
     provider_keys,
     get_random_emoji,
     provider_map,
     make_delete_markup,
+    make_regenerate_and_delete_markup,
 )
 from pytgpt_bot.models import session, Chat, create_all, drop_all
 from pytgpt_bot.filters import (
     IsActiveFilter,
     IsBotOwnerFilter,
     IsAdminFilter,
     IsBotTaggedFilter,
@@ -94,15 +95,15 @@
     "/total : Total chats available 📊\n"
     "/drop : Clear entire chat table and bot logs 🗑️\n"
     "/sql : Run sql statements against database ⏳\n"
     "/logs : View bot logs 📜"
 )
 
 
-def handler_formatter(text: bool = False, admin: bool = False, preserve: bool = False):
+def handler_formatter(text: bool = False, preserve: bool = False):
     """Handles common message handler verification and execptions
 
     Args:
         text (bool, optional): Command must contain text?. Defaults to False.
         admin (bool, optional): Needs admin privileges?. Defaults to False.
         preserve (bool, optional): Do not alter text?. Default to False.
     """
@@ -126,16 +127,18 @@
                         message,
                         f"{get_random_emoji()} Text is required❗️❗️.",
                         reply_markup=make_delete_markup(message),
                     )
 
                 return func(message)
             except Exception as e:
-                logging.exception(e)
-                logging.error(f"Error on function - {func.__name__} - {e}")
+                # logging.exception(e)
+                logging.error(
+                    f"Error on function - {func.__name__} - {e.args[1] if e.args and len(e.args)>1 else e}"
+                )
                 logging.debug(str(e))
                 bot.reply_to(
                     message,
                     text=f"{get_random_emoji('angry')} An error occured and I could't complete that request ❗️❗️❗️",
                     reply_markup=make_delete_markup(message),
                 )
 
@@ -171,29 +174,38 @@
     )
 
 
 def send_long_text(
     message: telebot.types.Message,
     text: str,
     add_delete: bool = False,
-    parse_mode="Markdown",
+    parse_mode: str = "Markdown",
+    as_reply: bool = False,
 ):
     """Send texts longer than 4096 long
 
     Args:
         message (telebot.types.Message): Message object.
         text (str): Text to be sent.
         add_delete (bool). Add delete button. Defaults to False.
         parse_mode (str): __. Defaults to Markdown.
+        as_reply (bool). Highlight the user message. Default to False.
     """
-    take_action = send_and_add_delete_button if add_delete else bot.send_message
-    for part in telebot_util.smart_split(text):
-        take_action(
-            message if add_delete else message.chat.id, part, parse_mode=parse_mode
-        )
+    parts: list = telebot_util.smart_split(text)
+    if add_delete:
+        for part in parts:
+            send_and_add_delete_button(
+                message, part, parse_mode=parse_mode, as_reply=as_reply
+            )
+    else:
+        for part in parts:
+            if as_reply:
+                bot.reply_to(message, part, parse_mode=parse_mode)
+            else:
+                bot.send_message(message.chat.id, part, parse_mode=parse_mode)
 
 
 @bot.message_handler(commands=["help", "start"], is_chat_active=True)
 @bot.channel_post_handler(commands=["help", "start"], is_chat_active=True)
 @handler_formatter()
 def home(message: telebot.types.Message):
     """Show help"""
@@ -254,15 +266,15 @@
         reply_markup=markup,
     )
 
 
 @bot.callback_query_handler(
     func=lambda call: call.data.split(":")[0] in audio_generator.all_voices
 )
-def set_new_speech_voice_callback(call: telebot.types.CallbackQuery):
+def set_new_speech_voice_callback_handler(call: telebot.types.CallbackQuery):
     """Set new voice for speech synthesis callback handler"""
     bot.delete_message(call.message.chat.id, call.message.id)
     voice, user_id = call.data.split(":")
     message = call.message
     markup = make_delete_markup(call.message)
     user = User(user_id=int(user_id))
     user.chat.voice = voice
@@ -273,15 +285,15 @@
         parse_mode="Markdown",
     )
 
 
 @bot.message_handler(commands=["provider"], is_chat_admin=True)
 @bot.channel_post_handler(commands=["provider"], is_chat_admin=True)
 @handler_formatter(text=False)
-def set_new_text_provider(message: telebot.types.Message):
+def set_new_chat_provider(message: telebot.types.Message):
     """Set new text provider"""
     user_id: str = message.from_user.id
     markup = telebot.types.InlineKeyboardMarkup(row_width=2)
     make_item = lambda provider: telebot.types.InlineKeyboardButton(
         provider, callback_data=f"{provider}:{user_id}"
     )
     markup.add(*map(make_item, provider_keys))
@@ -290,15 +302,15 @@
         message.chat.id,
         f"Choose a provider {get_random_emoji('love')}:",
         reply_markup=markup,
     )
 
 
 @bot.callback_query_handler(func=lambda call: call.data.split(":")[0] in provider_keys)
-def set_new_text_provider_callback(call: telebot.types.CallbackQuery):
+def set_new_chat_provider_callback_handler(call: telebot.types.CallbackQuery):
     """Set new text provider callback handler"""
     bot.delete_message(call.message.chat.id, call.message.id)
     provider, user_id = call.data.split(":")
     message = call.message
     markup = make_delete_markup(call.message)
     user = User(user_id=int(user_id))
     user.chat.provider = provider
@@ -378,70 +390,91 @@
         message,
         user.chat.history or f"{get_random_emoji()} Your chat history is empty ❗️",
         add_delete=True,
         parse_mode="Markdown",
     )
 
 
-@bot.message_handler(commands=["image", "img"], is_chat_active=True)
-@bot.channel_post_handler(commands=["image", "img"], is_chat_active=True)
-@handler_formatter(text=True)
 def text_to_image_default(message: telebot.types.Message):
-    """Generate image using `image`"""
+    """Shared obj : Generate image using `image`"""
     bot.send_chat_action(message.chat.id, "upload_photo", timeout=timeout)
     generator_obj = image_generator.Imager(
         timeout=timeout,
     )
     return bot.send_photo(
         message.chat.id,
         photo=generator_obj.generate(
             message.text,
         )[0],
-        caption=message.text,
-        reply_markup=make_delete_markup(message),
+        caption=message.text + " (default)",
+        reply_markup=make_regenerate_and_delete_markup(
+            message, provider="default", prompt=message.text
+        ),
     )
 
 
-@bot.message_handler(commands=["prodia", "prod"], is_chat_active=True)
-@bot.channel_post_handler(commands=["prodia", "prod"], is_chat_active=True)
+@bot.message_handler(commands=["image", "img"], is_chat_active=True)
+@bot.channel_post_handler(commands=["image", "img"], is_chat_active=True)
 @handler_formatter(text=True)
+def text_to_image_default_handler(message: telebot.types.Message):
+    """Handler for image generation - default"""
+    text_to_image_default(message)
+
+
 def text_to_image_prodia(message: telebot.types.Message):
-    """Generate image using `prodia`"""
+    """Shared obj : Generate image using `prodia` and respond"""
     bot.send_chat_action(message.chat.id, "upload_photo", timeout=timeout)
     generator_obj = image_generator.Prodia(timeout=timeout)
     return bot.send_photo(
         message.chat.id,
         photo=generator_obj.generate(message.text)[0],
-        caption=message.text,
-        reply_markup=make_delete_markup(message),
+        caption=message.text + " (prodia)",
+        reply_markup=make_regenerate_and_delete_markup(
+            message, provider="prodia", prompt=message.text
+        ),
     )
 
 
-@bot.message_handler(commands=["speak", "spe"], is_chat_active=True)
-@bot.channel_post_handler(commands=["speak", "spe"], is_chat_active=True)
+@bot.message_handler(commands=["prodia", "prod"], is_chat_active=True)
+@bot.channel_post_handler(commands=["prodia", "prod"], is_chat_active=True)
 @handler_formatter(text=True)
-def text_to_audio(message: telebot.types.Message):
-    """Convert text to audio"""
+def text_to_image_prodia_handler(message: telebot.types.Message):
+    """Handler for text to image"""
+    text_to_image_prodia(message)
+
+
+def text_to_speech(message: telebot.types.Message):
+    """Shared obj : Convert text to speech and respond"""
     bot.send_chat_action(message.chat.id, "upload_audio", timeout=timeout)
     voice = User(message).chat.voice
     audio_chunk = audio_generator.text_to_audio(
         message=message.text,
         voice=voice,
         timeout=timeout,
     )
     return bot.send_audio(
         message.chat.id,
         audio=audio_chunk,
         caption=message.text,
-        reply_markup=make_delete_markup(message),
+        reply_markup=make_regenerate_and_delete_markup(
+            message, provider="speech", prompt=message.text
+        ),
         performer=voice,
         title="Text-to-Speech",
     )
 
 
+@bot.message_handler(commands=["speak", "spe"], is_chat_active=True)
+@bot.channel_post_handler(commands=["speak", "spe"], is_chat_active=True)
+@handler_formatter(text=True)
+def text_to_speech_handler(message: telebot.types.Message):
+    """Handler for text to speech"""
+    text_to_speech(message)
+
+
 @bot.message_handler(commands=["reset"], is_chat_admin=True, is_chat_active=True)
 @bot.channel_post_handler(commands=["reset"], is_chat_admin=True, is_chat_active=True)
 @handler_formatter()
 def reset_chat(message: telebot.types.Message):
     """Reset current chat thread"""
     user = User(message)
     user.delete()
@@ -471,45 +504,45 @@
     chat.is_active = True
     return bot.reply_to(
         message, text=f"Service Resumed 🚀.", reply_markup=make_delete_markup(message)
     )
 
 
 @bot.message_handler(commands=["clear", "clear_chats"], is_bot_owner=True)
-@handler_formatter(admin=True)
+@handler_formatter()
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
 
 
 @bot.message_handler(commands=["total", "total_chats"], is_bot_owner=True)
-@handler_formatter(admin=True)
+@handler_formatter()
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
 
 
 @bot.message_handler(commands=["drop", "drop_chats"], is_bot_owner=True)
-@handler_formatter(admin=True)
+@handler_formatter()
 def total_chats_table_and_logs(message: telebot.types.Message):
     """Drop chat table and create new"""
     if logfile:
         with open(logfile, "w") as fh:
             fh.write(
                 f"ADMIN CLEARED LOGS & DROPPED CHAT TABLE [{message.from_user.id}] - ({message.from_user.full_name})\n"
             )
@@ -522,15 +555,15 @@
         message,
         f"{get_random_emoji('love')} Chat table and bot logs dropped and new one created.",
         reply_markup=make_delete_markup(message),
     )
 
 
 @bot.message_handler(commands=["sql"], is_bot_owner=True)
-@handler_formatter(admin=True, text=True)
+@handler_formatter(text=True)
 def run_sql_statement(message: telebot.types.Message):
     """Run sql statements against database"""
     logging.warning(
         f"Running SQL statements - [{message.from_user.full_name}] ({message.from_user.id}, {message.from_user.username})"
     )
     try:
         results = session.execute(text(message.text))
@@ -555,15 +588,15 @@
             message,
             response,
             add_delete=True,
         )
 
 
 @bot.message_handler(commands=["logs"], is_bot_owner=True)
-@handler_formatter(admin=True)
+@handler_formatter()
 def check_current_settings(message: telebot.types.Message):
     """View bot logs"""
     if not logfile:
         return bot.reply_to(
             message,
             f"{get_random_emoji()} Logfile not specified ❗️",
             reply_markup=make_delete_markup(message),
@@ -593,34 +626,85 @@
     ai_response = user_provider(is_conversation=False, timeout=timeout).chat(
         conversation_prompt
     )
     conversation.update_chat_history(
         prompt=message.text, response=ai_response, force=True
     )
     user.chat.history = conversation.chat_history
-    send_long_text(message, ai_response)
+    send_long_text(message, ai_response, as_reply=False if message.from_user else True)
+
+
+@bot.callback_query_handler(func=lambda call: call.data.startswith("media::"))
+def media_regeneration_callback_handler(
+    call: telebot.types.CallbackQuery,
+):
+    """Media regeneration callback handler"""
+    action, provider, prompt = call.data.split("::")
+    message = call.message
+    message.text = prompt
+    if provider == "prodia":
+        return text_to_image_prodia(message)
+    elif provider == "default":
+        return text_to_image_default(message)
+    elif provider == "speech":
+        return text_to_speech(message)
+
+
+@bot.inline_handler(lambda query: query.query.endswith("..."))
+def handle_inline_query(inline_query: telebot.types.InlineQuery):
+    """Process the inline query and return AI response"""
+    try:
+        logging.info("Serving INLINE-QUERY - [{inline_query.from_user.id}].")
+        prompt = inline_query.query[:-3]
+        user = User(user_id=inline_query.from_user.id)
+        conversation = Conversation(max_tokens=max_tokens)
+        user_provider = provider_map.get(user.chat.provider)
+        conversation_prompt = conversation.gen_complete_prompt(
+            prompt, intro=user.chat.intro
+        )
+        ai_response = user_provider(is_conversation=False, timeout=timeout).chat(
+            conversation_prompt
+        )
+        feedback_options = [
+            telebot.types.InlineQueryResultArticle(
+                id="1",
+                title=ai_response,  # "AI Generated",
+                input_message_content=telebot.types.InputTextMessageContent(
+                    ai_response
+                ),
+            )
+        ]
+        bot.answer_inline_query(inline_query.id, feedback_options)
+
+    except Exception as e:
+        logging.debug(
+            f"Error while handling inline query - [{inline_query.from_user.id}]. {e}"
+        )
+        logging.error(
+            f"Error while handling inline query - [{inline_query.from_user.id}] : {e.args[1] if e.args and len(e.args)>1 else e}"
+        )
 
 
 @bot.message_handler(is_chat_active=True)
 @bot.channel_post_handler(is_chat_active=True, is_bot_tagged=True)
 def any_other_action(message):
     return bot.reply_to(
         message,
         usage_info,
         reply_markup=make_delete_markup(message),
         parse_mode="Markdown",
     )
 
 
-@bot.callback_query_handler(func=lambda call: call.data.startswith("delete:"))
+@bot.callback_query_handler(func=lambda call: call.data.startswith("delete::"))
 def delete_callback_handler(
     call: telebot.types.CallbackQuery,
 ):
     """Delete callback handler"""
-    action, trigger_chat_id, trigger_message_id = call.data.split(":")
+    action, trigger_chat_id, trigger_message_id = call.data.split("::")
     try:
         bot.delete_message(trigger_chat_id, trigger_message_id)
     except:
         pass
     try:
         bot.delete_message(call.message.chat.id, call.message.id)
     except:
```

### Comparing `pytgpt_bot-0.1.2/pytgpt_bot/models.py` & `pytgpt_bot-0.1.3/pytgpt_bot/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from sqlalchemy import Column, Integer, Text, String, Boolean
 from pytgpt.utils import Conversation
 from pytgpt_bot.config import database as database_str
 from pytgpt_bot.config import provider as default_provider
 from pytgpt_bot.config import voice
 
 if not database_str:
-    from .utils import path_to_default_db
+    from pytgpt_bot.utils import path_to_default_db
 
     database_str: str = f"sqlite:///{path_to_default_db.as_posix()}"
 
 engine = create_engine(database_str)
 
 autocommit_engine = engine.execution_options(isolation_level="AUTOCOMMIT")
```

### Comparing `pytgpt_bot-0.1.2/pytgpt_bot.egg-info/PKG-INFO` & `pytgpt_bot-0.1.3/pytgpt_bot.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pytgpt-bot
-Version: 0.1.2
+Version: 0.1.3
 Summary: Telegram bot for chatting, text-to-image and text-to-speech conversions
 Home-page: https://github.com/Simatwa/pytgpt-bot
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/pytgpt-bot/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/pytgpt-bot
 Project-URL: Source Code, https://github.com/Simatwa/pytgpt-bot
 Project-URL: Issue Tracker, https://github.com/Simatwa/pytgpt-bot/issues
 Project-URL: Download, https://github.com/Simatwa/pytgpt-bot/releases
 Project-URL: Documentation, https://github.com/Simatwa/pytgpt-bot/blob/main/README.md
-Keywords: ai,tgpt,pytgpt,chatbot,telegrambot,pytelegrambot,chatbot,text-to-audio,text-to-image
+Keywords: ai,tgpt,pytgpt,chatbot,telegrambot,pytelegrambot,chatbot,text-to-speech,text-to-image
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: Free For Home Use
 Classifier: Intended Audience :: Customer Service
 Classifier: Programming Language :: Python
@@ -86,58 +86,89 @@
 
 Alternatively, using CLI:
 
    `$ pytgpt-bot run <Your Telegram Token>`
 
 ## Features
 
-- **/start**: Displays the help information, offering a comprehensive list of available commands and their functionalities. This command is essential for users to quickly understand how to interact with the bot.
+### Access Commands
 
-- **/chat**: Initiate a natural language conversation with the AI. This command allows users to engage in interactive dialogues, ask questions, or make requests.
+- **/start**: This command shows you how to use the bot. It's like a guidebook for all the commands and what they do.
 
-- **/image**: Generates images from textual descriptions using the default provider. This feature enables users to visualize ideas or concepts through images.
+- **/chat**: Use this to talk to the AI. You can ask questions, make requests, or just chat about anything.
 
-- **/prodia**: Generates images from textual descriptions using the Prodia provider. This command offers a unique style or interpretation of the text descriptions compared to the default method.
+- **/image**: Want to see what something looks like? Type a description, and this command will create an image for you.
 
-- **/speak**: Converts text to speech, providing users with the ability to listen to descriptions, instructions, or any text content read out by the AI.
+- **/prodia**: Similar to `/image`, but it gives you a different style of image.
 
-- **/intro**: Sets a new text for the chat intro. This command allows users to customize the chat introductory prompt which serves as a guide in the human-AI engagement.
+- **/speak**: If you prefer listening to text instead of reading it, use this command to have the AI read out text for you.
 
-- **/voice**: Sets a new voice for speech synthesis. This command enables users to choose from different voices for the AI to use when generating audio from text.
+- **/intro**: Sets a new text for the chat intro.
 
-- **/provider**: Sets a new chat provider. This command allows users to switch between different providers for various functionalities, such as `phind`, `llama2`, `koboldai` etc.
+- **/voice**: Choose how the AI's voice sounds when it reads out text.
 
-- **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of them.
+- **/provider**: Switch between different AI providers for various features.
 
-- **/history**: Provides users with the ability to view the history of their chats with the bot. This command is useful for reviewing past interactions or finding specific information from previous conversations.
+- **/awesome**: Browse through a selection of cool chat intros.
 
-- **/check**: Offers an overview of the bot's current configuration, including any custom settings applied by the user.
+- **/history**: See past conversations with the bot.
 
-- **/reset**: Resets the chat history and starts a new conversation thread. This command is useful for users who wish to start fresh or clear their chat history for privacy reasons.
+- **/check**: See what settings are currently active for your bot.
 
-- **/myid**: Echoes the user's Telegram ID. This command is useful for users who need to know their Telegram ID for various purposes, such as setting up bot admin.
+- **/reset**: Start a new conversation from scratch.
 
-- **/suspend**: Pauses the bot's service temporarily. This command is useful for channel administrators who need to temporarily halt the bot's operations without deleting its data or settings. It's a way to manage the bot's availability based on operational needs.
+- **/myid**: Find out your Telegram ID.
 
-- **/resume**: Resumes the bot's service after it has been suspended. This command allows administrators to quickly bring the bot back online after a pause, ensuring that users can continue interacting with the bot without interruption.
+- **/suspend**: Temporarily stop the bot from responding.
+
+- **/resume**: Restart the bot after it's been suspended.
+
+- **Any other text**: Just type anything to continue chatting.
+
+### Administrative Commands
+
+- **/clear**: Remove all chat data from the bot's database. Be careful with this one!
+
+- **/total**: See how many chats the bot has had.
+
+- **/drop**: Delete everything from the chat table and bot logs. This is more extreme than `/clear`.
+
+- **/sql**: Run SQL queries on the bot's database. Use this with caution!
+
+- **/logs**: Check the bot's logs for activity, errors, and user interactions.
 
 - `any other text`: An alias for `/chat`, allowing users to continue with chatting.
 
+> [!TIP]
+> For a better understanding of these commands, try interacting with a running bot from [@pytgpt_bot](https://t.me/pytgpt_bot). This can give you a practical idea of how the bot works and how to use it effectively.
 
 ### Administrative Commands
 
-- `/clear`: Clears all chats. This command is used to remove all chat data from the bot's database. It's a powerful command that should be used with caution, as it will delete all chat history.
+To make the administrative commands more understandable, let's simplify the descriptions and provide a bit more context for each command. This should help administrators manage the bot more effectively.
+
+### Simplified Administrative Commands
+
+- **/clear**: Use this command to remove all chat data from the bot's database. It's a powerful tool, so use it carefully to avoid losing important data.
+
+- **/total**: This command shows you the total number of chats the bot has handled. It's a quick way to see how much interaction the bot has had.
+
+- **/drop**: If you need to completely wipe out all chat data and logs, use this command. It's more extreme than `/clear` and should be used with caution to avoid losing all data.
+
+- **/sql**: Want to directly interact with the bot's database? This command lets you run SQL queries. It's a powerful feature for managing and analyzing data, but be cautious to avoid mistakes.
 
-- `/total`: Shows the total number of chats available. This command provides an overview of the current chat data stored in the bot's database, helping administrators understand the volume of interactions the bot has had.
+- **/logs**: This command gives you access to the bot's logs. It's useful for monitoring the bot's activity, spotting errors, and understanding user interactions.
 
-- `/drop`: Clears the entire chat table and bot logs. Similar to `/clear`, this command removes all data from the chat table in the database. It's a more drastic measure than `/clear`, as it completely wipes out all chat data and current contents of log file.
+> [!IMPORTANT]
+> Administrative commands are restricted to the users whose Telegram IDs are specified in the [.env](https://github.com/Simatwa/pytgpt-bot/blob/308f6079d153a429c445649896840fdc7cbfac11/env#L12) file.
 
-- `/sql`: Allows running SQL statements against the database. This command provides a way for administrators to directly interact with the bot's database using SQL queries. It's a powerful tool for managing and analyzing the bot's data but should be used with caution to avoid unintended data loss or corruption.
+## Further Tips
 
-- `/logs`: Checks the logs. This command is used to access the bot's logs, which can provide insights into the bot's activity, errors, and user interactions. It's a valuable tool for monitoring and troubleshooting the bot's performance.
+- The bot features inline query for text generation. The query must end with *three ellipsis* `...`. Remember to enable the mode from [@BotFather](https://t.me/pytgpt_bot). `/setinline`
+- You can as well add the bot to a Telegram channel. Grant it read and delete permissions. The access commands will still work out. `@bot_username <text>` will trigger **text generation**.
+- Channel Admin will control the bot access using the `/suspend` and `/resume` commands. *(Experimental).*
 
 ## Support and Feedback
 
 If you have any questions, feedback, or suggestions for `pytgpt`, please feel free to reach out. Your input is valuable in helping us improve and expand the bot's capabilities.
 
 ## License
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.2 Summary: Telegram bot for
+Metadata-Version: 2.1 Name: pytgpt-bot Version: 0.1.3 Summary: Telegram bot for
 chatting, text-to-image and text-to-speech conversions Home-page: https://
 github.com/Simatwa/pytgpt-bot Author: Smartwa Author-email:
 simatwacaleb@proton.me Maintainer: Smartwa License: MIT Project-URL: Bug
 Report, https://github.com/Simatwa/pytgpt-bot/issues/new Project-URL: Homepage,
 https://github.com/Simatwa/pytgpt-bot Project-URL: Source Code, https://
 github.com/Simatwa/pytgpt-bot Project-URL: Issue Tracker, https://github.com/
 Simatwa/pytgpt-bot/issues Project-URL: Download, https://github.com/Simatwa/
 pytgpt-bot/releases Project-URL: Documentation, https://github.com/Simatwa/
 pytgpt-bot/blob/main/README.md Keywords:
-ai,tgpt,pytgpt,chatbot,telegrambot,pytelegrambot,chatbot,text-to-audio,text-to-
-image Classifier: License :: OSI Approved :: MIT License Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Developers Classifier:
-Natural Language :: English Classifier: License :: Free For Home Use
-Classifier: Intended Audience :: Customer Service Classifier: Programming
+ai,tgpt,pytgpt,chatbot,telegrambot,pytelegrambot,chatbot,text-to-speech,text-
+to-image Classifier: License :: OSI Approved :: MIT License Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English Classifier: License :: Free For Home
+Use Classifier: Intended Audience :: Customer Service Classifier: Programming
 Language :: Python Classifier: Topic :: Software Development :: Libraries ::
 Python Modules Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
@@ -36,66 +36,63 @@
 [Python>=3.10](https://python.org) ## Installation 1. From Source Clone repo
 and install. ```bash git clone https://github.com/Simatwa/pytgpt-bot.git cd
 pytgpt-bot pip install . ``` 2. From Pypi *(recommended)* ```sh pip install
 pytgpt-bot ``` ## Usage Before getting started, ensure you've your Telegram bot
 token. If that's not the case then purpose to secure one from [@BotFather]
 (https://telegram.me/BotFather). Proceed to fill the [env](env) configuration
 file as per the needs and then rename it `.env` before firing up the bot
-`python3 run.py`. Alternatively, using CLI: `$ pytgpt-bot run ` ## Features -
-**/start**: Displays the help information, offering a comprehensive list of
-available commands and their functionalities. This command is essential for
-users to quickly understand how to interact with the bot. - **/chat**: Initiate
-a natural language conversation with the AI. This command allows users to
-engage in interactive dialogues, ask questions, or make requests. - **/image**:
-Generates images from textual descriptions using the default provider. This
-feature enables users to visualize ideas or concepts through images. - **/
-prodia**: Generates images from textual descriptions using the Prodia provider.
-This command offers a unique style or interpretation of the text descriptions
-compared to the default method. - **/speak**: Converts text to speech,
-providing users with the ability to listen to descriptions, instructions, or
-any text content read out by the AI. - **/intro**: Sets a new text for the chat
-intro. This command allows users to customize the chat introductory prompt
-which serves as a guide in the human-AI engagement. - **/voice**: Sets a new
-voice for speech synthesis. This command enables users to choose from different
-voices for the AI to use when generating audio from text. - **/provider**: Sets
-a new chat provider. This command allows users to switch between different
-providers for various functionalities, such as `phind`, `llama2`, `koboldai`
-etc. - **/awesome**: Sets predefined prompt as `chat intro`. Browse over 200 of
-them. - **/history**: Provides users with the ability to view the history of
-their chats with the bot. This command is useful for reviewing past
-interactions or finding specific information from previous conversations. - **/
-check**: Offers an overview of the bot's current configuration, including any
-custom settings applied by the user. - **/reset**: Resets the chat history and
-starts a new conversation thread. This command is useful for users who wish to
-start fresh or clear their chat history for privacy reasons. - **/myid**:
-Echoes the user's Telegram ID. This command is useful for users who need to
-know their Telegram ID for various purposes, such as setting up bot admin. -
-**/suspend**: Pauses the bot's service temporarily. This command is useful for
-channel administrators who need to temporarily halt the bot's operations
-without deleting its data or settings. It's a way to manage the bot's
-availability based on operational needs. - **/resume**: Resumes the bot's
-service after it has been suspended. This command allows administrators to
-quickly bring the bot back online after a pause, ensuring that users can
-continue interacting with the bot without interruption. - `any other text`: An
-alias for `/chat`, allowing users to continue with chatting. ### Administrative
-Commands - `/clear`: Clears all chats. This command is used to remove all chat
-data from the bot's database. It's a powerful command that should be used with
-caution, as it will delete all chat history. - `/total`: Shows the total number
-of chats available. This command provides an overview of the current chat data
-stored in the bot's database, helping administrators understand the volume of
-interactions the bot has had. - `/drop`: Clears the entire chat table and bot
-logs. Similar to `/clear`, this command removes all data from the chat table in
-the database. It's a more drastic measure than `/clear`, as it completely wipes
-out all chat data and current contents of log file. - `/sql`: Allows running
-SQL statements against the database. This command provides a way for
-administrators to directly interact with the bot's database using SQL queries.
-It's a powerful tool for managing and analyzing the bot's data but should be
-used with caution to avoid unintended data loss or corruption. - `/logs`:
-Checks the logs. This command is used to access the bot's logs, which can
-provide insights into the bot's activity, errors, and user interactions. It's a
-valuable tool for monitoring and troubleshooting the bot's performance. ##
-Support and Feedback If you have any questions, feedback, or suggestions for
+`python3 run.py`. Alternatively, using CLI: `$ pytgpt-bot run ` ## Features ###
+Access Commands - **/start**: This command shows you how to use the bot. It's
+like a guidebook for all the commands and what they do. - **/chat**: Use this
+to talk to the AI. You can ask questions, make requests, or just chat about
+anything. - **/image**: Want to see what something looks like? Type a
+description, and this command will create an image for you. - **/prodia**:
+Similar to `/image`, but it gives you a different style of image. - **/speak**:
+If you prefer listening to text instead of reading it, use this command to have
+the AI read out text for you. - **/intro**: Sets a new text for the chat intro.
+- **/voice**: Choose how the AI's voice sounds when it reads out text. - **/
+provider**: Switch between different AI providers for various features. - **/
+awesome**: Browse through a selection of cool chat intros. - **/history**: See
+past conversations with the bot. - **/check**: See what settings are currently
+active for your bot. - **/reset**: Start a new conversation from scratch. - **/
+myid**: Find out your Telegram ID. - **/suspend**: Temporarily stop the bot
+from responding. - **/resume**: Restart the bot after it's been suspended. -
+**Any other text**: Just type anything to continue chatting. ### Administrative
+Commands - **/clear**: Remove all chat data from the bot's database. Be careful
+with this one! - **/total**: See how many chats the bot has had. - **/drop**:
+Delete everything from the chat table and bot logs. This is more extreme than
+`/clear`. - **/sql**: Run SQL queries on the bot's database. Use this with
+caution! - **/logs**: Check the bot's logs for activity, errors, and user
+interactions. - `any other text`: An alias for `/chat`, allowing users to
+continue with chatting. > [!TIP] > For a better understanding of these
+commands, try interacting with a running bot from [@pytgpt_bot](https://t.me/
+pytgpt_bot). This can give you a practical idea of how the bot works and how to
+use it effectively. ### Administrative Commands To make the administrative
+commands more understandable, let's simplify the descriptions and provide a bit
+more context for each command. This should help administrators manage the bot
+more effectively. ### Simplified Administrative Commands - **/clear**: Use this
+command to remove all chat data from the bot's database. It's a powerful tool,
+so use it carefully to avoid losing important data. - **/total**: This command
+shows you the total number of chats the bot has handled. It's a quick way to
+see how much interaction the bot has had. - **/drop**: If you need to
+completely wipe out all chat data and logs, use this command. It's more extreme
+than `/clear` and should be used with caution to avoid losing all data. - **/
+sql**: Want to directly interact with the bot's database? This command lets you
+run SQL queries. It's a powerful feature for managing and analyzing data, but
+be cautious to avoid mistakes. - **/logs**: This command gives you access to
+the bot's logs. It's useful for monitoring the bot's activity, spotting errors,
+and understanding user interactions. > [!IMPORTANT] > Administrative commands
+are restricted to the users whose Telegram IDs are specified in the [.env]
+(https://github.com/Simatwa/pytgpt-bot/blob/
+308f6079d153a429c445649896840fdc7cbfac11/env#L12) file. ## Further Tips - The
+bot features inline query for text generation. The query must end with *three
+ellipsis* `...`. Remember to enable the mode from [@BotFather](https://t.me/
+pytgpt_bot). `/setinline` - You can as well add the bot to a Telegram channel.
+Grant it read and delete permissions. The access commands will still work out.
+`@bot_username ` will trigger **text generation**. - Channel Admin will control
+the bot access using the `/suspend` and `/resume` commands. *(Experimental).*
+## Support and Feedback If you have any questions, feedback, or suggestions for
 `pytgpt`, please feel free to reach out. Your input is valuable in helping us
 improve and expand the bot's capabilities. ## License `pytgpt-bot` is open-
 source and available under the [MIT License](LICENSE). Feel free to use,
 modify, and distribute the code as you see fit. --- Thank you for using
 `pytgpt-bot`. Enjoy your AI-powered interactions!
```

### Comparing `pytgpt_bot-0.1.2/setup.py` & `pytgpt_bot-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     full_path: Path = ROOT_PATH / path
     return full_path.read_text(encoding="utf-8")
 
 
 setup(
     name="pytgpt-bot",
     packages=["pytgpt_bot"],
-    version="0.1.2",
+    version="0.1.3",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Telegram bot for chatting, text-to-image and text-to-speech conversions",
     url="https://github.com/Simatwa/pytgpt-bot",
     project_urls={
@@ -45,15 +45,15 @@
         "ai",
         "tgpt",
         "pytgpt",
         "chatbot",
         "telegrambot",
         "pytelegrambot",
         "chatbot",
-        "text-to-audio",
+        "text-to-speech",
         "text-to-image",
     ],
     long_description=read_contents("README.md"),
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
```

