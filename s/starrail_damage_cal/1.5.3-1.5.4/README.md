# Comparing `tmp/starrail_damage_cal-1.5.3.tar.gz` & `tmp/starrail_damage_cal-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail_damage_cal-1.5.3.tar", last modified: Sat Mar 30 03:15:39 2024, max compression
+gzip compressed data, was "starrail_damage_cal-1.5.4.tar", last modified: Sat Apr 27 09:12:29 2024, max compression
```

## Comparing `starrail_damage_cal-1.5.3.tar` & `starrail_damage_cal-1.5.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1064 2024-03-30 03:15:22.599700 starrail_damage_cal-1.5.3/LICENSE
--rw-r--r--   0        0        0       20 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/README.md
--rw-r--r--   0        0        0     1246 2024-03-30 03:15:39.663837 starrail_damage_cal-1.5.3/pyproject.toml
--rw-r--r--   0        0        0       48 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/__init__.py
--rw-r--r--   0        0        0     4037 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/cal_damage.py
--rw-r--r--   0        0        0     4232 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Avatar.py
--rw-r--r--   0        0        0   159683 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/AvatarDamage/AvatarDamage.py
--rw-r--r--   0        0        0        0 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/AvatarDamage/__init__.py
--rw-r--r--   0        0        0     5587 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Base/AvatarBase.py
--rw-r--r--   0        0        0     3175 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Base/RelicBase.py
--rw-r--r--   0        0        0     1171 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Base/SkillBase.py
--rw-r--r--   0        0        0     2503 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Base/WeaponBase.py
--rw-r--r--   0        0        0        0 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Base/__init__.py
--rw-r--r--   0        0        0     2611 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Base/model.py
--rw-r--r--   0        0        0    68035 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Excel/SkillData.json
--rw-r--r--   0        0        0    20149 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Excel/weapon_effect.json
--rw-r--r--   0        0        0    35041 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Relic/Relic.py
--rw-r--r--   0        0        0        0 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Relic/__init__.py
--rw-r--r--   0        0        0    14397 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Role.py
--rw-r--r--   0        0        0    96037 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Weapon/Weapon.py
--rw-r--r--   0        0        0        0 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Weapon/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/__init__.py
--rw-r--r--   0        0        0     2738 2024-03-30 03:15:22.603700 starrail_damage_cal-1.5.3/starrail_damage_cal/damage/utils.py
--rw-r--r--   0        0        0   341001 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/excel/AvatarPromotionConfig.json
--rw-r--r--   0        0        0   485707 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/excel/EquipmentPromotionConfig.json
--rw-r--r--   0        0        0    30312 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/excel/RelicMainAffixConfig.json
--rw-r--r--   0        0        0    12017 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/excel/RelicSubAffixConfig.json
--rw-r--r--   0        0        0        0 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/excel/__init__.py
--rw-r--r--   0        0        0    95747 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/excel/light_cone_ranks.json
--rw-r--r--   0        0        0     9282 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/excel/model.py
--rw-r--r--   0        0        0      624 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/excel/read_excel.py
--rw-r--r--   0        0        0     1240 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/exception.py
--rw-r--r--   0        0        0       64 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/logger.py
--rw-r--r--   0        0        0     4645 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/SR_MAP_PATH.py
--rw-r--r--   0        0        0        0 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/__init__.py
--rw-r--r--   0        0        0    25390 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/AvatarRelicScore.json
--rw-r--r--   0        0        0    47199 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/EquipmentID2AbilityProperty_mapping_2.1.0.json
--rw-r--r--   0        0        0     3220 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/EquipmentID2EnName_mapping_2.1.0.json
--rw-r--r--   0        0        0     3004 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/EquipmentID2Name_mapping_2.1.0.json
--rw-r--r--   0        0        0     1503 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/EquipmentID2Rarity_mapping_2.1.0.json
--rw-r--r--   0        0        0    16428 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/ItemId2Name_mapping_2.1.0.json
--rw-r--r--   0        0        0     2423 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/Property2Name.json
--rw-r--r--   0        0        0     2423 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/Property2Name_mapping_2.1.0.json
--rw-r--r--   0        0        0     7314 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/RelicId2MainAffixGroup_mapping_2.1.0.json
--rw-r--r--   0        0        0     6896 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/RelicId2Rarity_mapping_2.1.0.json
--rw-r--r--   0        0        0     7714 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/RelicId2SetId_mapping_2.1.0.json
--rw-r--r--   0        0        0     4223 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/RelicSetSkill_mapping_2.1.0.json
--rw-r--r--   0        0        0     1184 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/SetId2Name_mapping_2.1.0.json
--rw-r--r--   0        0        0     1143 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/avatarId2DamageType_mapping_2.1.0.json
--rw-r--r--   0        0        0     1196 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/avatarId2EnName_mapping_2.1.0.json
--rw-r--r--   0        0        0     1222 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/avatarId2Name_mapping_2.1.0.json
--rw-r--r--   0        0        0      867 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/avatarId2Rarity_mapping_2.1.0.json
--rw-r--r--   0        0        0      867 2024-03-30 03:15:22.607700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/avatarId2Star_mapping_2.1.0.json
--rw-r--r--   0        0        0    23778 2024-03-30 03:15:22.611700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/avatarRankSkillUp_mapping_2.1.0.json
--rw-r--r--   0        0        0     9285 2024-03-30 03:15:22.611700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/char_alias.json
--rw-r--r--   0        0        0  1445499 2024-03-30 03:15:22.611700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/characterSkillTree_mapping_2.1.0.json
--rw-r--r--   0        0        0    10716 2024-03-30 03:15:22.611700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/rankId2Name_mapping_2.1.0.json
--rw-r--r--   0        0        0     7739 2024-03-30 03:15:22.611700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/skillId2AttackType_mapping_2.1.0.json
--rw-r--r--   0        0        0    10748 2024-03-30 03:15:22.611700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/skillId2Name_mapping_2.1.0.json
--rw-r--r--   0        0        0     7535 2024-03-30 03:15:22.615700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/skillId2Type_mapping_2.1.0.json
--rw-r--r--   0        0        0      701 2024-03-30 03:15:22.615700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/model/RelicSetSkill.py
--rw-r--r--   0        0        0        0 2024-03-30 03:15:22.615700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/model/__init__.py
--rw-r--r--   0        0        0      491 2024-03-30 03:15:22.615700 starrail_damage_cal-1.5.3/starrail_damage_cal/map/name_covert.py
--rw-r--r--   0        0        0      201 2024-03-30 03:15:22.615700 starrail_damage_cal-1.5.3/starrail_damage_cal/mihomo/__init__.py
--rw-r--r--   0        0        0     2120 2024-03-30 03:15:22.615700 starrail_damage_cal-1.5.3/starrail_damage_cal/mihomo/models.py
--rw-r--r--   0        0        0     1335 2024-03-30 03:15:22.615700 starrail_damage_cal-1.5.3/starrail_damage_cal/mihomo/requests.py
--rw-r--r--   0        0        0     4426 2024-03-30 03:15:22.615700 starrail_damage_cal-1.5.3/starrail_damage_cal/mono/Character.py
--rw-r--r--   0        0        0        0 2024-03-30 03:15:22.615700 starrail_damage_cal-1.5.3/starrail_damage_cal/mono/__init__.py
--rw-r--r--   0        0        0    11688 2024-03-30 03:15:22.615700 starrail_damage_cal-1.5.3/starrail_damage_cal/to_data.py
--rw-r--r--   0        0        0       28 2024-03-30 03:15:22.615700 starrail_damage_cal-1.5.3/starrail_damage_cal/version.py
--rw-r--r--   0        0        0        0 2024-03-30 03:15:22.615700 starrail_damage_cal-1.5.3/test/__init__.py
--rw-r--r--   0        0        0    12611 2024-03-30 03:15:22.615700 starrail_damage_cal-1.5.3/test/test.json
--rw-r--r--   0        0        0     1228 2024-03-30 03:15:22.615700 starrail_damage_cal-1.5.3/test/test_get_char.py
--rw-r--r--   0        0        0      325 1970-01-01 00:00:00.000000 starrail_damage_cal-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-27 09:12:11.351889 starrail_damage_cal-1.5.4/LICENSE
+-rw-r--r--   0        0        0       20 2024-04-27 09:12:11.351889 starrail_damage_cal-1.5.4/README.md
+-rw-r--r--   0        0        0     1246 2024-04-27 09:12:29.644013 starrail_damage_cal-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-04-27 09:12:11.351889 starrail_damage_cal-1.5.4/starrail_damage_cal/__init__.py
+-rw-r--r--   0        0        0     4037 2024-04-27 09:12:11.351889 starrail_damage_cal-1.5.4/starrail_damage_cal/cal_damage.py
+-rw-r--r--   0        0        0     4232 2024-04-27 09:12:11.351889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Avatar.py
+-rw-r--r--   0        0        0   159414 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/AvatarDamage/AvatarDamage.py
+-rw-r--r--   0        0        0        0 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/AvatarDamage/__init__.py
+-rw-r--r--   0        0        0     5563 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Base/AvatarBase.py
+-rw-r--r--   0        0        0     3199 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Base/RelicBase.py
+-rw-r--r--   0        0        0     1171 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Base/SkillBase.py
+-rw-r--r--   0        0        0     2567 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Base/WeaponBase.py
+-rw-r--r--   0        0        0        0 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Base/__init__.py
+-rw-r--r--   0        0        0     2611 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Base/model.py
+-rw-r--r--   0        0        0    68035 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Excel/SkillData.json
+-rw-r--r--   0        0        0    20149 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Excel/weapon_effect.json
+-rw-r--r--   0        0        0    35194 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Relic/Relic.py
+-rw-r--r--   0        0        0        0 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Relic/__init__.py
+-rw-r--r--   0        0        0    14474 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Role.py
+-rw-r--r--   0        0        0    96034 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Weapon/Weapon.py
+-rw-r--r--   0        0        0        0 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Weapon/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/__init__.py
+-rw-r--r--   0        0        0     2738 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/damage/utils.py
+-rw-r--r--   0        0        0   341001 2024-04-27 09:12:11.355889 starrail_damage_cal-1.5.4/starrail_damage_cal/excel/AvatarPromotionConfig.json
+-rw-r--r--   0        0        0   485707 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/excel/EquipmentPromotionConfig.json
+-rw-r--r--   0        0        0    30312 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/excel/RelicMainAffixConfig.json
+-rw-r--r--   0        0        0    12017 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/excel/RelicSubAffixConfig.json
+-rw-r--r--   0        0        0        0 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/excel/__init__.py
+-rw-r--r--   0        0        0    95747 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/excel/light_cone_ranks.json
+-rw-r--r--   0        0        0     9282 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/excel/model.py
+-rw-r--r--   0        0        0      624 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/excel/read_excel.py
+-rw-r--r--   0        0        0     1241 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/exception.py
+-rw-r--r--   0        0        0       64 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/logger.py
+-rw-r--r--   0        0        0     4645 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/SR_MAP_PATH.py
+-rw-r--r--   0        0        0        0 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/__init__.py
+-rw-r--r--   0        0        0    25390 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/AvatarRelicScore.json
+-rw-r--r--   0        0        0    47199 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/EquipmentID2AbilityProperty_mapping_2.1.0.json
+-rw-r--r--   0        0        0     3220 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/EquipmentID2EnName_mapping_2.1.0.json
+-rw-r--r--   0        0        0     3004 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/EquipmentID2Name_mapping_2.1.0.json
+-rw-r--r--   0        0        0     1503 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/EquipmentID2Rarity_mapping_2.1.0.json
+-rw-r--r--   0        0        0    16428 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/ItemId2Name_mapping_2.1.0.json
+-rw-r--r--   0        0        0     2423 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/Property2Name.json
+-rw-r--r--   0        0        0     2423 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/Property2Name_mapping_2.1.0.json
+-rw-r--r--   0        0        0     7314 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/RelicId2MainAffixGroup_mapping_2.1.0.json
+-rw-r--r--   0        0        0     6896 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/RelicId2Rarity_mapping_2.1.0.json
+-rw-r--r--   0        0        0     7714 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/RelicId2SetId_mapping_2.1.0.json
+-rw-r--r--   0        0        0     4223 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/RelicSetSkill_mapping_2.1.0.json
+-rw-r--r--   0        0        0     1184 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/SetId2Name_mapping_2.1.0.json
+-rw-r--r--   0        0        0     1143 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/avatarId2DamageType_mapping_2.1.0.json
+-rw-r--r--   0        0        0     1196 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/avatarId2EnName_mapping_2.1.0.json
+-rw-r--r--   0        0        0     1222 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/avatarId2Name_mapping_2.1.0.json
+-rw-r--r--   0        0        0      867 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/avatarId2Rarity_mapping_2.1.0.json
+-rw-r--r--   0        0        0      867 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/avatarId2Star_mapping_2.1.0.json
+-rw-r--r--   0        0        0    23778 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/avatarRankSkillUp_mapping_2.1.0.json
+-rw-r--r--   0        0        0     9285 2024-04-27 09:12:11.359889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/char_alias.json
+-rw-r--r--   0        0        0  1445499 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/characterSkillTree_mapping_2.1.0.json
+-rw-r--r--   0        0        0    10716 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/rankId2Name_mapping_2.1.0.json
+-rw-r--r--   0        0        0     7739 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/skillId2AttackType_mapping_2.1.0.json
+-rw-r--r--   0        0        0    10748 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/skillId2Name_mapping_2.1.0.json
+-rw-r--r--   0        0        0     7535 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/skillId2Type_mapping_2.1.0.json
+-rw-r--r--   0        0        0      701 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/model/RelicSetSkill.py
+-rw-r--r--   0        0        0        0 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/model/__init__.py
+-rw-r--r--   0        0        0      491 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/starrail_damage_cal/map/name_covert.py
+-rw-r--r--   0        0        0      202 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/starrail_damage_cal/mihomo/__init__.py
+-rw-r--r--   0        0        0     2120 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/starrail_damage_cal/mihomo/models.py
+-rw-r--r--   0        0        0     1335 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/starrail_damage_cal/mihomo/requests.py
+-rw-r--r--   0        0        0     4472 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/starrail_damage_cal/mono/Character.py
+-rw-r--r--   0        0        0        0 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/starrail_damage_cal/mono/__init__.py
+-rw-r--r--   0        0        0    11700 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/starrail_damage_cal/to_data.py
+-rw-r--r--   0        0        0       28 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/starrail_damage_cal/version.py
+-rw-r--r--   0        0        0        0 2024-04-27 09:12:11.363889 starrail_damage_cal-1.5.4/test/__init__.py
+-rw-r--r--   0        0        0    12611 2024-04-27 09:12:11.367889 starrail_damage_cal-1.5.4/test/test.json
+-rw-r--r--   0        0        0     1228 2024-04-27 09:12:11.367889 starrail_damage_cal-1.5.4/test/test_get_char.py
+-rw-r--r--   0        0        0      325 1970-01-01 00:00:00.000000 starrail_damage_cal-1.5.4/PKG-INFO
```

### Comparing `starrail_damage_cal-1.5.3/LICENSE` & `starrail_damage_cal-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/pyproject.toml` & `starrail_damage_cal-1.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "starrail_damage_cal"
-version = "1.5.3"
+version = "1.5.4"
 description = "For StarRail Role Damage Cal"
 authors = [
     { name = "qwerdvd", email = "105906879+qwerdvd@users.noreply.github.com" },
 ]
 dependencies = [
-    "msgspec>=0.18.4",
-    "httpx>=0.25.0",
+    "msgspec>=0.18.6",
+    "httpx>=0.27.0",
 ]
 repository = "https://github.com/baiqwerdvd/StarRailDamageCal"
 requires-python = ">=3.8"
 readme = "README.md"
 packages = [
     { include = "starrail_damage_cal" },
 ]
