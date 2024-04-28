# Comparing `tmp/diambra-engine-2.2.2.tar.gz` & `tmp/diambra-engine-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diambra-engine-2.2.2.tar", last modified: Sat Apr  6 12:13:25 2024, max compression
+gzip compressed data, was "diambra-engine-2.2.3.tar", last modified: Sun Apr 28 15:30:46 2024, max compression
```

## Comparing `diambra-engine-2.2.2.tar` & `diambra-engine-2.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:13:25.184984 diambra-engine-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-06 12:13:25.184984 diambra-engine-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-06 12:13:10.000000 diambra-engine-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:13:25.180984 diambra-engine-2.2.2/diambra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:13:10.000000 diambra-engine-2.2.2/diambra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:13:25.180984 diambra-engine-2.2.2/diambra/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-06 12:13:10.000000 diambra-engine-2.2.2/diambra/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28509 2024-04-06 12:13:23.000000 diambra-engine-2.2.2/diambra/engine/interface_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10562 2024-04-06 12:13:23.000000 diambra-engine-2.2.2/diambra/engine/interface_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:13:25.184984 diambra-engine-2.2.2/diambra_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-06 12:13:25.000000 diambra-engine-2.2.2/diambra_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-06 12:13:25.000000 diambra-engine-2.2.2/diambra_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 12:13:25.000000 diambra-engine-2.2.2/diambra_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-06 12:13:25.000000 diambra-engine-2.2.2/diambra_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 12:13:25.000000 diambra-engine-2.2.2/diambra_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 12:13:25.184984 diambra-engine-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-06 12:13:10.000000 diambra-engine-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:30:46.820932 diambra-engine-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-28 15:30:46.820932 diambra-engine-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-28 15:30:36.000000 diambra-engine-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:30:46.816932 diambra-engine-2.2.3/diambra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 15:30:36.000000 diambra-engine-2.2.3/diambra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:30:46.816932 diambra-engine-2.2.3/diambra/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-28 15:30:36.000000 diambra-engine-2.2.3/diambra/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28742 2024-04-28 15:30:45.000000 diambra-engine-2.2.3/diambra/engine/interface_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8969 2024-04-28 15:30:45.000000 diambra-engine-2.2.3/diambra/engine/interface_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 15:30:46.816932 diambra-engine-2.2.3/diambra_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-28 15:30:46.000000 diambra-engine-2.2.3/diambra_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-28 15:30:46.000000 diambra-engine-2.2.3/diambra_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 15:30:46.000000 diambra-engine-2.2.3/diambra_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-28 15:30:46.000000 diambra-engine-2.2.3/diambra_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 15:30:46.000000 diambra-engine-2.2.3/diambra_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 15:30:46.820932 diambra-engine-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-28 15:30:36.000000 diambra-engine-2.2.3/setup.py
```

### Comparing `diambra-engine-2.2.2/PKG-INFO` & `diambra-engine-2.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-engine
-Version: 2.2.2
+Version: 2.2.3
 Summary: DIAMBRA™ Arena Engine API Client
 Home-page: https://diambra.ai
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

