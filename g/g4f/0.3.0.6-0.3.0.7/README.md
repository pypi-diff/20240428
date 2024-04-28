# Comparing `tmp/g4f-0.3.0.6.tar.gz` & `tmp/g4f-0.3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.3.0.6.tar", last modified: Tue Apr 23 18:00:04 2024, max compression
+gzip compressed data, was "g4f-0.3.0.7.tar", last modified: Sun Apr 28 20:50:03 2024, max compression
```

## Comparing `g4f-0.3.0.6.tar` & `g4f-0.3.0.7.tar`

### file list

```diff
@@ -1,245 +1,247 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.395059 g4f-0.3.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-23 17:59:55.000000 g4f-0.3.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-23 17:59:55.000000 g4f-0.3.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    53734 2024-04-23 18:00:04.395059 g4f-0.3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    50538 2024-04-23 17:59:55.000000 g4f-0.3.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.359059 g4f-0.3.0.6/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.367059 g4f-0.3.0.6/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Aichatos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    21322 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Cnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Ecosia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Feedough.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/MetaAI.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/MetaAIAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.367059 g4f-0.3.0.6/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.375059 g4f-0.3.0.6/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.375059 g4f-0.3.0.6/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.375059 g4f-0.3.0.6/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/needs_auth/OpenaiAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    32130 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.379059 g4f-0.3.0.6/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.379059 g4f-0.3.0.6/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.379059 g4f-0.3.0.6/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.379059 g4f-0.3.0.6/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.379059 g4f-0.3.0.6/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/openai/har_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.379059 g4f-0.3.0.6/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.383059 g4f-0.3.0.6/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.383059 g4f-0.3.0.6/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.383059 g4f-0.3.0.6/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.383059 g4f-0.3.0.6/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.383059 g4f-0.3.0.6/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.383059 g4f-0.3.0.6/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.355059 g4f-0.3.0.6/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.383059 g4f-0.3.0.6/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    22896 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.387060 g4f-0.3.0.6/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.387060 g4f-0.3.0.6/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    47420 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.387060 g4f-0.3.0.6/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.387060 g4f-0.3.0.6/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.391059 g4f-0.3.0.6/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.391059 g4f-0.3.0.6/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.391059 g4f-0.3.0.6/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.391059 g4f-0.3.0.6/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-23 17:59:55.000000 g4f-0.3.0.6/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:00:04.391059 g4f-0.3.0.6/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    53734 2024-04-23 18:00:04.000000 g4f-0.3.0.6/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-23 18:00:04.000000 g4f-0.3.0.6/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:00:04.000000 g4f-0.3.0.6/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-23 18:00:04.000000 g4f-0.3.0.6/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-23 18:00:04.000000 g4f-0.3.0.6/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 18:00:04.000000 g4f-0.3.0.6/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:00:04.395059 g4f-0.3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-23 17:59:55.000000 g4f-0.3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.210319 g4f-0.3.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-28 20:49:59.000000 g4f-0.3.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-28 20:49:59.000000 g4f-0.3.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    55397 2024-04-28 20:50:03.210319 g4f-0.3.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    52201 2024-04-28 20:49:59.000000 g4f-0.3.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.170319 g4f-0.3.0.7/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.178319 g4f-0.3.0.7/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21322 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Ecosia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/MetaAI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/MetaAIAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Reka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.178319 g4f-0.3.0.7/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.186319 g4f-0.3.0.7/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.186319 g4f-0.3.0.7/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.186319 g4f-0.3.0.7/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/OpenaiAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33742 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.190319 g4f-0.3.0.7/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.190319 g4f-0.3.0.7/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.190319 g4f-0.3.0.7/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.190319 g4f-0.3.0.7/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.190319 g4f-0.3.0.7/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/openai/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/openai/proofofwork.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.190319 g4f-0.3.0.7/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.194319 g4f-0.3.0.7/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.194319 g4f-0.3.0.7/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.194319 g4f-0.3.0.7/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.194319 g4f-0.3.0.7/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.194319 g4f-0.3.0.7/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.194319 g4f-0.3.0.7/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.166319 g4f-0.3.0.7/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.198319 g4f-0.3.0.7/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    22896 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.198319 g4f-0.3.0.7/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.198319 g4f-0.3.0.7/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    47420 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.198319 g4f-0.3.0.7/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.202319 g4f-0.3.0.7/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.202319 g4f-0.3.0.7/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.202319 g4f-0.3.0.7/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9263 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.202319 g4f-0.3.0.7/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.202319 g4f-0.3.0.7/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-28 20:49:59.000000 g4f-0.3.0.7/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:50:03.206319 g4f-0.3.0.7/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55397 2024-04-28 20:50:03.000000 g4f-0.3.0.7/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-04-28 20:50:03.000000 g4f-0.3.0.7/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 20:50:03.000000 g4f-0.3.0.7/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-28 20:50:03.000000 g4f-0.3.0.7/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-28 20:50:03.000000 g4f-0.3.0.7/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-28 20:50:03.000000 g4f-0.3.0.7/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 20:50:03.210319 g4f-0.3.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-28 20:49:59.000000 g4f-0.3.0.7/setup.py
```

### Comparing `g4f-0.3.0.6/LICENSE` & `g4f-0.3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/PKG-INFO` & `g4f-0.3.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.0.6
+Version: 0.3.0.7
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -80,15 +80,15 @@
 
 <a href="https://trendshift.io/repositories/1692" target="_blank"><img src="https://trendshift.io/api/badge/repositories/1692" alt="xtekky%2Fgpt4free | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>
 
 Written by [@xtekky](https://github.com/hlohaus) & maintained by [@hlohaus](https://github.com/hlohaus)
 
 <div id="top"></div>
 
-> By using this repository or any code related to it, you agree to the [legal notice](LEGAL_NOTICE.md). The author is **not responsible for the usage of this repository nor endorses it**, nor is the author responsible for any copies, forks, re-uploads made by other users, or anything else related to GPT4Free. This is the author's only account and repository. To prevent impersonation or irresponsible actions, please comply with the GNU GPL license this Repository uses.  
+> By using this repository or any code related to it, you agree to the [legal notice](https://github.com/xtekky/gpt4free/blob/main/LEGAL_NOTICE.md). The author is **not responsible for the usage of this repository nor endorses it**, nor is the author responsible for any copies, forks, re-uploads made by other users, or anything else related to GPT4Free. This is the author's only account and repository. To prevent impersonation or irresponsible actions, please comply with the GNU GPL license this Repository uses.  
 
 > [!Warning]
 *"gpt4free"* serves as a **PoC** (proof of concept), demonstrating the development of an API package with multi-provider requests, with features like timeouts, load balance and flow control.
 
 > [!Note]
 <sup><strong>Lastet version:</strong></sup> [![PyPI version](https://img.shields.io/pypi/v/g4f?color=blue)](https://pypi.org/project/g4f) [![Docker version](https://img.shields.io/docker/v/hlohaus789/g4f?label=docker&color=blue)](https://hub.docker.com/r/hlohaus789/g4f)  
 > <sup><strong>Stats:</strong></sup>  [![Downloads](https://static.pepy.tech/badge/g4f)](https://pepy.tech/project/g4f) [![Downloads](https://static.pepy.tech/badge/g4f/month)](https://pepy.tech/project/g4f)
@@ -188,20 +188,20 @@
 3. **File Placement**: Once downloaded, transfer the `.exe` file from your downloads folder to a directory of your choice on your system, and then execute it to run the app.
 ##### Post-Installation Adjustment
 4. **Firewall Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your Windows Firewall settings to allow the application to operate correctly. To do this, access your Windows Firewall settings and allow the application.
 
 By following these steps, you should be able to successfully install and run the application on your Windows system. If you encounter any issues during the installation process, please refer to our Issue Tracker or try to get contact over Discord for assistance.
 
 Run the **Webview UI** on other Platfroms:
-- [/docs/guides/webview](/docs/webview.md)
+- [/docs/guides/webview](https://github.com/xtekky/gpt4free/blob/main/docs/webview.md)
 
 ##### Use your smartphone:
 
 Run the Web UI on Your Smartphone:
-- [/docs/guides/phone](/docs/guides/phone.md)
+- [/docs/guides/phone](https://github.com/xtekky/gpt4free/blob/main/docs/guides/phone.md)
 
 #### Use python
 
 ##### Prerequisites:
 
 1. [Download and install Python](https://www.python.org/downloads/) (Version 3.10+ is recommended).
 2. [Install Google Chrome](https://www.google.com/chrome/) for providers with webdriver
@@ -209,26 +209,26 @@
 ##### Install using PyPI package:
 
 ```
 pip install -U g4f[all]
 ```
 
 How do I install only parts or do disable parts?
-Use partial requirements: [/docs/requirements](/docs/requirements.md)
+Use partial requirements: [/docs/requirements](https://github.com/xtekky/gpt4free/blob/main/docs/requirements.md)
 
 ##### Install from source:
 
 How do I load the project using git and installing the project requirements?
-Read this tutorial and follow it step by step: [/docs/git](/docs/git.md)
+Read this tutorial and follow it step by step: [/docs/git](https://github.com/xtekky/gpt4free/blob/main/docs/git.md)
 
 
 ##### Install using Docker:
 
 How do I build and run composer image from source?
-Use docker-compose: [/docs/docker](/docs/docker.md)
+Use docker-compose: [/docs/docker](https://github.com/xtekky/gpt4free/blob/main/docs/docker.md)
 
 
 ## 💡 Usage
 
 #### Text Generation
 
 ```python
@@ -258,21 +258,21 @@
   prompt="a white siamese cat",
   ...
 )
 image_url = response.data[0].url
 ```
 
 
-[![Image with cat](/docs/cat.jpeg)](/docs/client.md)
+[![Image with cat](/docs/cat.jpeg)](https://github.com/xtekky/gpt4free/blob/main/docs/client.md)
 
 **Full Documentation for Python API**
 
-- New AsyncClient API from G4F: [/docs/async_client](/docs/async_client.md)
-- Client API like the OpenAI Python library: [/docs/client](/docs/client.md)
-- Legacy API with python modules: [/docs/legacy](/docs/legacy.md)
+- New AsyncClient API from G4F: [/docs/async_client](https://github.com/xtekky/gpt4free/blob/main/docs/async_client.md)
+- Client API like the OpenAI Python library: [/docs/client](https://github.com/xtekky/gpt4free/blob/main/docs/client.md)
+- Legacy API with python modules: [/docs/legacy](https://github.com/xtekky/gpt4free/blob/main/docs/legacy.md)
 
 #### Web UI
 
 To start the web interface, type the following codes in python:
 
 ```python
 from g4f.gui import run_gui
@@ -283,15 +283,15 @@
 python -m g4f.cli gui -port 8080 -debug
 ```
 
 #### Interference API
 
 You can use the Interference API to serve other OpenAI integrations with G4F.
 
-See docs: [/docs/interference](/docs/interference.md)
+See docs: [/docs/interference](https://github.com/xtekky/gpt4free/blob/main/docs/interference.md)
 
 Access with: http://localhost:1337/v1
 
 ### Configuration
 
 #### Cookies
 
@@ -376,18 +376,21 @@
 | [you.com](https://you.com) | `g4f.Provider.You` | ✔️ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 
 ## Best OpenSource Models
 While we wait for gpt-5, here is a list of new models that are at least better than gpt-3.5-turbo. **Some are better than gpt-4**. Expect this list to grow.
 
 | Website | Provider |  parameters | better than |
 | ------  | -------  |  ------ |  ------ | 
-| [mixtral-8x22b](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-turbo |
+| [claude-3-opus](https://anthropic.com/) | `g4f.Provider.You` | ?B | gpt-4-0125-preview |
+| [command-r+](https://txt.cohere.com/command-r-plus-microsoft-azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0314 |
+| [llama-3-70b](https://meta.ai/) | `g4f.Provider.Llama` or `DeepInfra` | 70B | gpt-4-0314 |
+| [claude-3-sonnet](https://anthropic.com/) | `g4f.Provider.You` | ?B | gpt-4-0314 |
+| [reka-core](https://chat.reka.ai/) | `g4f.Provider.Reka` | 21B | gpt-4-vision |
 | [dbrx-instruct](https://www.databricks.com/blog/introducing-dbrx-new-state-art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active| gpt-3.5-turbo |
-| [command-r+](https://txt.cohere.com/command-r-plus-microsoft-azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0613 |
-
+| [mixtral-8x22b](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-turbo |
 
 ### GPT-3.5
 
 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth |
 | ------  | -------  | ------- | ----- | ------ | ------ | ---- |
 | [chat3.aiyunos.top](https://chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | ✔️ | ❌ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ❌ |
 | [chat10.aichatos.xyz](https://chat10.aichatos.xyz) | `g4f.Provider.Aichatos` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
@@ -484,17 +487,34 @@
 | ----- | -------- | ----------- | ------------ | ------- |
 | Microsoft Copilot in Bing | `g4f.Provider.Bing` | dall-e-3 | gpt-4-vision | [bing.com](https://bing.com/chat) |
 | DeepInfra | `g4f.Provider.DeepInfra` | stability-ai/sdxl | llava-1.5-7b-hf | [deepinfra.com](https://deepinfra.com) |
 | Gemini | `g4f.Provider.Gemini` | ✔️ | ✔️ | [gemini.google.com](https://gemini.google.com) |
 | Gemini API | `g4f.Provider.GeminiPro` | ❌ | gemini-1.5-pro | [ai.google.dev](https://ai.google.dev) |
 | Meta AI | `g4f.Provider.MetaAI` | ✔️ | ❌ | [meta.ai](https://www.meta.ai) |
 | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) |
+| Reka | `g4f.Provider.Reka` | ❌ | ✔️ | [chat.reka.ai](https://chat.reka.ai/) |
 | Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b | [replicate.com](https://replicate.com) |
 | You.com | `g4f.Provider.You` | dall-e-3| ✔️ | [you.com](https://you.com) |
 
+```python
+from g4f.client import Client
+from g4f.Provider.GeminiPro import GeminiPro
+
+client = Client(
+    api_key="...",
+    provider=GeminiPro
+)
+response = client.chat.completions.create(
+    model="gemini-pro-vision",
+    messages=[{"role": "user", "content": "What are on this image?"}],
+    image=open("docs/waterfall.jpeg", "rb")
+)
+print(response.choices[0].message.content)
+```
+
 ## 🔗 Powered by gpt4free
 
 <table>
   <thead align="center">
     <tr border: none;>
       <td>
         <b>🎁 Projects</b>
@@ -897,19 +917,19 @@
 
 ## 🤝 Contribute
 
 We welcome contributions from the community. Whether you're adding new providers or features, or simply fixing typos and making small improvements, your input is valued. Creating a pull request is all it takes – our co-pilot will handle the code review process. Once all changes have been addressed, we'll merge the pull request into the main branch and release the updates at a later time.
 
 ###### Guide: How do i create a new Provider?
 
- - Read: [/docs/guides/create_provider](/docs/guides/create_provider.md)
+ - Read: [/docs/guides/create_provider](https://github.com/xtekky/gpt4free/blob/main/docs/guides/create_provider.md)
 
 ###### Guide: How can AI help me with writing code?
 
- - Read: [/docs/guides/help_me](/docs/guides/help_me.md)
+ - Read: [/docs/guides/help_me](https://github.com/xtekky/gpt4free/blob/main/docs/guides/help_me.md)
 
 ## 🙌 Contributors
 
 A list of all contributors is available [here](https://github.com/xtekky/gpt4free/graphs/contributors)
 
 <a href="https://github.com/xtekky" target="_blank"><img src="https://avatars.githubusercontent.com/u/98614666?v=4&s=45" width="45" title="xtekky"></a>
 <a href="https://github.com/hlohaus" target="_blank"><img src="https://avatars.githubusercontent.com/u/983577?v=4&s=45" width="45" title="hlohaus"></a>
@@ -943,19 +963,19 @@
 <a href="https://github.com/ggindinson" target="_blank"><img src="https://avatars.githubusercontent.com/u/97807772?v=4&s=45" width="45" title="ggindinson"></a>
 <span></span>
 <img src="https://avatars.githubusercontent.com/u/71154407?s=45&v=4" width="45" title="ading2210">
 <img src="https://avatars.githubusercontent.com/u/12299238?s=45&v=4" width="45" title="xqdoo00o">
 <img src="https://avatars.githubusercontent.com/u/97126670?s=45&v=4" width="45" title="nathanrchn">
 <img src="https://avatars.githubusercontent.com/u/81407603?v=4&s=45" width="45" title="dsdanielpark">
 
-- The [`Vercel.py`](g4f/Provider/Vercel.py) file contains code from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210)
-- The [`har_file.py`](g4f/Provider/openai/har_file.py) has input from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API)
-- The [`PerplexityLabs.py`](g4f/Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai)
-- The [`Gemini.py`](g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API)
-- The [`MetaAI.py`](g4f/Provider/MetaAI.py) file contains code from [meta-ai-api](https://github.com/Strvm/meta-ai-api) by [@Strvm](https://github.com/Strvm)
+- The [`Vercel.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/Vercel.py) file contains code from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210)
+- The [`har_file.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API)
+- The [`PerplexityLabs.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai)
+- The [`Gemini.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API)
+- The [`MetaAI.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/MetaAI.py) file contains code from [meta-ai-api](https://github.com/Strvm/meta-ai-api) by [@Strvm](https://github.com/Strvm)
 
 *Having input implies that the AI's code generation utilized it as one of many sources.*
 
 ## ©️ Copyright
 
 This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt)
 
@@ -987,13 +1007,13 @@
 <table>
   <tr>
      <td>
        <p align="center"> <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/93/GPLv3_Logo.svg/1200px-GPLv3_Logo.svg.png" width="80%"></img>
     </td>
     <td> 
       <img src="https://img.shields.io/badge/License-GNU_GPL_v3.0-red.svg"/> <br> 
-This project is licensed under <a href="./LICENSE">GNU_GPL_v3.0</a>.
+This project is licensed under <a href="https://github.com/xtekky/gpt4free/blob/main/LICENSE">GNU_GPL_v3.0</a>.
     </td>
   </tr>
 </table>
 
 <p align="right">(<a href="#top">🔼 Back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.0.6 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.0.7 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -41,28 +41,29 @@
 local Requires-Dist: gpt4all; extra == "local" Provides-Extra: curl-cffi
 Requires-Dist: curl_cffi>=0.6.2; extra == "curl-cffi" ![248433934-7886223b-
 c1d1-4260-82aa-da5741f303bb](https://github.com/xtekky/gpt4free/assets/
 98614666/ea012c87-76e0-496a-8ac4-e2de090cc6c9) _[_x_t_e_k_k_y_%_2_F_g_p_t_4_f_r_e_e_ _|
 _T_r_e_n_d_s_h_i_f_t_]Written by [@xtekky](https://github.com/hlohaus) & maintained by
 [@hlohaus](https://github.com/hlohaus)
 > By using this repository or any code related to it, you agree to the [legal
-notice](LEGAL_NOTICE.md). The author is **not responsible for the usage of this
-repository nor endorses it**, nor is the author responsible for any copies,
-forks, re-uploads made by other users, or anything else related to GPT4Free.
-This is the author's only account and repository. To prevent impersonation or
-irresponsible actions, please comply with the GNU GPL license this Repository
-uses. > [!Warning] *"gpt4free"* serves as a **PoC** (proof of concept),
-demonstrating the development of an API package with multi-provider requests,
-with features like timeouts, load balance and flow control. > [!Note] LLaasstteett
-vveerrssiioonn:: [![PyPI version](https://img.shields.io/pypi/v/g4f?color=blue)](https:
-//pypi.org/project/g4f) [![Docker version](https://img.shields.io/docker/v/
-hlohaus789/g4f?label=docker&color=blue)](https://hub.docker.com/r/hlohaus789/
-g4f) > SSttaattss:: [![Downloads](https://static.pepy.tech/badge/g4f)](https://
-pepy.tech/project/g4f) [![Downloads](https://static.pepy.tech/badge/g4f/month)]
-(https://pepy.tech/project/g4f) ```sh pip install -U g4f ``` ```sh docker pull
+notice](https://github.com/xtekky/gpt4free/blob/main/LEGAL_NOTICE.md). The
+author is **not responsible for the usage of this repository nor endorses it**,
+nor is the author responsible for any copies, forks, re-uploads made by other
+users, or anything else related to GPT4Free. This is the author's only account
+and repository. To prevent impersonation or irresponsible actions, please
+comply with the GNU GPL license this Repository uses. > [!Warning] *"gpt4free"*
+serves as a **PoC** (proof of concept), demonstrating the development of an API
+package with multi-provider requests, with features like timeouts, load balance
+and flow control. > [!Note] LLaasstteett vveerrssiioonn:: [![PyPI version](https://
+img.shields.io/pypi/v/g4f?color=blue)](https://pypi.org/project/g4f) [![Docker
+version](https://img.shields.io/docker/v/hlohaus789/
+g4f?label=docker&color=blue)](https://hub.docker.com/r/hlohaus789/g4f) > SSttaattss::
+[![Downloads](https://static.pepy.tech/badge/g4f)](https://pepy.tech/project/
+g4f) [![Downloads](https://static.pepy.tech/badge/g4f/month)](https://
+pepy.tech/project/g4f) ```sh pip install -U g4f ``` ```sh docker pull
 hlohaus789/g4f ``` ## ð What's New - Installation Guide for Windows (.exe):
 ð» [#installation-guide-for-windows](#installation-guide-for-windows-exe) -
 Join our Telegram Channel: ð¨ [telegram.me/g4f_channel](https://telegram.me/
 g4f_channel) - Join our Discord Group: ð¬ [discord.gg/XfybzPXPH5](https://
 discord.gg/XfybzPXPH5) - `g4f` now supports 100% local inference: ð§  [local-
 docs](https://g4f.mintlify.app/docs/core/usage/local) ## ð» Site Takedown Is
 your site on this repository and you want to take it down? Send an email to
@@ -124,48 +125,54 @@
 Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your
 Windows Firewall settings to allow the application to operate correctly. To do
 this, access your Windows Firewall settings and allow the application. By
 following these steps, you should be able to successfully install and run the
 application on your Windows system. If you encounter any issues during the
 installation process, please refer to our Issue Tracker or try to get contact
 over Discord for assistance. Run the **Webview UI** on other Platfroms: - [/
-docs/guides/webview](/docs/webview.md) ##### Use your smartphone: Run the Web
-UI on Your Smartphone: - [/docs/guides/phone](/docs/guides/phone.md) #### Use
-python ##### Prerequisites: 1. [Download and install Python](https://
-www.python.org/downloads/) (Version 3.10+ is recommended). 2. [Install Google
-Chrome](https://www.google.com/chrome/) for providers with webdriver #####
-Install using PyPI package: ``` pip install -U g4f[all] ``` How do I install
-only parts or do disable parts? Use partial requirements: [/docs/requirements]
-(/docs/requirements.md) ##### Install from source: How do I load the project
-using git and installing the project requirements? Read this tutorial and
-follow it step by step: [/docs/git](/docs/git.md) ##### Install using Docker:
-How do I build and run composer image from source? Use docker-compose: [/docs/
-docker](/docs/docker.md) ## ð¡ Usage #### Text Generation ```python from
+docs/guides/webview](https://github.com/xtekky/gpt4free/blob/main/docs/
+webview.md) ##### Use your smartphone: Run the Web UI on Your Smartphone: - [/
+docs/guides/phone](https://github.com/xtekky/gpt4free/blob/main/docs/guides/
+phone.md) #### Use python ##### Prerequisites: 1. [Download and install Python]
+(https://www.python.org/downloads/) (Version 3.10+ is recommended). 2. [Install
+Google Chrome](https://www.google.com/chrome/) for providers with webdriver
+##### Install using PyPI package: ``` pip install -U g4f[all] ``` How do I
+install only parts or do disable parts? Use partial requirements: [/docs/
+requirements](https://github.com/xtekky/gpt4free/blob/main/docs/
+requirements.md) ##### Install from source: How do I load the project using git
+and installing the project requirements? Read this tutorial and follow it step
+by step: [/docs/git](https://github.com/xtekky/gpt4free/blob/main/docs/git.md)
+##### Install using Docker: How do I build and run composer image from source?
+Use docker-compose: [/docs/docker](https://github.com/xtekky/gpt4free/blob/
+main/docs/docker.md) ## ð¡ Usage #### Text Generation ```python from
 g4f.client import Client client = Client() response =
 client.chat.completions.create( model="gpt-3.5-turbo", messages=[{"role":
 "user", "content": "Hello"}], ... ) print(response.choices[0].message.content)
 ``` ``` Hello! How can I assist you today? ``` #### Image Generation ```python
 from g4f.client import Client client = Client() response =
 client.images.generate( model="gemini", prompt="a white siamese cat", ... )
-image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](/docs/
-client.md) **Full Documentation for Python API** - New AsyncClient API from
-G4F: [/docs/async_client](/docs/async_client.md) - Client API like the OpenAI
-Python library: [/docs/client](/docs/client.md) - Legacy API with python
-modules: [/docs/legacy](/docs/legacy.md) #### Web UI To start the web
-interface, type the following codes in python: ```python from g4f.gui import
-run_gui run_gui() ``` or execute the following command: ```bash python -
-m g4f.cli gui -port 8080 -debug ``` #### Interference API You can use the
-Interference API to serve other OpenAI integrations with G4F. See docs: [/docs/
-interference](/docs/interference.md) Access with: http://localhost:1337/v1 ###
-Configuration #### Cookies Cookies are essential for using Meta AI and
-Microsoft Designer to create images. Additionally, cookies are required for the
-Google Gemini and WhiteRabbitNeo Provider. From Bing, ensure you have the "_U"
-cookie, and from Google, all cookies starting with "__Secure-1PSID" are needed.
-You can pass these cookies directly to the create function or set them using
-the `set_cookies` method before running G4F: ```python from g4f.cookies import
+image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](https:
+//github.com/xtekky/gpt4free/blob/main/docs/client.md) **Full Documentation for
+Python API** - New AsyncClient API from G4F: [/docs/async_client](https://
+github.com/xtekky/gpt4free/blob/main/docs/async_client.md) - Client API like
+the OpenAI Python library: [/docs/client](https://github.com/xtekky/gpt4free/
+blob/main/docs/client.md) - Legacy API with python modules: [/docs/legacy]
+(https://github.com/xtekky/gpt4free/blob/main/docs/legacy.md) #### Web UI To
+start the web interface, type the following codes in python: ```python from
+g4f.gui import run_gui run_gui() ``` or execute the following command: ```bash
+python -m g4f.cli gui -port 8080 -debug ``` #### Interference API You can use
+the Interference API to serve other OpenAI integrations with G4F. See docs: [/
+docs/interference](https://github.com/xtekky/gpt4free/blob/main/docs/
+interference.md) Access with: http://localhost:1337/v1 ### Configuration ####
+Cookies Cookies are essential for using Meta AI and Microsoft Designer to
+create images. Additionally, cookies are required for the Google Gemini and
+WhiteRabbitNeo Provider. From Bing, ensure you have the "_U" cookie, and from
+Google, all cookies starting with "__Secure-1PSID" are needed. You can pass
+these cookies directly to the create function or set them using the
+`set_cookies` method before running G4F: ```python from g4f.cookies import
 set_cookies set_cookies(".bing.com", { "_U": "cookie value" }) set_cookies
 (".google.com", { "__Secure-1PSID": "cookie value" }) ``` Alternatively, you
 can place your .har and cookie files in the `/har_and_cookies` directory. To
 export a cookie file, use the EditThisCookie extension available on the Chrome
 Web Store: [EditThisCookie Extension](https://chromewebstore.google.com/detail/
 editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg). You can also create .har
 files to capture cookies. If you need further assistance, refer to the next
@@ -207,37 +214,42 @@
 beta.theb.ai) | `g4f.Provider.Theb` | âï¸ | âï¸ | âï¸ | ![Unknown]
 (https://img.shields.io/badge/Unknown-grey) | â | | [you.com](https://
 you.com) | `g4f.Provider.You` | âï¸ | âï¸ | âï¸ | ![Active](https://
 img.shields.io/badge/Active-brightgreen) | â | ## Best OpenSource Models
 While we wait for gpt-5, here is a list of new models that are at least better
 than gpt-3.5-turbo. **Some are better than gpt-4**. Expect this list to grow. |
 Website | Provider | parameters | better than | | ------ | ------- | ------ | -
------ | | [mixtral-8x22b](https://huggingface.co/mistral-community/Mixtral-
-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-turbo | |
-[dbrx-instruct](https://www.databricks.com/blog/introducing-dbrx-new-state-art-
-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active| gpt-3.5-turbo | |
-[command-r+](https://txt.cohere.com/command-r-plus-microsoft-azure/) |
-`g4f.Provider.HuggingChat` | 104B | gpt-4-0613 | ### GPT-3.5 | Website |
-Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | ------ | ------- | ----
---- | ----- | ------ | ------ | ---- | | [chat3.aiyunos.top](https://
-chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | âï¸ | â | âï¸ | !
+----- | | [claude-3-opus](https://anthropic.com/) | `g4f.Provider.You` | ?B |
+gpt-4-0125-preview | | [command-r+](https://txt.cohere.com/command-r-plus-
+microsoft-azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0314 | | [llama-
+3-70b](https://meta.ai/) | `g4f.Provider.Llama` or `DeepInfra` | 70B | gpt-4-
+0314 | | [claude-3-sonnet](https://anthropic.com/) | `g4f.Provider.You` | ?B |
+gpt-4-0314 | | [reka-core](https://chat.reka.ai/) | `g4f.Provider.Reka` | 21B |
+gpt-4-vision | | [dbrx-instruct](https://www.databricks.com/blog/introducing-
+dbrx-new-state-art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active|
+gpt-3.5-turbo | | [mixtral-8x22b](https://huggingface.co/mistral-community/
+Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-
+turbo | ### GPT-3.5 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status |
+Auth | | ------ | ------- | ------- | ----- | ------ | ------ | ---- | |
+[chat3.aiyunos.top](https://chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace`
+| âï¸ | â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey)
+| â | | [chat10.aichatos.xyz](https://chat10.aichatos.xyz) |
+`g4f.Provider.Aichatos` | âï¸ | â | âï¸ | ![Active](https://
+img.shields.io/badge/Active-brightgreen) | â | | [chatforai.store](https://
+chatforai.store) | `g4f.Provider.ChatForAi` | âï¸ | â | âï¸ | !
 [Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
-[chat10.aichatos.xyz](https://chat10.aichatos.xyz) | `g4f.Provider.Aichatos` |
-âï¸ | â | âï¸ | ![Active](https://img.shields.io/badge/Active-
-brightgreen) | â | | [chatforai.store](https://chatforai.store) |
-`g4f.Provider.ChatForAi` | âï¸ | â | âï¸ | ![Unknown](https://
-img.shields.io/badge/Unknown-grey) | â | | [chatgpt4online.org](https://
-chatgpt4online.org) | `g4f.Provider.Chatgpt4Online` | âï¸ | â | âï¸ | !
-[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [chatgpt-
-free.cc](https://www.chatgpt-free.cc) | `g4f.Provider.ChatgptNext` | âï¸ |
-â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
-[chatgptx.de](https://chatgptx.de) | `g4f.Provider.ChatgptX` | âï¸ | â |
-âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
-[f1.cnote.top](https://f1.cnote.top) | `g4f.Provider.Cnote` | âï¸ | â |
-âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) | â | |
+[chatgpt4online.org](https://chatgpt4online.org) |
+`g4f.Provider.Chatgpt4Online` | âï¸ | â | âï¸ | ![Unknown](https://
+img.shields.io/badge/Unknown-grey) | â | | [chatgpt-free.cc](https://
+www.chatgpt-free.cc) | `g4f.Provider.ChatgptNext` | âï¸ | â | âï¸ | !
+[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [chatgptx.de]
+(https://chatgptx.de) | `g4f.Provider.ChatgptX` | âï¸ | â | âï¸ | !
+[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [f1.cnote.top]
+(https://f1.cnote.top) | `g4f.Provider.Cnote` | âï¸ | â | âï¸ | !
+[Active](https://img.shields.io/badge/Active-brightgreen) | â | |
 [duckduckgo.com](https://duckduckgo.com/duckchat) | `g4f.Provider.DuckDuckGo` |
 âï¸ | â | âï¸ | ![Active](https://img.shields.io/badge/Active-
 brightgreen) | â | | [ecosia.org](https://www.ecosia.org) |
 `g4f.Provider.Ecosia` | âï¸ | â | âï¸ | ![Active](https://
 img.shields.io/badge/Active-brightgreen) | â | | [feedough.com](https://
 www.feedough.com) | `g4f.Provider.Feedough` | âï¸ | â | âï¸ | ![Active]
 (https://img.shields.io/badge/Active-brightgreen) | â | | [flowgpt.com]
@@ -371,18 +383,24 @@
 gpt-4-vision | [bing.com](https://bing.com/chat) | | DeepInfra |
 `g4f.Provider.DeepInfra` | stability-ai/sdxl | llava-1.5-7b-hf |
 [deepinfra.com](https://deepinfra.com) | | Gemini | `g4f.Provider.Gemini` |
 âï¸ | âï¸ | [gemini.google.com](https://gemini.google.com) | | Gemini API
 | `g4f.Provider.GeminiPro` | â | gemini-1.5-pro | [ai.google.dev](https://
 ai.google.dev) | | Meta AI | `g4f.Provider.MetaAI` | âï¸ | â | [meta.ai]
 (https://www.meta.ai) | | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-
-3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) | | Replicate |
-`g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b | [replicate.com]
-(https://replicate.com) | | You.com | `g4f.Provider.You` | dall-e-3| âï¸ |
-[you.com](https://you.com) | ## ð Powered by gpt4free
+3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) | | Reka |
+`g4f.Provider.Reka` | â | âï¸ | [chat.reka.ai](https://chat.reka.ai/) | |
+Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b |
+[replicate.com](https://replicate.com) | | You.com | `g4f.Provider.You` | dall-
+e-3| âï¸ | [you.com](https://you.com) | ```python from g4f.client import
+Client from g4f.Provider.GeminiPro import GeminiPro client = Client
+( api_key="...", provider=GeminiPro ) response = client.chat.completions.create
+( model="gemini-pro-vision", messages=[{"role": "user", "content": "What are on
+this image?"}], image=open("docs/waterfall.jpeg", "rb") ) print
+(response.choices[0].message.content) ``` ## ð Powered by gpt4free
 ?ð??? PPrroojjeeccttss             ?â?­? SSttaarrss ?ð??? FFoorrkkss ?ð??? IIssssuueess ?ð???¬ PPuullll rreeqquueessttss
 _gg_pp_tt_44_ff_rr_ee_ee                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _FF_rr_ee_ee_ _AA_II_ _AA_PP_II_''_ss_ _&&_ _PP_oo_tt_ee_nn_tt_ii_aa_ll _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _PP_rr_oo_vv_ii_dd_ee_rr_ss_ _LL_ii_ss_tt
 _CC_hh_aa_tt_GG_PP_TT_--_CC_ll_oo_nn_ee             _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _AA_ii_ _aa_gg_ee_nn_tt                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _CC_hh_aa_tt_GG_pp_tt_ _DD_ii_ss_cc_oo_rr_dd_ _BB_oo_tt       _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
@@ -396,19 +414,20 @@
 _pp_yy_tt_hh_oo_nn_--_tt_gg_pp_tt               _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 ## ð¤ Contribute We welcome contributions from the community. Whether you're
 adding new providers or features, or simply fixing typos and making small
 improvements, your input is valued. Creating a pull request is all it takes â
 our co-pilot will handle the code review process. Once all changes have been
 addressed, we'll merge the pull request into the main branch and release the
 updates at a later time. ###### Guide: How do i create a new Provider? - Read:
-[/docs/guides/create_provider](/docs/guides/create_provider.md) ###### Guide:
-How can AI help me with writing code? - Read: [/docs/guides/help_me](/docs/
-guides/help_me.md) ## ð Contributors A list of all contributors is available
-[here](https://github.com/xtekky/gpt4free/graphs/contributors) _[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_6_1_4_6_6_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+[/docs/guides/create_provider](https://github.com/xtekky/gpt4free/blob/main/
+docs/guides/create_provider.md) ###### Guide: How can AI help me with writing
+code? - Read: [/docs/guides/help_me](https://github.com/xtekky/gpt4free/blob/
+main/docs/guides/help_me.md) ## ð Contributors A list of all contributors is
+available [here](https://github.com/xtekky/gpt4free/graphs/contributors)
+_[_h_t_t_p_s_:_/_/_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_6_1_4_6_6_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_3_5_7_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_8_3_0_5_3_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_4_1_5_4_6_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_9_6_6_2_2_8_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_0_5_1_6_0_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_0_5_8_5_2_3_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_3_4_8_5_4_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
@@ -433,36 +452,39 @@
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_7_6_3_6_0_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_5_6_6_3_2_2_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_9_3_2_2_7_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_7_8_0_7_7_7_2_?_v_=_4_&_s_=_4_5_][https://
 avatars.githubusercontent.com/u/71154407?s=45&v=4][https://
 avatars.githubusercontent.com/u/12299238?s=45&v=4][https://
 avatars.githubusercontent.com/u/97126670?s=45&v=4][https://
-avatars.githubusercontent.com/u/81407603?v=4&s=45]- The [`Vercel.py`](g4f/
-Provider/Vercel.py) file contains code from [vercel-llm-api](https://
-github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/
-ading2210) - The [`har_file.py`](g4f/Provider/openai/har_file.py) has input
+avatars.githubusercontent.com/u/81407603?v=4&s=45]- The [`Vercel.py`](https://
+github.com/xtekky/gpt4free/blob/main/g4f/Provider/Vercel.py) file contains code
+from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by
+[@ading2210](https://github.com/ading2210) - The [`har_file.py`](https://
+github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input
 from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API) -
-The [`PerplexityLabs.py`](g4f/Provider/openai/har_file.py) has input from
-[nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai) - The
-[`Gemini.py`](g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/
-Gemini-API](https://github.com/dsdanielpark/Gemini-API) - The [`MetaAI.py`]
-(g4f/Provider/MetaAI.py) file contains code from [meta-ai-api](https://
-github.com/Strvm/meta-ai-api) by [@Strvm](https://github.com/Strvm) *Having
-input implies that the AI's code generation utilized it as one of many
-sources.* ## Â©ï¸ Copyright This program is licensed under the [GNU GPL v3]
-(https://www.gnu.org/licenses/gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C)
-2023 xtekky This program is free software: you can redistribute it and/or
-modify it under the terms of the GNU General Public License as published by the
-Free Software Foundation, either version 3 of the License, or (at your option)
-any later version. This program is distributed in the hope that it will be
-useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public
-License for more details. You should have received a copy of the GNU General
-Public License along with this program. If not, see
+The [`PerplexityLabs.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/
+Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://
+github.com/nathanrchn/perplexityai) - The [`Gemini.py`](https://github.com/
+xtekky/gpt4free/blob/main/g4f/Provider/needs_auth/Gemini.py) has input from
+[dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API) - The
+[`MetaAI.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/
+MetaAI.py) file contains code from [meta-ai-api](https://github.com/Strvm/meta-
+ai-api) by [@Strvm](https://github.com/Strvm) *Having input implies that the
+AI's code generation utilized it as one of many sources.* ## Â©ï¸ Copyright
+This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/
+gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C) 2023 xtekky This program is
+free software: you can redistribute it and/or modify it under the terms of the
+GNU General Public License as published by the Free Software Foundation, either
+version 3 of the License, or (at your option) any later version. This program
+is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+PARTICULAR PURPOSE. See the GNU General Public License for more details. You
+should have received a copy of the GNU General Public License along with this
+program. If not, see
 www.gnu.org/licenses/>. ``` ## â­ Star History _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]## ð
 License
 [https://upload.wikimedia.org/wikipedia/ [https://img.shields.io/badge/License-
    commons/thumb/9/93/GPLv3_Logo.svg/    GNU_GPL_v3.0-red.svg]
        1200px-GPLv3_Logo.svg.png]        This project is licensed under
                                          _G_N_U___G_P_L___v_3_._0.
                                                              (_ð___¼_ _B_a_c_k_ _t_o_ _t_o_p)
```

### Comparing `g4f-0.3.0.6/README.md` & `g4f-0.3.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <a href="https://trendshift.io/repositories/1692" target="_blank"><img src="https://trendshift.io/api/badge/repositories/1692" alt="xtekky%2Fgpt4free | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>
 
 Written by [@xtekky](https://github.com/hlohaus) & maintained by [@hlohaus](https://github.com/hlohaus)
 
 <div id="top"></div>
 
-> By using this repository or any code related to it, you agree to the [legal notice](LEGAL_NOTICE.md). The author is **not responsible for the usage of this repository nor endorses it**, nor is the author responsible for any copies, forks, re-uploads made by other users, or anything else related to GPT4Free. This is the author's only account and repository. To prevent impersonation or irresponsible actions, please comply with the GNU GPL license this Repository uses.  
+> By using this repository or any code related to it, you agree to the [legal notice](https://github.com/xtekky/gpt4free/blob/main/LEGAL_NOTICE.md). The author is **not responsible for the usage of this repository nor endorses it**, nor is the author responsible for any copies, forks, re-uploads made by other users, or anything else related to GPT4Free. This is the author's only account and repository. To prevent impersonation or irresponsible actions, please comply with the GNU GPL license this Repository uses.  
 
 > [!Warning]
 *"gpt4free"* serves as a **PoC** (proof of concept), demonstrating the development of an API package with multi-provider requests, with features like timeouts, load balance and flow control.
 
 > [!Note]
 <sup><strong>Lastet version:</strong></sup> [![PyPI version](https://img.shields.io/pypi/v/g4f?color=blue)](https://pypi.org/project/g4f) [![Docker version](https://img.shields.io/docker/v/hlohaus789/g4f?label=docker&color=blue)](https://hub.docker.com/r/hlohaus789/g4f)  
 > <sup><strong>Stats:</strong></sup>  [![Downloads](https://static.pepy.tech/badge/g4f)](https://pepy.tech/project/g4f) [![Downloads](https://static.pepy.tech/badge/g4f/month)](https://pepy.tech/project/g4f)
@@ -110,20 +110,20 @@
 3. **File Placement**: Once downloaded, transfer the `.exe` file from your downloads folder to a directory of your choice on your system, and then execute it to run the app.
 ##### Post-Installation Adjustment
 4. **Firewall Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your Windows Firewall settings to allow the application to operate correctly. To do this, access your Windows Firewall settings and allow the application.
 
 By following these steps, you should be able to successfully install and run the application on your Windows system. If you encounter any issues during the installation process, please refer to our Issue Tracker or try to get contact over Discord for assistance.
 
 Run the **Webview UI** on other Platfroms:
-- [/docs/guides/webview](/docs/webview.md)
+- [/docs/guides/webview](https://github.com/xtekky/gpt4free/blob/main/docs/webview.md)
 
 ##### Use your smartphone:
 
 Run the Web UI on Your Smartphone:
-- [/docs/guides/phone](/docs/guides/phone.md)
+- [/docs/guides/phone](https://github.com/xtekky/gpt4free/blob/main/docs/guides/phone.md)
 
 #### Use python
 
 ##### Prerequisites:
 
 1. [Download and install Python](https://www.python.org/downloads/) (Version 3.10+ is recommended).
 2. [Install Google Chrome](https://www.google.com/chrome/) for providers with webdriver
@@ -131,26 +131,26 @@
 ##### Install using PyPI package:
 
 ```
 pip install -U g4f[all]
 ```
 
 How do I install only parts or do disable parts?
-Use partial requirements: [/docs/requirements](/docs/requirements.md)
+Use partial requirements: [/docs/requirements](https://github.com/xtekky/gpt4free/blob/main/docs/requirements.md)
 
 ##### Install from source:
 
 How do I load the project using git and installing the project requirements?
-Read this tutorial and follow it step by step: [/docs/git](/docs/git.md)
+Read this tutorial and follow it step by step: [/docs/git](https://github.com/xtekky/gpt4free/blob/main/docs/git.md)
 
 
 ##### Install using Docker:
 
 How do I build and run composer image from source?
-Use docker-compose: [/docs/docker](/docs/docker.md)
+Use docker-compose: [/docs/docker](https://github.com/xtekky/gpt4free/blob/main/docs/docker.md)
 
 
 ## 💡 Usage
 
 #### Text Generation
 
 ```python
@@ -180,21 +180,21 @@
   prompt="a white siamese cat",
   ...
 )
 image_url = response.data[0].url
 ```
 
 
-[![Image with cat](/docs/cat.jpeg)](/docs/client.md)
+[![Image with cat](/docs/cat.jpeg)](https://github.com/xtekky/gpt4free/blob/main/docs/client.md)
 
 **Full Documentation for Python API**
 
-- New AsyncClient API from G4F: [/docs/async_client](/docs/async_client.md)
-- Client API like the OpenAI Python library: [/docs/client](/docs/client.md)
-- Legacy API with python modules: [/docs/legacy](/docs/legacy.md)
+- New AsyncClient API from G4F: [/docs/async_client](https://github.com/xtekky/gpt4free/blob/main/docs/async_client.md)
+- Client API like the OpenAI Python library: [/docs/client](https://github.com/xtekky/gpt4free/blob/main/docs/client.md)
+- Legacy API with python modules: [/docs/legacy](https://github.com/xtekky/gpt4free/blob/main/docs/legacy.md)
 
 #### Web UI
 
 To start the web interface, type the following codes in python:
 
 ```python
 from g4f.gui import run_gui
@@ -205,15 +205,15 @@
 python -m g4f.cli gui -port 8080 -debug
 ```
 
 #### Interference API
 
 You can use the Interference API to serve other OpenAI integrations with G4F.
 
-See docs: [/docs/interference](/docs/interference.md)
+See docs: [/docs/interference](https://github.com/xtekky/gpt4free/blob/main/docs/interference.md)
 
 Access with: http://localhost:1337/v1
 
 ### Configuration
 
 #### Cookies
 
@@ -298,18 +298,21 @@
 | [you.com](https://you.com) | `g4f.Provider.You` | ✔️ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 
 ## Best OpenSource Models
 While we wait for gpt-5, here is a list of new models that are at least better than gpt-3.5-turbo. **Some are better than gpt-4**. Expect this list to grow.
 
 | Website | Provider |  parameters | better than |
 | ------  | -------  |  ------ |  ------ | 
-| [mixtral-8x22b](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-turbo |
+| [claude-3-opus](https://anthropic.com/) | `g4f.Provider.You` | ?B | gpt-4-0125-preview |
+| [command-r+](https://txt.cohere.com/command-r-plus-microsoft-azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0314 |
+| [llama-3-70b](https://meta.ai/) | `g4f.Provider.Llama` or `DeepInfra` | 70B | gpt-4-0314 |
+| [claude-3-sonnet](https://anthropic.com/) | `g4f.Provider.You` | ?B | gpt-4-0314 |
+| [reka-core](https://chat.reka.ai/) | `g4f.Provider.Reka` | 21B | gpt-4-vision |
 | [dbrx-instruct](https://www.databricks.com/blog/introducing-dbrx-new-state-art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active| gpt-3.5-turbo |
-| [command-r+](https://txt.cohere.com/command-r-plus-microsoft-azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0613 |
-
+| [mixtral-8x22b](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-turbo |
 
 ### GPT-3.5
 
 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth |
 | ------  | -------  | ------- | ----- | ------ | ------ | ---- |
 | [chat3.aiyunos.top](https://chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | ✔️ | ❌ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ❌ |
 | [chat10.aichatos.xyz](https://chat10.aichatos.xyz) | `g4f.Provider.Aichatos` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
@@ -406,17 +409,34 @@
 | ----- | -------- | ----------- | ------------ | ------- |
 | Microsoft Copilot in Bing | `g4f.Provider.Bing` | dall-e-3 | gpt-4-vision | [bing.com](https://bing.com/chat) |
 | DeepInfra | `g4f.Provider.DeepInfra` | stability-ai/sdxl | llava-1.5-7b-hf | [deepinfra.com](https://deepinfra.com) |
 | Gemini | `g4f.Provider.Gemini` | ✔️ | ✔️ | [gemini.google.com](https://gemini.google.com) |
 | Gemini API | `g4f.Provider.GeminiPro` | ❌ | gemini-1.5-pro | [ai.google.dev](https://ai.google.dev) |
 | Meta AI | `g4f.Provider.MetaAI` | ✔️ | ❌ | [meta.ai](https://www.meta.ai) |
 | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) |
+| Reka | `g4f.Provider.Reka` | ❌ | ✔️ | [chat.reka.ai](https://chat.reka.ai/) |
 | Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b | [replicate.com](https://replicate.com) |
 | You.com | `g4f.Provider.You` | dall-e-3| ✔️ | [you.com](https://you.com) |
 
+```python
+from g4f.client import Client
+from g4f.Provider.GeminiPro import GeminiPro
+
+client = Client(
+    api_key="...",
+    provider=GeminiPro
+)
+response = client.chat.completions.create(
+    model="gemini-pro-vision",
+    messages=[{"role": "user", "content": "What are on this image?"}],
+    image=open("docs/waterfall.jpeg", "rb")
+)
+print(response.choices[0].message.content)
+```
+
 ## 🔗 Powered by gpt4free
 
 <table>
   <thead align="center">
     <tr border: none;>
       <td>
         <b>🎁 Projects</b>
@@ -819,19 +839,19 @@
 
 ## 🤝 Contribute
 
 We welcome contributions from the community. Whether you're adding new providers or features, or simply fixing typos and making small improvements, your input is valued. Creating a pull request is all it takes – our co-pilot will handle the code review process. Once all changes have been addressed, we'll merge the pull request into the main branch and release the updates at a later time.
 
 ###### Guide: How do i create a new Provider?
 
- - Read: [/docs/guides/create_provider](/docs/guides/create_provider.md)
+ - Read: [/docs/guides/create_provider](https://github.com/xtekky/gpt4free/blob/main/docs/guides/create_provider.md)
 
 ###### Guide: How can AI help me with writing code?
 
- - Read: [/docs/guides/help_me](/docs/guides/help_me.md)
+ - Read: [/docs/guides/help_me](https://github.com/xtekky/gpt4free/blob/main/docs/guides/help_me.md)
 
 ## 🙌 Contributors
 
 A list of all contributors is available [here](https://github.com/xtekky/gpt4free/graphs/contributors)
 
 <a href="https://github.com/xtekky" target="_blank"><img src="https://avatars.githubusercontent.com/u/98614666?v=4&s=45" width="45" title="xtekky"></a>
 <a href="https://github.com/hlohaus" target="_blank"><img src="https://avatars.githubusercontent.com/u/983577?v=4&s=45" width="45" title="hlohaus"></a>
@@ -865,19 +885,19 @@
 <a href="https://github.com/ggindinson" target="_blank"><img src="https://avatars.githubusercontent.com/u/97807772?v=4&s=45" width="45" title="ggindinson"></a>
 <span></span>
 <img src="https://avatars.githubusercontent.com/u/71154407?s=45&v=4" width="45" title="ading2210">
 <img src="https://avatars.githubusercontent.com/u/12299238?s=45&v=4" width="45" title="xqdoo00o">
 <img src="https://avatars.githubusercontent.com/u/97126670?s=45&v=4" width="45" title="nathanrchn">
 <img src="https://avatars.githubusercontent.com/u/81407603?v=4&s=45" width="45" title="dsdanielpark">
 
-- The [`Vercel.py`](g4f/Provider/Vercel.py) file contains code from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210)
-- The [`har_file.py`](g4f/Provider/openai/har_file.py) has input from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API)
-- The [`PerplexityLabs.py`](g4f/Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai)
-- The [`Gemini.py`](g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API)
-- The [`MetaAI.py`](g4f/Provider/MetaAI.py) file contains code from [meta-ai-api](https://github.com/Strvm/meta-ai-api) by [@Strvm](https://github.com/Strvm)
+- The [`Vercel.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/Vercel.py) file contains code from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210)
+- The [`har_file.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API)
+- The [`PerplexityLabs.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai)
+- The [`Gemini.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API)
+- The [`MetaAI.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/MetaAI.py) file contains code from [meta-ai-api](https://github.com/Strvm/meta-ai-api) by [@Strvm](https://github.com/Strvm)
 
 *Having input implies that the AI's code generation utilized it as one of many sources.*
 
 ## ©️ Copyright
 
 This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt)
 
@@ -909,13 +929,13 @@
 <table>
   <tr>
      <td>
        <p align="center"> <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/93/GPLv3_Logo.svg/1200px-GPLv3_Logo.svg.png" width="80%"></img>
     </td>
     <td> 
       <img src="https://img.shields.io/badge/License-GNU_GPL_v3.0-red.svg"/> <br> 
-This project is licensed under <a href="./LICENSE">GNU_GPL_v3.0</a>.
+This project is licensed under <a href="https://github.com/xtekky/gpt4free/blob/main/LICENSE">GNU_GPL_v3.0</a>.
     </td>
   </tr>
 </table>
 
 <p align="right">(<a href="#top">🔼 Back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
 ![248433934-7886223b-c1d1-4260-82aa-da5741f303bb](https://github.com/xtekky/
 gpt4free/assets/98614666/ea012c87-76e0-496a-8ac4-e2de090cc6c9)
 _[_x_t_e_k_k_y_%_2_F_g_p_t_4_f_r_e_e_ _|_ _T_r_e_n_d_s_h_i_f_t_]Written by [@xtekky](https://github.com/
 hlohaus) & maintained by [@hlohaus](https://github.com/hlohaus)
 > By using this repository or any code related to it, you agree to the [legal
-notice](LEGAL_NOTICE.md). The author is **not responsible for the usage of this
-repository nor endorses it**, nor is the author responsible for any copies,
-forks, re-uploads made by other users, or anything else related to GPT4Free.
-This is the author's only account and repository. To prevent impersonation or
-irresponsible actions, please comply with the GNU GPL license this Repository
-uses. > [!Warning] *"gpt4free"* serves as a **PoC** (proof of concept),
-demonstrating the development of an API package with multi-provider requests,
-with features like timeouts, load balance and flow control. > [!Note] LLaasstteett
-vveerrssiioonn:: [![PyPI version](https://img.shields.io/pypi/v/g4f?color=blue)](https:
-//pypi.org/project/g4f) [![Docker version](https://img.shields.io/docker/v/
-hlohaus789/g4f?label=docker&color=blue)](https://hub.docker.com/r/hlohaus789/
-g4f) > SSttaattss:: [![Downloads](https://static.pepy.tech/badge/g4f)](https://
-pepy.tech/project/g4f) [![Downloads](https://static.pepy.tech/badge/g4f/month)]
-(https://pepy.tech/project/g4f) ```sh pip install -U g4f ``` ```sh docker pull
+notice](https://github.com/xtekky/gpt4free/blob/main/LEGAL_NOTICE.md). The
+author is **not responsible for the usage of this repository nor endorses it**,
+nor is the author responsible for any copies, forks, re-uploads made by other
+users, or anything else related to GPT4Free. This is the author's only account
+and repository. To prevent impersonation or irresponsible actions, please
+comply with the GNU GPL license this Repository uses. > [!Warning] *"gpt4free"*
+serves as a **PoC** (proof of concept), demonstrating the development of an API
+package with multi-provider requests, with features like timeouts, load balance
+and flow control. > [!Note] LLaasstteett vveerrssiioonn:: [![PyPI version](https://
+img.shields.io/pypi/v/g4f?color=blue)](https://pypi.org/project/g4f) [![Docker
+version](https://img.shields.io/docker/v/hlohaus789/
+g4f?label=docker&color=blue)](https://hub.docker.com/r/hlohaus789/g4f) > SSttaattss::
+[![Downloads](https://static.pepy.tech/badge/g4f)](https://pepy.tech/project/
+g4f) [![Downloads](https://static.pepy.tech/badge/g4f/month)](https://
+pepy.tech/project/g4f) ```sh pip install -U g4f ``` ```sh docker pull
 hlohaus789/g4f ``` ## ð What's New - Installation Guide for Windows (.exe):
 ð» [#installation-guide-for-windows](#installation-guide-for-windows-exe) -
 Join our Telegram Channel: ð¨ [telegram.me/g4f_channel](https://telegram.me/
 g4f_channel) - Join our Discord Group: ð¬ [discord.gg/XfybzPXPH5](https://
 discord.gg/XfybzPXPH5) - `g4f` now supports 100% local inference: ð§  [local-
 docs](https://g4f.mintlify.app/docs/core/usage/local) ## ð» Site Takedown Is
 your site on this repository and you want to take it down? Send an email to
@@ -82,48 +83,54 @@
 Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your
 Windows Firewall settings to allow the application to operate correctly. To do
 this, access your Windows Firewall settings and allow the application. By
 following these steps, you should be able to successfully install and run the
 application on your Windows system. If you encounter any issues during the
 installation process, please refer to our Issue Tracker or try to get contact
 over Discord for assistance. Run the **Webview UI** on other Platfroms: - [/
-docs/guides/webview](/docs/webview.md) ##### Use your smartphone: Run the Web
-UI on Your Smartphone: - [/docs/guides/phone](/docs/guides/phone.md) #### Use
-python ##### Prerequisites: 1. [Download and install Python](https://
-www.python.org/downloads/) (Version 3.10+ is recommended). 2. [Install Google
-Chrome](https://www.google.com/chrome/) for providers with webdriver #####
-Install using PyPI package: ``` pip install -U g4f[all] ``` How do I install
-only parts or do disable parts? Use partial requirements: [/docs/requirements]
-(/docs/requirements.md) ##### Install from source: How do I load the project
-using git and installing the project requirements? Read this tutorial and
-follow it step by step: [/docs/git](/docs/git.md) ##### Install using Docker:
-How do I build and run composer image from source? Use docker-compose: [/docs/
-docker](/docs/docker.md) ## ð¡ Usage #### Text Generation ```python from
+docs/guides/webview](https://github.com/xtekky/gpt4free/blob/main/docs/
+webview.md) ##### Use your smartphone: Run the Web UI on Your Smartphone: - [/
+docs/guides/phone](https://github.com/xtekky/gpt4free/blob/main/docs/guides/
+phone.md) #### Use python ##### Prerequisites: 1. [Download and install Python]
+(https://www.python.org/downloads/) (Version 3.10+ is recommended). 2. [Install
+Google Chrome](https://www.google.com/chrome/) for providers with webdriver
+##### Install using PyPI package: ``` pip install -U g4f[all] ``` How do I
+install only parts or do disable parts? Use partial requirements: [/docs/
+requirements](https://github.com/xtekky/gpt4free/blob/main/docs/
+requirements.md) ##### Install from source: How do I load the project using git
+and installing the project requirements? Read this tutorial and follow it step
+by step: [/docs/git](https://github.com/xtekky/gpt4free/blob/main/docs/git.md)
+##### Install using Docker: How do I build and run composer image from source?
+Use docker-compose: [/docs/docker](https://github.com/xtekky/gpt4free/blob/
+main/docs/docker.md) ## ð¡ Usage #### Text Generation ```python from
 g4f.client import Client client = Client() response =
 client.chat.completions.create( model="gpt-3.5-turbo", messages=[{"role":
 "user", "content": "Hello"}], ... ) print(response.choices[0].message.content)
 ``` ``` Hello! How can I assist you today? ``` #### Image Generation ```python
 from g4f.client import Client client = Client() response =
 client.images.generate( model="gemini", prompt="a white siamese cat", ... )
-image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](/docs/
-client.md) **Full Documentation for Python API** - New AsyncClient API from
-G4F: [/docs/async_client](/docs/async_client.md) - Client API like the OpenAI
-Python library: [/docs/client](/docs/client.md) - Legacy API with python
-modules: [/docs/legacy](/docs/legacy.md) #### Web UI To start the web
-interface, type the following codes in python: ```python from g4f.gui import
-run_gui run_gui() ``` or execute the following command: ```bash python -
-m g4f.cli gui -port 8080 -debug ``` #### Interference API You can use the
-Interference API to serve other OpenAI integrations with G4F. See docs: [/docs/
-interference](/docs/interference.md) Access with: http://localhost:1337/v1 ###
-Configuration #### Cookies Cookies are essential for using Meta AI and
-Microsoft Designer to create images. Additionally, cookies are required for the
-Google Gemini and WhiteRabbitNeo Provider. From Bing, ensure you have the "_U"
-cookie, and from Google, all cookies starting with "__Secure-1PSID" are needed.
-You can pass these cookies directly to the create function or set them using
-the `set_cookies` method before running G4F: ```python from g4f.cookies import
+image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](https:
+//github.com/xtekky/gpt4free/blob/main/docs/client.md) **Full Documentation for
+Python API** - New AsyncClient API from G4F: [/docs/async_client](https://
+github.com/xtekky/gpt4free/blob/main/docs/async_client.md) - Client API like
+the OpenAI Python library: [/docs/client](https://github.com/xtekky/gpt4free/
+blob/main/docs/client.md) - Legacy API with python modules: [/docs/legacy]
+(https://github.com/xtekky/gpt4free/blob/main/docs/legacy.md) #### Web UI To
+start the web interface, type the following codes in python: ```python from
+g4f.gui import run_gui run_gui() ``` or execute the following command: ```bash
+python -m g4f.cli gui -port 8080 -debug ``` #### Interference API You can use
+the Interference API to serve other OpenAI integrations with G4F. See docs: [/
+docs/interference](https://github.com/xtekky/gpt4free/blob/main/docs/
+interference.md) Access with: http://localhost:1337/v1 ### Configuration ####
+Cookies Cookies are essential for using Meta AI and Microsoft Designer to
+create images. Additionally, cookies are required for the Google Gemini and
+WhiteRabbitNeo Provider. From Bing, ensure you have the "_U" cookie, and from
+Google, all cookies starting with "__Secure-1PSID" are needed. You can pass
+these cookies directly to the create function or set them using the
+`set_cookies` method before running G4F: ```python from g4f.cookies import
 set_cookies set_cookies(".bing.com", { "_U": "cookie value" }) set_cookies
 (".google.com", { "__Secure-1PSID": "cookie value" }) ``` Alternatively, you
 can place your .har and cookie files in the `/har_and_cookies` directory. To
 export a cookie file, use the EditThisCookie extension available on the Chrome
 Web Store: [EditThisCookie Extension](https://chromewebstore.google.com/detail/
 editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg). You can also create .har
 files to capture cookies. If you need further assistance, refer to the next
@@ -165,37 +172,42 @@
 beta.theb.ai) | `g4f.Provider.Theb` | âï¸ | âï¸ | âï¸ | ![Unknown]
 (https://img.shields.io/badge/Unknown-grey) | â | | [you.com](https://
 you.com) | `g4f.Provider.You` | âï¸ | âï¸ | âï¸ | ![Active](https://
 img.shields.io/badge/Active-brightgreen) | â | ## Best OpenSource Models
 While we wait for gpt-5, here is a list of new models that are at least better
 than gpt-3.5-turbo. **Some are better than gpt-4**. Expect this list to grow. |
 Website | Provider | parameters | better than | | ------ | ------- | ------ | -
------ | | [mixtral-8x22b](https://huggingface.co/mistral-community/Mixtral-
-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-turbo | |
-[dbrx-instruct](https://www.databricks.com/blog/introducing-dbrx-new-state-art-
-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active| gpt-3.5-turbo | |
-[command-r+](https://txt.cohere.com/command-r-plus-microsoft-azure/) |
-`g4f.Provider.HuggingChat` | 104B | gpt-4-0613 | ### GPT-3.5 | Website |
-Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | ------ | ------- | ----
---- | ----- | ------ | ------ | ---- | | [chat3.aiyunos.top](https://
-chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | âï¸ | â | âï¸ | !
+----- | | [claude-3-opus](https://anthropic.com/) | `g4f.Provider.You` | ?B |
+gpt-4-0125-preview | | [command-r+](https://txt.cohere.com/command-r-plus-
+microsoft-azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0314 | | [llama-
+3-70b](https://meta.ai/) | `g4f.Provider.Llama` or `DeepInfra` | 70B | gpt-4-
+0314 | | [claude-3-sonnet](https://anthropic.com/) | `g4f.Provider.You` | ?B |
+gpt-4-0314 | | [reka-core](https://chat.reka.ai/) | `g4f.Provider.Reka` | 21B |
+gpt-4-vision | | [dbrx-instruct](https://www.databricks.com/blog/introducing-
+dbrx-new-state-art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active|
+gpt-3.5-turbo | | [mixtral-8x22b](https://huggingface.co/mistral-community/
+Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-
+turbo | ### GPT-3.5 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status |
+Auth | | ------ | ------- | ------- | ----- | ------ | ------ | ---- | |
+[chat3.aiyunos.top](https://chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace`
+| âï¸ | â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey)
+| â | | [chat10.aichatos.xyz](https://chat10.aichatos.xyz) |
+`g4f.Provider.Aichatos` | âï¸ | â | âï¸ | ![Active](https://
+img.shields.io/badge/Active-brightgreen) | â | | [chatforai.store](https://
+chatforai.store) | `g4f.Provider.ChatForAi` | âï¸ | â | âï¸ | !
 [Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
-[chat10.aichatos.xyz](https://chat10.aichatos.xyz) | `g4f.Provider.Aichatos` |
-âï¸ | â | âï¸ | ![Active](https://img.shields.io/badge/Active-
-brightgreen) | â | | [chatforai.store](https://chatforai.store) |
-`g4f.Provider.ChatForAi` | âï¸ | â | âï¸ | ![Unknown](https://
-img.shields.io/badge/Unknown-grey) | â | | [chatgpt4online.org](https://
-chatgpt4online.org) | `g4f.Provider.Chatgpt4Online` | âï¸ | â | âï¸ | !
-[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [chatgpt-
-free.cc](https://www.chatgpt-free.cc) | `g4f.Provider.ChatgptNext` | âï¸ |
-â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
-[chatgptx.de](https://chatgptx.de) | `g4f.Provider.ChatgptX` | âï¸ | â |
-âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
-[f1.cnote.top](https://f1.cnote.top) | `g4f.Provider.Cnote` | âï¸ | â |
-âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) | â | |
+[chatgpt4online.org](https://chatgpt4online.org) |
+`g4f.Provider.Chatgpt4Online` | âï¸ | â | âï¸ | ![Unknown](https://
+img.shields.io/badge/Unknown-grey) | â | | [chatgpt-free.cc](https://
+www.chatgpt-free.cc) | `g4f.Provider.ChatgptNext` | âï¸ | â | âï¸ | !
+[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [chatgptx.de]
+(https://chatgptx.de) | `g4f.Provider.ChatgptX` | âï¸ | â | âï¸ | !
+[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [f1.cnote.top]
+(https://f1.cnote.top) | `g4f.Provider.Cnote` | âï¸ | â | âï¸ | !
+[Active](https://img.shields.io/badge/Active-brightgreen) | â | |
 [duckduckgo.com](https://duckduckgo.com/duckchat) | `g4f.Provider.DuckDuckGo` |
 âï¸ | â | âï¸ | ![Active](https://img.shields.io/badge/Active-
 brightgreen) | â | | [ecosia.org](https://www.ecosia.org) |
 `g4f.Provider.Ecosia` | âï¸ | â | âï¸ | ![Active](https://
 img.shields.io/badge/Active-brightgreen) | â | | [feedough.com](https://
 www.feedough.com) | `g4f.Provider.Feedough` | âï¸ | â | âï¸ | ![Active]
 (https://img.shields.io/badge/Active-brightgreen) | â | | [flowgpt.com]
@@ -329,18 +341,24 @@
 gpt-4-vision | [bing.com](https://bing.com/chat) | | DeepInfra |
 `g4f.Provider.DeepInfra` | stability-ai/sdxl | llava-1.5-7b-hf |
 [deepinfra.com](https://deepinfra.com) | | Gemini | `g4f.Provider.Gemini` |
 âï¸ | âï¸ | [gemini.google.com](https://gemini.google.com) | | Gemini API
 | `g4f.Provider.GeminiPro` | â | gemini-1.5-pro | [ai.google.dev](https://
 ai.google.dev) | | Meta AI | `g4f.Provider.MetaAI` | âï¸ | â | [meta.ai]
 (https://www.meta.ai) | | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-
-3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) | | Replicate |
-`g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b | [replicate.com]
-(https://replicate.com) | | You.com | `g4f.Provider.You` | dall-e-3| âï¸ |
-[you.com](https://you.com) | ## ð Powered by gpt4free
+3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) | | Reka |
+`g4f.Provider.Reka` | â | âï¸ | [chat.reka.ai](https://chat.reka.ai/) | |
+Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b |
+[replicate.com](https://replicate.com) | | You.com | `g4f.Provider.You` | dall-
+e-3| âï¸ | [you.com](https://you.com) | ```python from g4f.client import
+Client from g4f.Provider.GeminiPro import GeminiPro client = Client
+( api_key="...", provider=GeminiPro ) response = client.chat.completions.create
+( model="gemini-pro-vision", messages=[{"role": "user", "content": "What are on
+this image?"}], image=open("docs/waterfall.jpeg", "rb") ) print
+(response.choices[0].message.content) ``` ## ð Powered by gpt4free
 ?ð??? PPrroojjeeccttss             ?â?­? SSttaarrss ?ð??? FFoorrkkss ?ð??? IIssssuueess ?ð???¬ PPuullll rreeqquueessttss
 _gg_pp_tt_44_ff_rr_ee_ee                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _FF_rr_ee_ee_ _AA_II_ _AA_PP_II_''_ss_ _&&_ _PP_oo_tt_ee_nn_tt_ii_aa_ll _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _PP_rr_oo_vv_ii_dd_ee_rr_ss_ _LL_ii_ss_tt
 _CC_hh_aa_tt_GG_PP_TT_--_CC_ll_oo_nn_ee             _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _AA_ii_ _aa_gg_ee_nn_tt                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _CC_hh_aa_tt_GG_pp_tt_ _DD_ii_ss_cc_oo_rr_dd_ _BB_oo_tt       _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
@@ -354,19 +372,20 @@
 _pp_yy_tt_hh_oo_nn_--_tt_gg_pp_tt               _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 ## ð¤ Contribute We welcome contributions from the community. Whether you're
 adding new providers or features, or simply fixing typos and making small
 improvements, your input is valued. Creating a pull request is all it takes â
 our co-pilot will handle the code review process. Once all changes have been
 addressed, we'll merge the pull request into the main branch and release the
 updates at a later time. ###### Guide: How do i create a new Provider? - Read:
-[/docs/guides/create_provider](/docs/guides/create_provider.md) ###### Guide:
-How can AI help me with writing code? - Read: [/docs/guides/help_me](/docs/
-guides/help_me.md) ## ð Contributors A list of all contributors is available
-[here](https://github.com/xtekky/gpt4free/graphs/contributors) _[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_6_1_4_6_6_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+[/docs/guides/create_provider](https://github.com/xtekky/gpt4free/blob/main/
+docs/guides/create_provider.md) ###### Guide: How can AI help me with writing
+code? - Read: [/docs/guides/help_me](https://github.com/xtekky/gpt4free/blob/
+main/docs/guides/help_me.md) ## ð Contributors A list of all contributors is
+available [here](https://github.com/xtekky/gpt4free/graphs/contributors)
+_[_h_t_t_p_s_:_/_/_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_6_1_4_6_6_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_3_5_7_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_8_3_0_5_3_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_4_1_5_4_6_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_9_6_6_2_2_8_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_0_5_1_6_0_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_0_5_8_5_2_3_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_3_4_8_5_4_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
@@ -391,36 +410,39 @@
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_7_6_3_6_0_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_5_6_6_3_2_2_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_9_3_2_2_7_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_7_8_0_7_7_7_2_?_v_=_4_&_s_=_4_5_][https://
 avatars.githubusercontent.com/u/71154407?s=45&v=4][https://
 avatars.githubusercontent.com/u/12299238?s=45&v=4][https://
 avatars.githubusercontent.com/u/97126670?s=45&v=4][https://
-avatars.githubusercontent.com/u/81407603?v=4&s=45]- The [`Vercel.py`](g4f/
-Provider/Vercel.py) file contains code from [vercel-llm-api](https://
-github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/
-ading2210) - The [`har_file.py`](g4f/Provider/openai/har_file.py) has input
+avatars.githubusercontent.com/u/81407603?v=4&s=45]- The [`Vercel.py`](https://
+github.com/xtekky/gpt4free/blob/main/g4f/Provider/Vercel.py) file contains code
+from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by
+[@ading2210](https://github.com/ading2210) - The [`har_file.py`](https://
+github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input
 from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API) -
-The [`PerplexityLabs.py`](g4f/Provider/openai/har_file.py) has input from
-[nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai) - The
-[`Gemini.py`](g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/
-Gemini-API](https://github.com/dsdanielpark/Gemini-API) - The [`MetaAI.py`]
-(g4f/Provider/MetaAI.py) file contains code from [meta-ai-api](https://
-github.com/Strvm/meta-ai-api) by [@Strvm](https://github.com/Strvm) *Having
-input implies that the AI's code generation utilized it as one of many
-sources.* ## Â©ï¸ Copyright This program is licensed under the [GNU GPL v3]
-(https://www.gnu.org/licenses/gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C)
-2023 xtekky This program is free software: you can redistribute it and/or
-modify it under the terms of the GNU General Public License as published by the
-Free Software Foundation, either version 3 of the License, or (at your option)
-any later version. This program is distributed in the hope that it will be
-useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public
-License for more details. You should have received a copy of the GNU General
-Public License along with this program. If not, see
+The [`PerplexityLabs.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/
+Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://
+github.com/nathanrchn/perplexityai) - The [`Gemini.py`](https://github.com/
+xtekky/gpt4free/blob/main/g4f/Provider/needs_auth/Gemini.py) has input from
+[dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API) - The
+[`MetaAI.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/
+MetaAI.py) file contains code from [meta-ai-api](https://github.com/Strvm/meta-
+ai-api) by [@Strvm](https://github.com/Strvm) *Having input implies that the
+AI's code generation utilized it as one of many sources.* ## Â©ï¸ Copyright
+This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/
+gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C) 2023 xtekky This program is
+free software: you can redistribute it and/or modify it under the terms of the
+GNU General Public License as published by the Free Software Foundation, either
+version 3 of the License, or (at your option) any later version. This program
+is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+PARTICULAR PURPOSE. See the GNU General Public License for more details. You
+should have received a copy of the GNU General Public License along with this
+program. If not, see
 www.gnu.org/licenses/>. ``` ## â­ Star History _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]## ð
 License
 [https://upload.wikimedia.org/wikipedia/ [https://img.shields.io/badge/License-
    commons/thumb/9/93/GPLv3_Logo.svg/    GNU_GPL_v3.0-red.svg]
        1200px-GPLv3_Logo.svg.png]        This project is licensed under
                                          _G_N_U___G_P_L___v_3_._0.
                                                              (_ð___¼_ _B_a_c_k_ _t_o_ _t_o_p)
```

### Comparing `g4f-0.3.0.6/g4f/Provider/Aichatos.py` & `g4f-0.3.0.7/g4f/Provider/Aichatos.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/Aura.py` & `g4f-0.3.0.7/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/Bing.py` & `g4f-0.3.0.7/g4f/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/BingCreateImages.py` & `g4f-0.3.0.7/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/Blackbox.py` & `g4f-0.3.0.7/g4f/Provider/Blackbox.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/ChatForAi.py` & `g4f-0.3.0.7/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/Chatgpt4Online.py` & `g4f-0.3.0.7/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/ChatgptAi.py` & `g4f-0.3.0.7/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/ChatgptFree.py` & `g4f-0.3.0.7/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/ChatgptNext.py` & `g4f-0.3.0.7/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/ChatgptX.py` & `g4f-0.3.0.7/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/Cnote.py` & `g4f-0.3.0.7/g4f/Provider/Cnote.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/Cohere.py` & `g4f-0.3.0.7/g4f/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/DeepInfra.py` & `g4f-0.3.0.7/g4f/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/DeepInfraImage.py` & `g4f-0.3.0.7/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/DuckDuckGo.py` & `g4f-0.3.0.7/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/Ecosia.py` & `g4f-0.3.0.7/g4f/Provider/Ecosia.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/Feedough.py` & `g4f-0.3.0.7/g4f/Provider/Feedough.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/FlowGpt.py` & `g4f-0.3.0.7/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/FreeChatgpt.py` & `g4f-0.3.0.7/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/FreeGpt.py` & `g4f-0.3.0.7/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/GeminiPro.py` & `g4f-0.3.0.7/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/GeminiProChat.py` & `g4f-0.3.0.7/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/GigaChat.py` & `g4f-0.3.0.7/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/GptTalkRu.py` & `g4f-0.3.0.7/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/HuggingChat.py` & `g4f-0.3.0.7/g4f/Provider/HuggingChat.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     models = [
         "HuggingFaceH4/zephyr-orpo-141b-A35b-v0.1",
         'CohereForAI/c4ai-command-r-plus',
         'mistralai/Mixtral-8x7B-Instruct-v0.1',
         'google/gemma-1.1-7b-it',
         'NousResearch/Nous-Hermes-2-Mixtral-8x7B-DPO',
         'mistralai/Mistral-7B-Instruct-v0.2',
-        'meta-llama/Meta-Llama-3-70B-Instruct'
+        'meta-llama/Meta-Llama-3-70B-Instruct',
+        'microsoft/Phi-3-mini-4k-instruct'
     ]
     model_aliases = {
         "mistralai/Mistral-7B-Instruct-v0.1": "mistralai/Mistral-7B-Instruct-v0.2"
     }
 
     @classmethod
     def get_models(cls):
@@ -108,8 +109,8 @@
                         break
             if delete_conversation:
                 async with session.delete(f"{cls.url}/conversation/{conversation_id}") as response:
                     await raise_for_status(response)
 
 class Conversation(BaseConversation):
     def __init__(self, conversation_id: str) -> None:
-        self.conversation_id = conversation_id
+        self.conversation_id = conversation_id
```

### Comparing `g4f-0.3.0.6/g4f/Provider/HuggingFace.py` & `g4f-0.3.0.7/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/Koala.py` & `g4f-0.3.0.7/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/Liaobots.py` & `g4f-0.3.0.7/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/Llama.py` & `g4f-0.3.0.7/g4f/Provider/Llama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/Local.py` & `g4f-0.3.0.7/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/MetaAI.py` & `g4f-0.3.0.7/g4f/Provider/MetaAI.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/MetaAIAccount.py` & `g4f-0.3.0.7/g4f/Provider/MetaAIAccount.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/PerplexityLabs.py` & `g4f-0.3.0.7/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/Pi.py` & `g4f-0.3.0.7/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/Replicate.py` & `g4f-0.3.0.7/g4f/Provider/Replicate.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/ReplicateImage.py` & `g4f-0.3.0.7/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/Vercel.py` & `g4f-0.3.0.7/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.3.0.7/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/You.py` & `g4f-0.3.0.7/g4f/Provider/You.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/__init__.py` & `g4f-0.3.0.7/g4f/Provider/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 from .PerplexityLabs   import PerplexityLabs
 from .Pi               import Pi
 from .Replicate        import Replicate
 from .ReplicateImage   import ReplicateImage
 from .Vercel           import Vercel
 from .WhiteRabbitNeo   import WhiteRabbitNeo
 from .You              import You
+from .Reka             import Reka
 
 import sys
 
 __modules__: list = [
     getattr(sys.modules[__name__], provider) for provider in dir()
     if not provider.startswith("__")
 ]
```

### Comparing `g4f-0.3.0.6/g4f/Provider/bing/conversation.py` & `g4f-0.3.0.7/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/bing/create_images.py` & `g4f-0.3.0.7/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/bing/upload_image.py` & `g4f-0.3.0.7/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/AiService.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Aibn.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Aichat.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Ails.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Berlin.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Equing.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Forefront.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/H2o.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Myshell.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Phind.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/V50.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Vercel.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/deprecated/__init__.py` & `g4f-0.3.0.7/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.3.0.7/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.3.0.7/g4f/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/needs_auth/Groq.py` & `g4f-0.3.0.7/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.3.0.7/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/needs_auth/Openai.py` & `g4f-0.3.0.7/g4f/Provider/needs_auth/Openai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.3.0.7/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,39 @@
     from selenium.webdriver.support import expected_conditions as EC
 except ImportError:
     pass
 
 from ..base_provider import AsyncGeneratorProvider, ProviderModelMixin
 from ...webdriver import get_browser
 from ...typing import AsyncResult, Messages, Cookies, ImageType, AsyncIterator
-from ...requests import DEFAULT_HEADERS, get_args_from_browser, raise_for_status
+from ...requests import get_args_from_browser, raise_for_status
 from ...requests.aiohttp import StreamSession
 from ...image import to_image, to_bytes, ImageResponse, ImageRequest
 from ...errors import MissingAuthError, ResponseError
 from ...providers.conversation import BaseConversation
 from ..helper import format_cookies
 from ..openai.har_file import getArkoseAndAccessToken, NoValidHarFileError
+from ..openai.proofofwork import generate_proof_token
 from ... import debug
 
+DEFAULT_HEADERS = {
+    "accept": "*/*",
+    "accept-encoding": "gzip, deflate, br, zstd",
+    "accept-language": "en-US,en;q=0.5",
+    "referer": "https://chat.openai.com/",
+    "sec-ch-ua": "\"Brave\";v=\"123\", \"Not:A-Brand\";v=\"8\", \"Chromium\";v=\"123\"",
+    "sec-ch-ua-mobile": "?0",
+    "sec-ch-ua-platform": "\"Windows\"",
+    "sec-fetch-dest": "empty",
+    "sec-fetch-mode": "cors",
+    "sec-fetch-site": "same-origin",
+    "sec-gpc": "1",
+    "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36"
+}
+
 class OpenaiChat(AsyncGeneratorProvider, ProviderModelMixin):
     """A class for creating and managing conversations with OpenAI chat service"""
 
     label = "OpenAI ChatGPT"
     url = "https://chat.openai.com"
     working = True
     supports_gpt_35_turbo = True
@@ -351,19 +367,29 @@
             if cls._headers is None or cookies is not None:
                 cls._create_request_args(cookies)
             api_key = kwargs["access_token"] if "access_token" in kwargs else api_key
             if api_key is not None:
                 cls._set_api_key(api_key)
 
             if cls.default_model is None and (not cls.needs_auth or cls._api_key is not None):
+                if cls._api_key is None:
+                    cls._create_request_args(cookies)
+                    async with session.get(
+                        f"{cls.url}/",
+                        headers=DEFAULT_HEADERS
+                    ) as response:
+                        cls._update_request_args(session)
+                        await raise_for_status(response)
                 try:
                     if not model:
                         cls.default_model = cls.get_model(await cls.get_default_model(session, cls._headers))
                     else:
                         cls.default_model = cls.get_model(model)
+                except MissingAuthError:
+                    pass
                 except Exception as e:
                     api_key = cls._api_key = None
                     cls._create_request_args()
                     if debug.logging:
                         print("OpenaiChat: Load default model failed")
                         print(f"{e.__class__.__name__}: {e}")
 
@@ -391,24 +417,31 @@
             ) as response:
                 cls._update_request_args(session)
                 await raise_for_status(response)
                 data = await response.json()
                 blob = data["arkose"]["dx"]
                 need_arkose = data["arkose"]["required"]
                 chat_token = data["token"]
-
-                if debug.logging:
-                    print(f'Arkose: {need_arkose} Turnstile: {data["turnstile"]["required"]}')
+                proofofwork = ""
+                if "proofofwork" in data:
+                    proofofwork = generate_proof_token(**data["proofofwork"], user_agent=cls._headers["user-agent"])
 
             if need_arkose and arkose_token is None:
                 arkose_token, api_key, cookies, headers = await getArkoseAndAccessToken(proxy)
                 cls._create_request_args(cookies, headers)
                 cls._set_api_key(api_key)
                 if arkose_token is None:
                     raise MissingAuthError("No arkose token found in .har file")
+                            
+            if debug.logging:
+                print(
+                    'Arkose:', False if not need_arkose else arkose_token[:12]+"...",
+                    'Turnstile:', data["turnstile"]["required"],
+                    'Proofofwork:', False if proofofwork is None else proofofwork[:12]+"...",
+                )
 
             try:
                 image_request = await cls.upload_image(session, cls._headers, image, image_name) if image else None
             except Exception as e:
                 if debug.logging:
                     print("OpenaiChat: Upload image failed")
                     print(f"{e.__class__.__name__}: {e}")
@@ -435,20 +468,22 @@
                     "history_and_training_disabled": history_disabled and not auto_continue and not return_conversation,
                     "websocket_request_id": websocket_request_id
                 }
                 if action != "continue":
                     messages = messages if conversation_id is None else [messages[-1]]
                     data["messages"] = cls.create_messages(messages, image_request)
                 headers = {
-                    "Accept": "text/event-stream",
-                    "OpenAI-Sentinel-Chat-Requirements-Token": chat_token,
+                    "accept": "text/event-stream",
+                    "Openai-Sentinel-Chat-Requirements-Token": chat_token,
                     **cls._headers
                 }
                 if need_arkose:
-                    headers["OpenAI-Sentinel-Arkose-Token"] = arkose_token
+                    headers["Openai-Sentinel-Arkose-Token"] = arkose_token
+                if proofofwork is not None:
+                    headers["Openai-Sentinel-Proof-Token"] = proofofwork
                 async with session.post(
                     f"{cls.url}/backend-anon/conversation" if cls._api_key is None else
                     f"{cls.url}/backend-api/conversation",
                     json=data,
                     headers=headers
                 ) as response:
                     cls._update_request_args(session)
@@ -667,16 +702,14 @@
                     return data["accessToken"]
 
     @staticmethod
     def get_default_headers() -> dict:
         return {
             **DEFAULT_HEADERS,
             "content-type": "application/json",
-            "oai-device-id": str(uuid.uuid4()),
-            "oai-language": "en-US",
         }
 
     @classmethod
     def _create_request_args(cls, cookies: Cookies = None, headers: dict = None, user_agent: str = None):
         cls._headers = cls.get_default_headers() if headers is None else headers
         if user_agent is not None:
             cls._headers["user-agent"] = user_agent
@@ -694,14 +727,16 @@
         cls._api_key = api_key
         cls._expires = int(time.time()) + 60 * 60 * 4
         cls._headers["authorization"] = f"Bearer {api_key}"
 
     @classmethod
     def _update_cookie_header(cls):
         cls._headers["cookie"] = format_cookies(cls._cookies)
+        if "oai-did" in cls._cookies:
+            cls._headers["oai-device-id"] = cls._cookies["oai-did"]
 
 class Conversation(BaseConversation):
     """
     Class to encapsulate response fields.
     """
     def __init__(self, conversation_id: str = None, message_id: str = None, finish_reason: str = None):
         self.conversation_id = conversation_id
```

### Comparing `g4f-0.3.0.6/g4f/Provider/needs_auth/Poe.py` & `g4f-0.3.0.7/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.3.0.7/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/needs_auth/Theb.py` & `g4f-0.3.0.7/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.3.0.7/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/not_working/AItianhu.py` & `g4f-0.3.0.7/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/not_working/Bestim.py` & `g4f-0.3.0.7/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/not_working/ChatBase.py` & `g4f-0.3.0.7/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.3.0.7/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.3.0.7/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.3.0.7/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.3.0.7/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/not_working/Gpt6.py` & `g4f-0.3.0.7/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/not_working/GptChatly.py` & `g4f-0.3.0.7/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/not_working/GptForLove.py` & `g4f-0.3.0.7/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/not_working/GptGo.py` & `g4f-0.3.0.7/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/not_working/GptGod.py` & `g4f-0.3.0.7/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.3.0.7/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.3.0.7/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.3.0.7/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/npm/package-lock.json` & `g4f-0.3.0.7/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/openai/crypt.py` & `g4f-0.3.0.7/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/openai/har_file.py` & `g4f-0.3.0.7/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.3.0.7/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/selenium/Bard.py` & `g4f-0.3.0.7/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/selenium/MyShell.py` & `g4f-0.3.0.7/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.3.0.7/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/selenium/Phind.py` & `g4f-0.3.0.7/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/selenium/TalkAi.py` & `g4f-0.3.0.7/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.3.0.7/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.3.0.7/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/unfinished/Komo.py` & `g4f-0.3.0.7/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.3.0.7/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/Provider/you/har_file.py` & `g4f-0.3.0.7/g4f/Provider/you/har_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,24 +81,25 @@
             print(e)
     if debug.logging:
         print('Getting telemetry_id for you.com with nodriver')
     try:
         from nodriver import start
     except ImportError:
         raise MissingRequirementsError('Add .har file from you.com or install "nodriver" package | pip install -U nodriver')
+    page = None
     try:
         browser = await start()
-        tab = browser.main_tab
-        await browser.get("https://you.com")
+        page = await browser.get("https://you.com")
 
-        while not await tab.evaluate('"GetTelemetryID" in this'):
-            await tab.sleep(1)
+        while not await page.evaluate('"GetTelemetryID" in this'):
+            await page.sleep(1)
 
         async def get_telemetry_id():
-            return await tab.evaluate(
+            return await page.evaluate(
                 f'this.GetTelemetryID("{public_token}", "{telemetry_url}");',
                 await_promise=True
             )
 
-        return [await get_telemetry_id() for _ in range(1)]
+        return [await get_telemetry_id()]
     finally:
-        await tab.close()
+        if page is not None:
+            await page.close()
```

### Comparing `g4f-0.3.0.6/g4f/__init__.py` & `g4f-0.3.0.7/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/api/__init__.py` & `g4f-0.3.0.7/g4f/api/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from __future__ import annotations
 
 import logging
 import json
 import uvicorn
+import secrets
 
 from fastapi import FastAPI, Response, Request
 from fastapi.responses import StreamingResponse, RedirectResponse, HTMLResponse, JSONResponse
 from fastapi.exceptions import RequestValidationError
-from starlette.status import HTTP_422_UNPROCESSABLE_ENTITY
+from fastapi.security import APIKeyHeader
+from starlette.exceptions import HTTPException
+from starlette.status import HTTP_422_UNPROCESSABLE_ENTITY, HTTP_401_UNAUTHORIZED, HTTP_403_FORBIDDEN
 from fastapi.encoders import jsonable_encoder
 from pydantic import BaseModel
 from typing import Union, Optional
 
 import g4f
 import g4f.debug
 from g4f.client import AsyncClient
 from g4f.typing import Messages
 
-def create_app() -> FastAPI:
+def create_app(g4f_api_key:str = None):
     app = FastAPI()
-    api = Api(app)
+    api = Api(app, g4f_api_key=g4f_api_key)
     api.register_routes()
+    api.register_authorization()
     api.register_validation_exception_handler()
     return app
 
 class ChatCompletionsConfig(BaseModel):
     messages: Messages
     model: str
     provider: Optional[str] = None
@@ -39,17 +43,40 @@
 list_ignored_providers: list[str] = None
 
 def set_list_ignored_providers(ignored: list[str]):
     global list_ignored_providers
     list_ignored_providers = ignored
 
 class Api:
-    def __init__(self, app: FastAPI) -> None:
+    def __init__(self, app: FastAPI, g4f_api_key=None) -> None:
         self.app = app
         self.client = AsyncClient()
+        self.g4f_api_key = g4f_api_key
+        self.get_g4f_api_key = APIKeyHeader(name="g4f-api-key")
+
+    def register_authorization(self):
+        @self.app.middleware("http")
+        async def authorization(request: Request, call_next):
+            if self.g4f_api_key and request.url.path in ["/v1/chat/completions", "/v1/completions"]:
+                try:
+                    user_g4f_api_key = await self.get_g4f_api_key(request)
+                except HTTPException as e:
+                    if e.status_code == 403:
+                        return JSONResponse(
+                            status_code=HTTP_401_UNAUTHORIZED,
+                            content=jsonable_encoder({"detail": "G4F API key required"}),
+                        )
+                if not secrets.compare_digest(self.g4f_api_key, user_g4f_api_key):
+                    return JSONResponse(
+                    status_code=HTTP_403_FORBIDDEN,
+                    content=jsonable_encoder({"detail": "Invalid G4F API key"}),
+                )
+            
+            response = await call_next(request)
+            return response
 
     def register_validation_exception_handler(self):
         @self.app.exception_handler(RequestValidationError)
         async def validation_exception_handler(request: Request, exc: RequestValidationError):
             details = exc.errors()
             modified_details = []
             for error in details:
@@ -149,17 +176,18 @@
 
 def run_api(
     host: str = '0.0.0.0',
     port: int = 1337,
     bind: str = None,
     debug: bool = False,
     workers: int = None,
-    use_colors: bool = None
+    use_colors: bool = None,
+    g4f_api_key: str = None
 ) -> None:
     print(f'Starting server... [g4f v-{g4f.version.utils.current_version}]' + (" (debug)" if debug else ""))
     if use_colors is None:
         use_colors = debug
     if bind is not None:
         host, port = bind.split(":")
     if debug:
         g4f.debug.logging = True
-    uvicorn.run("g4f.api:create_app", host=host, port=int(port), workers=workers, use_colors=use_colors, factory=True)#
+    uvicorn.run(create_app(g4f_api_key), host=host, port=int(port), workers=workers, use_colors=use_colors)
```

### Comparing `g4f-0.3.0.6/g4f/api/_logging.py` & `g4f-0.3.0.7/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/cli.py` & `g4f-0.3.0.7/g4f/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     subparsers = parser.add_subparsers(dest="mode", help="Mode to run the g4f in.")
     api_parser = subparsers.add_parser("api")
     api_parser.add_argument("--bind", default="0.0.0.0:1337", help="The bind string.")
     api_parser.add_argument("--debug", action="store_true", help="Enable verbose logging.")
     api_parser.add_argument("--workers", type=int, default=None, help="Number of workers.")
     api_parser.add_argument("--disable-colors", action="store_true", help="Don't use colors.")
     api_parser.add_argument("--ignore-cookie-files", action="store_true", help="Don't read .har and cookie files.")
+    api_parser.add_argument("--g4f-api-key", type=str, default=None, help="Sets an authentication key for your API.")
     api_parser.add_argument("--ignored-providers", nargs="+", choices=[provider for provider in Provider.__map__],
                             default=[], help="List of providers to ignore when processing request.")
     subparsers.add_parser("gui", parents=[gui_parser()], add_help=False)
 
     args = parser.parse_args()
     if args.mode == "api":
         run_api_args(args)
@@ -38,12 +39,13 @@
     g4f.api.set_list_ignored_providers(
         args.ignored_providers
     )
     g4f.api.run_api(
         bind=args.bind,
         debug=args.debug,
         workers=args.workers,
+        g4f_api_key=args.g4f_api_key,
         use_colors=not args.disable_colors
     )
 
 if __name__ == "__main__":
     main()
```

### Comparing `g4f-0.3.0.6/g4f/client/async_client.py` & `g4f-0.3.0.7/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/client/client.py` & `g4f-0.3.0.7/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/client/helper.py` & `g4f-0.3.0.7/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/client/image_models.py` & `g4f-0.3.0.7/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/client/service.py` & `g4f-0.3.0.7/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/client/stubs.py` & `g4f-0.3.0.7/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/client/types.py` & `g4f-0.3.0.7/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/cookies.py` & `g4f-0.3.0.7/g4f/cookies.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 _cookies: Dict[str, Cookies] = {}
 
 DOMAINS = [
     ".bing.com",
     ".meta.ai",
     ".google.com",
     "www.whiterabbitneo.com",
-    "huggingface.co"
+    "huggingface.co",
+    "chat.reka.ai",
 ]
 
 if has_browser_cookie3 and os.environ.get('DBUS_SESSION_BUS_ADDRESS') == "/dev/null":
     _LinuxPasswordManager.get_password = lambda a, b: b"secret"
 
 def get_cookies(domain_name: str = '', raise_requirements_error: bool = True, single_browser: bool = False) -> Dict[str, str]:
     """
```

### Comparing `g4f-0.3.0.6/g4f/errors.py` & `g4f-0.3.0.7/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/__init__.py` & `g4f-0.3.0.7/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/client/index.html` & `g4f-0.3.0.7/g4f/gui/client/index.html`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/client/static/css/style.css` & `g4f-0.3.0.7/g4f/gui/client/static/css/style.css`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.3.0.7/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.3.0.7/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.3.0.7/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.3.0.7/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/client/static/img/gpt.png` & `g4f-0.3.0.7/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/client/static/img/user.png` & `g4f-0.3.0.7/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.3.0.7/g4f/gui/client/static/js/chat.v1.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.3.0.7/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.3.0.7/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/client/static/js/icons.js` & `g4f-0.3.0.7/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.3.0.7/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.3.0.7/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.3.0.7/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/server/android_gallery.py` & `g4f-0.3.0.7/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/server/api.py` & `g4f-0.3.0.7/g4f/gui/server/api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/server/backend.py` & `g4f-0.3.0.7/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/server/config.py` & `g4f-0.3.0.7/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/server/internet.py` & `g4f-0.3.0.7/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/server/js_api.py` & `g4f-0.3.0.7/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/server/website.py` & `g4f-0.3.0.7/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/gui/webview.py` & `g4f-0.3.0.7/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/image.py` & `g4f-0.3.0.7/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/local/__init__.py` & `g4f-0.3.0.7/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/locals/models.py` & `g4f-0.3.0.7/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/locals/provider.py` & `g4f-0.3.0.7/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/models.py` & `g4f-0.3.0.7/g4f/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     Llama,
     OpenaiChat,
     PerplexityLabs,
     Replicate,
     Pi,
     Vercel,
     You,
+    Reka
 )
 
 
 @dataclass(unsafe_hash=True)
 class Model:
     """
     Represents a machine learning model configuration.
@@ -302,14 +303,20 @@
 
 blackbox = Model(
     name = 'blackbox',
     base_provider = 'blackbox',
     best_provider = Blackbox
 )
 
+reka_core = Model(
+    name = 'reka-core',
+    base_provider = 'Reka AI',
+    best_provider = Reka
+)
+
 class ModelUtils:
     """
     Utility class for mapping string identifiers to Model instances.
 
     Attributes:
         convert (dict[str, Model]): Dictionary mapping model string identifiers to Model instances.
     """
@@ -329,16 +336,20 @@
         'gpt-4-32k-0613' : gpt_4_32k_0613,
         'gpt-4-turbo'    : gpt_4_turbo,
 
         # Llama
         'llama2-7b' : llama2_7b,
         'llama2-13b': llama2_13b,
         'llama2-70b': llama2_70b,
+        
+        'llama3-8b' : llama3_8b_instruct, # alias
+        'llama3-70b': llama3_70b_instruct, # alias
         'llama3-8b-instruct' : llama3_8b_instruct,
         'llama3-70b-instruct': llama3_70b_instruct,
+        
         'codellama-34b-instruct': codellama_34b_instruct,
         'codellama-70b-instruct': codellama_70b_instruct,
 
         # GigaChat
         'gigachat'     : gigachat,
         'gigachat_plus': gigachat_plus,
         'gigachat_pro' : gigachat_pro,
@@ -355,14 +366,19 @@
         'gemini-pro': gemini_pro,
         
         # anthropic
         'claude-v2': claude_v2,
         'claude-3-opus': claude_3_opus,
         'claude-3-sonnet': claude_3_sonnet,
         
+        # reka core
+        'reka-core': reka_core,
+        'reka': reka_core,
+        'Reka Core': reka_core,
+        
         # other
         'blackbox': blackbox,
         'command-r+': command_r_plus,
         'dbrx-instruct': dbrx_instruct,
         'lzlv-70b': lzlv_70b,
         'airoboros-70b': airoboros_70b,
         'openchat_3.5': openchat_35,
```

### Comparing `g4f-0.3.0.6/g4f/providers/base_provider.py` & `g4f-0.3.0.7/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/providers/create_images.py` & `g4f-0.3.0.7/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/providers/helper.py` & `g4f-0.3.0.7/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/providers/retry_provider.py` & `g4f-0.3.0.7/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/providers/types.py` & `g4f-0.3.0.7/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/requests/__init__.py` & `g4f-0.3.0.7/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/requests/aiohttp.py` & `g4f-0.3.0.7/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/requests/curl_cffi.py` & `g4f-0.3.0.7/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/requests/defaults.py` & `g4f-0.3.0.7/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/requests/raise_for_status.py` & `g4f-0.3.0.7/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/stubs.py` & `g4f-0.3.0.7/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/typing.py` & `g4f-0.3.0.7/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/version.py` & `g4f-0.3.0.7/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f/webdriver.py` & `g4f-0.3.0.7/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/g4f.egg-info/PKG-INFO` & `g4f-0.3.0.7/g4f.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.0.6
+Version: 0.3.0.7
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -80,15 +80,15 @@
 
 <a href="https://trendshift.io/repositories/1692" target="_blank"><img src="https://trendshift.io/api/badge/repositories/1692" alt="xtekky%2Fgpt4free | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>
 
 Written by [@xtekky](https://github.com/hlohaus) & maintained by [@hlohaus](https://github.com/hlohaus)
 
 <div id="top"></div>
 
-> By using this repository or any code related to it, you agree to the [legal notice](LEGAL_NOTICE.md). The author is **not responsible for the usage of this repository nor endorses it**, nor is the author responsible for any copies, forks, re-uploads made by other users, or anything else related to GPT4Free. This is the author's only account and repository. To prevent impersonation or irresponsible actions, please comply with the GNU GPL license this Repository uses.  
+> By using this repository or any code related to it, you agree to the [legal notice](https://github.com/xtekky/gpt4free/blob/main/LEGAL_NOTICE.md). The author is **not responsible for the usage of this repository nor endorses it**, nor is the author responsible for any copies, forks, re-uploads made by other users, or anything else related to GPT4Free. This is the author's only account and repository. To prevent impersonation or irresponsible actions, please comply with the GNU GPL license this Repository uses.  
 
 > [!Warning]
 *"gpt4free"* serves as a **PoC** (proof of concept), demonstrating the development of an API package with multi-provider requests, with features like timeouts, load balance and flow control.
 
 > [!Note]
 <sup><strong>Lastet version:</strong></sup> [![PyPI version](https://img.shields.io/pypi/v/g4f?color=blue)](https://pypi.org/project/g4f) [![Docker version](https://img.shields.io/docker/v/hlohaus789/g4f?label=docker&color=blue)](https://hub.docker.com/r/hlohaus789/g4f)  
 > <sup><strong>Stats:</strong></sup>  [![Downloads](https://static.pepy.tech/badge/g4f)](https://pepy.tech/project/g4f) [![Downloads](https://static.pepy.tech/badge/g4f/month)](https://pepy.tech/project/g4f)
@@ -188,20 +188,20 @@
 3. **File Placement**: Once downloaded, transfer the `.exe` file from your downloads folder to a directory of your choice on your system, and then execute it to run the app.
 ##### Post-Installation Adjustment
 4. **Firewall Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your Windows Firewall settings to allow the application to operate correctly. To do this, access your Windows Firewall settings and allow the application.
 
 By following these steps, you should be able to successfully install and run the application on your Windows system. If you encounter any issues during the installation process, please refer to our Issue Tracker or try to get contact over Discord for assistance.
 
 Run the **Webview UI** on other Platfroms:
-- [/docs/guides/webview](/docs/webview.md)
+- [/docs/guides/webview](https://github.com/xtekky/gpt4free/blob/main/docs/webview.md)
 
 ##### Use your smartphone:
 
 Run the Web UI on Your Smartphone:
-- [/docs/guides/phone](/docs/guides/phone.md)
+- [/docs/guides/phone](https://github.com/xtekky/gpt4free/blob/main/docs/guides/phone.md)
 
 #### Use python
 
 ##### Prerequisites:
 
 1. [Download and install Python](https://www.python.org/downloads/) (Version 3.10+ is recommended).
 2. [Install Google Chrome](https://www.google.com/chrome/) for providers with webdriver
@@ -209,26 +209,26 @@
 ##### Install using PyPI package:
 
 ```
 pip install -U g4f[all]
 ```
 
 How do I install only parts or do disable parts?
-Use partial requirements: [/docs/requirements](/docs/requirements.md)
+Use partial requirements: [/docs/requirements](https://github.com/xtekky/gpt4free/blob/main/docs/requirements.md)
 
 ##### Install from source:
 
 How do I load the project using git and installing the project requirements?
-Read this tutorial and follow it step by step: [/docs/git](/docs/git.md)
+Read this tutorial and follow it step by step: [/docs/git](https://github.com/xtekky/gpt4free/blob/main/docs/git.md)
 
 
 ##### Install using Docker:
 
 How do I build and run composer image from source?
-Use docker-compose: [/docs/docker](/docs/docker.md)
+Use docker-compose: [/docs/docker](https://github.com/xtekky/gpt4free/blob/main/docs/docker.md)
 
 
 ## 💡 Usage
 
 #### Text Generation
 
 ```python
@@ -258,21 +258,21 @@
   prompt="a white siamese cat",
   ...
 )
 image_url = response.data[0].url
 ```
 
 
-[![Image with cat](/docs/cat.jpeg)](/docs/client.md)
+[![Image with cat](/docs/cat.jpeg)](https://github.com/xtekky/gpt4free/blob/main/docs/client.md)
 
 **Full Documentation for Python API**
 
-- New AsyncClient API from G4F: [/docs/async_client](/docs/async_client.md)
-- Client API like the OpenAI Python library: [/docs/client](/docs/client.md)
-- Legacy API with python modules: [/docs/legacy](/docs/legacy.md)
+- New AsyncClient API from G4F: [/docs/async_client](https://github.com/xtekky/gpt4free/blob/main/docs/async_client.md)
+- Client API like the OpenAI Python library: [/docs/client](https://github.com/xtekky/gpt4free/blob/main/docs/client.md)
+- Legacy API with python modules: [/docs/legacy](https://github.com/xtekky/gpt4free/blob/main/docs/legacy.md)
 
 #### Web UI
 
 To start the web interface, type the following codes in python:
 
 ```python
 from g4f.gui import run_gui
@@ -283,15 +283,15 @@
 python -m g4f.cli gui -port 8080 -debug
 ```
 
 #### Interference API
 
 You can use the Interference API to serve other OpenAI integrations with G4F.
 
-See docs: [/docs/interference](/docs/interference.md)
+See docs: [/docs/interference](https://github.com/xtekky/gpt4free/blob/main/docs/interference.md)
 
 Access with: http://localhost:1337/v1
 
 ### Configuration
 
 #### Cookies
 
@@ -376,18 +376,21 @@
 | [you.com](https://you.com) | `g4f.Provider.You` | ✔️ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 
 ## Best OpenSource Models
 While we wait for gpt-5, here is a list of new models that are at least better than gpt-3.5-turbo. **Some are better than gpt-4**. Expect this list to grow.
 
 | Website | Provider |  parameters | better than |
 | ------  | -------  |  ------ |  ------ | 
-| [mixtral-8x22b](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-turbo |
+| [claude-3-opus](https://anthropic.com/) | `g4f.Provider.You` | ?B | gpt-4-0125-preview |
+| [command-r+](https://txt.cohere.com/command-r-plus-microsoft-azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0314 |
+| [llama-3-70b](https://meta.ai/) | `g4f.Provider.Llama` or `DeepInfra` | 70B | gpt-4-0314 |
+| [claude-3-sonnet](https://anthropic.com/) | `g4f.Provider.You` | ?B | gpt-4-0314 |
+| [reka-core](https://chat.reka.ai/) | `g4f.Provider.Reka` | 21B | gpt-4-vision |
 | [dbrx-instruct](https://www.databricks.com/blog/introducing-dbrx-new-state-art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active| gpt-3.5-turbo |
-| [command-r+](https://txt.cohere.com/command-r-plus-microsoft-azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0613 |
-
+| [mixtral-8x22b](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-turbo |
 
 ### GPT-3.5
 
 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth |
 | ------  | -------  | ------- | ----- | ------ | ------ | ---- |
 | [chat3.aiyunos.top](https://chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | ✔️ | ❌ | ✔️ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | ❌ |
 | [chat10.aichatos.xyz](https://chat10.aichatos.xyz) | `g4f.Provider.Aichatos` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
@@ -484,17 +487,34 @@
 | ----- | -------- | ----------- | ------------ | ------- |
 | Microsoft Copilot in Bing | `g4f.Provider.Bing` | dall-e-3 | gpt-4-vision | [bing.com](https://bing.com/chat) |
 | DeepInfra | `g4f.Provider.DeepInfra` | stability-ai/sdxl | llava-1.5-7b-hf | [deepinfra.com](https://deepinfra.com) |
 | Gemini | `g4f.Provider.Gemini` | ✔️ | ✔️ | [gemini.google.com](https://gemini.google.com) |
 | Gemini API | `g4f.Provider.GeminiPro` | ❌ | gemini-1.5-pro | [ai.google.dev](https://ai.google.dev) |
 | Meta AI | `g4f.Provider.MetaAI` | ✔️ | ❌ | [meta.ai](https://www.meta.ai) |
 | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) |
+| Reka | `g4f.Provider.Reka` | ❌ | ✔️ | [chat.reka.ai](https://chat.reka.ai/) |
 | Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b | [replicate.com](https://replicate.com) |
 | You.com | `g4f.Provider.You` | dall-e-3| ✔️ | [you.com](https://you.com) |
 
+```python
+from g4f.client import Client
+from g4f.Provider.GeminiPro import GeminiPro
+
+client = Client(
+    api_key="...",
+    provider=GeminiPro
+)
+response = client.chat.completions.create(
+    model="gemini-pro-vision",
+    messages=[{"role": "user", "content": "What are on this image?"}],
+    image=open("docs/waterfall.jpeg", "rb")
+)
+print(response.choices[0].message.content)
+```
+
 ## 🔗 Powered by gpt4free
 
 <table>
   <thead align="center">
     <tr border: none;>
       <td>
         <b>🎁 Projects</b>
@@ -897,19 +917,19 @@
 
 ## 🤝 Contribute
 
 We welcome contributions from the community. Whether you're adding new providers or features, or simply fixing typos and making small improvements, your input is valued. Creating a pull request is all it takes – our co-pilot will handle the code review process. Once all changes have been addressed, we'll merge the pull request into the main branch and release the updates at a later time.
 
 ###### Guide: How do i create a new Provider?
 
- - Read: [/docs/guides/create_provider](/docs/guides/create_provider.md)
+ - Read: [/docs/guides/create_provider](https://github.com/xtekky/gpt4free/blob/main/docs/guides/create_provider.md)
 
 ###### Guide: How can AI help me with writing code?
 
- - Read: [/docs/guides/help_me](/docs/guides/help_me.md)
+ - Read: [/docs/guides/help_me](https://github.com/xtekky/gpt4free/blob/main/docs/guides/help_me.md)
 
 ## 🙌 Contributors
 
 A list of all contributors is available [here](https://github.com/xtekky/gpt4free/graphs/contributors)
 
 <a href="https://github.com/xtekky" target="_blank"><img src="https://avatars.githubusercontent.com/u/98614666?v=4&s=45" width="45" title="xtekky"></a>
 <a href="https://github.com/hlohaus" target="_blank"><img src="https://avatars.githubusercontent.com/u/983577?v=4&s=45" width="45" title="hlohaus"></a>
@@ -943,19 +963,19 @@
 <a href="https://github.com/ggindinson" target="_blank"><img src="https://avatars.githubusercontent.com/u/97807772?v=4&s=45" width="45" title="ggindinson"></a>
 <span></span>
 <img src="https://avatars.githubusercontent.com/u/71154407?s=45&v=4" width="45" title="ading2210">
 <img src="https://avatars.githubusercontent.com/u/12299238?s=45&v=4" width="45" title="xqdoo00o">
 <img src="https://avatars.githubusercontent.com/u/97126670?s=45&v=4" width="45" title="nathanrchn">
 <img src="https://avatars.githubusercontent.com/u/81407603?v=4&s=45" width="45" title="dsdanielpark">
 
-- The [`Vercel.py`](g4f/Provider/Vercel.py) file contains code from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210)
-- The [`har_file.py`](g4f/Provider/openai/har_file.py) has input from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API)
-- The [`PerplexityLabs.py`](g4f/Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai)
-- The [`Gemini.py`](g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API)
-- The [`MetaAI.py`](g4f/Provider/MetaAI.py) file contains code from [meta-ai-api](https://github.com/Strvm/meta-ai-api) by [@Strvm](https://github.com/Strvm)
+- The [`Vercel.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/Vercel.py) file contains code from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210)
+- The [`har_file.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API)
+- The [`PerplexityLabs.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai)
+- The [`Gemini.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API)
+- The [`MetaAI.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/MetaAI.py) file contains code from [meta-ai-api](https://github.com/Strvm/meta-ai-api) by [@Strvm](https://github.com/Strvm)
 
 *Having input implies that the AI's code generation utilized it as one of many sources.*
 
 ## ©️ Copyright
 
 This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt)
 
@@ -987,13 +1007,13 @@
 <table>
   <tr>
      <td>
        <p align="center"> <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/93/GPLv3_Logo.svg/1200px-GPLv3_Logo.svg.png" width="80%"></img>
     </td>
     <td> 
       <img src="https://img.shields.io/badge/License-GNU_GPL_v3.0-red.svg"/> <br> 
-This project is licensed under <a href="./LICENSE">GNU_GPL_v3.0</a>.
+This project is licensed under <a href="https://github.com/xtekky/gpt4free/blob/main/LICENSE">GNU_GPL_v3.0</a>.
     </td>
   </tr>
 </table>
 
 <p align="right">(<a href="#top">🔼 Back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.0.6 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.0.7 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -41,28 +41,29 @@
 local Requires-Dist: gpt4all; extra == "local" Provides-Extra: curl-cffi
 Requires-Dist: curl_cffi>=0.6.2; extra == "curl-cffi" ![248433934-7886223b-
 c1d1-4260-82aa-da5741f303bb](https://github.com/xtekky/gpt4free/assets/
 98614666/ea012c87-76e0-496a-8ac4-e2de090cc6c9) _[_x_t_e_k_k_y_%_2_F_g_p_t_4_f_r_e_e_ _|
 _T_r_e_n_d_s_h_i_f_t_]Written by [@xtekky](https://github.com/hlohaus) & maintained by
 [@hlohaus](https://github.com/hlohaus)
 > By using this repository or any code related to it, you agree to the [legal
-notice](LEGAL_NOTICE.md). The author is **not responsible for the usage of this
-repository nor endorses it**, nor is the author responsible for any copies,
-forks, re-uploads made by other users, or anything else related to GPT4Free.
-This is the author's only account and repository. To prevent impersonation or
-irresponsible actions, please comply with the GNU GPL license this Repository
-uses. > [!Warning] *"gpt4free"* serves as a **PoC** (proof of concept),
-demonstrating the development of an API package with multi-provider requests,
-with features like timeouts, load balance and flow control. > [!Note] LLaasstteett
-vveerrssiioonn:: [![PyPI version](https://img.shields.io/pypi/v/g4f?color=blue)](https:
-//pypi.org/project/g4f) [![Docker version](https://img.shields.io/docker/v/
-hlohaus789/g4f?label=docker&color=blue)](https://hub.docker.com/r/hlohaus789/
-g4f) > SSttaattss:: [![Downloads](https://static.pepy.tech/badge/g4f)](https://
-pepy.tech/project/g4f) [![Downloads](https://static.pepy.tech/badge/g4f/month)]
-(https://pepy.tech/project/g4f) ```sh pip install -U g4f ``` ```sh docker pull
+notice](https://github.com/xtekky/gpt4free/blob/main/LEGAL_NOTICE.md). The
+author is **not responsible for the usage of this repository nor endorses it**,
+nor is the author responsible for any copies, forks, re-uploads made by other
+users, or anything else related to GPT4Free. This is the author's only account
+and repository. To prevent impersonation or irresponsible actions, please
+comply with the GNU GPL license this Repository uses. > [!Warning] *"gpt4free"*
+serves as a **PoC** (proof of concept), demonstrating the development of an API
+package with multi-provider requests, with features like timeouts, load balance
+and flow control. > [!Note] LLaasstteett vveerrssiioonn:: [![PyPI version](https://
+img.shields.io/pypi/v/g4f?color=blue)](https://pypi.org/project/g4f) [![Docker
+version](https://img.shields.io/docker/v/hlohaus789/
+g4f?label=docker&color=blue)](https://hub.docker.com/r/hlohaus789/g4f) > SSttaattss::
+[![Downloads](https://static.pepy.tech/badge/g4f)](https://pepy.tech/project/
+g4f) [![Downloads](https://static.pepy.tech/badge/g4f/month)](https://
+pepy.tech/project/g4f) ```sh pip install -U g4f ``` ```sh docker pull
 hlohaus789/g4f ``` ## ð What's New - Installation Guide for Windows (.exe):
 ð» [#installation-guide-for-windows](#installation-guide-for-windows-exe) -
 Join our Telegram Channel: ð¨ [telegram.me/g4f_channel](https://telegram.me/
 g4f_channel) - Join our Discord Group: ð¬ [discord.gg/XfybzPXPH5](https://
 discord.gg/XfybzPXPH5) - `g4f` now supports 100% local inference: ð§  [local-
 docs](https://g4f.mintlify.app/docs/core/usage/local) ## ð» Site Takedown Is
 your site on this repository and you want to take it down? Send an email to
@@ -124,48 +125,54 @@
 Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your
 Windows Firewall settings to allow the application to operate correctly. To do
 this, access your Windows Firewall settings and allow the application. By
 following these steps, you should be able to successfully install and run the
 application on your Windows system. If you encounter any issues during the
 installation process, please refer to our Issue Tracker or try to get contact
 over Discord for assistance. Run the **Webview UI** on other Platfroms: - [/
-docs/guides/webview](/docs/webview.md) ##### Use your smartphone: Run the Web
-UI on Your Smartphone: - [/docs/guides/phone](/docs/guides/phone.md) #### Use
-python ##### Prerequisites: 1. [Download and install Python](https://
-www.python.org/downloads/) (Version 3.10+ is recommended). 2. [Install Google
-Chrome](https://www.google.com/chrome/) for providers with webdriver #####
-Install using PyPI package: ``` pip install -U g4f[all] ``` How do I install
-only parts or do disable parts? Use partial requirements: [/docs/requirements]
-(/docs/requirements.md) ##### Install from source: How do I load the project
-using git and installing the project requirements? Read this tutorial and
-follow it step by step: [/docs/git](/docs/git.md) ##### Install using Docker:
-How do I build and run composer image from source? Use docker-compose: [/docs/
-docker](/docs/docker.md) ## ð¡ Usage #### Text Generation ```python from
+docs/guides/webview](https://github.com/xtekky/gpt4free/blob/main/docs/
+webview.md) ##### Use your smartphone: Run the Web UI on Your Smartphone: - [/
+docs/guides/phone](https://github.com/xtekky/gpt4free/blob/main/docs/guides/
+phone.md) #### Use python ##### Prerequisites: 1. [Download and install Python]
+(https://www.python.org/downloads/) (Version 3.10+ is recommended). 2. [Install
+Google Chrome](https://www.google.com/chrome/) for providers with webdriver
+##### Install using PyPI package: ``` pip install -U g4f[all] ``` How do I
+install only parts or do disable parts? Use partial requirements: [/docs/
+requirements](https://github.com/xtekky/gpt4free/blob/main/docs/
+requirements.md) ##### Install from source: How do I load the project using git
+and installing the project requirements? Read this tutorial and follow it step
+by step: [/docs/git](https://github.com/xtekky/gpt4free/blob/main/docs/git.md)
+##### Install using Docker: How do I build and run composer image from source?
+Use docker-compose: [/docs/docker](https://github.com/xtekky/gpt4free/blob/
+main/docs/docker.md) ## ð¡ Usage #### Text Generation ```python from
 g4f.client import Client client = Client() response =
 client.chat.completions.create( model="gpt-3.5-turbo", messages=[{"role":
 "user", "content": "Hello"}], ... ) print(response.choices[0].message.content)
 ``` ``` Hello! How can I assist you today? ``` #### Image Generation ```python
 from g4f.client import Client client = Client() response =
 client.images.generate( model="gemini", prompt="a white siamese cat", ... )
-image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](/docs/
-client.md) **Full Documentation for Python API** - New AsyncClient API from
-G4F: [/docs/async_client](/docs/async_client.md) - Client API like the OpenAI
-Python library: [/docs/client](/docs/client.md) - Legacy API with python
-modules: [/docs/legacy](/docs/legacy.md) #### Web UI To start the web
-interface, type the following codes in python: ```python from g4f.gui import
-run_gui run_gui() ``` or execute the following command: ```bash python -
-m g4f.cli gui -port 8080 -debug ``` #### Interference API You can use the
-Interference API to serve other OpenAI integrations with G4F. See docs: [/docs/
-interference](/docs/interference.md) Access with: http://localhost:1337/v1 ###
-Configuration #### Cookies Cookies are essential for using Meta AI and
-Microsoft Designer to create images. Additionally, cookies are required for the
-Google Gemini and WhiteRabbitNeo Provider. From Bing, ensure you have the "_U"
-cookie, and from Google, all cookies starting with "__Secure-1PSID" are needed.
-You can pass these cookies directly to the create function or set them using
-the `set_cookies` method before running G4F: ```python from g4f.cookies import
+image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](https:
+//github.com/xtekky/gpt4free/blob/main/docs/client.md) **Full Documentation for
+Python API** - New AsyncClient API from G4F: [/docs/async_client](https://
+github.com/xtekky/gpt4free/blob/main/docs/async_client.md) - Client API like
+the OpenAI Python library: [/docs/client](https://github.com/xtekky/gpt4free/
+blob/main/docs/client.md) - Legacy API with python modules: [/docs/legacy]
+(https://github.com/xtekky/gpt4free/blob/main/docs/legacy.md) #### Web UI To
+start the web interface, type the following codes in python: ```python from
+g4f.gui import run_gui run_gui() ``` or execute the following command: ```bash
+python -m g4f.cli gui -port 8080 -debug ``` #### Interference API You can use
+the Interference API to serve other OpenAI integrations with G4F. See docs: [/
+docs/interference](https://github.com/xtekky/gpt4free/blob/main/docs/
+interference.md) Access with: http://localhost:1337/v1 ### Configuration ####
+Cookies Cookies are essential for using Meta AI and Microsoft Designer to
+create images. Additionally, cookies are required for the Google Gemini and
+WhiteRabbitNeo Provider. From Bing, ensure you have the "_U" cookie, and from
+Google, all cookies starting with "__Secure-1PSID" are needed. You can pass
+these cookies directly to the create function or set them using the
+`set_cookies` method before running G4F: ```python from g4f.cookies import
 set_cookies set_cookies(".bing.com", { "_U": "cookie value" }) set_cookies
 (".google.com", { "__Secure-1PSID": "cookie value" }) ``` Alternatively, you
 can place your .har and cookie files in the `/har_and_cookies` directory. To
 export a cookie file, use the EditThisCookie extension available on the Chrome
 Web Store: [EditThisCookie Extension](https://chromewebstore.google.com/detail/
 editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg). You can also create .har
 files to capture cookies. If you need further assistance, refer to the next
@@ -207,37 +214,42 @@
 beta.theb.ai) | `g4f.Provider.Theb` | âï¸ | âï¸ | âï¸ | ![Unknown]
 (https://img.shields.io/badge/Unknown-grey) | â | | [you.com](https://
 you.com) | `g4f.Provider.You` | âï¸ | âï¸ | âï¸ | ![Active](https://
 img.shields.io/badge/Active-brightgreen) | â | ## Best OpenSource Models
 While we wait for gpt-5, here is a list of new models that are at least better
 than gpt-3.5-turbo. **Some are better than gpt-4**. Expect this list to grow. |
 Website | Provider | parameters | better than | | ------ | ------- | ------ | -
------ | | [mixtral-8x22b](https://huggingface.co/mistral-community/Mixtral-
-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-turbo | |
-[dbrx-instruct](https://www.databricks.com/blog/introducing-dbrx-new-state-art-
-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active| gpt-3.5-turbo | |
-[command-r+](https://txt.cohere.com/command-r-plus-microsoft-azure/) |
-`g4f.Provider.HuggingChat` | 104B | gpt-4-0613 | ### GPT-3.5 | Website |
-Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | ------ | ------- | ----
---- | ----- | ------ | ------ | ---- | | [chat3.aiyunos.top](https://
-chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | âï¸ | â | âï¸ | !
+----- | | [claude-3-opus](https://anthropic.com/) | `g4f.Provider.You` | ?B |
+gpt-4-0125-preview | | [command-r+](https://txt.cohere.com/command-r-plus-
+microsoft-azure/) | `g4f.Provider.HuggingChat` | 104B | gpt-4-0314 | | [llama-
+3-70b](https://meta.ai/) | `g4f.Provider.Llama` or `DeepInfra` | 70B | gpt-4-
+0314 | | [claude-3-sonnet](https://anthropic.com/) | `g4f.Provider.You` | ?B |
+gpt-4-0314 | | [reka-core](https://chat.reka.ai/) | `g4f.Provider.Reka` | 21B |
+gpt-4-vision | | [dbrx-instruct](https://www.databricks.com/blog/introducing-
+dbrx-new-state-art-open-llm) | `g4f.Provider.DeepInfra` | 132B / 36B active|
+gpt-3.5-turbo | | [mixtral-8x22b](https://huggingface.co/mistral-community/
+Mixtral-8x22B-v0.1) | `g4f.Provider.DeepInfra` | 176B / 44b active | gpt-3.5-
+turbo | ### GPT-3.5 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status |
+Auth | | ------ | ------- | ------- | ----- | ------ | ------ | ---- | |
+[chat3.aiyunos.top](https://chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace`
+| âï¸ | â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey)
+| â | | [chat10.aichatos.xyz](https://chat10.aichatos.xyz) |
+`g4f.Provider.Aichatos` | âï¸ | â | âï¸ | ![Active](https://
+img.shields.io/badge/Active-brightgreen) | â | | [chatforai.store](https://
+chatforai.store) | `g4f.Provider.ChatForAi` | âï¸ | â | âï¸ | !
 [Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
-[chat10.aichatos.xyz](https://chat10.aichatos.xyz) | `g4f.Provider.Aichatos` |
-âï¸ | â | âï¸ | ![Active](https://img.shields.io/badge/Active-
-brightgreen) | â | | [chatforai.store](https://chatforai.store) |
-`g4f.Provider.ChatForAi` | âï¸ | â | âï¸ | ![Unknown](https://
-img.shields.io/badge/Unknown-grey) | â | | [chatgpt4online.org](https://
-chatgpt4online.org) | `g4f.Provider.Chatgpt4Online` | âï¸ | â | âï¸ | !
-[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [chatgpt-
-free.cc](https://www.chatgpt-free.cc) | `g4f.Provider.ChatgptNext` | âï¸ |
-â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
-[chatgptx.de](https://chatgptx.de) | `g4f.Provider.ChatgptX` | âï¸ | â |
-âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
-[f1.cnote.top](https://f1.cnote.top) | `g4f.Provider.Cnote` | âï¸ | â |
-âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) | â | |
+[chatgpt4online.org](https://chatgpt4online.org) |
+`g4f.Provider.Chatgpt4Online` | âï¸ | â | âï¸ | ![Unknown](https://
+img.shields.io/badge/Unknown-grey) | â | | [chatgpt-free.cc](https://
+www.chatgpt-free.cc) | `g4f.Provider.ChatgptNext` | âï¸ | â | âï¸ | !
+[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [chatgptx.de]
+(https://chatgptx.de) | `g4f.Provider.ChatgptX` | âï¸ | â | âï¸ | !
+[Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [f1.cnote.top]
+(https://f1.cnote.top) | `g4f.Provider.Cnote` | âï¸ | â | âï¸ | !
+[Active](https://img.shields.io/badge/Active-brightgreen) | â | |
 [duckduckgo.com](https://duckduckgo.com/duckchat) | `g4f.Provider.DuckDuckGo` |
 âï¸ | â | âï¸ | ![Active](https://img.shields.io/badge/Active-
 brightgreen) | â | | [ecosia.org](https://www.ecosia.org) |
 `g4f.Provider.Ecosia` | âï¸ | â | âï¸ | ![Active](https://
 img.shields.io/badge/Active-brightgreen) | â | | [feedough.com](https://
 www.feedough.com) | `g4f.Provider.Feedough` | âï¸ | â | âï¸ | ![Active]
 (https://img.shields.io/badge/Active-brightgreen) | â | | [flowgpt.com]
@@ -371,18 +383,24 @@
 gpt-4-vision | [bing.com](https://bing.com/chat) | | DeepInfra |
 `g4f.Provider.DeepInfra` | stability-ai/sdxl | llava-1.5-7b-hf |
 [deepinfra.com](https://deepinfra.com) | | Gemini | `g4f.Provider.Gemini` |
 âï¸ | âï¸ | [gemini.google.com](https://gemini.google.com) | | Gemini API
 | `g4f.Provider.GeminiPro` | â | gemini-1.5-pro | [ai.google.dev](https://
 ai.google.dev) | | Meta AI | `g4f.Provider.MetaAI` | âï¸ | â | [meta.ai]
 (https://www.meta.ai) | | OpenAI ChatGPT | `g4f.Provider.OpenaiChat` | dall-e-
-3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) | | Replicate |
-`g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b | [replicate.com]
-(https://replicate.com) | | You.com | `g4f.Provider.You` | dall-e-3| âï¸ |
-[you.com](https://you.com) | ## ð Powered by gpt4free
+3 | gpt-4-vision | [chat.openai.com](https://chat.openai.com) | | Reka |
+`g4f.Provider.Reka` | â | âï¸ | [chat.reka.ai](https://chat.reka.ai/) | |
+Replicate | `g4f.Provider.Replicate` | stability-ai/sdxl| llava-v1.6-34b |
+[replicate.com](https://replicate.com) | | You.com | `g4f.Provider.You` | dall-
+e-3| âï¸ | [you.com](https://you.com) | ```python from g4f.client import
+Client from g4f.Provider.GeminiPro import GeminiPro client = Client
+( api_key="...", provider=GeminiPro ) response = client.chat.completions.create
+( model="gemini-pro-vision", messages=[{"role": "user", "content": "What are on
+this image?"}], image=open("docs/waterfall.jpeg", "rb") ) print
+(response.choices[0].message.content) ``` ## ð Powered by gpt4free
 ?ð??? PPrroojjeeccttss             ?â?­? SSttaarrss ?ð??? FFoorrkkss ?ð??? IIssssuueess ?ð???¬ PPuullll rreeqquueessttss
 _gg_pp_tt_44_ff_rr_ee_ee                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _FF_rr_ee_ee_ _AA_II_ _AA_PP_II_''_ss_ _&&_ _PP_oo_tt_ee_nn_tt_ii_aa_ll _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _PP_rr_oo_vv_ii_dd_ee_rr_ss_ _LL_ii_ss_tt
 _CC_hh_aa_tt_GG_PP_TT_--_CC_ll_oo_nn_ee             _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _AA_ii_ _aa_gg_ee_nn_tt                  _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 _CC_hh_aa_tt_GG_pp_tt_ _DD_ii_ss_cc_oo_rr_dd_ _BB_oo_tt       _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
@@ -396,19 +414,20 @@
 _pp_yy_tt_hh_oo_nn_--_tt_gg_pp_tt               _[_S_t_a_r_s_]   _[_F_o_r_k_s_]    _[_I_s_s_u_e_s_]    _[_P_u_l_l_ _R_e_q_u_e_s_t_s_]
 ## ð¤ Contribute We welcome contributions from the community. Whether you're
 adding new providers or features, or simply fixing typos and making small
 improvements, your input is valued. Creating a pull request is all it takes â
 our co-pilot will handle the code review process. Once all changes have been
 addressed, we'll merge the pull request into the main branch and release the
 updates at a later time. ###### Guide: How do i create a new Provider? - Read:
-[/docs/guides/create_provider](/docs/guides/create_provider.md) ###### Guide:
-How can AI help me with writing code? - Read: [/docs/guides/help_me](/docs/
-guides/help_me.md) ## ð Contributors A list of all contributors is available
-[here](https://github.com/xtekky/gpt4free/graphs/contributors) _[_h_t_t_p_s_:_/_/
-_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_6_1_4_6_6_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+[/docs/guides/create_provider](https://github.com/xtekky/gpt4free/blob/main/
+docs/guides/create_provider.md) ###### Guide: How can AI help me with writing
+code? - Read: [/docs/guides/help_me](https://github.com/xtekky/gpt4free/blob/
+main/docs/guides/help_me.md) ## ð Contributors A list of all contributors is
+available [here](https://github.com/xtekky/gpt4free/graphs/contributors)
+_[_h_t_t_p_s_:_/_/_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_6_1_4_6_6_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_3_5_7_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_8_3_0_5_3_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_4_1_5_4_6_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_9_6_6_2_2_8_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_0_5_1_6_0_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_0_5_8_5_2_3_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_3_4_8_5_4_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
@@ -433,36 +452,39 @@
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_7_6_3_6_0_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_5_6_6_3_2_2_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_9_3_2_2_7_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
 _a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_7_8_0_7_7_7_2_?_v_=_4_&_s_=_4_5_][https://
 avatars.githubusercontent.com/u/71154407?s=45&v=4][https://
 avatars.githubusercontent.com/u/12299238?s=45&v=4][https://
 avatars.githubusercontent.com/u/97126670?s=45&v=4][https://
-avatars.githubusercontent.com/u/81407603?v=4&s=45]- The [`Vercel.py`](g4f/
-Provider/Vercel.py) file contains code from [vercel-llm-api](https://
-github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/
-ading2210) - The [`har_file.py`](g4f/Provider/openai/har_file.py) has input
+avatars.githubusercontent.com/u/81407603?v=4&s=45]- The [`Vercel.py`](https://
+github.com/xtekky/gpt4free/blob/main/g4f/Provider/Vercel.py) file contains code
+from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by
+[@ading2210](https://github.com/ading2210) - The [`har_file.py`](https://
+github.com/xtekky/gpt4free/blob/main/g4f/Provider/openai/har_file.py) has input
 from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API) -
-The [`PerplexityLabs.py`](g4f/Provider/openai/har_file.py) has input from
-[nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai) - The
-[`Gemini.py`](g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/
-Gemini-API](https://github.com/dsdanielpark/Gemini-API) - The [`MetaAI.py`]
-(g4f/Provider/MetaAI.py) file contains code from [meta-ai-api](https://
-github.com/Strvm/meta-ai-api) by [@Strvm](https://github.com/Strvm) *Having
-input implies that the AI's code generation utilized it as one of many
-sources.* ## Â©ï¸ Copyright This program is licensed under the [GNU GPL v3]
-(https://www.gnu.org/licenses/gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C)
-2023 xtekky This program is free software: you can redistribute it and/or
-modify it under the terms of the GNU General Public License as published by the
-Free Software Foundation, either version 3 of the License, or (at your option)
-any later version. This program is distributed in the hope that it will be
-useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public
-License for more details. You should have received a copy of the GNU General
-Public License along with this program. If not, see
+The [`PerplexityLabs.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/
+Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://
+github.com/nathanrchn/perplexityai) - The [`Gemini.py`](https://github.com/
+xtekky/gpt4free/blob/main/g4f/Provider/needs_auth/Gemini.py) has input from
+[dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API) - The
+[`MetaAI.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/
+MetaAI.py) file contains code from [meta-ai-api](https://github.com/Strvm/meta-
+ai-api) by [@Strvm](https://github.com/Strvm) *Having input implies that the
+AI's code generation utilized it as one of many sources.* ## Â©ï¸ Copyright
+This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/
+gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C) 2023 xtekky This program is
+free software: you can redistribute it and/or modify it under the terms of the
+GNU General Public License as published by the Free Software Foundation, either
+version 3 of the License, or (at your option) any later version. This program
+is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+PARTICULAR PURPOSE. See the GNU General Public License for more details. You
+should have received a copy of the GNU General Public License along with this
+program. If not, see
 www.gnu.org/licenses/>. ``` ## â­ Star History _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]## ð
 License
 [https://upload.wikimedia.org/wikipedia/ [https://img.shields.io/badge/License-
    commons/thumb/9/93/GPLv3_Logo.svg/    GNU_GPL_v3.0-red.svg]
        1200px-GPLv3_Logo.svg.png]        This project is licensed under
                                          _G_N_U___G_P_L___v_3_._0.
                                                              (_ð___¼_ _B_a_c_k_ _t_o_ _t_o_p)
```

### Comparing `g4f-0.3.0.6/g4f.egg-info/SOURCES.txt` & `g4f-0.3.0.7/g4f.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 g4f/Provider/Liaobots.py
 g4f/Provider/Llama.py
 g4f/Provider/Local.py
 g4f/Provider/MetaAI.py
 g4f/Provider/MetaAIAccount.py
 g4f/Provider/PerplexityLabs.py
 g4f/Provider/Pi.py
+g4f/Provider/Reka.py
 g4f/Provider/Replicate.py
 g4f/Provider/ReplicateImage.py
 g4f/Provider/Vercel.py
 g4f/Provider/WhiteRabbitNeo.py
 g4f/Provider/You.py
 g4f/Provider/__init__.py
 g4f/Provider/base_provider.py
@@ -135,14 +136,15 @@
 g4f/Provider/npm/package.json
 g4f/Provider/npm/node_modules/.package-lock.json
 g4f/Provider/npm/node_modules/crypto-js/README.md
 g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
 g4f/Provider/openai/__init__.py
 g4f/Provider/openai/crypt.py
 g4f/Provider/openai/har_file.py
+g4f/Provider/openai/proofofwork.py
 g4f/Provider/selenium/AItianhuSpace.py
 g4f/Provider/selenium/Bard.py
 g4f/Provider/selenium/MyShell.py
 g4f/Provider/selenium/PerplexityAi.py
 g4f/Provider/selenium/Phind.py
 g4f/Provider/selenium/TalkAi.py
 g4f/Provider/selenium/__init__.py
```

### Comparing `g4f-0.3.0.6/g4f.egg-info/requires.txt` & `g4f-0.3.0.7/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.0.6/setup.py` & `g4f-0.3.0.7/setup.py`

 * *Files identical despite different names*