```

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/cal_damage.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/cal_damage.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Avatar.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Avatar.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/damage/AvatarDamage/AvatarDamage.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/damage/AvatarDamage/AvatarDamage.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,14 @@
 
         # 希尔天赋再现加伤害
         attribute_bonus["AllDamageAddedRatio"] = self.Skill_num(
             "Talent",
             "Talent",
         ) + attribute_bonus.get("AllDamageAddedRatio", 0)
 
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -149,16 +147,14 @@
         self.extra_ability_attribute["CriticalChanceBase"] = 0.1
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -236,16 +232,14 @@
         self.extra_ability_attribute["AllDamageAddedRatio"] = 0.20
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -577,16 +571,14 @@
                 "CriticalDamageBase",
                 0,
             )
             attribute_bonus["CriticalChanceBase"] = (
                 talent_cc_add * 2 + attribute_bonus.get("CriticalChanceBase", 0)
             )
 
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -677,16 +669,14 @@
         self.extra_ability_attribute["TalentDmgAdd"] = 0.3
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -803,31 +793,29 @@
             self.extra_ability_attribute["AllDamageAddedRatio"] = 1
 
     def extra_ability(self):
         logger.info("额外能力")
         logger.info("战技降抗")
         logger.info("战技使目标全属性抗性降低的效果额外降低3%")
         enemy_status_resistance = self.Skill_num("BPSkill", "BPSkill_D") + 0.03
-        self.extra_ability_attribute[
-            "QuantumResistancePenetration"
-        ] = enemy_status_resistance
+        self.extra_ability_attribute["QuantumResistancePenetration"] = (
+            enemy_status_resistance
+        )
         logger.info("终结技降防")
         ultra_defence = self.Skill_num("Ultra", "Ultra_D")
         logger.info("天赋降防")
         talent_defence = self.Skill_num("Talent", "Talent")
         ignore_defence = ultra_defence + talent_defence
         self.extra_ability_attribute["ignore_defence"] = ignore_defence
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -892,16 +880,14 @@
         pass
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -999,16 +985,14 @@
         )
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -1146,16 +1130,14 @@
         )
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal_HP")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -1228,16 +1210,14 @@
         self.extra_ability_attribute["CriticalChanceBase"] = critical_chance_base + 0.6
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -1321,16 +1301,14 @@
         self.extra_ability_attribute["CriticalChanceBase"] = 0.15
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -1414,16 +1392,14 @@
         )
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -1492,28 +1468,26 @@
         logger.info("额外能力")
         logger.info("【转魄】状态下, 终结技造成的伤害提高20%。")
         logger.info("【转魄】状态下, 暴击率提高。")
         logger.info("【转魄】状态下, 攻击力提高。")
         self.extra_ability_attribute["UltraDmgAdd"] = 0.2
         critical_chance_base = self.Skill_num("Talent", "Talent_CC")
         self.extra_ability_attribute["Ultra_CriticalChanceBase"] = critical_chance_base
-        self.extra_ability_attribute[
-            "BPSkill1_CriticalChanceBase"
-        ] = critical_chance_base
+        self.extra_ability_attribute["BPSkill1_CriticalChanceBase"] = (
+            critical_chance_base
+        )
         attack_added_ratio = self.Skill_num("Talent", "Talent_atk")
         self.extra_ability_attribute["BPSkill1AttackAddedRatio"] = attack_added_ratio
         self.extra_ability_attribute["UltraAttackAddedRatio"] = attack_added_ratio
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -1605,16 +1579,14 @@
         )
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -1685,16 +1657,14 @@
             )
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -1769,16 +1739,14 @@
         pass
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -1839,16 +1807,14 @@
         pass
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -1968,16 +1934,14 @@
         self.extra_ability_attribute["HPAddedRatio"] = 0.10
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -2064,16 +2028,14 @@
         pass
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         # 计算战技生命上限
         skill_multiplier = self.Skill_num("BPSkill", "BPSkill_HP")
         skill_num = self.Skill_num("BPSkill", "BPSkill_HP_G")
         if self.avatar_rank >= 6:
             skill_multiplier += 0.06
         hp = (
             base_attr["hp"] * (1 + attribute_bonus["HPAddedRatio"])
@@ -2184,16 +2146,14 @@
         )
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -2277,16 +2237,14 @@
         pass
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -2379,16 +2337,14 @@
         self.extra_ability_attribute["DefenceAddedRatio"] = 0.2
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         # 终结技增加伤害
         attribute_bonus["AttackAddedRatio"] = attribute_bonus.get(
             "AttackAddedRatio",
             0,
         ) + self.Skill_num("Ultra", "Ultra_A")
         add_critical_damage_base = (
             attribute_bonus.get("CriticalDamageBase", 0)
@@ -2444,16 +2400,14 @@
         self.extra_ability_attribute["ImaginaryAddedRatio"] = 0.15
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         # 终结技增加伤害
         attribute_bonus["AttackAddedRatio"] = attribute_bonus.get(
             "AttackAddedRatio",
             0,
         ) + self.Skill_num("BPSkill", "BPSkill")
         attribute_bonus["CriticalChanceBase"] = attribute_bonus.get(
             "CriticalChanceBase",
@@ -2531,16 +2485,14 @@
         self.extra_ability_attribute["jianshiDmgAdd"] = 0.2
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -2640,16 +2592,14 @@
     ):
         # 计算终结技提供的易伤加成
         attribute_bonus["DmgRatio"] = attribute_bonus.get(
             "DmgRatio",
             0,
         ) + self.Skill_num("Ultra", "Ultra_d")
 
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -2759,16 +2709,14 @@
     ):
         # 计算穿透加成
         attribute_bonus["WindResistancePenetration"] = attribute_bonus.get(
             "WindResistancePenetration",
             0,
         ) + self.Skill_num("Talent", "Talent")
 
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -2840,16 +2788,14 @@
     ):
         # 计算天赋伤害加成
         attribute_bonus["AllDamageAddedRatio"] = attribute_bonus.get(
             "AllDamageAddedRatio",
             0,
         ) + self.Skill_num("Talent", "Talent")
 
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -2919,16 +2865,14 @@
             + self.Skill_num("Talent", "Talent") * 5
         )
         attribute_bonus["SpeedDelta"] = attribute_bonus.get(
             "SpeedDelta",
             0,
         ) + self.Skill_num("Ultra", "Ultra")
 
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -2987,16 +2931,14 @@
         self.extra_ability_attribute["UltraDmgAdd"] = 0.2
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         if self.avatar_rank >= 1:
             skill_multiplier += 0.4
         damagelist1 = await calculate_damage(
             base_attr,
@@ -3073,16 +3015,14 @@
         self.extra_ability_attribute["AttackAddedRatio"] = 0.2
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -3178,16 +3118,14 @@
     ):
         # 计算终结技降防
         attribute_bonus["ignore_defence"] = attribute_bonus.get(
             "ignore_defence",
             0,
         ) + self.Skill_num("Ultra", "Ultra_d")
 
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -3266,16 +3204,14 @@
     ):
         # 计算终结技持续伤害加成
         attribute_bonus["DOTDmgAdd"] = attribute_bonus.get(
             "DOTDmgAdd",
             0,
         ) + self.Skill_num("Ultra", "Ultra_d")
 
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -3356,16 +3292,14 @@
         pass
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -3466,16 +3400,14 @@
         self.eidolon_attribute["NormalDmgAdd"] = 0.4
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -3528,16 +3460,14 @@
     ):
         # 计算天赋攻击加成
         attribute_bonus["AttackAddedRatio"] = (
             attribute_bonus.get("AttackAddedRatio", 0)
             + self.Skill_num("Talent", "Talent") * 2
         )
 
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -3611,16 +3541,14 @@
         self.extra_ability_attribute["AttackAddedRatio"] = 0.15
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -3740,16 +3668,14 @@
         pass
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -3857,16 +3783,14 @@
             attribute_bonus["DmgRatio"] = attribute_bonus.get("DmgRatio", 0) + 0.1
 
         attribute_bonus["AttackAddedRatio"] = attribute_bonus.get(
             "AttackAddedRatio",
             0,
         ) + self.Skill_num("Ultra", "Ultra_A")
 
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -3930,16 +3854,14 @@
         self.extra_ability_attribute["CriticalDamageBase"] = 0.3
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -4054,16 +3976,14 @@
             add_all_damage_added_ratio = ((Break_Damage_Added_Ratio - 1.2) / 0.1) * 0.06
             add_all_damage_added_ratio = min(0.36, add_all_damage_added_ratio)
             attribute_bonus["AllDamageAddedRatio"] = (
                 attribute_bonus.get("AllDamageAddedRatio", 0)
                 + add_all_damage_added_ratio
             )
 
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -4136,16 +4056,14 @@
     ):
         # 使自身造成的伤害提高, 提高数值等同于击破特攻的100%, 最多使造成的伤害提高240%。
         Break_Damage_Added_Ratio = attribute_bonus.get("BreakDamageAddedRatioBase", 0)
         attribute_bonus["AllDamageAddedRatio"] = attribute_bonus.get(
             "AllDamageAddedRatio", 0
         ) + min(2.4, Break_Damage_Added_Ratio)
 
-        
-
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
@@ -4196,14 +4114,15 @@
         damagelist4[0] += damagelist4[0] * 3
         damagelist4[1] += damagelist4[1] * 3
         damagelist4[2] += damagelist4[2] * 3
         skill_info_list.append({"name": "天赋追加攻击", "damagelist": damagelist4})
 
         return skill_info_list
 
+
 class BlackSwan(BaseAvatar):
     Buff: BaseAvatarBuff
 
     def __init__(self, char: DamageInstanceAvatar, skills: List[DamageInstanceSkill]):
         super().__init__(char=char, skills=skills)
         self.eidolon_attribute: Dict[str, float] = {}
         self.extra_ability_attribute: Dict[str, float] = {}
@@ -4217,32 +4136,32 @@
         if self.avatar_rank >= 1:
             self.eidolon_attribute["WindResistancePenetration"] = 0.25
             self.eidolon_attribute["PhysicalResistancePenetration"] = 0.25
             self.eidolon_attribute["FireResistancePenetration"] = 0.25
             self.eidolon_attribute["ThunderResistancePenetration"] = 0.25
 
     def extra_ability(self):
-        #战技降防计算
+        # 战技降防计算
         bpskill_defence = self.Skill_num("BPSkill", "BPSkill_D")
         self.extra_ability_attribute["ignore_defence"] = bpskill_defence
-        #终结技加伤害
-        self.extra_ability_attribute["AllDamageAddedRatio"] = self.Skill_num("Ultra", "Ultra_A")
+        # 终结技加伤害
+        self.extra_ability_attribute["AllDamageAddedRatio"] = self.Skill_num(
+            "Ultra", "Ultra_A"
+        )
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        # 使自身造成的伤害提高，提高数值等同于效果命中的60%，最多使造成的伤害提高72%。
+        # 使自身造成的伤害提高, 提高数值等同于效果命中的60%, 最多使造成的伤害提高72%。
         Break_Damage_Added_Ratio = attribute_bonus.get("StatusProbabilityBase", 0) * 0.6
         attribute_bonus["AllDamageAddedRatio"] = attribute_bonus.get(
             "AllDamageAddedRatio", 0
         ) + min(0.72, Break_Damage_Added_Ratio)
-        
-        
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
@@ -4289,34 +4208,33 @@
             "DOT",
             "DOT",
             self.avatar_element,
             skill_multiplier,
             self.avatar_level,
         )
         skill_info_list.append({"name": "1层奥迹伤害", "damagelist": damagelist4})
-        
+
         # 计算50层奥迹持续伤害
         skill_multiplier = self.Skill_num("Talent", "Talent")
         skill_multiplier += self.Skill_num("Talent", "Talent_UP") * 50
         add_attr_bonus = copy.deepcopy(attribute_bonus)
-        add_attr_bonus["ignore_defence"] = (
-            add_attr_bonus.get("ignore_defence", 0) + 0.2
-        )
+        add_attr_bonus["ignore_defence"] = add_attr_bonus.get("ignore_defence", 0) + 0.2
         damagelist5 = await calculate_damage(
             base_attr,
             add_attr_bonus,
             "DOT",
             "DOT",
             self.avatar_element,
             skill_multiplier,
             self.avatar_level,
         )
         skill_info_list.append({"name": "50层奥迹伤害", "damagelist": damagelist5})
         return skill_info_list
 
+
 class Sparkle(BaseAvatar):
     Buff: BaseAvatarBuff
 
     def __init__(self, char: DamageInstanceAvatar, skills: List[DamageInstanceSkill]):
         super().__init__(char=char, skills=skills)
         self.eidolon_attribute: Dict[str, float] = {}
         self.extra_ability_attribute: Dict[str, float] = {}
@@ -4333,31 +4251,36 @@
         self.extra_ability_attribute["AttackAddedRatio"] = 0.45
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-       
         # 终结技天赋增加伤害
-        All_Damage_Add = (self.Skill_num("Talent", "Talent") + self.Skill_num("Ultra", "Ultra")) * 3
-        attribute_bonus["AllDamageAddedRatio"] = attribute_bonus.get(
-            "AllDamageAddedRatio", 0
-        ) + All_Damage_Add
-        
-        #战技增加暴击伤害
+        All_Damage_Add = (
+            self.Skill_num("Talent", "Talent") + self.Skill_num("Ultra", "Ultra")
+        ) * 3
+        attribute_bonus["AllDamageAddedRatio"] = (
+            attribute_bonus.get("AllDamageAddedRatio", 0) + All_Damage_Add
+        )
+
+        # 战技增加暴击伤害
         if self.avatar_rank >= 6:
-            add_critical_damage_base = attribute_bonus.get("CriticalDamageBase", 0) * (self.Skill_num("BPSkill", "BPSkill") + 0.3) + self.Skill_num("BPSkill", "BPSkill_G")
+            add_critical_damage_base = attribute_bonus.get("CriticalDamageBase", 0) * (
+                self.Skill_num("BPSkill", "BPSkill") + 0.3
+            ) + self.Skill_num("BPSkill", "BPSkill_G")
         else:
-            add_critical_damage_base = attribute_bonus.get("CriticalDamageBase", 0) * self.Skill_num("BPSkill", "BPSkill") + self.Skill_num("BPSkill", "BPSkill_G")
+            add_critical_damage_base = attribute_bonus.get(
+                "CriticalDamageBase", 0
+            ) * self.Skill_num("BPSkill", "BPSkill") + self.Skill_num(
+                "BPSkill", "BPSkill_G"
+            )
         attribute_bonus["CriticalDamageBase"] = (
             attribute_bonus.get("CriticalDamageBase", 0) + add_critical_damage_base
         )
-        
-        
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
@@ -4373,14 +4296,15 @@
         critical_damage_base_str = add_critical_damage_base * 100
         damagelist2 = []
         damagelist2.append(critical_damage_base_str)
         skill_info_list.append({"name": "战技提升爆伤(%)", "damagelist": damagelist2})
 
         return skill_info_list
 
+
 class Acheron(BaseAvatar):
     Buff: BaseAvatarBuff
 
     def __init__(self, char: DamageInstanceAvatar, skills: List[DamageInstanceSkill]):
         super().__init__(char=char, skills=skills)
         self.eidolon_attribute: Dict[str, float] = {}
         self.extra_ability_attribute: Dict[str, float] = {}
@@ -4402,18 +4326,17 @@
         self.extra_ability_attribute["AttackAddedRatio"] = 0.45
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        
-        attribute_bonus["AllDamageAddedRatio"] = attribute_bonus.get("AllDamageAddedRatio", 0) + 0.9
-        
-        
+        attribute_bonus["AllDamageAddedRatio"] = (
+            attribute_bonus.get("AllDamageAddedRatio", 0) + 0.9
+        )
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         if self.avatar_rank >= 6:
             damagelist1 = await calculate_damage(
                 base_attr,
@@ -4434,15 +4357,15 @@
                 skill_multiplier,
                 self.avatar_level,
             )
         damagelist1[0] = damagelist1[0] * 1.6
         damagelist1[1] = damagelist1[1] * 1.6
         damagelist1[2] = damagelist1[2] * 1.6
         skill_info_list.append({"name": "普攻", "damagelist": damagelist1})
-        
+
         # 计算战技伤害
         skill_multiplier = self.Skill_num("BPSkill", "BPSkill")
         if self.avatar_rank >= 6:
             damagelist2 = await calculate_damage(
                 base_attr,
                 attribute_bonus,
                 "BPSkill",
@@ -4461,21 +4384,21 @@
                 skill_multiplier,
                 self.avatar_level,
             )
         damagelist2[0] = damagelist2[0] * 1.6
         damagelist2[1] = damagelist2[1] * 1.6
         damagelist2[2] = damagelist2[2] * 1.6
         skill_info_list.append({"name": "战技", "damagelist": damagelist2})
-        
+
         # 计算终结技
         add_attr_bonus = copy.deepcopy(attribute_bonus)
         add_attr_bonus["AllDamageResistancePenetration"] = (
             add_attr_bonus.get("AllDamageResistancePenetration", 0) + 0.2
         )
-        #啼泽雨斩
+        # 啼泽雨斩
         skill_multiplier = self.Skill_num("Ultra", "Ultra_1_d")
         damagelist_u_1_d = await calculate_damage(
             base_attr,
             add_attr_bonus,
             "Ultra",
             "Ultra",
             self.avatar_element,
@@ -4491,15 +4414,15 @@
             0.6,
             self.avatar_level,
         )
         damagelist_u_1_d[0] = damagelist_u_1_d[0] * 1.6 + damagelist_u_2_d[0] * 1.6
         damagelist_u_1_d[1] = damagelist_u_1_d[1] * 1.6 + damagelist_u_2_d[1] * 1.6
         damagelist_u_1_d[2] = damagelist_u_1_d[2] * 1.6 + damagelist_u_2_d[2] * 1.6
         skill_info_list.append({"name": "啼泽雨斩", "damagelist": damagelist_u_1_d})
-        #黄泉返渡
+        # 黄泉返渡
         skill_multiplier = self.Skill_num("Ultra", "Ultra_1_a")
         damagelist_u_1_a = await calculate_damage(
             base_attr,
             add_attr_bonus,
             "Ultra",
             "Ultra",
             self.avatar_element,
@@ -4511,27 +4434,34 @@
             add_attr_bonus,
             "Ultra",
             "Ultra",
             self.avatar_element,
             0.25,
             self.avatar_level,
         )
-        damagelist_u_1_a[0] = damagelist_u_1_a[0] * 1.6 + (damagelist_u_1_a_e[0] * 1.6) * 6
-        damagelist_u_1_a[1] = damagelist_u_1_a[1] * 1.6 + (damagelist_u_1_a_e[1] * 1.6) * 6
-        damagelist_u_1_a[2] = damagelist_u_1_a[2] * 1.6 + (damagelist_u_1_a_e[2] * 1.6) * 6
+        damagelist_u_1_a[0] = (
+            damagelist_u_1_a[0] * 1.6 + (damagelist_u_1_a_e[0] * 1.6) * 6
+        )
+        damagelist_u_1_a[1] = (
+            damagelist_u_1_a[1] * 1.6 + (damagelist_u_1_a_e[1] * 1.6) * 6
+        )
+        damagelist_u_1_a[2] = (
+            damagelist_u_1_a[2] * 1.6 + (damagelist_u_1_a_e[2] * 1.6) * 6
+        )
         skill_info_list.append({"name": "黄泉返渡", "damagelist": damagelist_u_1_a})
-        
-        #总伤害
+
+        # 总伤害
         damagelist_u = {}
         damagelist_u[0] = damagelist_u_1_d[0] * 3 + damagelist_u_1_a[0]
         damagelist_u[1] = damagelist_u_1_d[1] * 3 + damagelist_u_1_a[1]
         damagelist_u[2] = damagelist_u_1_d[2] * 3 + damagelist_u_1_a[2]
         skill_info_list.append({"name": "终结技总伤", "damagelist": damagelist_u})
         return skill_info_list
 
+
 class Aventurine(BaseAvatar):
     Buff: BaseAvatarBuff
 
     def __init__(self, char: DamageInstanceAvatar, skills: List[DamageInstanceSkill]):
         super().__init__(char=char, skills=skills)
         self.eidolon_attribute: Dict[str, float] = {}
         self.extra_ability_attribute: Dict[str, float] = {}
@@ -4555,27 +4485,31 @@
         pass
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-       
         # 天赋增加暴击
-        defence = base_attr["defence"] * (1 + attribute_bonus["DefenceAddedRatio"]) + attribute_bonus["DefenceDelta"]
+        defence = (
+            base_attr["defence"] * (1 + attribute_bonus["DefenceAddedRatio"])
+            + attribute_bonus["DefenceDelta"]
+        )
         if defence > 1600:
             adddefrnce = defence - 1600
-            Critical_Chance_Base = (defence/100) * 0.02
+            Critical_Chance_Base = (defence / 100) * 0.02
             Critical_Chance_Base = min(Critical_Chance_Base, 0.48)
-            attribute_bonus["CriticalChanceBase"] = attribute_bonus.get("CriticalChanceBase", 0) + Critical_Chance_Base
-        
-        #终结技增加暴击伤害
-        attribute_bonus["CriticalDamageBase"] = attribute_bonus.get("CriticalDamageBase", 0) + self.Skill_num("Ultra", "Ultra_CD")
-        
-        
+            attribute_bonus["CriticalChanceBase"] = (
+                attribute_bonus.get("CriticalChanceBase", 0) + Critical_Chance_Base
+            )
+
+        # 终结技增加暴击伤害
+        attribute_bonus["CriticalDamageBase"] = attribute_bonus.get(
+            "CriticalDamageBase", 0
+        ) + self.Skill_num("Ultra", "Ultra_CD")
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
@@ -4594,32 +4528,32 @@
         damagelist2 = await calculate_shield(
             base_attr,
             attribute_bonus,
             skill_multiplier,
             skill_num,
         )
         skill_info_list.append({"name": "战技(护盾)", "damagelist": damagelist2})
-        
+
         # 计算终结技伤害
         skill_multiplier = self.Skill_num("Ultra", "Ultra")
         damagelist3 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Ultra",
             "Ultra",
             self.avatar_element,
             skill_multiplier,
             self.avatar_level,
             2,
         )
         skill_info_list.append({"name": "终结技", "damagelist": damagelist3})
-        
-        duanshu = 10
+
+        duanshu = 7
         if self.avatar_rank >= 4:
-            duanshu = 13
+            duanshu = 10
         damagelist5 = {}
         # 计算天赋追加攻击伤害
         skill_multiplier = self.Skill_num("Talent", "Talent")
         damagelist4 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Talent",
@@ -4630,17 +4564,18 @@
             2,
         )
         damagelist5[0] = damagelist4[0] * duanshu
         damagelist5[1] = damagelist4[1] * duanshu
         damagelist5[2] = damagelist4[2] * duanshu
         skill_info_list.append({"name": "单层【盲注】追击", "damagelist": damagelist4})
         skill_info_list.append({"name": "满层【盲注】追击", "damagelist": damagelist5})
-        
+
         return skill_info_list
 
+
 class Gallagher(BaseAvatar):
     Buff: BaseAvatarBuff
 
     def __init__(self, char: DamageInstanceAvatar, skills: List[DamageInstanceSkill]):
         super().__init__(char=char, skills=skills)
         self.eidolon_attribute: Dict[str, float] = {}
         self.extra_ability_attribute: Dict[str, float] = {}
@@ -4658,87 +4593,89 @@
         pass
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-       
-        # 使自身提供的治疗量提高，提高数值等同于击破特攻的50%，最多使提供的治疗量提高75%
-        Break_Damage_Added_Ratio_Base = attribute_bonus.get("BreakDamageAddedRatioBase", 0)
+        # 使自身提供的治疗量提高, 提高数值等同于击破特攻的50%, 最多使提供的治疗量提高75%
+        Break_Damage_Added_Ratio_Base = attribute_bonus.get(
+            "BreakDamageAddedRatioBase", 0
+        )
         Heal_Ratio_Base = Break_Damage_Added_Ratio_Base * 0.5
         Heal_Ratio_Base = min(0.75, Heal_Ratio_Base)
-        attribute_bonus["HealRatioBase"] = attribute_bonus.get("HealRatioBase", 0) + Heal_Ratio_Base
-        
-        
+        attribute_bonus["HealRatioBase"] = (
+            attribute_bonus.get("HealRatioBase", 0) + Heal_Ratio_Base
+        )
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
             "Normal",
             self.avatar_element,
             skill_multiplier,
             self.avatar_level,
         )
         skill_info_list.append({"name": "普攻", "damagelist": damagelist1})
-        
+
         # 计算强化普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal1")
         damagelist2 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
             "Normal1",
             self.avatar_element,
             skill_multiplier,
             self.avatar_level,
         )
         skill_info_list.append({"name": "强化普攻", "damagelist": damagelist2})
-        
+
         # 计算战技治疗量
         skill_num = self.Skill_num("BPSkill", "BPSkill")
         damagelist3 = await calculate_heal(
             base_attr,
             attribute_bonus,
             "BPSkill",
             0,
             skill_num,
         )
         skill_info_list.append({"name": "战技治疗量", "damagelist": damagelist3})
-        
+
         # 计算终结技伤害
         skill_multiplier = self.Skill_num("Ultra", "Ultra")
         damagelist4 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Ultra",
             "Ultra",
             self.avatar_element,
             skill_multiplier,
             self.avatar_level,
         )
         skill_info_list.append({"name": "结技", "damagelist": damagelist4})
-        
+
         # 计算天赋治疗量
         skill_num = self.Skill_num("Talent", "Talent")
         damagelist5 = await calculate_heal(
             base_attr,
             attribute_bonus,
             "Talent",
             0,
             skill_num,
         )
         skill_info_list.append({"name": "天赋治疗量", "damagelist": damagelist5})
-        
+
         return skill_info_list
 
+
 class Robin(BaseAvatar):
     Buff: BaseAvatarBuff
 
     def __init__(self, char: DamageInstanceAvatar, skills: List[DamageInstanceSkill]):
         super().__init__(char=char, skills=skills)
         self.eidolon_attribute: Dict[str, float] = {}
         self.extra_ability_attribute: Dict[str, float] = {}
@@ -4749,84 +4686,90 @@
         pass
 
     def eidolons(self):
         if self.avatar_rank >= 2:
             self.eidolon_attribute["CriticalDamageBase"] = 0.2
         if self.avatar_rank >= 6:
             self.eidolon_attribute["AllDamageResistancePenetration"] = 0.2
-        
+
     def extra_ability(self):
         pass
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-       
         # 战技伤害加成
         all_damage_added_ratio = attribute_bonus.get("AllDamageAddedRatio", 0)
-        attribute_bonus["AllDamageAddedRatio"] = all_damage_added_ratio + self.Skill_num("BPSkill", "BPSkill")
-        
+        attribute_bonus["AllDamageAddedRatio"] = (
+            all_damage_added_ratio + self.Skill_num("BPSkill", "BPSkill")
+        )
+
         # 终结技攻击加成计算
         attack = (
             base_attr["attack"] * (1 + attribute_bonus["AttackAddedRatio"])
             + attribute_bonus["AttackDelta"]
         )
-        add_attack = (attack * self.Skill_num("Ultra", "Ultra_A")) + self.Skill_num("Ultra", "Ultra_G")
-        attribute_bonus["AttackDelta"] = attribute_bonus.get("AttackDelta", 0) + add_attack
-        
+        add_attack = (attack * self.Skill_num("Ultra", "Ultra_A")) + self.Skill_num(
+            "Ultra", "Ultra_G"
+        )
+        attribute_bonus["AttackDelta"] = (
+            attribute_bonus.get("AttackDelta", 0) + add_attack
+        )
+
         # 天赋爆伤加成
         Critical_Damage_Base = attribute_bonus.get("CriticalDamageBase", 0)
-        attribute_bonus["CriticalDamageBase"] =  Critical_Damage_Base + self.Skill_num("Talent", "Talent")
-        
-        
+        attribute_bonus["CriticalDamageBase"] = Critical_Damage_Base + self.Skill_num(
+            "Talent", "Talent"
+        )
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
             attribute_bonus,
             "Normal",
             "Normal",
             self.avatar_element,
             skill_multiplier,
             self.avatar_level,
         )
         skill_info_list.append({"name": "普攻", "damagelist": damagelist1})
-        
+
         # 计算战技治疗量
         skill_num = self.Skill_num("BPSkill", "BPSkill")
         damagelist2 = {}
         damagelist2[0] = add_attack
         skill_info_list.append({"name": "终结技攻击提高", "damagelist": damagelist2})
-        
+
         # 计算追击伤害
         skill_multiplier = self.Skill_num("Ultra", "Ultra")
         add_attr_bonus = copy.deepcopy(attribute_bonus)
-        add_attr_bonus['CriticalDamageBase'] = 1
-        add_attr_bonus['CriticalChanceBase'] = 0.95
+        add_attr_bonus["CriticalDamageBase"] = 1
+        add_attr_bonus["CriticalChanceBase"] = 0.95
         if self.avatar_rank >= 1:
             skill_multiplier = skill_multiplier + 0.72
         if self.avatar_rank >= 6:
-            add_attr_bonus['CriticalDamageBase'] = 3
+            add_attr_bonus["CriticalDamageBase"] = 3
         damagelist4 = await calculate_damage(
             base_attr,
             add_attr_bonus,
             "Talent",
             "Talent",
             self.avatar_element,
             skill_multiplier,
             self.avatar_level,
         )
         skill_info_list.append({"name": "【协奏】追加伤害", "damagelist": damagelist4})
-        
+
         return skill_info_list
 
+
 class AvatarDamage:
     @classmethod
     def create(cls, char: DamageInstanceAvatar, skills: List[DamageInstanceSkill]):
         if char.id_ == 1214:
             return XueYi(char, skills)
         if char.id_ == 1306:
             return Sparkle(char, skills)
```

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Base/AvatarBase.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Base/AvatarBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,24 +45,21 @@
         cls.extra_ability_id = []
         if char.extra_ability:
             for extra_ability in char.extra_ability:
                 cls.extra_ability_id.append(extra_ability["extraAbilityId"])
         return cls
 
     @abstractmethod