### Comparing `diambra-engine-2.2.2/diambra/engine/__init__.py` & `diambra-engine-2.2.3/diambra/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `diambra-engine-2.2.2/diambra/engine/interface_pb2.py` & `diambra-engine-2.2.3/diambra/engine/interface_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x64iambra/engine/interface.proto\x12\tinterface\"\x07\n\x05\x45mpty\"-\n\nFrameShape\x12\t\n\x01h\x18\x01 \x01(\x05\x12\t\n\x01w\x18\x02 \x01(\x05\x12\t\n\x01\x63\x18\x03 \x01(\x05\"6\n\x0cRamStateInfo\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x0b\n\x03min\x18\x02 \x01(\x05\x12\x0b\n\x03max\x18\x03 \x01(\x05\"%\n\x0c\x45rrorMessage\x12\x15\n\rerror_message\x18\x01 \x01(\t\"\x9e\t\n\x0b\x45nvSettings\x12\x0f\n\x07game_id\x18\x01 \x01(\t\x12*\n\x0b\x66rame_shape\x18\x02 \x01(\x0b\x32\x15.interface.FrameShape\x12\x12\n\nstep_ratio\x18\x03 \x01(\x05\x12\x11\n\tn_players\x18\x04 \x01(\x05\x12\x18\n\x10\x64isable_keyboard\x18\x05 \x01(\x08\x12\x18\n\x10\x64isable_joystick\x18\x06 \x01(\x08\x12\x0c\n\x04rank\x18\x07 \x01(\x05\x12,\n\raction_spaces\x18\x08 \x03(\x0e\x32\x15.interface.SpaceTypes\x12@\n\x10\x65pisode_settings\x18\t \x01(\x0b\x32&.interface.EnvSettings.EpisodeSettings\x12\x38\n\x0csys_settings\x18\n \x01(\x0b\x32\".interface.EnvSettings.SysSettings\x1a\xce\x02\n\x0bSysSettings\x12G\n\x0b\x62uttons_cfg\x18\x01 \x03(\x0b\x32\x32.interface.EnvSettings.SysSettings.ButtonsCfgEntry\x12\x11\n\trecording\x18\x02 \x01(\x08\x12\x16\n\x0e\x65mu_pipes_path\x18\x03 \x01(\t\x12\x11\n\troms_path\x18\x04 \x01(\t\x12\x13\n\x0b\x62inary_path\x18\x05 \x01(\t\x12\x0e\n\x06sha256\x18\x06 \x01(\t\x12\x0e\n\x06render\x18\x07 \x01(\x08\x12\x10\n\x08lock_fps\x18\x08 \x01(\x08\x12\r\n\x05sound\x18\t \x01(\x08\x12\r\n\x05\x64\x65\x62ug\x18\n \x01(\x08\x12\x0e\n\x06\x63heats\x18\x0b \x01(\x08\x12\x10\n\x08username\x18\x0c \x01(\t\x1a\x31\n\x0f\x42uttonsCfgEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xed\x03\n\x0f\x45pisodeSettings\x12\x13\n\x0brandom_seed\x18\x01 \x01(\x05\x12\x12\n\ndifficulty\x18\x02 \x01(\x05\x12\x15\n\rcontinue_game\x18\x03 \x01(\x01\x12\x12\n\nshow_final\x18\x04 \x01(\x08\x12\r\n\x05tower\x18\x05 \x01(\x05\x12N\n\x0fplayer_settings\x18\x06 \x03(\x0b\x32\x35.interface.EnvSettings.EpisodeSettings.PlayerSettings\x1a\xa6\x02\n\x0ePlayerSettings\x12,\n\x04role\x18\x01 \x01(\x0e\x32\x1e.interface.RamStatesCategories\x12\x12\n\ncharacters\x18\x02 \x03(\t\x12\x0f\n\x07outfits\x18\x03 \x01(\x05\x12\x11\n\tsuper_art\x18\x04 \x01(\x05\x12\x16\n\x0e\x66ighting_style\x18\x05 \x01(\x05\x12[\n\x0eultimate_style\x18\x06 \x01(\x0b\x32\x43.interface.EnvSettings.EpisodeSettings.PlayerSettings.UltimateStyle\x1a\x39\n\rUltimateStyle\x12\x0c\n\x04\x64\x61sh\x18\x01 \x01(\x05\x12\r\n\x05\x65vade\x18\x02 \x01(\x05\x12\x0b\n\x03\x62\x61r\x18\x03 \x01(\x05\"\xce\n\n\x0f\x45nvInitResponse\x12\x46\n\x11\x61vailable_actions\x18\x01 \x01(\x0b\x32+.interface.EnvInitResponse.AvailableActions\x12*\n\x0b\x66rame_shape\x18\x02 \x01(\x0b\x32\x15.interface.FrameShape\x12S\n\x18\x63umulative_reward_bounds\x18\x03 \x01(\x0b\x32\x31.interface.EnvInitResponse.CumulativeRewardBounds\x12\x42\n\x0f\x63haracters_info\x18\x04 \x01(\x0b\x32).interface.EnvInitResponse.CharactersInfo\x12\x46\n\x11\x64ifficulty_bounds\x18\x05 \x01(\x0b\x32+.interface.EnvInitResponse.DifficultyBounds\x12R\n\x15ram_states_categories\x18\x06 \x03(\x0b\x32\x33.interface.EnvInitResponse.RamStatesCategoriesEntry\x1a\xff\x01\n\x10\x41vailableActions\x12\x0f\n\x07n_moves\x18\x01 \x01(\x05\x12\x11\n\tn_attacks\x18\x02 \x01(\x05\x12\x19\n\x11n_attacks_no_comb\x18\x03 \x01(\x05\x12\x41\n\x05moves\x18\x04 \x03(\x0b\x32\x32.interface.EnvInitResponse.AvailableActions.Button\x12\x43\n\x07\x61ttacks\x18\x05 \x03(\x0b\x32\x32.interface.EnvInitResponse.AvailableActions.Button\x1a$\n\x06\x42utton\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x1a\x32\n\x16\x43umulativeRewardBounds\x12\x0b\n\x03min\x18\x01 \x01(\x05\x12\x0b\n\x03max\x18\x02 \x01(\x05\x1a,\n\x10\x44ifficultyBounds\x12\x0b\n\x03min\x18\x01 \x01(\x05\x12\x0b\n\x03max\x18\x02 \x01(\x05\x1a\x85\x02\n\x0e\x43haractersInfo\x12\x11\n\tchar_list\x18\x01 \x03(\t\x12\x1b\n\x13\x63har_forbidden_list\x18\x02 \x03(\t\x12Y\n\x11\x63har_homonymy_map\x18\x03 \x03(\x0b\x32>.interface.EnvInitResponse.CharactersInfo.CharHomonymyMapEntry\x12\x17\n\x0f\x63hars_per_round\x18\x04 \x01(\x05\x12\x17\n\x0f\x63hars_to_select\x18\x05 \x01(\x05\x1a\x36\n\x14\x43harHomonymyMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xb7\x01\n\x15\x43\x61tegoryRamStatesInfo\x12S\n\nram_states\x18\x01 \x03(\x0b\x32?.interface.EnvInitResponse.CategoryRamStatesInfo.RamStatesEntry\x1aI\n\x0eRamStatesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.interface.RamStateInfo:\x02\x38\x01\x1al\n\x18RamStatesCategoriesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12?\n\x05value\x18\x02 \x01(\x0b\x32\x30.interface.EnvInitResponse.CategoryRamStatesInfo:\x02\x38\x01\"]\n\x07\x41\x63tions\x12*\n\x07\x61\x63tions\x18\x01 \x03(\x0b\x32\x19.interface.Actions.Action\x1a&\n\x06\x41\x63tion\x12\x0c\n\x04move\x18\x01 \x01(\x05\x12\x0e\n\x06\x61ttack\x18\x02 \x01(\x05\"\xb7\x05\n\x11StepResetResponse\x12=\n\x0bobservation\x18\x01 \x01(\x0b\x32(.interface.StepResetResponse.Observation\x12\x0e\n\x06reward\x18\x02 \x01(\x05\x12/\n\x04info\x18\x03 \x01(\x0b\x32!.interface.StepResetResponse.Info\x1a\x9d\x03\n\x0bObservation\x12\r\n\x05\x66rame\x18\x01 \x01(\x0c\x12`\n\x15ram_states_categories\x18\x02 \x03(\x0b\x32\x41.interface.StepResetResponse.Observation.RamStatesCategoriesEntry\x1a\xa4\x01\n\x11\x43\x61tegoryRamStates\x12]\n\nram_states\x18\x01 \x03(\x0b\x32I.interface.StepResetResponse.Observation.CategoryRamStates.RamStatesEntry\x1a\x30\n\x0eRamStatesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x1av\n\x18RamStatesCategoriesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12I\n\x05value\x18\x02 \x01(\x0b\x32:.interface.StepResetResponse.Observation.CategoryRamStates:\x02\x38\x01\x1a\x81\x01\n\x04Info\x12\x46\n\x0bgame_states\x18\x01 \x03(\x0b\x32\x31.interface.StepResetResponse.Info.GameStatesEntry\x1a\x31\n\x0fGameStatesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01*C\n\nSpaceTypes\x12\n\n\x06\x42INARY\x10\x00\x12\x0c\n\x08\x44ISCRETE\x10\x01\x12\x12\n\x0eMULTI_DISCRETE\x10\x02\x12\x07\n\x03\x42OX\x10\x03*[\n\nGameStates\x12\x0e\n\nround_done\x10\x00\x12\x0e\n\nstage_done\x10\x01\x12\r\n\tgame_done\x10\x02\x12\x10\n\x0c\x65pisode_done\x10\x03\x12\x0c\n\x08\x65nv_done\x10\x04*?\n\x13RamStatesCategories\x12\x0c\n\x08internal\x10\x00\x12\n\n\x06\x63ommon\x10\x01\x12\x06\n\x02P1\x10\x02\x12\x06\n\x02P2\x10\x03*\xa5\x05\n\tRamStates\x12\x0c\n\x08\x66ighting\x10\x00\x12\x0e\n\nfighting_1\x10\x01\x12\x0e\n\nfighting_2\x10\x02\x12\x14\n\x10round_time_elaps\x10\x03\x12\x15\n\x11on_fighting_stage\x10\x04\x12\x0f\n\x0bround_phase\x10\x05\x12\r\n\ttest_mode\x10\x06\x12\x16\n\x12\x63haracter_1_P2_fix\x10\x07\x12\x16\n\x12\x63haracter_2_P2_fix\x10\x08\x12\x16\n\x12\x63haracter_3_P2_fix\x10\t\x12\t\n\x05stage\x10\x64\x12\t\n\x05timer\x10\x65\x12\t\n\x04side\x10\xc8\x01\x12\t\n\x04wins\x10\xc9\x01\x12\x0e\n\tcharacter\x10\xca\x01\x12\x0b\n\x06health\x10\xcb\x01\x12\x0e\n\tsuper_bar\x10\xcc\x01\x12\x10\n\x0bsuper_count\x10\xcd\x01\x12\x14\n\x0fsuper_max_count\x10\xce\x01\x12\x0f\n\nsuper_type\x10\xcf\x01\x12\r\n\x08stun_bar\x10\xd0\x01\x12\x0c\n\x07stunned\x10\xd1\x01\x12\r\n\x08health_1\x10\xd2\x01\x12\r\n\x08health_2\x10\xd3\x01\x12\x15\n\x10\x61\x63tive_character\x10\xd4\x01\x12\x10\n\x0b\x63haracter_1\x10\xd5\x01\x12\x10\n\x0b\x63haracter_2\x10\xd6\x01\x12\x0f\n\nbar_status\x10\xd7\x01\x12\x12\n\raggressor_bar\x10\xd8\x01\x12\x0f\n\nweapon_bar\x10\xd9\x01\x12\x0e\n\tpower_bar\x10\xda\x01\x12\x11\n\x0cweapon_fight\x10\xdb\x01\x12\x10\n\x0bweapon_lost\x10\xdc\x01\x12\x0c\n\x07rage_on\x10\xdd\x01\x12\r\n\x08rage_bar\x10\xde\x01\x12\x0e\n\trage_used\x10\xdf\x01\x12\x14\n\x0fspecial_attacks\x10\xe0\x01\x12\r\n\x08\x62\x61r_type\x10\xe1\x01\x12\x10\n\x0b\x63haracter_3\x10\xe2\x01\x32\xf3\x02\n\tEnvServer\x12\x37\n\x08GetError\x12\x10.interface.Empty\x1a\x17.interface.ErrorMessage\"\x00\x12?\n\x07\x45nvInit\x12\x16.interface.EnvSettings\x1a\x1a.interface.EnvInitResponse\"\x00\x12O\n\x05Reset\x12&.interface.EnvSettings.EpisodeSettings\x1a\x1c.interface.StepResetResponse\"\x00\x12:\n\x04Step\x12\x12.interface.Actions\x1a\x1c.interface.StepResetResponse\"\x00\x12-\n\x05\x43lose\x12\x10.interface.Empty\x1a\x10.interface.Empty\"\x00\x12\x30\n\x08Shutdown\x12\x10.interface.Empty\x1a\x10.interface.Empty\"\x00\x42\x06\xa2\x02\x03HLWb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x64iambra/engine/interface.proto\x12\tinterface\"\x07\n\x05\x45mpty\"-\n\nFrameShape\x12\t\n\x01h\x18\x01 \x01(\x05\x12\t\n\x01w\x18\x02 \x01(\x05\x12\t\n\x01\x63\x18\x03 \x01(\x05\"6\n\x0cRamStateInfo\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x0b\n\x03min\x18\x02 \x01(\x05\x12\x0b\n\x03max\x18\x03 \x01(\x05\"%\n\x0c\x45rrorMessage\x12\x15\n\rerror_message\x18\x01 \x01(\t\"\xb2\t\n\x0b\x45nvSettings\x12\x0f\n\x07game_id\x18\x01 \x01(\t\x12*\n\x0b\x66rame_shape\x18\x02 \x01(\x0b\x32\x15.interface.FrameShape\x12\x12\n\nstep_ratio\x18\x03 \x01(\x05\x12\x11\n\tn_players\x18\x04 \x01(\x05\x12\x18\n\x10\x64isable_keyboard\x18\x05 \x01(\x08\x12\x18\n\x10\x64isable_joystick\x18\x06 \x01(\x08\x12\x0c\n\x04rank\x18\x07 \x01(\x05\x12,\n\raction_spaces\x18\x08 \x03(\x0e\x32\x15.interface.SpaceTypes\x12@\n\x10\x65pisode_settings\x18\t \x01(\x0b\x32&.interface.EnvSettings.EpisodeSettings\x12\x38\n\x0csys_settings\x18\n \x01(\x0b\x32\".interface.EnvSettings.SysSettings\x1a\xce\x02\n\x0bSysSettings\x12G\n\x0b\x62uttons_cfg\x18\x01 \x03(\x0b\x32\x32.interface.EnvSettings.SysSettings.ButtonsCfgEntry\x12\x11\n\trecording\x18\x02 \x01(\x08\x12\x16\n\x0e\x65mu_pipes_path\x18\x03 \x01(\t\x12\x11\n\troms_path\x18\x04 \x01(\t\x12\x13\n\x0b\x62inary_path\x18\x05 \x01(\t\x12\x0e\n\x06sha256\x18\x06 \x01(\t\x12\x0e\n\x06render\x18\x07 \x01(\x08\x12\x10\n\x08lock_fps\x18\x08 \x01(\x08\x12\r\n\x05sound\x18\t \x01(\x08\x12\r\n\x05\x64\x65\x62ug\x18\n \x01(\x08\x12\x0e\n\x06\x63heats\x18\x0b \x01(\x08\x12\x10\n\x08username\x18\x0c \x01(\t\x1a\x31\n\x0f\x42uttonsCfgEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x81\x04\n\x0f\x45pisodeSettings\x12\x13\n\x0brandom_seed\x18\x01 \x01(\x05\x12\x12\n\ndifficulty\x18\x02 \x01(\x05\x12\x15\n\rcontinue_game\x18\x03 \x01(\x01\x12\x12\n\nshow_final\x18\x04 \x01(\x08\x12\r\n\x05tower\x18\x05 \x01(\x05\x12N\n\x0fplayer_settings\x18\x06 \x03(\x0b\x32\x35.interface.EnvSettings.EpisodeSettings.PlayerSettings\x1a\xba\x02\n\x0ePlayerSettings\x12,\n\x04role\x18\x01 \x01(\x0e\x32\x1e.interface.RamStatesCategories\x12\x12\n\ncharacters\x18\x02 \x03(\t\x12\x0f\n\x07outfits\x18\x03 \x01(\x05\x12\x11\n\tsuper_art\x18\x04 \x01(\x05\x12\x16\n\x0e\x66ighting_style\x18\x05 \x01(\x05\x12[\n\x0eultimate_style\x18\x06 \x01(\x0b\x32\x43.interface.EnvSettings.EpisodeSettings.PlayerSettings.UltimateStyle\x12\x12\n\nspeed_mode\x18\x07 \x01(\x05\x1a\x39\n\rUltimateStyle\x12\x0c\n\x04\x64\x61sh\x18\x01 \x01(\x05\x12\r\n\x05\x65vade\x18\x02 \x01(\x05\x12\x0b\n\x03\x62\x61r\x18\x03 \x01(\x05\"\xe4\n\n\x0f\x45nvInitResponse\x12\x46\n\x11\x61vailable_actions\x18\x01 \x01(\x0b\x32+.interface.EnvInitResponse.AvailableActions\x12*\n\x0b\x66rame_shape\x18\x02 \x01(\x0b\x32\x15.interface.FrameShape\x12S\n\x18\x63umulative_reward_bounds\x18\x03 \x01(\x0b\x32\x31.interface.EnvInitResponse.CumulativeRewardBounds\x12\x42\n\x0f\x63haracters_info\x18\x04 \x01(\x0b\x32).interface.EnvInitResponse.CharactersInfo\x12\x46\n\x11\x64ifficulty_bounds\x18\x05 \x01(\x0b\x32+.interface.EnvInitResponse.DifficultyBounds\x12R\n\x15ram_states_categories\x18\x06 \x03(\x0b\x32\x33.interface.EnvInitResponse.RamStatesCategoriesEntry\x1a\xff\x01\n\x10\x41vailableActions\x12\x0f\n\x07n_moves\x18\x01 \x01(\x05\x12\x11\n\tn_attacks\x18\x02 \x01(\x05\x12\x19\n\x11n_attacks_no_comb\x18\x03 \x01(\x05\x12\x41\n\x05moves\x18\x04 \x03(\x0b\x32\x32.interface.EnvInitResponse.AvailableActions.Button\x12\x43\n\x07\x61ttacks\x18\x05 \x03(\x0b\x32\x32.interface.EnvInitResponse.AvailableActions.Button\x1a$\n\x06\x42utton\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x1a\x32\n\x16\x43umulativeRewardBounds\x12\x0b\n\x03min\x18\x01 \x01(\x05\x12\x0b\n\x03max\x18\x02 \x01(\x05\x1a,\n\x10\x44ifficultyBounds\x12\x0b\n\x03min\x18\x01 \x01(\x05\x12\x0b\n\x03max\x18\x02 \x01(\x05\x1a\x9b\x02\n\x0e\x43haractersInfo\x12\x11\n\tchar_list\x18\x01 \x03(\t\x12\x1b\n\x13\x63har_forbidden_list\x18\x02 \x03(\t\x12Y\n\x11\x63har_homonymy_map\x18\x03 \x03(\x0b\x32>.interface.EnvInitResponse.CharactersInfo.CharHomonymyMapEntry\x12\x17\n\x0f\x63hars_per_round\x18\x04 \x01(\x05\x12\x17\n\x0f\x63hars_to_select\x18\x05 \x01(\x05\x12\x14\n\x0cpartner_list\x18\x06 \x03(\t\x1a\x36\n\x14\x43harHomonymyMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xb7\x01\n\x15\x43\x61tegoryRamStatesInfo\x12S\n\nram_states\x18\x01 \x03(\x0b\x32?.interface.EnvInitResponse.CategoryRamStatesInfo.RamStatesEntry\x1aI\n\x0eRamStatesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.interface.RamStateInfo:\x02\x38\x01\x1al\n\x18RamStatesCategoriesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12?\n\x05value\x18\x02 \x01(\x0b\x32\x30.interface.EnvInitResponse.CategoryRamStatesInfo:\x02\x38\x01\"]\n\x07\x41\x63tions\x12*\n\x07\x61\x63tions\x18\x01 \x03(\x0b\x32\x19.interface.Actions.Action\x1a&\n\x06\x41\x63tion\x12\x0c\n\x04move\x18\x01 \x01(\x05\x12\x0e\n\x06\x61ttack\x18\x02 \x01(\x05\"\xb7\x05\n\x11StepResetResponse\x12=\n\x0bobservation\x18\x01 \x01(\x0b\x32(.interface.StepResetResponse.Observation\x12\x0e\n\x06reward\x18\x02 \x01(\x05\x12/\n\x04info\x18\x03 \x01(\x0b\x32!.interface.StepResetResponse.Info\x1a\x9d\x03\n\x0bObservation\x12\r\n\x05\x66rame\x18\x01 \x01(\x0c\x12`\n\x15ram_states_categories\x18\x02 \x03(\x0b\x32\x41.interface.StepResetResponse.Observation.RamStatesCategoriesEntry\x1a\xa4\x01\n\x11\x43\x61tegoryRamStates\x12]\n\nram_states\x18\x01 \x03(\x0b\x32I.interface.StepResetResponse.Observation.CategoryRamStates.RamStatesEntry\x1a\x30\n\x0eRamStatesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x1av\n\x18RamStatesCategoriesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12I\n\x05value\x18\x02 \x01(\x0b\x32:.interface.StepResetResponse.Observation.CategoryRamStates:\x02\x38\x01\x1a\x81\x01\n\x04Info\x12\x46\n\x0bgame_states\x18\x01 \x03(\x0b\x32\x31.interface.StepResetResponse.Info.GameStatesEntry\x1a\x31\n\x0fGameStatesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01*C\n\nSpaceTypes\x12\n\n\x06\x42INARY\x10\x00\x12\x0c\n\x08\x44ISCRETE\x10\x01\x12\x12\n\x0eMULTI_DISCRETE\x10\x02\x12\x07\n\x03\x42OX\x10\x03*[\n\nGameStates\x12\x0e\n\nround_done\x10\x00\x12\x0e\n\nstage_done\x10\x01\x12\r\n\tgame_done\x10\x02\x12\x10\n\x0c\x65pisode_done\x10\x03\x12\x0c\n\x08\x65nv_done\x10\x04*?\n\x13RamStatesCategories\x12\x0c\n\x08internal\x10\x00\x12\n\n\x06\x63ommon\x10\x01\x12\x06\n\x02P1\x10\x02\x12\x06\n\x02P2\x10\x03*\xf5\x05\n\tRamStates\x12\x0c\n\x08\x66ighting\x10\x00\x12\x0e\n\nfighting_1\x10\x01\x12\x0e\n\nfighting_2\x10\x02\x12\x14\n\x10round_time_elaps\x10\x03\x12\x15\n\x11on_fighting_stage\x10\x04\x12\x0f\n\x0bround_phase\x10\x05\x12\r\n\ttest_mode\x10\x06\x12\x16\n\x12\x63haracter_1_P2_fix\x10\x07\x12\x16\n\x12\x63haracter_2_P2_fix\x10\x08\x12\x16\n\x12\x63haracter_3_P2_fix\x10\t\x12\x14\n\x10\x63ontinue_time_p1\x10\n\x12\x14\n\x10\x63ontinue_time_p2\x10\x0b\x12\t\n\x05stage\x10\x64\x12\t\n\x05timer\x10\x65\x12\t\n\x04side\x10\xc8\x01\x12\t\n\x04wins\x10\xc9\x01\x12\x0e\n\tcharacter\x10\xca\x01\x12\x0b\n\x06health\x10\xcb\x01\x12\x0e\n\tsuper_bar\x10\xcc\x01\x12\x10\n\x0bsuper_count\x10\xcd\x01\x12\x14\n\x0fsuper_max_count\x10\xce\x01\x12\x0f\n\nsuper_type\x10\xcf\x01\x12\r\n\x08stun_bar\x10\xd0\x01\x12\x0c\n\x07stunned\x10\xd1\x01\x12\r\n\x08health_1\x10\xd2\x01\x12\r\n\x08health_2\x10\xd3\x01\x12\x15\n\x10\x61\x63tive_character\x10\xd4\x01\x12\x10\n\x0b\x63haracter_1\x10\xd5\x01\x12\x10\n\x0b\x63haracter_2\x10\xd6\x01\x12\x0f\n\nbar_status\x10\xd7\x01\x12\x12\n\raggressor_bar\x10\xd8\x01\x12\x0f\n\nweapon_bar\x10\xd9\x01\x12\x0e\n\tpower_bar\x10\xda\x01\x12\x11\n\x0cweapon_fight\x10\xdb\x01\x12\x10\n\x0bweapon_lost\x10\xdc\x01\x12\x0c\n\x07rage_on\x10\xdd\x01\x12\r\n\x08rage_bar\x10\xde\x01\x12\x0e\n\trage_used\x10\xdf\x01\x12\x14\n\x0fspecial_attacks\x10\xe0\x01\x12\r\n\x08\x62\x61r_type\x10\xe1\x01\x12\x10\n\x0b\x63haracter_3\x10\xe2\x01\x12\x0c\n\x07partner\x10\xe3\x01\x12\x14\n\x0fpartner_attacks\x10\xe4\x01\x32\xba\x02\n\tEnvServer\x12?\n\x07\x45nvInit\x12\x16.interface.EnvSettings\x1a\x1a.interface.EnvInitResponse\"\x00\x12O\n\x05Reset\x12&.interface.EnvSettings.EpisodeSettings\x1a\x1c.interface.StepResetResponse\"\x00\x12:\n\x04Step\x12\x12.interface.Actions\x1a\x1c.interface.StepResetResponse\"\x00\x12-\n\x05\x43lose\x12\x10.interface.Empty\x1a\x10.interface.Empty\"\x00\x12\x30\n\x08Shutdown\x12\x10.interface.Empty\x1a\x10.interface.Empty\"\x00\x42\x06\xa2\x02\x03HLWb\x06proto3')
 
 _SPACETYPES = DESCRIPTOR.enum_types_by_name['SpaceTypes']
 SpaceTypes = enum_type_wrapper.EnumTypeWrapper(_SPACETYPES)
 _GAMESTATES = DESCRIPTOR.enum_types_by_name['GameStates']
 GameStates = enum_type_wrapper.EnumTypeWrapper(_GAMESTATES)
 _RAMSTATESCATEGORIES = DESCRIPTOR.enum_types_by_name['RamStatesCategories']
 RamStatesCategories = enum_type_wrapper.EnumTypeWrapper(_RAMSTATESCATEGORIES)
