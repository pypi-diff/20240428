# Comparing `tmp/freegenius-0.1.7.tar.gz` & `tmp/freegenius-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freegenius-0.1.7.tar", last modified: Sat Apr 27 18:29:38 2024, max compression
+gzip compressed data, was "freegenius-0.1.8.tar", last modified: Sun Apr 28 21:39:08 2024, max compression
```

## Comparing `freegenius-0.1.7.tar` & `freegenius-0.1.8.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.713379 freegenius-0.1.7/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    14938 2024-04-27 18:29:38.713379 freegenius-0.1.7/PKG-INFO
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.665380 freegenius-0.1.7/freegenius/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11766 2024-04-27 18:29:38.000000 freegenius-0.1.7/freegenius/README.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.1.7/freegenius/__init__.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.669380 freegenius-0.1.7/freegenius/audio/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.1.7/freegenius/audio/notification1.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.1.7/freegenius/audio/notification1_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.1.7/freegenius/audio/notification2.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.1.7/freegenius/audio/notification2_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6992 2024-04-27 18:28:23.000000 freegenius-0.1.7/freegenius/autoassist.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.1.7/freegenius/autobuilder.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11067 2024-04-27 18:28:32.000000 freegenius-0.1.7/freegenius/autoretriever.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.1.7/freegenius/chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.1.7/freegenius/codey.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.1.7/freegenius/commandprompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.000000 freegenius-0.1.7/freegenius/config.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.1.7/freegenius/eTextEdit.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.669380 freegenius-0.1.7/freegenius/files/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.1.7/freegenius/files/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.1.7/freegenius/geminipro.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.1.7/freegenius/geminiprovision.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6515 2024-04-27 12:11:29.000000 freegenius-0.1.7/freegenius/groqchat.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.669380 freegenius-0.1.7/freegenius/gui/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.1.7/freegenius/gui/chatgui.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.1.7/freegenius/gui/worker.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.669380 freegenius-0.1.7/freegenius/history/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.1.7/freegenius/history/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.689379 freegenius-0.1.7/freegenius/icons/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.1.7/freegenius/icons/FreeGenius.ico
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.1.7/freegenius/icons/FreeGenius.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.1.7/freegenius/icons/FreeGenius_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.1.7/freegenius/icons/ai.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.1.7/freegenius/icons/ai_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.1.7/freegenius/llamacpp.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.661380 freegenius-0.1.7/freegenius/macOS_service/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.661380 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Download_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.693379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.693379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.661380 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.693379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.693379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.661380 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Files_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.693379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.693379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.661380 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.697379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.697379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.661380 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Summary_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.697379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.697379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.661380 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Text_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.697379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.697379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.661380 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Translation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.697379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.697379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.661380 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.697379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.697379 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.1.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.1.7/freegenius/main.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.1.7/freegenius/ollamachat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-04-27 18:29:38.000000 freegenius-0.1.7/freegenius/package_name.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.1.7/freegenius/palm2.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.709379 freegenius-0.1.7/freegenius/plugins/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.1.7/freegenius/plugins/000_check_ffmpeg.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-04-25 10:21:23.000000 freegenius-0.1.7/freegenius/plugins/000_check_pyaudio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.1.7/freegenius/plugins/000_check_vlc.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.1.7/freegenius/plugins/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.1.7/freegenius/plugins/add calendar event.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.1.7/freegenius/plugins/aliases.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7437 2024-04-27 13:00:33.000000 freegenius-0.1.7/freegenius/plugins/analyze audio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.1.7/freegenius/plugins/analyze files.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4677 2024-04-27 13:03:55.000000 freegenius-0.1.7/freegenius/plugins/analyze images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.1.7/freegenius/plugins/analyze web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2559 2024-04-14 22:20:21.000000 freegenius-0.1.7/freegenius/plugins/auto correct python code.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.1.7/freegenius/plugins/awesome prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.1.7/freegenius/plugins/character analysis.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.1.7/freegenius/plugins/chat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.1.7/freegenius/plugins/contexts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.1.7/freegenius/plugins/counselling.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.1.7/freegenius/plugins/create ai assistants.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5160 2024-04-27 13:04:35.000000 freegenius-0.1.7/freegenius/plugins/create images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.1.7/freegenius/plugins/create maps.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.1.7/freegenius/plugins/create qrcode.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.1.7/freegenius/plugins/create statistical graphics.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.1.7/freegenius/plugins/dates and times.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.1.7/freegenius/plugins/download youtube or web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.1.7/freegenius/plugins/edit text.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.1.7/freegenius/plugins/execute computing tasks.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.1.7/freegenius/plugins/execute termux command.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.1.7/freegenius/plugins/global finance.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.1.7/freegenius/plugins/improve British English.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2315 2024-04-25 10:21:23.000000 freegenius-0.1.7/freegenius/plugins/input suggestions.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.1.7/freegenius/plugins/install python package.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.1.7/freegenius/plugins/integrate google searches.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.1.7/freegenius/plugins/memory.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8646 2024-04-27 13:03:30.000000 freegenius-0.1.7/freegenius/plugins/modify images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.1.7/freegenius/plugins/open web browser.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.1.7/freegenius/plugins/pronounce words.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.1.7/freegenius/plugins/remove image background.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5906 2024-04-27 11:30:39.000000 freegenius-0.1.7/freegenius/plugins/search chat records.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1156 2024-04-10 07:42:48.000000 freegenius-0.1.7/freegenius/plugins/search financial data.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.1.7/freegenius/plugins/search latest news.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.1.7/freegenius/plugins/search sqlite.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.1.7/freegenius/plugins/search weather info.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.1.7/freegenius/plugins/send email.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.1.7/freegenius/plugins/send tweet.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.1.7/freegenius/plugins/send whatsapp messages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.1.7/freegenius/plugins/simplified Chinese to traditional Chinese.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.1.7/freegenius/qt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.1.7/freegenius/rag.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      840 2024-04-26 22:24:44.000000 freegenius-0.1.7/freegenius/requirements.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1359 2024-04-25 20:30:31.000000 freegenius-0.1.7/freegenius/servers.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7714 2024-04-27 15:10:04.000000 freegenius-0.1.7/freegenius/systemtray.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.709379 freegenius-0.1.7/freegenius/temp/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.1.7/freegenius/temp/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.713379 freegenius-0.1.7/freegenius/utils/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   112155 2024-04-27 15:16:32.000000 freegenius-0.1.7/freegenius/utils/assistant.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29734 2024-04-26 22:27:56.000000 freegenius-0.1.7/freegenius/utils/call_chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    17269 2024-04-25 20:53:07.000000 freegenius-0.1.7/freegenius/utils/call_gemini.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    17313 2024-04-27 14:53:19.000000 freegenius-0.1.7/freegenius/utils/call_groq.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    24612 2024-04-25 20:52:45.000000 freegenius-0.1.7/freegenius/utils/call_llamacpp.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8528 2024-04-27 07:40:12.000000 freegenius-0.1.7/freegenius/utils/call_llm.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    18713 2024-04-25 20:53:07.000000 freegenius-0.1.7/freegenius/utils/call_ollama.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    18391 2024-04-27 12:12:56.000000 freegenius-0.1.7/freegenius/utils/config_essential.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.1.7/freegenius/utils/config_tools.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.1.7/freegenius/utils/download.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.1.7/freegenius/utils/get_path_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4888 2024-04-23 21:13:11.000000 freegenius-0.1.7/freegenius/utils/ollama_models.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.1.7/freegenius/utils/promptValidator.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.1.7/freegenius/utils/prompt_multiline_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.1.7/freegenius/utils/prompt_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.1.7/freegenius/utils/prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.1.7/freegenius/utils/python_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    50100 2024-04-27 15:07:24.000000 freegenius-0.1.7/freegenius/utils/shared_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.1.7/freegenius/utils/shortcuts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.1.7/freegenius/utils/single_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.1.7/freegenius/utils/streaming_word_wrapper.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.1.7/freegenius/utils/sttLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.1.7/freegenius/utils/terminal_mode_dialogs.py
--rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.1.7/freegenius/utils/terminal_system_command_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.1.7/freegenius/utils/text_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4352 2024-04-12 22:26:19.000000 freegenius-0.1.7/freegenius/utils/tool_plugins.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7640 2024-02-22 00:47:05.000000 freegenius-0.1.7/freegenius/utils/ttsLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8563 2024-03-28 23:38:45.000000 freegenius-0.1.7/freegenius/utils/tts_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4651 2024-04-09 22:46:08.000000 freegenius-0.1.7/freegenius/utils/vlc_utils.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-27 18:29:38.713379 freegenius-0.1.7/freegenius.egg-info/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    14938 2024-04-27 18:29:38.000000 freegenius-0.1.7/freegenius.egg-info/PKG-INFO
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5909 2024-04-27 18:29:38.000000 freegenius-0.1.7/freegenius.egg-info/SOURCES.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-04-27 18:29:38.000000 freegenius-0.1.7/freegenius.egg-info/dependency_links.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-27 18:29:38.000000 freegenius-0.1.7/freegenius.egg-info/entry_points.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      841 2024-04-27 18:29:38.000000 freegenius-0.1.7/freegenius.egg-info/requires.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-04-27 18:29:38.000000 freegenius-0.1.7/freegenius.egg-info/top_level.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-04-27 18:29:38.713379 freegenius-0.1.7/setup.cfg
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10449 2024-04-27 18:29:06.000000 freegenius-0.1.7/setup.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.818296 freegenius-0.1.8/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    14938 2024-04-28 21:39:08.818296 freegenius-0.1.8/PKG-INFO
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.786296 freegenius-0.1.8/freegenius/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11766 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius/README.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.1.8/freegenius/__init__.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.790296 freegenius-0.1.8/freegenius/audio/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.1.8/freegenius/audio/notification1.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.1.8/freegenius/audio/notification1_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.1.8/freegenius/audio/notification2.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.1.8/freegenius/audio/notification2_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7006 2024-04-28 21:17:47.000000 freegenius-0.1.8/freegenius/autoassist.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.1.8/freegenius/autobuilder.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11081 2024-04-28 21:19:22.000000 freegenius-0.1.8/freegenius/autoretriever.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.1.8/freegenius/chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.1.8/freegenius/codey.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.1.8/freegenius/commandprompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius/config.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.1.8/freegenius/eTextEdit.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.790296 freegenius-0.1.8/freegenius/files/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.1.8/freegenius/files/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.1.8/freegenius/geminipro.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.1.8/freegenius/geminiprovision.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6492 2024-04-28 21:26:13.000000 freegenius-0.1.8/freegenius/groqchat.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.790296 freegenius-0.1.8/freegenius/gui/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.1.8/freegenius/gui/chatgui.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.1.8/freegenius/gui/worker.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.790296 freegenius-0.1.8/freegenius/history/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.1.8/freegenius/history/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.802296 freegenius-0.1.8/freegenius/icons/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.1.8/freegenius/icons/FreeGenius.ico
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.1.8/freegenius/icons/FreeGenius.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.1.8/freegenius/icons/FreeGenius_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.1.8/freegenius/icons/ai.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.1.8/freegenius/icons/ai_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.1.8/freegenius/llamacpp.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.782297 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.806296 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.1.8/freegenius/main.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.1.8/freegenius/ollamachat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius/package_name.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.1.8/freegenius/palm2.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.814296 freegenius-0.1.8/freegenius/plugins/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.1.8/freegenius/plugins/000_check_ffmpeg.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-04-25 10:21:23.000000 freegenius-0.1.8/freegenius/plugins/000_check_pyaudio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.1.8/freegenius/plugins/000_check_vlc.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.1.8/freegenius/plugins/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.1.8/freegenius/plugins/add calendar event.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.1.8/freegenius/plugins/aliases.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7437 2024-04-27 13:00:33.000000 freegenius-0.1.8/freegenius/plugins/analyze audio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.1.8/freegenius/plugins/analyze files.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4677 2024-04-27 13:03:55.000000 freegenius-0.1.8/freegenius/plugins/analyze images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.1.8/freegenius/plugins/analyze web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2559 2024-04-14 22:20:21.000000 freegenius-0.1.8/freegenius/plugins/auto correct python code.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.1.8/freegenius/plugins/awesome prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.1.8/freegenius/plugins/character analysis.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.1.8/freegenius/plugins/chat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.1.8/freegenius/plugins/contexts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.1.8/freegenius/plugins/counselling.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.1.8/freegenius/plugins/create ai assistants.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5160 2024-04-27 13:04:35.000000 freegenius-0.1.8/freegenius/plugins/create images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.1.8/freegenius/plugins/create maps.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.1.8/freegenius/plugins/create qrcode.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.1.8/freegenius/plugins/create statistical graphics.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.1.8/freegenius/plugins/dates and times.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.1.8/freegenius/plugins/download youtube or web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.1.8/freegenius/plugins/edit text.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.1.8/freegenius/plugins/execute computing tasks.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.1.8/freegenius/plugins/execute termux command.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.1.8/freegenius/plugins/global finance.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.1.8/freegenius/plugins/improve British English.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2315 2024-04-25 10:21:23.000000 freegenius-0.1.8/freegenius/plugins/input suggestions.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.1.8/freegenius/plugins/install python package.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.1.8/freegenius/plugins/integrate google searches.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.1.8/freegenius/plugins/memory.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8646 2024-04-27 13:03:30.000000 freegenius-0.1.8/freegenius/plugins/modify images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.1.8/freegenius/plugins/open web browser.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.1.8/freegenius/plugins/pronounce words.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.1.8/freegenius/plugins/remove image background.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5906 2024-04-27 11:30:39.000000 freegenius-0.1.8/freegenius/plugins/search chat records.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1156 2024-04-10 07:42:48.000000 freegenius-0.1.8/freegenius/plugins/search financial data.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.1.8/freegenius/plugins/search latest news.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.1.8/freegenius/plugins/search sqlite.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.1.8/freegenius/plugins/search weather info.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.1.8/freegenius/plugins/send email.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.1.8/freegenius/plugins/send tweet.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.1.8/freegenius/plugins/send whatsapp messages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.1.8/freegenius/plugins/simplified Chinese to traditional Chinese.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.1.8/freegenius/qt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.1.8/freegenius/rag.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      840 2024-04-26 22:24:44.000000 freegenius-0.1.8/freegenius/requirements.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1359 2024-04-25 20:30:31.000000 freegenius-0.1.8/freegenius/servers.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7714 2024-04-27 15:10:04.000000 freegenius-0.1.8/freegenius/systemtray.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.814296 freegenius-0.1.8/freegenius/temp/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.1.8/freegenius/temp/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.818296 freegenius-0.1.8/freegenius/utils/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   112155 2024-04-27 15:16:32.000000 freegenius-0.1.8/freegenius/utils/assistant.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29734 2024-04-26 22:27:56.000000 freegenius-0.1.8/freegenius/utils/call_chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    17269 2024-04-25 20:53:07.000000 freegenius-0.1.8/freegenius/utils/call_gemini.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    17228 2024-04-28 21:27:08.000000 freegenius-0.1.8/freegenius/utils/call_groq.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    24612 2024-04-25 20:52:45.000000 freegenius-0.1.8/freegenius/utils/call_llamacpp.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8528 2024-04-27 07:40:12.000000 freegenius-0.1.8/freegenius/utils/call_llm.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    18713 2024-04-25 20:53:07.000000 freegenius-0.1.8/freegenius/utils/call_ollama.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    18372 2024-04-28 21:23:25.000000 freegenius-0.1.8/freegenius/utils/config_essential.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.1.8/freegenius/utils/config_tools.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.1.8/freegenius/utils/download.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.1.8/freegenius/utils/get_path_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4888 2024-04-23 21:13:11.000000 freegenius-0.1.8/freegenius/utils/ollama_models.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.1.8/freegenius/utils/promptValidator.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.1.8/freegenius/utils/prompt_multiline_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.1.8/freegenius/utils/prompt_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.1.8/freegenius/utils/prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.1.8/freegenius/utils/python_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    50846 2024-04-28 21:25:47.000000 freegenius-0.1.8/freegenius/utils/shared_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.1.8/freegenius/utils/shortcuts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.1.8/freegenius/utils/single_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.1.8/freegenius/utils/streaming_word_wrapper.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.1.8/freegenius/utils/sttLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.1.8/freegenius/utils/terminal_mode_dialogs.py
+-rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.1.8/freegenius/utils/terminal_system_command_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.1.8/freegenius/utils/text_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4352 2024-04-12 22:26:19.000000 freegenius-0.1.8/freegenius/utils/tool_plugins.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7640 2024-02-22 00:47:05.000000 freegenius-0.1.8/freegenius/utils/ttsLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8563 2024-03-28 23:38:45.000000 freegenius-0.1.8/freegenius/utils/tts_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4651 2024-04-09 22:46:08.000000 freegenius-0.1.8/freegenius/utils/vlc_utils.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-28 21:39:08.818296 freegenius-0.1.8/freegenius.egg-info/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    14938 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius.egg-info/PKG-INFO
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5909 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius.egg-info/SOURCES.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius.egg-info/dependency_links.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius.egg-info/entry_points.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      841 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius.egg-info/requires.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-04-28 21:39:08.000000 freegenius-0.1.8/freegenius.egg-info/top_level.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-04-28 21:39:08.818296 freegenius-0.1.8/setup.cfg
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10449 2024-04-28 21:39:01.000000 freegenius-0.1.8/setup.py
```

### Comparing `freegenius-0.1.7/PKG-INFO` & `freegenius-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.1.7
+Version: 0.1.8
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.1.7/freegenius/README.md` & `freegenius-0.1.8/freegenius/README.md`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/__init__.py` & `freegenius-0.1.8/freegenius/__init__.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/audio/notification1.mp3` & `freegenius-0.1.8/freegenius/audio/notification1.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/audio/notification1_mild.mp3` & `freegenius-0.1.8/freegenius/audio/notification1_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/audio/notification2.mp3` & `freegenius-0.1.8/freegenius/audio/notification2.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/audio/notification2_mild.mp3` & `freegenius-0.1.8/freegenius/audio/notification2_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/autoassist.py` & `freegenius-0.1.8/freegenius/autoassist.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not os.path.isfile(configFile):
     open(configFile, "a", encoding="utf-8").close()
 from freegenius import config
 if not hasattr(config, "max_consecutive_auto_reply"):
     config.max_consecutive_auto_reply = 10
 
 import autogen, os, json, traceback
-from freegenius import getDeviceInfo, startLlamacppServer, stopLlamacppServer, tokenLimits
+from freegenius import getDeviceInfo, startLlamacppServer, stopLlamacppServer, getGroqApi_key, tokenLimits
 from freegenius.utils.prompts import Prompts
 from prompt_toolkit import print_formatted_text, HTML
 from prompt_toolkit.styles import Style
 #from prompt_toolkit import PromptSession
 #from prompt_toolkit.history import FileHistory
 
 
@@ -78,15 +78,15 @@
             ]
         elif config.llmInterface == "groq":
             config_list = [
                 {
                     "model": config.groqApi_main_model,
                     "base_url": "https://api.groq.com/openai/v1",
                     "api_type": "open_ai",
-                    "api_key": config.groqApi_key,
+                    "api_key": getGroqApi_key(),
                 }
             ]
         else:
         #elif config.llmInterface == "chatgpt":
             config_list = autogen.config_list_from_json(
                 env_or_file="OAI_CONFIG_LIST",  # or OAI_CONFIG_LIST.json if file extension is added
                 filter_dict={
```