-    async def Technique(self):
-        ...
+    async def Technique(self): ...
 
     @abstractmethod
-    async def eidolons(self):
-        ...
+    async def eidolons(self): ...
 
     @abstractmethod
-    async def extra_ability(self):
-        ...
+    async def extra_ability(self): ...
 
 
 class BaseAvatarinfo:
     def __init__(self, char: DamageInstanceAvatar):
         self.avatar_id = char.id_
         self.avatar_level = char.level
         self.avatar_rank = char.rank
```

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Base/RelicBase.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Base/RelicBase.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,21 @@
         self.relic_type = relic.Type
         self.relic_level = relic.Level
         self.relic_attribute_bonus: Dict[str, float] = {}
 
     def get_attribute_(self):
         # MainAffix
         if self.raw_relic.MainAffix.Property in self.relic_attribute_bonus:
-            self.relic_attribute_bonus[
-                self.raw_relic.MainAffix.Property
-            ] += self.raw_relic.MainAffix.Value
+            self.relic_attribute_bonus[self.raw_relic.MainAffix.Property] += (
+                self.raw_relic.MainAffix.Value
+            )
         else:
-            self.relic_attribute_bonus[
-                self.raw_relic.MainAffix.Property
-            ] = self.raw_relic.MainAffix.Value
+            self.relic_attribute_bonus[self.raw_relic.MainAffix.Property] = (
+                self.raw_relic.MainAffix.Value
+            )
 
         # SubAffix
         if self.raw_relic.SubAffixList:
             for sub_affix in self.raw_relic.SubAffixList:
                 sub_affix_property = sub_affix.Property
                 value = sub_affix.Value
                 if sub_affix_property in self.relic_attribute_bonus:
@@ -54,23 +54,22 @@
         self.relicSetAttribute = self.set_skill_property_ability()
 
     @abstractmethod
     async def check(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
-    ):
-        ...
+    ) -> bool: ...
 
     @abstractmethod
     async def set_skill_ability(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
-    ):
+    ) -> Dict[str, float]:
         """战斗加成属性, 与 set_skill_property() 互斥"""
         ...
 
     def set_skill_property_ability(self):
         def add_relic_set_attribute(status_add: RelicSetStatusAdd):
             set_property = status_add.Property
             set_value = status_add.Value
```

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Base/SkillBase.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Base/SkillBase.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Base/WeaponBase.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Base/WeaponBase.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,17 @@
         self.weapon_promotion = weapon.promotion
         self.weapon_base_attribute = self.get_attribute()
         self.weapon_attribute: Dict[str, float] = {}
         self.get_attribute()
         self.weapon_property_ability()
 
     @abstractmethod