@@ -44,14 +44,16 @@
 round_time_elaps = 3
 on_fighting_stage = 4
 round_phase = 5
 test_mode = 6
 character_1_P2_fix = 7
 character_2_P2_fix = 8
 character_3_P2_fix = 9
+continue_time_p1 = 10
+continue_time_p2 = 11
 stage = 100
 timer = 101
 side = 200
 wins = 201
 character = 202
 health = 203
 super_bar = 204
@@ -73,14 +75,16 @@
 weapon_lost = 220
 rage_on = 221
 rage_bar = 222
 rage_used = 223
 special_attacks = 224
 bar_type = 225
 character_3 = 226
+partner = 227
+partner_attacks = 228
 
 
 _EMPTY = DESCRIPTOR.message_types_by_name['Empty']
 _FRAMESHAPE = DESCRIPTOR.message_types_by_name['FrameShape']
 _RAMSTATEINFO = DESCRIPTOR.message_types_by_name['RamStateInfo']
 _ERRORMESSAGE = DESCRIPTOR.message_types_by_name['ErrorMessage']
 _ENVSETTINGS = DESCRIPTOR.message_types_by_name['EnvSettings']
@@ -347,76 +351,76 @@
   _ENVINITRESPONSE_RAMSTATESCATEGORIESENTRY._serialized_options = b'8\001'
   _STEPRESETRESPONSE_OBSERVATION_CATEGORYRAMSTATES_RAMSTATESENTRY._options = None
   _STEPRESETRESPONSE_OBSERVATION_CATEGORYRAMSTATES_RAMSTATESENTRY._serialized_options = b'8\001'
   _STEPRESETRESPONSE_OBSERVATION_RAMSTATESCATEGORIESENTRY._options = None
   _STEPRESETRESPONSE_OBSERVATION_RAMSTATESCATEGORIESENTRY._serialized_options = b'8\001'
   _STEPRESETRESPONSE_INFO_GAMESTATESENTRY._options = None
   _STEPRESETRESPONSE_INFO_GAMESTATESENTRY._serialized_options = b'8\001'