### Comparing `freegenius-0.1.7/freegenius/autobuilder.py` & `freegenius-0.1.8/freegenius/autobuilder.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/autoretriever.py` & `freegenius-0.1.8/freegenius/autoretriever.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     open(configFile, "a", encoding="utf-8").close()
 from freegenius import config
 if not hasattr(config, "max_consecutive_auto_reply"):
     config.max_consecutive_auto_reply = 10
 
 from freegenius import print2, print3, tokenLimits
 
-from freegenius import getEmbeddingFunction, startLlamacppServer, stopLlamacppServer
+from freegenius import getEmbeddingFunction, startLlamacppServer, stopLlamacppServer, getGroqApi_key
 import autogen, os, json, traceback, chromadb, re, zipfile, datetime, traceback
 from chromadb.config import Settings
 from pathlib import Path
 from freegenius.utils.prompts import Prompts
 from prompt_toolkit import print_formatted_text, HTML
 from prompt_toolkit.styles import Style
 from autogen.retrieve_utils import TEXT_FORMATS
@@ -111,15 +111,15 @@
         elif config.llmInterface == "groq":
             llm = config.groqApi_main_model
             config_list = [
                 {
                     "model": llm,
                     "base_url": "https://api.groq.com/openai/v1",
                     "api_type": "open_ai",
-                    "api_key": config.groqApi_key,
+                    "api_key": getGroqApi_key(),
                 }
             ]
         else:
         #if config.llmInterface in ("chatgpt", "letmedoit", "gemini"):
             llm = config.chatGPTApiModel
             config_list = autogen.config_list_from_json(
                 env_or_file="OAI_CONFIG_LIST",  # or OAI_CONFIG_LIST.json if file extension is added
```

### Comparing `freegenius-0.1.7/freegenius/chatgpt.py` & `freegenius-0.1.8/freegenius/chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/codey.py` & `freegenius-0.1.8/freegenius/codey.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/commandprompt.py` & `freegenius-0.1.8/freegenius/commandprompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/eTextEdit.py` & `freegenius-0.1.8/freegenius/eTextEdit.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/geminipro.py` & `freegenius-0.1.8/freegenius/geminipro.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/geminiprovision.py` & `freegenius-0.1.8/freegenius/geminiprovision.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/groqchat.py` & `freegenius-0.1.8/freegenius/groqchat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from freegenius import config
-from freegenius import print2
+from freegenius import print2, getGroqClient
 from freegenius.utils.streaming_word_wrapper import StreamingWordWrapper
 from freegenius.utils.single_prompt import SinglePrompt
 
 from groq import Groq
 from prompt_toolkit.styles import Style
 from prompt_toolkit import PromptSession
 from prompt_toolkit.history import FileHistory
@@ -16,15 +16,15 @@
     """
     A simple Groq chatbot, without function calling.
     It is created for use with 3rd-party applications.
     """
 
     def __init__(self, name="Groq Chatbot", temperature=config.llmTemperature, max_output_tokens=config.groqApi_max_tokens):
         self.name, self.temperature, self.max_output_tokens = name, temperature, max_output_tokens
-        self.client = config.groq_client = Groq(api_key=config.groqApi_key)
+        self.client = getGroqClient()
         self.messages = self.resetMessages()
         if hasattr(config, "currentMessages") and config.currentMessages:
             self.messages += config.currentMessages[:-1]
         self.defaultPrompt = ""
 
     def resetMessages(self):
         return [{"role": "system", "content": config.systemMessage_groq},]
```

### Comparing `freegenius-0.1.7/freegenius/gui/chatgui.py` & `freegenius-0.1.8/freegenius/gui/chatgui.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/gui/worker.py` & `freegenius-0.1.8/freegenius/gui/worker.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/icons/FreeGenius.ico` & `freegenius-0.1.8/freegenius/icons/FreeGenius.ico`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/icons/FreeGenius.png` & `freegenius-0.1.8/freegenius/icons/FreeGenius.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/icons/FreeGenius_original.png` & `freegenius-0.1.8/freegenius/icons/FreeGenius_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/icons/ai.png` & `freegenius-0.1.8/freegenius/icons/ai.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/icons/ai_original.png` & `freegenius-0.1.8/freegenius/icons/ai_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/llamacpp.py` & `freegenius-0.1.8/freegenius/llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow` & `freegenius-0.1.8/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/main.py` & `freegenius-0.1.8/freegenius/main.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/ollamachat.py` & `freegenius-0.1.8/freegenius/ollamachat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/palm2.py` & `freegenius-0.1.8/freegenius/palm2.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/000_check_ffmpeg.py` & `freegenius-0.1.8/freegenius/plugins/000_check_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/000_check_pyaudio.py` & `freegenius-0.1.8/freegenius/plugins/000_check_pyaudio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/000_check_vlc.py` & `freegenius-0.1.8/freegenius/plugins/000_check_vlc.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/add calendar event.py` & `freegenius-0.1.8/freegenius/plugins/add calendar event.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/aliases.py` & `freegenius-0.1.8/freegenius/plugins/aliases.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/analyze audio.py` & `freegenius-0.1.8/freegenius/plugins/analyze audio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/analyze files.py` & `freegenius-0.1.8/freegenius/plugins/analyze files.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/analyze images.py` & `freegenius-0.1.8/freegenius/plugins/analyze images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/analyze web content.py` & `freegenius-0.1.8/freegenius/plugins/analyze web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/auto correct python code.py` & `freegenius-0.1.8/freegenius/plugins/auto correct python code.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/awesome prompts.py` & `freegenius-0.1.8/freegenius/plugins/awesome prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/character analysis.py` & `freegenius-0.1.8/freegenius/plugins/character analysis.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/chat.py` & `freegenius-0.1.8/freegenius/plugins/chat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/contexts.py` & `freegenius-0.1.8/freegenius/plugins/contexts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/counselling.py` & `freegenius-0.1.8/freegenius/plugins/counselling.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/create ai assistants.py` & `freegenius-0.1.8/freegenius/plugins/create ai assistants.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/create images.py` & `freegenius-0.1.8/freegenius/plugins/create images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/create maps.py` & `freegenius-0.1.8/freegenius/plugins/create maps.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/create qrcode.py` & `freegenius-0.1.8/freegenius/plugins/create qrcode.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/create statistical graphics.py` & `freegenius-0.1.8/freegenius/plugins/create statistical graphics.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/dates and times.py` & `freegenius-0.1.8/freegenius/plugins/dates and times.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/download youtube or web content.py` & `freegenius-0.1.8/freegenius/plugins/download youtube or web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/edit text.py` & `freegenius-0.1.8/freegenius/plugins/edit text.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/execute computing tasks.py` & `freegenius-0.1.8/freegenius/plugins/execute computing tasks.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/execute termux command.py` & `freegenius-0.1.8/freegenius/plugins/execute termux command.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/global finance.py` & `freegenius-0.1.8/freegenius/plugins/global finance.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/improve British English.py` & `freegenius-0.1.8/freegenius/plugins/improve British English.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/input suggestions.py` & `freegenius-0.1.8/freegenius/plugins/input suggestions.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/install python package.py` & `freegenius-0.1.8/freegenius/plugins/install python package.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/integrate google searches.py` & `freegenius-0.1.8/freegenius/plugins/integrate google searches.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/memory.py` & `freegenius-0.1.8/freegenius/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/modify images.py` & `freegenius-0.1.8/freegenius/plugins/modify images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/open web browser.py` & `freegenius-0.1.8/freegenius/plugins/open web browser.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/pronounce words.py` & `freegenius-0.1.8/freegenius/plugins/pronounce words.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/remove image background.py` & `freegenius-0.1.8/freegenius/plugins/remove image background.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/search chat records.py` & `freegenius-0.1.8/freegenius/plugins/search chat records.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/search financial data.py` & `freegenius-0.1.8/freegenius/plugins/search financial data.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/search latest news.py` & `freegenius-0.1.8/freegenius/plugins/search latest news.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/search sqlite.py` & `freegenius-0.1.8/freegenius/plugins/search sqlite.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/search weather info.py` & `freegenius-0.1.8/freegenius/plugins/search weather info.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/send email.py` & `freegenius-0.1.8/freegenius/plugins/send email.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/send tweet.py` & `freegenius-0.1.8/freegenius/plugins/send tweet.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/send whatsapp messages.py` & `freegenius-0.1.8/freegenius/plugins/send whatsapp messages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/plugins/simplified Chinese to traditional Chinese.py` & `freegenius-0.1.8/freegenius/plugins/simplified Chinese to traditional Chinese.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/rag.py` & `freegenius-0.1.8/freegenius/rag.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/requirements.txt` & `freegenius-0.1.8/freegenius/requirements.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/servers.py` & `freegenius-0.1.8/freegenius/servers.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/systemtray.py` & `freegenius-0.1.8/freegenius/systemtray.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/assistant.py` & `freegenius-0.1.8/freegenius/utils/assistant.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/call_chatgpt.py` & `freegenius-0.1.8/freegenius/utils/call_chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/call_gemini.py` & `freegenius-0.1.8/freegenius/utils/call_gemini.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/call_groq.py` & `freegenius-0.1.8/freegenius/utils/call_groq.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from freegenius import showErrors, get_or_create_collection, query_vectors, showRisk, executeToolFunction, getPythonFunctionResponse, getPygmentsStyle, fineTunePythonCode, confirmExecution
 from freegenius import config
-from freegenius import print1, print2, print3, selectTool, check_llm_errors
+from freegenius import print1, print2, print3, selectTool, check_llm_errors, getGroqClient
 import re, traceback, pprint, copy, textwrap, json, pygments
 from pygments.lexers.python import PythonLexer
 from prompt_toolkit import print_formatted_text, HTML
 from prompt_toolkit.formatted_text import PygmentsTokens
 from prompt_toolkit import prompt
 from groq import Groq
 
@@ -34,18 +34,15 @@
     @staticmethod
     def convertFunctionSignaturesIntoTools(functionSignatures):
         return [{"type": "function", "function": functionSignature} for functionSignature in functionSignatures]
 
     @staticmethod
     @check_llm_errors
     def checkCompletion():
-        config.groq_client = Groq(
-            api_key=config.groqApi_key,
-        )
-        config.groq_client.chat.completions.create(
+        getGroqClient().chat.completions.create(
             model=config.groqApi_main_model,
             messages=[{"role": "user", "content" : "hello"}],
             n=1,
             max_tokens=10,
         )
 
     @staticmethod
@@ -88,15 +85,15 @@
     @check_llm_errors
     def getSingleChatResponse(userInput, messages=[], temperature=None):
         """
         non-streaming single call
         """
         messages.append({"role": "user", "content" : userInput})
         try:
-            completion = config.groq_client.chat.completions.create(
+            completion = getGroqClient().chat.completions.create(
                 model=config.groqApi_main_model,
                 messages=messages,
                 n=1,
                 temperature=temperature if temperature is not None else config.llmTemperature,
                 max_tokens=config.groqApi_max_tokens,
             )
             return completion.choices[0].message.content
@@ -192,15 +189,15 @@
             return messagesCopy
         return messages
 
     @staticmethod
     @check_llm_errors
     def getSingleFunctionCallResponse(messages: list[dict], function_name: str, temperature=None, **kwargs):
         functionSignatures = [config.toolFunctionSchemas[function_name]]
-        completion = config.groq_client.chat.completions.create(
+        completion = getGroqClient().chat.completions.create(
             model=config.groqApi_main_model,
             messages=messages,
             n=1,
             temperature=temperature if temperature is not None else config.llmTemperature,
             max_tokens=config.groqApi_max_tokens,
             tools=CallGroq.convertFunctionSignaturesIntoTools(functionSignatures),
             tool_choice={"type": "function", "function": {"name": function_name}},
@@ -220,28 +217,28 @@
         }
         function_call_response = CallGroq.finetuneSingleFunctionCallResponse(func_arguments, function_name)
         return function_call_message_mini, function_call_response
 
     @staticmethod
     @check_llm_errors
     def regularCall(messages: dict, **kwargs):
-        return config.groq_client.chat.completions.create(
+        return getGroqClient().chat.completions.create(
             model=config.groqApi_main_model,
             messages=messages,
             n=1,
             temperature=config.llmTemperature,
             max_tokens=config.groqApi_max_tokens,
             stream=True,
             **kwargs,
         )
 
     @staticmethod
     @check_llm_errors
     def getResponseDict(messages: list, schema: dict, **kwargs) -> dict:
-        completion = config.groq_client.chat.completions.create(
+        completion = getGroqClient().chat.completions.create(
             model=config.groqApi_main_model,
             messages=messages,
             n=1,
             temperature=config.llmTemperature,
             max_tokens=config.groqApi_max_tokens,
             tools=[{"type": "function", "function": schema}],
             tool_choice={"type": "function", "function": {"name": schema["name"]}},
```

### Comparing `freegenius-0.1.7/freegenius/utils/call_llamacpp.py` & `freegenius-0.1.8/freegenius/utils/call_llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/call_llm.py` & `freegenius-0.1.8/freegenius/utils/call_llm.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/call_ollama.py` & `freegenius-0.1.8/freegenius/utils/call_ollama.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/config_essential.py` & `freegenius-0.1.8/freegenius/utils/config_essential.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,14 @@
     "freeGeniusActionExamples",
     "freeGeniusActionParameters",
     "freeGeniusActionMethods",
     "google_cloud_credentials_file",
     "actionHelp",
     "isTermux",
     "oai_client",
-    "groq_client",
     "includeIpInDeviceInfoTemp",
     "initialCompletionCheck",
     "promptStyle1",
     "promptStyle2",
     "selectedTool",
     "pluginsWithFunctionCall",
     "restartApp",
```

### Comparing `freegenius-0.1.7/freegenius/utils/config_tools.py` & `freegenius-0.1.8/freegenius/utils/config_tools.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/download.py` & `freegenius-0.1.8/freegenius/utils/download.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/get_path_prompt.py` & `freegenius-0.1.8/freegenius/utils/get_path_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/ollama_models.py` & `freegenius-0.1.8/freegenius/utils/ollama_models.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/promptValidator.py` & `freegenius-0.1.8/freegenius/utils/promptValidator.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/prompt_multiline_shared_key_bindings.py` & `freegenius-0.1.8/freegenius/utils/prompt_multiline_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/prompt_shared_key_bindings.py` & `freegenius-0.1.8/freegenius/utils/prompt_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/prompts.py` & `freegenius-0.1.8/freegenius/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/python_utils.py` & `freegenius-0.1.8/freegenius/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/shared_utils.py` & `freegenius-0.1.8/freegenius/utils/shared_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 from openai import OpenAI
 from huggingface_hub import hf_hub_download
 from bs4 import BeautifulSoup
 from urllib.parse import quote
 from guidance import select, gen
 from typing import Union
 from transformers import pipeline
-from functools import wraps
-
+from groq import Groq
 
 # non-Android only
 if not config.isTermux:
     from autogen.retrieve_utils import TEXT_FORMATS
 
 # a dummy import line to resolve ALSA error display on Linux
 import sounddevice
@@ -166,14 +165,35 @@
 Thought: {gen(stop=".")}.
 Action: {select(tool_names, name="tool")}"""
     
     return lm.get("tool")
 
 # local llm
 
+def getGroqApi_key():
+    '''
+    support multiple grop api keys to work around rate limit
+    User can manually edit config to change the value of config.groqApi_key to a list of multiple api keys instead of a string of a single api key
+    '''
+    if config.groqApi_key:
+        if isinstance(config.groqApi_key, str):
+            return config.groqApi_key
+        elif isinstance(config.groqApi_key, list):
+            if len(config.groqApi_key) > 1:
+                # rotate multiple api keys
+                config.groqApi_key = config.groqApi_key[1:] + [config.groqApi_key[0]]
+            return config.groqApi_key[0]
+        else:
+            return ""
+    else:
+        return ""
+
+def getGroqClient():
+    return Groq(api_key=getGroqApi_key())
+
 def downloadStableDiffusionFiles():
     # llm directory
     llm_directory = os.path.join(config.localStorage, "LLMs", "stable_diffusion")
     Path(llm_directory).mkdir(parents=True, exist_ok=True)
     filename = "v1-5-pruned-emaonly.safetensors"
     stableDiffusion_model_path = os.path.join(llm_directory, filename)
     if not config.stableDiffusion_model_path or not os.path.isfile(config.stableDiffusion_model_path):
```

### Comparing `freegenius-0.1.7/freegenius/utils/shortcuts.py` & `freegenius-0.1.8/freegenius/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/single_prompt.py` & `freegenius-0.1.8/freegenius/utils/single_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/streaming_word_wrapper.py` & `freegenius-0.1.8/freegenius/utils/streaming_word_wrapper.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/sttLanguages.py` & `freegenius-0.1.8/freegenius/utils/sttLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/terminal_mode_dialogs.py` & `freegenius-0.1.8/freegenius/utils/terminal_mode_dialogs.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/terminal_system_command_prompt.py` & `freegenius-0.1.8/freegenius/utils/terminal_system_command_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/text_utils.py` & `freegenius-0.1.8/freegenius/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/tool_plugins.py` & `freegenius-0.1.8/freegenius/utils/tool_plugins.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/ttsLanguages.py` & `freegenius-0.1.8/freegenius/utils/ttsLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/tts_utils.py` & `freegenius-0.1.8/freegenius/utils/tts_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius/utils/vlc_utils.py` & `freegenius-0.1.8/freegenius/utils/vlc_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius.egg-info/PKG-INFO` & `freegenius-0.1.8/freegenius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.1.7
+Version: 0.1.8
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.1.7/freegenius.egg-info/SOURCES.txt` & `freegenius-0.1.8/freegenius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius.egg-info/entry_points.txt` & `freegenius-0.1.8/freegenius.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/freegenius.egg-info/requires.txt` & `freegenius-0.1.8/freegenius.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.1.7/setup.py` & `freegenius-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 # make sure config.py is empty
 open(os.path.join(package, "config.py"), "w").close()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="0.1.7",
+    version="0.1.8",
     python_requires=">=3.8, <3.12",
     description=f"{appFullName}, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     cmdclass={
         'install': PreInstallCommand,
```