-    async def weapon_ability(self, base_attr: Dict, attribute_bonus: Dict):
+    async def weapon_ability(
+        self, Ultra_Use: float, base_attr: Dict[str, float], attribute_bonus: Dict
+    ) -> Dict[str, float]:
         """战斗加成属性, 与 weapon_property_ability() 互斥"""
         ...
 
     def weapon_property_ability(self):
         """面板加成属性, 与 weapon_ability() 互斥"""
         ability_property = EquipmentID2AbilityProperty[str(self.weapon_id)]
         equip_ability_property = ability_property[str(self.weapon_rank)]
@@ -46,16 +48,15 @@
             value = equip_ability["Value"]["Value"]
             if property_type in self.weapon_attribute:
                 self.weapon_attribute[property_type] += value
             else:
                 self.weapon_attribute[property_type] = value
 
     @abstractmethod
-    async def check(self):
-        ...
+    async def check(self) -> bool: ...
 
     def get_attribute(self):
         promotion = EquipmentPromotionConfig.Equipment[str(self.weapon_id)][
             str(self.weapon_promotion)
         ]
 
         return BaseWeaponAttribute(
```

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Base/model.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Base/model.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Excel/SkillData.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Excel/SkillData.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Excel/weapon_effect.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Excel/weapon_effect.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Relic/Relic.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Relic/Relic.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,68 +424,81 @@
         attribute_bonus: Dict[str, float],
     ):
         if self.pieces4 and await self.check(base_attr, attribute_bonus):
             ignore_defence = attribute_bonus.get("ignore_defence", 0)
             attribute_bonus["ignore_defence"] = ignore_defence + 0.06000000009313226 * 3
         return attribute_bonus
 
+
 class Relic117(BaseRelicSetSkill):
     def __init__(self, set_id: int, count: int):
         super().__init__(set_id, count)
         self._count = count
 
     async def check(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         """2件: 对受负面状态影响的敌人造成的伤害提高12%。"""
-        # 暴击率提高4%，装备者对陷入不少于2/3个负面效果的敌方目标造成的暴击伤害提高8%/12%。装备者对敌方目标施加负面效果后，上述效果提高100%，持续1回合
+        # 暴击率提高4%, 装备者对陷入不少于2/3个负面效果的敌方目标造成的暴击伤害提高8%/12%。装备者对敌方目标施加负面效果后, 上述效果提高100%, 持续1回合
         logger.info("Relic114 check success")
         return True
 
     async def set_skill_ability(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         if self.pieces2 and await self.check(base_attr, attribute_bonus):
             All_Damage_Added_Ratio = attribute_bonus.get("AllDamageAddedRatio", 0)
-            attribute_bonus["AllDamageAddedRatio"] = All_Damage_Added_Ratio + 0.12000000011175871
+            attribute_bonus["AllDamageAddedRatio"] = (
+                All_Damage_Added_Ratio + 0.12000000011175871
+            )
         if self.pieces4 and await self.check(base_attr, attribute_bonus):
             Critical_Chance_Base = attribute_bonus.get("CriticalChanceBase", 0)
-            attribute_bonus["CriticalChanceBase"] = Critical_Chance_Base + 0.0400000000372529
+            attribute_bonus["CriticalChanceBase"] = (
+                Critical_Chance_Base + 0.0400000000372529
+            )
             Critical_Damage_Base = attribute_bonus.get("CriticalDamageBase", 0)
-            attribute_bonus["CriticalDamageBase"] = Critical_Damage_Base + 0.12000000011175871 * 2
+            attribute_bonus["CriticalDamageBase"] = (
+                Critical_Damage_Base + 0.12000000011175871 * 2
+            )
         return attribute_bonus
 
+
 class Relic118(BaseRelicSetSkill):
     def __init__(self, set_id: int, count: int):
         super().__init__(set_id, count)
         self._count = count
 
     async def check(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        """当装备者对我方目标施放终结技时，我方全体击破特攻提高30%，持续2回合，该效果无法叠加。"""
+        """当装备者对我方目标施放终结技时, 我方全体击破特攻提高30%, 持续2回合, 该效果无法叠加。"""
         logger.info("Relic114 check success")
         return True
 
     async def set_skill_ability(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         if self.pieces4 and await self.check(base_attr, attribute_bonus):
-            Break_Damage_Added_Ratio_Base = attribute_bonus.get("BreakDamageAddedRatioBase", 0)
-            attribute_bonus["BreakDamageAddedRatioBase"] = Break_Damage_Added_Ratio_Base + 0.3000000002793968
+            Break_Damage_Added_Ratio_Base = attribute_bonus.get(
+                "BreakDamageAddedRatioBase", 0
+            )
+            attribute_bonus["BreakDamageAddedRatioBase"] = (
+                Break_Damage_Added_Ratio_Base + 0.3000000002793968
+            )
         return attribute_bonus
 
+
 class Relic301(BaseRelicSetSkill):
     def __init__(self, set_id: int, count: int):
         super().__init__(set_id, count)
 
     async def check(
         self,
         base_attr: Dict[str, float],
@@ -827,62 +840,65 @@
         if self.pieces2 and await self.check(base_attr, attribute_bonus):
             attribute_bonus["AllDamageAddedRatio"] = (
                 attribute_bonus.get("AllDamageAddedRatio", 0) + 0.10000000018626451
             )
 
         return attribute_bonus
 
+
 class Relic313(BaseRelicSetSkill):
     def __init__(self, set_id: int, count: int):
         super().__init__(set_id, count)
 
     async def check(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        """当敌方目标被消灭时，装备者暴击伤害提高4%，最多叠加10层。"""
+        """当敌方目标被消灭时, 装备者暴击伤害提高4%, 最多叠加10层。"""
         return True
 
     async def set_skill_ability(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         if self.pieces2 and await self.check(base_attr, attribute_bonus):
-            attribute_bonus["CriticalDamageBase"] = (
-                attribute_bonus.get("CriticalDamageBase", 0) + (0.0400000000372529 * 10)
-            )
+            attribute_bonus["CriticalDamageBase"] = attribute_bonus.get(
+                "CriticalDamageBase", 0
+            ) + (0.0400000000372529 * 10)
 
         return attribute_bonus
 
+
 class Relic314(BaseRelicSetSkill):
     def __init__(self, set_id: int, count: int):
         super().__init__(set_id, count)
 
     async def check(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
-        """若至少存在一名与装备者命途相同的队友，装备者的暴击率提高12%。"""
+        """若至少存在一名与装备者命途相同的队友, 装备者的暴击率提高12%。"""
         return True
 
     async def set_skill_ability(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         if self.pieces2 and await self.check(base_attr, attribute_bonus):
             attribute_bonus["CriticalChanceBase"] = (
                 attribute_bonus.get("CriticalChanceBase", 0) + 0.12000000011175871
             )
 
         return attribute_bonus
 
+
 class RelicSet:
     HEAD: SingleRelic
     HAND: SingleRelic
     BODY: SingleRelic
     FOOT: SingleRelic
     NECK: SingleRelic
     OBJECT: SingleRelic
```

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Role.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Role.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 ):
     add_attr_bonus = copy.deepcopy(attribute_bonus)
 
     add_attr_bonus = apply_attribute_bonus(add_attr_bonus, skill_type, add_skill_type)
 
     merged_attr = await merge_attribute(base_attr, add_attr_bonus)
 