-  _SPACETYPES._serialized_start=3535
-  _SPACETYPES._serialized_end=3602
-  _GAMESTATES._serialized_start=3604
-  _GAMESTATES._serialized_end=3695
-  _RAMSTATESCATEGORIES._serialized_start=3697
-  _RAMSTATESCATEGORIES._serialized_end=3760
-  _RAMSTATES._serialized_start=3763
-  _RAMSTATES._serialized_end=4440
+  _SPACETYPES._serialized_start=3577
+  _SPACETYPES._serialized_end=3644
+  _GAMESTATES._serialized_start=3646
+  _GAMESTATES._serialized_end=3737
+  _RAMSTATESCATEGORIES._serialized_start=3739
+  _RAMSTATESCATEGORIES._serialized_end=3802
+  _RAMSTATES._serialized_start=3805
+  _RAMSTATES._serialized_end=4562
   _EMPTY._serialized_start=45
   _EMPTY._serialized_end=52
   _FRAMESHAPE._serialized_start=54
   _FRAMESHAPE._serialized_end=99
   _RAMSTATEINFO._serialized_start=101
   _RAMSTATEINFO._serialized_end=155
   _ERRORMESSAGE._serialized_start=157
   _ERRORMESSAGE._serialized_end=194
   _ENVSETTINGS._serialized_start=197
-  _ENVSETTINGS._serialized_end=1379
+  _ENVSETTINGS._serialized_end=1399
   _ENVSETTINGS_SYSSETTINGS._serialized_start=549
   _ENVSETTINGS_SYSSETTINGS._serialized_end=883
   _ENVSETTINGS_SYSSETTINGS_BUTTONSCFGENTRY._serialized_start=834
   _ENVSETTINGS_SYSSETTINGS_BUTTONSCFGENTRY._serialized_end=883
   _ENVSETTINGS_EPISODESETTINGS._serialized_start=886
-  _ENVSETTINGS_EPISODESETTINGS._serialized_end=1379
+  _ENVSETTINGS_EPISODESETTINGS._serialized_end=1399
   _ENVSETTINGS_EPISODESETTINGS_PLAYERSETTINGS._serialized_start=1085
-  _ENVSETTINGS_EPISODESETTINGS_PLAYERSETTINGS._serialized_end=1379
-  _ENVSETTINGS_EPISODESETTINGS_PLAYERSETTINGS_ULTIMATESTYLE._serialized_start=1322
-  _ENVSETTINGS_EPISODESETTINGS_PLAYERSETTINGS_ULTIMATESTYLE._serialized_end=1379
-  _ENVINITRESPONSE._serialized_start=1382
-  _ENVINITRESPONSE._serialized_end=2740
-  _ENVINITRESPONSE_AVAILABLEACTIONS._serialized_start=1827
-  _ENVINITRESPONSE_AVAILABLEACTIONS._serialized_end=2082
-  _ENVINITRESPONSE_AVAILABLEACTIONS_BUTTON._serialized_start=2046
-  _ENVINITRESPONSE_AVAILABLEACTIONS_BUTTON._serialized_end=2082
-  _ENVINITRESPONSE_CUMULATIVEREWARDBOUNDS._serialized_start=2084
-  _ENVINITRESPONSE_CUMULATIVEREWARDBOUNDS._serialized_end=2134
-  _ENVINITRESPONSE_DIFFICULTYBOUNDS._serialized_start=2136
-  _ENVINITRESPONSE_DIFFICULTYBOUNDS._serialized_end=2180
-  _ENVINITRESPONSE_CHARACTERSINFO._serialized_start=2183
-  _ENVINITRESPONSE_CHARACTERSINFO._serialized_end=2444
-  _ENVINITRESPONSE_CHARACTERSINFO_CHARHOMONYMYMAPENTRY._serialized_start=2390
-  _ENVINITRESPONSE_CHARACTERSINFO_CHARHOMONYMYMAPENTRY._serialized_end=2444
-  _ENVINITRESPONSE_CATEGORYRAMSTATESINFO._serialized_start=2447
-  _ENVINITRESPONSE_CATEGORYRAMSTATESINFO._serialized_end=2630
-  _ENVINITRESPONSE_CATEGORYRAMSTATESINFO_RAMSTATESENTRY._serialized_start=2557
-  _ENVINITRESPONSE_CATEGORYRAMSTATESINFO_RAMSTATESENTRY._serialized_end=2630
-  _ENVINITRESPONSE_RAMSTATESCATEGORIESENTRY._serialized_start=2632
-  _ENVINITRESPONSE_RAMSTATESCATEGORIESENTRY._serialized_end=2740
-  _ACTIONS._serialized_start=2742
-  _ACTIONS._serialized_end=2835
-  _ACTIONS_ACTION._serialized_start=2797
-  _ACTIONS_ACTION._serialized_end=2835
-  _STEPRESETRESPONSE._serialized_start=2838
-  _STEPRESETRESPONSE._serialized_end=3533
-  _STEPRESETRESPONSE_OBSERVATION._serialized_start=2988
-  _STEPRESETRESPONSE_OBSERVATION._serialized_end=3401
-  _STEPRESETRESPONSE_OBSERVATION_CATEGORYRAMSTATES._serialized_start=3117
-  _STEPRESETRESPONSE_OBSERVATION_CATEGORYRAMSTATES._serialized_end=3281
-  _STEPRESETRESPONSE_OBSERVATION_CATEGORYRAMSTATES_RAMSTATESENTRY._serialized_start=3233
-  _STEPRESETRESPONSE_OBSERVATION_CATEGORYRAMSTATES_RAMSTATESENTRY._serialized_end=3281
-  _STEPRESETRESPONSE_OBSERVATION_RAMSTATESCATEGORIESENTRY._serialized_start=3283
-  _STEPRESETRESPONSE_OBSERVATION_RAMSTATESCATEGORIESENTRY._serialized_end=3401
-  _STEPRESETRESPONSE_INFO._serialized_start=3404
-  _STEPRESETRESPONSE_INFO._serialized_end=3533
-  _STEPRESETRESPONSE_INFO_GAMESTATESENTRY._serialized_start=3484
-  _STEPRESETRESPONSE_INFO_GAMESTATESENTRY._serialized_end=3533
-  _ENVSERVER._serialized_start=4443
-  _ENVSERVER._serialized_end=4814
+  _ENVSETTINGS_EPISODESETTINGS_PLAYERSETTINGS._serialized_end=1399
+  _ENVSETTINGS_EPISODESETTINGS_PLAYERSETTINGS_ULTIMATESTYLE._serialized_start=1342
+  _ENVSETTINGS_EPISODESETTINGS_PLAYERSETTINGS_ULTIMATESTYLE._serialized_end=1399
+  _ENVINITRESPONSE._serialized_start=1402
+  _ENVINITRESPONSE._serialized_end=2782
+  _ENVINITRESPONSE_AVAILABLEACTIONS._serialized_start=1847
+  _ENVINITRESPONSE_AVAILABLEACTIONS._serialized_end=2102
+  _ENVINITRESPONSE_AVAILABLEACTIONS_BUTTON._serialized_start=2066
+  _ENVINITRESPONSE_AVAILABLEACTIONS_BUTTON._serialized_end=2102
+  _ENVINITRESPONSE_CUMULATIVEREWARDBOUNDS._serialized_start=2104
+  _ENVINITRESPONSE_CUMULATIVEREWARDBOUNDS._serialized_end=2154
+  _ENVINITRESPONSE_DIFFICULTYBOUNDS._serialized_start=2156
+  _ENVINITRESPONSE_DIFFICULTYBOUNDS._serialized_end=2200
+  _ENVINITRESPONSE_CHARACTERSINFO._serialized_start=2203
+  _ENVINITRESPONSE_CHARACTERSINFO._serialized_end=2486
+  _ENVINITRESPONSE_CHARACTERSINFO_CHARHOMONYMYMAPENTRY._serialized_start=2432
+  _ENVINITRESPONSE_CHARACTERSINFO_CHARHOMONYMYMAPENTRY._serialized_end=2486
+  _ENVINITRESPONSE_CATEGORYRAMSTATESINFO._serialized_start=2489
+  _ENVINITRESPONSE_CATEGORYRAMSTATESINFO._serialized_end=2672
+  _ENVINITRESPONSE_CATEGORYRAMSTATESINFO_RAMSTATESENTRY._serialized_start=2599
+  _ENVINITRESPONSE_CATEGORYRAMSTATESINFO_RAMSTATESENTRY._serialized_end=2672
+  _ENVINITRESPONSE_RAMSTATESCATEGORIESENTRY._serialized_start=2674
+  _ENVINITRESPONSE_RAMSTATESCATEGORIESENTRY._serialized_end=2782
+  _ACTIONS._serialized_start=2784
+  _ACTIONS._serialized_end=2877
+  _ACTIONS_ACTION._serialized_start=2839
+  _ACTIONS_ACTION._serialized_end=2877
+  _STEPRESETRESPONSE._serialized_start=2880
+  _STEPRESETRESPONSE._serialized_end=3575
+  _STEPRESETRESPONSE_OBSERVATION._serialized_start=3030
+  _STEPRESETRESPONSE_OBSERVATION._serialized_end=3443
+  _STEPRESETRESPONSE_OBSERVATION_CATEGORYRAMSTATES._serialized_start=3159
+  _STEPRESETRESPONSE_OBSERVATION_CATEGORYRAMSTATES._serialized_end=3323
+  _STEPRESETRESPONSE_OBSERVATION_CATEGORYRAMSTATES_RAMSTATESENTRY._serialized_start=3275
+  _STEPRESETRESPONSE_OBSERVATION_CATEGORYRAMSTATES_RAMSTATESENTRY._serialized_end=3323
+  _STEPRESETRESPONSE_OBSERVATION_RAMSTATESCATEGORIESENTRY._serialized_start=3325
+  _STEPRESETRESPONSE_OBSERVATION_RAMSTATESCATEGORIESENTRY._serialized_end=3443
+  _STEPRESETRESPONSE_INFO._serialized_start=3446
+  _STEPRESETRESPONSE_INFO._serialized_end=3575
+  _STEPRESETRESPONSE_INFO_GAMESTATESENTRY._serialized_start=3526
+  _STEPRESETRESPONSE_INFO_GAMESTATESENTRY._serialized_end=3575
+  _ENVSERVER._serialized_start=4565
+  _ENVSERVER._serialized_end=4879
 # @@protoc_insertion_point(module_scope)