-    injury_area, element_area = calculate_injury_area(
+    injury_area = calculate_injury_area(
         merged_attr,
         skill_type,
         add_skill_type,
         element,
     )
 
     critical_damage = calculate_critical_damage(merged_attr, skill_type, add_skill_type)
@@ -438,27 +438,37 @@
     add_attr_bonus: Dict[str, float],
     skill_type: str,
     add_skill_type: str,
     element: str,
     is_hp=0,
 ):
     add_attr_bonus_tz = copy.deepcopy(add_attr_bonus)
-    add_attr_bonus_tz['AttackAddedRatio'] = add_attr_bonus_tz.get('AttackAddedRatio',0) + 1.694
-    add_attr_bonus_tz['ignore_defence'] = add_attr_bonus_tz.get('ignore_defence',0) + 0.44
-    add_attr_bonus_tz['AllDamageResistancePenetration'] = add_attr_bonus_tz.get('AllDamageResistancePenetration',0) + 0.27
-    add_attr_bonus_tz['AllDamageAddedRatio'] = add_attr_bonus_tz.get('AllDamageAddedRatio',0) + 2.06
-    add_attr_bonus_tz['CriticalDamageBase'] = add_attr_bonus_tz.get('CriticalDamageBase',0) + 4.578
+    add_attr_bonus_tz["AttackAddedRatio"] = (
+        add_attr_bonus_tz.get("AttackAddedRatio", 0) + 1.694
+    )
+    add_attr_bonus_tz["ignore_defence"] = (
+        add_attr_bonus_tz.get("ignore_defence", 0) + 0.44
+    )
+    add_attr_bonus_tz["AllDamageResistancePenetration"] = (
+        add_attr_bonus_tz.get("AllDamageResistancePenetration", 0) + 0.27
+    )
+    add_attr_bonus_tz["AllDamageAddedRatio"] = (
+        add_attr_bonus_tz.get("AllDamageAddedRatio", 0) + 2.06
+    )
+    add_attr_bonus_tz["CriticalDamageBase"] = (
+        add_attr_bonus_tz.get("CriticalDamageBase", 0) + 4.578
+    )
     merged_attr_tz = await merge_attribute(base_attr, add_attr_bonus_tz)
     if is_hp == 1:
         attack_tz = merged_attr_tz.get("hp", 0)
     elif is_hp == 2:
         attack_tz = merged_attr_tz.get("defence", 0)
     else:
         attack_tz = merged_attr_tz.get("attack", 0)