```

### Comparing `diambra-engine-2.2.2/diambra/engine/interface_pb2_grpc.py` & `diambra-engine-2.2.3/diambra/engine/interface_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,19 +11,14 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.GetError = channel.unary_unary(
-                '/interface.EnvServer/GetError',
-                request_serializer=diambra_dot_engine_dot_interface__pb2.Empty.SerializeToString,
-                response_deserializer=diambra_dot_engine_dot_interface__pb2.ErrorMessage.FromString,
-                )
         self.EnvInit = channel.unary_unary(
                 '/interface.EnvServer/EnvInit',
                 request_serializer=diambra_dot_engine_dot_interface__pb2.EnvSettings.SerializeToString,
                 response_deserializer=diambra_dot_engine_dot_interface__pb2.EnvInitResponse.FromString,
                 )
         self.Reset = channel.unary_unary(
                 '/interface.EnvServer/Reset',
@@ -47,21 +42,14 @@
                 )
 
 
 class EnvServerServicer(object):
     """The DIAMBRA service definition.
     """
 
-    def GetError(self, request, context):
-        """Receives back environment error message
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def EnvInit(self, request, context):
         """Sends environment settings, receives back environment info and int data vars
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -92,19 +80,14 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_EnvServerServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'GetError': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetError,
-                    request_deserializer=diambra_dot_engine_dot_interface__pb2.Empty.FromString,
-                    response_serializer=diambra_dot_engine_dot_interface__pb2.ErrorMessage.SerializeToString,
-            ),
             'EnvInit': grpc.unary_unary_rpc_method_handler(
                     servicer.EnvInit,
                     request_deserializer=diambra_dot_engine_dot_interface__pb2.EnvSettings.FromString,
                     response_serializer=diambra_dot_engine_dot_interface__pb2.EnvInitResponse.SerializeToString,
             ),
             'Reset': grpc.unary_unary_rpc_method_handler(
                     servicer.Reset,
@@ -134,31 +117,14 @@
 
  # This class is part of an EXPERIMENTAL API.
 class EnvServer(object):
     """The DIAMBRA service definition.
     """
 
     @staticmethod
-    def GetError(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/interface.EnvServer/GetError',
-            diambra_dot_engine_dot_interface__pb2.Empty.SerializeToString,
-            diambra_dot_engine_dot_interface__pb2.ErrorMessage.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def EnvInit(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `diambra-engine-2.2.2/diambra_engine.egg-info/PKG-INFO` & `diambra-engine-2.2.3/diambra_engine.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-engine
-Version: 2.2.2
+Version: 2.2.3
 Summary: DIAMBRA™ Arena Engine API Client
 Home-page: https://diambra.ai
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

### Comparing `diambra-engine-2.2.2/setup.py` & `diambra-engine-2.2.3/setup.py`

 * *Files identical despite different names*