-    
+
     resistance_area_tz = calculate_resistance_area(
         merged_attr_tz,
         skill_type,
         add_skill_type,
         element,
     )
     # print(f'抗性区:{resistance_area_tz}')
@@ -469,17 +479,19 @@
     injury_area_tz = calculate_injury_area(
         merged_attr_tz,
         skill_type,
         add_skill_type,
         element,
     )
     # print(f'增伤区:{injury_area_tz}')
-    critical_damage_tz = calculate_critical_damage(merged_attr_tz, skill_type, add_skill_type)
+    critical_damage_tz = calculate_critical_damage(
+        merged_attr_tz, skill_type, add_skill_type
+    )
     # print(f'爆伤区:{critical_damage_tz}')
-    
+
     return (
         attack_tz
         * skill_multiplier
         * damage_ratio
         * injury_area_tz
         * defence_multiplier_tz
         * resistance_area_tz
```

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/damage/Weapon/Weapon.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/damage/Weapon/Weapon.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,15 +242,15 @@
 class BeforeDawn(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -275,15 +275,15 @@
 class IntheNight(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -426,15 +426,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 根据装备者的能量上限, 提高装备者造成的伤害: 每点能量提高0.2%, 最多计入160点
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -487,15 +487,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 终结技造成的伤害提高32%。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -701,15 +701,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 使装备者的攻击力提高24%
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -947,15 +947,15 @@
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 使装备者的击破特攻提高20%
         # 装备者施放终结技时, 使装备者造成的持续伤害提高24%
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -967,15 +967,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 当装备者攻击防御力被降低的敌方目标后, 恢复4点能量。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -988,15 +988,15 @@
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 装备者施放普攻或战技后,
         # 对随机1个受到攻击的敌方目标造成等同于自身48%攻击力的附加伤害。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1064,15 +1064,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 造成的持续伤害提高24%。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1179,15 +1179,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # ...
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1199,15 +1199,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 装备者施放终结技时造成的伤害值提高, 提高数值等同于装备者防御力的60%
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1219,15 +1219,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 战斗开始时, 使我方全体受到的伤害降低8%
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1240,15 +1240,15 @@
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 当装备者受到攻击后, 有100%的基础概率使敌方目标陷入灼烧状态,
         # 每回合造成等同于装备者40%防御力的持续伤害
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1260,15 +1260,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 装备者受到攻击的概率提高, 同时受到的伤害降低16%。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1280,15 +1280,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 进入战斗后, 使我方全体的全属性抗性提高8%
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1300,15 +1300,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 进入战斗后, 使我方全体的全属性抗性提高8%
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1320,15 +1320,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 进入战斗后, 使我方全体的全属性抗性提高8%
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1424,15 +1424,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 使装备者普攻和战技造成的伤害提高20%。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1454,15 +1454,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 施放战技后, 使装备者的下一次普攻对敌方目标造成等同于自身60%攻击力的附加伤害。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1558,15 +1558,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 使装备者施放战技后额外恢复8点能量
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1578,15 +1578,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 使装备者终结技造成的伤害提高28%。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1605,15 +1605,15 @@
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 当队友受到攻击或消耗生命值后, 装备者获得1层【月蚀】,
         # 最多叠加3层。每层【月蚀】使装备者下一次攻击造成的伤害提高14%。
         # 叠满3层时, 额外使该次攻击无视目标12%的防御力。该效果在装备者施放攻击后解除。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1739,15 +1739,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 当装备者对我方目标提供治疗时,记录治疗量。当任意我方目标施放攻击后,根据记录治疗量的36%,对随机1个受到攻击的敌方目标造成基于装备者属性的附加伤害
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1846,15 +1846,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 在施放战技时为我方全体恢复2点能量。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1902,15 +1902,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 随机为1个当前能量百分比小于50%的我方其他目标恢复8点能量。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -1922,15 +1922,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 施放普攻或战技后, 为我方全体回复等同于各自生命上限2%的生命值。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -2011,15 +2011,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 战斗开始时, 立即为我方全体恢复6点能量。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -2031,15 +2031,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 战斗开始时, 立即为我方全体恢复6点能量。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -2051,15 +2051,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 当装备者施放战技后, 使下一个行动的我方【其他目标】造成的伤害提高30%
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -2071,15 +2071,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 装备者施放攻击后, 额外恢复4点能量
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -2091,15 +2091,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 当我方目标造成与装备者相同属性的伤害时, 造成的伤害提高12%。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -2120,15 +2120,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 当装备者施放终结技后, 我方全体行动提前16%。
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -2140,15 +2140,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 使下一个行动的我方【其他目标】造成的伤害提高16%
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -2163,15 +2163,15 @@
         super().__init__(weapon)
 
     async def check(self):
         # 在战斗开始时以及当装备者回合开始时,随机生效1个效果
         # 使我方全体攻击力提高10%
         # 使我方全体暴击伤害提高12%
         # 暂时固定只算攻击
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -2192,15 +2192,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 进入战斗后,使我方全体的攻击力提高8%
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -2221,15 +2221,15 @@
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
         # 使装备者施放攻击或受到攻击后,额外恢复4点能量
-        pass
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
@@ -2338,54 +2338,60 @@
                     weapon_effect["23019"]["Param"]["AllDamageAddedRatio"][
                         self.weapon_rank - 1
                     ]
                 )
             )
         return attribute_bonus
 
+
 # 游戏尘寰
 class EarthlyEscapade(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        # 战斗开始时，使装备者获得【假面】，持续3回合。当装备者持有【假面】时，装备者的队友暴击率提高10%，暴击伤害提高28%。
+        # 战斗开始时, 使装备者获得【假面】, 持续3回合。当装备者持有【假面】时, 装备者的队友暴击率提高10%, 暴击伤害提高28%。
         return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         if await self.check():
             critical_damage_base = attribute_bonus.get("CriticalDamageBase", 0)
             attribute_bonus["CriticalDamageBase"] = (
                 critical_damage_base
-                + weapon_effect["23021"]["Param"]["CriticalDamageBase"][self.weapon_rank - 1]
+                + weapon_effect["23021"]["Param"]["CriticalDamageBase"][
+                    self.weapon_rank - 1
+                ]
             )
-            
+
             critical_chance_base = attribute_bonus.get("CriticalChanceBase", 0)
             attribute_bonus["CriticalChanceBase"] = (
                 critical_chance_base
-                + weapon_effect["23021"]["Param"]["CriticalChance"][self.weapon_rank - 1]
+                + weapon_effect["23021"]["Param"]["CriticalChance"][
+                    self.weapon_rank - 1
+                ]
             )
         return attribute_bonus
 
+
 # 重塑时光之忆
 class ReforgedRemembrance(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        # 装备者对陷入风化、灼烧、触电、裂伤状态的敌方目标造成伤害时，分别获得1层【先知】，最多叠加4层。单场战斗中，每种持续伤害状态类型仅可叠加1次【先知】效果。每层【先知】使装备者的攻击力提高5%，造成的持续伤害无视目标7.2%的防御力。
+        # 装备者对陷入风化、灼烧、触电、裂伤状态的敌方目标造成伤害时, 分别获得1层【先知】, 最多叠加4层。单场战斗中, 每种持续伤害状态类型仅可叠加1次【先知】效果。每层【先知】使装备者的攻击力提高5%, 造成的持续伤害无视目标7.2%的防御力。
         return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
@@ -2397,55 +2403,57 @@
                 + (
                     weapon_effect["23022"]["Param"]["AttackAddedRatio"][
                         self.weapon_rank - 1
                     ]
                 )
                 * 4
             )
-            
+
             resistance_penetration = attribute_bonus.get("DOTignore_defence", 0)
             attribute_bonus["DOTignore_defence"] = (
                 resistance_penetration
                 + (
                     weapon_effect["23022"]["Param"]["ignore_defence"][
                         self.weapon_rank - 1
                     ]
                 )
                 * 4
             )
         return attribute_bonus
 
+
 # 何物为真
 class WhatIsReal(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        # 施放普攻后，装备者回复等同于2%生命上限+800点的生命值。
-        pass
+        # 施放普攻后, 装备者回复等同于2%生命上限+800点的生命值。
+        return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         return attribute_bonus
 
+
 # 美梦小镇大冒险
 class DreamvilleAdventure(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        # 装备者施放普攻、战技、终结技中某一类型的技能后，为我方全体附加【童心】，【童心】可以使我方目标对应类型的技能所造成的伤害提高12%
+        # 装备者施放普攻、战技、终结技中某一类型的技能后, 为我方全体附加【童心】, 【童心】可以使我方目标对应类型的技能所造成的伤害提高12%
         return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
@@ -2458,44 +2466,43 @@
                     weapon_effect["21036"]["Param"]["AllDamageAddedRatio"][
                         self.weapon_rank - 1
                     ]
                 )
             )
         return attribute_bonus
 
+
 # 最后的赢家
 class FinalVictor(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        # 当装备者对敌方目标造成暴击后获得一层【好运】，最多叠加4层。每层【好运】使装备者的暴击伤害提高8%
+        # 当装备者对敌方目标造成暴击后获得一层【好运】, 最多叠加4层。每层【好运】使装备者的暴击伤害提高8%
         return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         if await self.check():
             Critical_Damage_Base = attribute_bonus.get("CriticalDamageBase", 0)
-            attribute_bonus["CriticalDamageBase"] = (
-                Critical_Damage_Base
-                + (
-                    weapon_effect["21037"]["Param"]["CriticalDamageBase"][
-                        self.weapon_rank - 1
-                    ]
-                    * 4
-                )
+            attribute_bonus["CriticalDamageBase"] = Critical_Damage_Base + (
+                weapon_effect["21037"]["Param"]["CriticalDamageBase"][
+                    self.weapon_rank - 1
+                ]
+                * 4
             )
         return attribute_bonus
 
+
 # 在火的远处
 class FlamesAfar(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
@@ -2517,48 +2524,62 @@
                     weapon_effect["21038"]["Param"]["AllDamageAddedRatio"][
                         self.weapon_rank - 1
                     ]
                 )
             )
         return attribute_bonus
 
+
 # 织造命运之线
 class DestinysThreadsForewoven(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        # 装备者每有100点防御力，使装备者造成的伤害提高0.8%，最多使造成的伤害提高32%。
+        # 装备者每有100点防御力, 使装备者造成的伤害提高0.8%, 最多使造成的伤害提高32%。
         return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         if await self.check():
-            defence = base_attr["defence"] * (1 + attribute_bonus["DefenceAddedRatio"]) + attribute_bonus["DefenceDelta"]
-            damage_added = (defence/100) * weapon_effect["21039"]["Param"]["AllDamageAddedRatio"][self.weapon_rank - 1]
-            damage_added = min(damage_added, weapon_effect["21039"]["Param"]["AllDamageAddedRatio_max"][self.weapon_rank - 1])
+            defence = (
+                base_attr["defence"] * (1 + attribute_bonus["DefenceAddedRatio"])
+                + attribute_bonus["DefenceDelta"]
+            )
+            damage_added = (defence / 100) * weapon_effect["21039"]["Param"][
+                "AllDamageAddedRatio"
+            ][self.weapon_rank - 1]
+            damage_added = min(
+                damage_added,
+                weapon_effect["21039"]["Param"]["AllDamageAddedRatio_max"][
+                    self.weapon_rank - 1
+                ],
+            )
             all_damage_added_ratio = attribute_bonus.get("AllDamageAddedRatio", 0)
-            attribute_bonus["AllDamageAddedRatio"] = all_damage_added_ratio + damage_added
+            attribute_bonus["AllDamageAddedRatio"] = (
+                all_damage_added_ratio + damage_added
+            )
         return attribute_bonus
 
+
 # 银河沦陷日
 class TheDayTheCosmosFell(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        # 装备者施放攻击后，若有不少于2个被攻击的敌方目标具有对应属性弱点，装备者的暴击伤害提高20%，持续2回合。
+        # 装备者施放攻击后, 若有不少于2个被攻击的敌方目标具有对应属性弱点, 装备者的暴击伤害提高20%, 持续2回合。
         return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
@@ -2571,64 +2592,63 @@
                     weapon_effect["21040"]["Param"]["CriticalDamageBase"][
                         self.weapon_rank - 1
                     ]
                 )
             )
         return attribute_bonus
 
+
 # 好戏开演
 class ItsShowtime(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        # 装备者对敌方目标施加负面状态后，获得一层【戏法】，每层【戏法】使装备者造成的伤害提高6%，最多叠加3层，持续1回合。当装备者的效果命中大于等于80%时，攻击力提高20%。
+        # 装备者对敌方目标施加负面状态后, 获得一层【戏法】, 每层【戏法】使装备者造成的伤害提高6%, 最多叠加3层, 持续1回合。当装备者的效果命中大于等于80%时, 攻击力提高20%。
         return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         if await self.check():
             all_damage_added_ratio = attribute_bonus.get("AllDamageAddedRatio", 0)
-            attribute_bonus["AllDamageAddedRatio"] = (
-                all_damage_added_ratio
-                + (
-                    weapon_effect["21041"]["Param"]["AllDamageAddedRatio"][
-                        self.weapon_rank - 1
-                    ]
-                    * 3
-                )
+            attribute_bonus["AllDamageAddedRatio"] = all_damage_added_ratio + (
+                weapon_effect["21041"]["Param"]["AllDamageAddedRatio"][
+                    self.weapon_rank - 1
+                ]
+                * 3
             )
             Status_Probability_Base = attribute_bonus.get("StatusProbabilityBase", 0)
             if Status_Probability_Base >= 0.8:
                 Attack_Added_Ratio = attribute_bonus.get("AttackAddedRatio", 0)
                 attribute_bonus["AttackAddedRatio"] = (
                     Attack_Added_Ratio
                     + (
                         weapon_effect["21041"]["Param"]["AttackAddedRatio"][
                             self.weapon_rank - 1
                         ]
                     )
                 )
         return attribute_bonus
 
+
 # 铭记于心的约定
 class IndeliblePromise(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        # 当装备者释放终结技时，暴击率提高15%，持续2回合。
+        # 当装备者释放终结技时, 暴击率提高15%, 持续2回合。
         return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
@@ -2641,53 +2661,52 @@
                     weapon_effect["21042"]["Param"]["CriticalChanceBase"][
                         self.weapon_rank - 1
                     ]
                 )
             )
         return attribute_bonus
 
+
 # 两个人的演唱会
 class ConcertforTwo(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        # 场上每有一名持有护盾的角色，装备者造成的伤害提高4%。
+        # 场上每有一名持有护盾的角色, 装备者造成的伤害提高4%。
         return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         if await self.check():
             all_damage_added_ratio = attribute_bonus.get("AllDamageAddedRatio", 0)
-            attribute_bonus["AllDamageAddedRatio"] = (
-                all_damage_added_ratio
-                + (
-                    weapon_effect["21043"]["Param"]["AllDamageAddedRatio"][
-                        self.weapon_rank - 1
-                    ]
-                    * 4
-                )
+            attribute_bonus["AllDamageAddedRatio"] = all_damage_added_ratio + (
+                weapon_effect["21043"]["Param"]["AllDamageAddedRatio"][
+                    self.weapon_rank - 1
+                ]
+                * 4
             )
         return attribute_bonus
 
+
 # 行于流逝的岸
 class AlongthePassingShore(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        # 装备者对陷入【泡影】状态的目标造成的伤害提高24%，终结技造成的伤害额外提高24%
+        # 装备者对陷入【泡影】状态的目标造成的伤害提高24%, 终结技造成的伤害额外提高24%
         return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
@@ -2701,31 +2720,28 @@
                         self.weapon_rank - 1
                     ]
                 )
             )
             Ultra_Dmg_Add = attribute_bonus.get("UltraDmgAdd", 0)
             attribute_bonus["UltraDmgAdd"] = (
                 Ultra_Dmg_Add
-                + (
-                    weapon_effect["23024"]["Param"]["UltraDmgAdd"][
-                        self.weapon_rank - 1
-                    ]
-                )
+                + (weapon_effect["23024"]["Param"]["UltraDmgAdd"][self.weapon_rank - 1])
             )
         return attribute_bonus
 
+
 # 命运从未公平
 class InherentlyUnjustDestiny(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        # 当装备者为我方目标提供护盾时，使装备者的暴击伤害提高40%，持续2回合。当装备者发动追加攻击击中敌方目标时，有100%的基础概率使受到攻击的敌方目标受到的伤害提高10%，持续2回合。
+        # 当装备者为我方目标提供护盾时, 使装备者的暴击伤害提高40%, 持续2回合。当装备者发动追加攻击击中敌方目标时, 有100%的基础概率使受到攻击的敌方目标受到的伤害提高10%, 持续2回合。
         return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
@@ -2739,31 +2755,28 @@
                         self.weapon_rank - 1
                     ]
                 )
             )
             Dmg_Ratio = attribute_bonus.get("DmgRatio", 0)
             attribute_bonus["DmgRatio"] = (
                 Dmg_Ratio
-                + (
-                    weapon_effect["23023"]["Param"]["DmgRatio"][
-                        self.weapon_rank - 1
-                    ]
-                )
+                + (weapon_effect["23023"]["Param"]["DmgRatio"][self.weapon_rank - 1])
             )
         return attribute_bonus
 
+
 # 夜色流光溢彩
 class FlowingNightglow(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        # 【华彩】使装备者的攻击力提高48%，使我方全体造成的伤害提高24%，持续1回合。
+        # 【华彩】使装备者的攻击力提高48%, 使我方全体造成的伤害提高24%, 持续1回合。
         return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
@@ -2785,23 +2798,24 @@
                     weapon_effect["23026"]["Param"]["AllDamageAddedRatio"][
                         self.weapon_rank - 1
                     ]
                 )
             )
         return attribute_bonus
 
+
 # 驶向第二次生命
 class SailingTowardsASecondLife(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        # 造成的击破伤害无视目标20%的防御力。当装备者击中敌方目标时，使目标受到的伤害提高1%，该状态最多叠加6层
+        # 造成的击破伤害无视目标20%的防御力。当装备者击中敌方目标时, 使目标受到的伤害提高1%, 该状态最多叠加6层
         return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
@@ -2813,25 +2827,20 @@
                 + (
                     weapon_effect["23027"]["Param"]["ignore_defence"][
                         self.weapon_rank - 1
                     ]
                 )
             )
             Dmg_Ratio = attribute_bonus.get("DmgRatio", 0)
-            attribute_bonus["DmgRatio"] = (
-                Dmg_Ratio
-                + (
-                    weapon_effect["23027"]["Param"]["DmgRatio"][
-                        self.weapon_rank - 1
-                    ]
-                    * 6
-                )
+            attribute_bonus["DmgRatio"] = Dmg_Ratio + (
+                weapon_effect["23027"]["Param"]["DmgRatio"][self.weapon_rank - 1] * 6
             )
         return attribute_bonus
 
+
 # 无边曼舞
 class BoundlessChoreo(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
@@ -2853,23 +2862,24 @@
                     weapon_effect["21044"]["Param"]["CriticalDamageBase"][
                         self.weapon_rank - 1
                     ]
                 )
             )
         return attribute_bonus
 
+
 # 为了明日的旅途
 class ForTomorrowsJourney(BaseWeapon):
     weapon_base_attributes: Dict
 
     def __init__(self, weapon: DamageInstanceWeapon):
         super().__init__(weapon)
 
     async def check(self):
-        # 装备者施放终结技后，造成的伤害提高18%
+        # 装备者施放终结技后, 造成的伤害提高18%
         return True
 
     async def weapon_ability(
         self,
         Ultra_Use: float,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
@@ -2882,14 +2892,15 @@
                     weapon_effect["22002"]["Param"]["AllDamageAddedRatio"][
                         self.weapon_rank - 1
                     ]
                 )
             )
         return attribute_bonus
 
+
 class Weapon:
     @classmethod
     def create(cls, weapon: DamageInstanceWeapon):
         if weapon.id_ == 23019:
             return PastSelfinMirror(weapon)
         if weapon.id_ == 23024:
             return AlongthePassingShore(weapon)
```

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/damage/utils.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/damage/utils.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/excel/AvatarPromotionConfig.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/excel/AvatarPromotionConfig.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/excel/EquipmentPromotionConfig.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/excel/EquipmentPromotionConfig.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/excel/RelicMainAffixConfig.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/excel/RelicMainAffixConfig.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/excel/RelicSubAffixConfig.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/excel/RelicSubAffixConfig.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/excel/light_cone_ranks.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/excel/light_cone_ranks.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/excel/model.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/excel/model.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/excel/read_excel.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/excel/read_excel.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/exception.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/exception.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 class UidNotfoundError(Exception):
     def __init__(self, uid: str):
         self.uid = uid
 
     def __str__(self):
         return self.uid
 
+
 class InvalidUidError(Exception):
     def __init__(self, uid: str):
         self.uid = uid
 
     def __str__(self):
         return self.uid
```

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/SR_MAP_PATH.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/SR_MAP_PATH.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/AvatarRelicScore.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/AvatarRelicScore.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/EquipmentID2AbilityProperty_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/EquipmentID2AbilityProperty_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/EquipmentID2EnName_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/EquipmentID2EnName_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/EquipmentID2Name_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/EquipmentID2Name_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/EquipmentID2Rarity_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/EquipmentID2Rarity_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/ItemId2Name_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/ItemId2Name_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/Property2Name.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/Property2Name.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/Property2Name_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/Property2Name_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/RelicId2MainAffixGroup_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/RelicId2MainAffixGroup_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/RelicId2Rarity_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/RelicId2Rarity_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/RelicId2SetId_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/RelicId2SetId_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/RelicSetSkill_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/RelicSetSkill_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/SetId2Name_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/SetId2Name_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/avatarId2DamageType_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/avatarId2DamageType_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/avatarId2EnName_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/avatarId2EnName_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/avatarId2Name_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/avatarId2Name_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/avatarId2Rarity_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/avatarId2Rarity_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/avatarId2Star_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/avatarId2Star_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/avatarRankSkillUp_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/avatarRankSkillUp_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/char_alias.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/char_alias.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/characterSkillTree_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/characterSkillTree_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/rankId2Name_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/rankId2Name_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/skillId2AttackType_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/skillId2AttackType_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/skillId2Name_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/skillId2Name_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/data/skillId2Type_mapping_2.1.0.json` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/data/skillId2Type_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/map/model/RelicSetSkill.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/map/model/RelicSetSkill.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/mihomo/models.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/mihomo/models.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/mihomo/requests.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/mihomo/requests.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/mono/Character.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/mono/Character.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     RelicSetSkill,
 )
 
 
 class Character:
     def __init__(self, card_prop: Dict):
         self.char_level: int = int(card_prop["avatarLevel"])
-        self.char_id: str = card_prop["avatarId"]
+        self.char_id: int = card_prop["avatarId"]
         self.char_name: str = card_prop["avatarName"]
         self.char_rank = card_prop["rank"] if card_prop.get("rank") else 0
         self.char_rarity = card_prop["avatarRarity"]
         self.char_element = card_prop["avatarElement"]
         self.char_promotion = card_prop["avatarPromotion"]
         self.char_skill = card_prop["avatarSkill"]
         self.extra_ability = card_prop["avatarExtraAbility"]
@@ -24,32 +24,33 @@
         self.add_attr = {}
         self.equipment = card_prop["equipmentInfo"]
         self.rarity = card_prop["avatarRarity"]
         self.eidolons = card_prop["rankList"] if card_prop.get("rankList") else []
 
     async def get_equipment_info(self):
         if self.equipment == {}:
-            return
+            return None
         base_attr = self.base_attributes
         equip = self.equipment
         ability_property = EquipmentID2AbilityProperty[str(equip["equipmentID"])]
         equip_rank = equip["equipmentRank"]
 
         equip_ability_property = ability_property[str(equip_rank)]
 
         equip_add_base_attr = equip["baseAttributes"]
         base_attr["hp"] = base_attr["hp"] + equip_add_base_attr["hp"]
         base_attr["attack"] = base_attr["attack"] + equip_add_base_attr["attack"]
         base_attr["defence"] = base_attr["defence"] + equip_add_base_attr["defence"]
         self.base_attributes = base_attr
 
         for equip_ability in equip_ability_property:
-            property_type = equip_ability["PropertyType"]
-            value = equip_ability["Value"]["Value"]
+            property_type: str = equip_ability["PropertyType"]
+            value: float = equip_ability["Value"]["Value"]
             self.add_attr[property_type] = value + self.add_attr.get(property_type, 0)
+        return self.add_attr
 
     async def get_char_attribute_bonus(self):
         attribute_bonus = self.attribute_bonus
         for bonus in attribute_bonus:
             status_add = bonus["statusAdd"]
             bonus_property = status_add["property"]
             value = status_add["value"]
```

### Comparing `starrail_damage_cal-1.5.3/starrail_damage_cal/to_data.py` & `starrail_damage_cal-1.5.4/starrail_damage_cal/to_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,18 +61,20 @@
     if sr_data.detailInfo is None:
         raise CharacterShowcaseNotOpenError(player_uid)
 
     char_name_list: List[str] = []
     char_id_list: List[str] = []
     char_data_list: Dict[str, Dict] = {}
     nickName = PlayerDetailInfo.nickname
-    avatarList = (PlayerDetailInfo.avatarDetailList if PlayerDetailInfo.avatarDetailList else []) + (PlayerDetailInfo.assistAvatarList if PlayerDetailInfo.assistAvatarList else [])
+    avatarList = (
+        PlayerDetailInfo.avatarDetailList if PlayerDetailInfo.avatarDetailList else []
+    ) + (PlayerDetailInfo.assistAvatarList if PlayerDetailInfo.assistAvatarList else [])
     for char in avatarList:
         if str(char.avatarId) in char_id_list:
-                continue
+            continue
         char_data, avatarName = await get_data(
             char,
             nickName,
             player_uid,
             save_path,
         )
         char_name_list.append(avatarName)
@@ -207,17 +209,17 @@
             if level_up_skill:
                 for item in level_up_skill:
                     skill_id = item["id"]
                     skill_up_num = item["num"]
                     # 查找skill_id在不在avatarSkill中
                     for index, skill_item in enumerate(char_data["avatarSkill"]):
                         if str(skill_id) == str(skill_item["skillId"]):
-                            char_data["avatarSkill"][index][
-                                "skillLevel"
-                            ] += skill_up_num
+                            char_data["avatarSkill"][index]["skillLevel"] += (
+                                skill_up_num
+                            )
                             break
 
     # 处理基础属性
     base_attributes = {}
     avatar_promotion_base = AvatarPromotionConfig.Avatar[str(char.avatarId)][
         str(char.promotion)
     ]
```

### Comparing `starrail_damage_cal-1.5.3/test/test.json` & `starrail_damage_cal-1.5.4/test/test.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.3/test/test_get_char.py` & `starrail_damage_cal-1.5.4/test/test_get_char.py`

 * *Files identical despite different names*

