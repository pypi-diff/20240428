# Comparing `tmp/ogl-2.1.31.tar.gz` & `tmp/ogl-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogl-2.1.31.tar", last modified: Sun Apr 28 18:52:02 2024, max compression
+gzip compressed data, was "ogl-2.1.5.tar", last modified: Wed Jan 17 19:09:25 2024, max compression
```

## Comparing `ogl-2.1.31.tar` & `ogl-2.1.5.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 18:52:02.548687 ogl-2.1.31/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-07-05 13:40:50.000000 ogl-2.1.31/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2391 2024-04-28 18:52:02.548510 ogl-2.1.31/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1812 2023-09-18 19:13:40.000000 ogl-2.1.31/README.md
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      885 2024-03-10 15:04:29.000000 ogl-2.1.31/pyproject.toml
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2024-04-28 18:52:02.548723 ogl-2.1.31/setup.cfg
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 18:52:02.528391 ogl-2.1.31/src/
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 18:52:02.535898 ogl-2.1.31/src/miniogl/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5038 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/AnchorPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3100 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       87 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/Constants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1365 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/ControlPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3743 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/Diagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    40731 2024-04-16 20:02:01.000000 ogl-2.1.31/src/miniogl/DiagramFrame.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4713 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/DlgDebugDiagramFrame.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1669 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/LinePoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13685 2024-02-05 15:39:13.000000 ogl-2.1.31/src/miniogl/LineShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3606 2024-01-11 17:39:29.000000 ogl-2.1.31/src/miniogl/LollipopLine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1746 2024-04-14 16:30:05.000000 ogl-2.1.31/src/miniogl/MiniOglColorEnum.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1684 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/MiniOglPenStyle.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      170 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/MiniOglUtils.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2771 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/PointShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10767 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/RectangleShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1076 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/RectangleShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4772 2024-02-05 15:39:00.000000 ogl-2.1.31/src/miniogl/RotatableShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2176 2024-01-11 17:37:44.000000 ogl-2.1.31/src/miniogl/SelectAnchorPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21669 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/Shape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2336 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/ShapeEventHandler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1632 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/ShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1452 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/SizerShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7511 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/TextShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      649 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/TextShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5650 2024-02-05 15:38:50.000000 ogl-2.1.31/src/miniogl/VShapes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/miniogl/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 18:52:02.541001 ogl-2.1.31/src/ogl/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1457 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/EventEngineMixin.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      126 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/IllegalOperationException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4648 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/OglActor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1463 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/OglAggregation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12295 2024-04-28 18:03:40.000000 ogl-2.1.31/src/ogl/OglAssociation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1085 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/OglAssociationLabel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    18240 2024-03-06 01:14:33.000000 ogl-2.1.31/src/ogl/OglClass.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1411 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/OglComposition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      647 2024-01-12 21:20:02.000000 ogl-2.1.31/src/ogl/OglConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      717 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/OglDimensions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1464 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/OglInheritance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3567 2024-02-05 01:38:31.000000 ogl-2.1.31/src/ogl/OglInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6213 2024-01-11 15:42:53.000000 ogl-2.1.31/src/ogl/OglInterface2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15751 2024-02-04 23:51:59.000000 ogl-2.1.31/src/ogl/OglLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3591 2024-04-28 18:31:36.000000 ogl-2.1.31/src/ogl/OglLinkFactory.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2695 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/OglNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1183 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/OglNoteLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4936 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/OglObject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      474 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/OglPosition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8636 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/OglText.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      226 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/OglTextFontFamily.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2201 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/OglUseCase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4349 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/OglUtils.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       37 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       23 2024-04-28 18:15:07.000000 ogl-2.1.31/src/ogl/_version.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 18:52:02.543058 ogl-2.1.31/src/ogl/events/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      546 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/events/IOglEventEngine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/events/InvalidKeywordException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4573 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/events/OglEventEngine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      806 2024-04-14 13:48:57.000000 ogl-2.1.31/src/ogl/events/OglEvents.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      239 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/events/ShapeSelectedEventData.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/events/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/events/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 18:52:02.543599 ogl-2.1.31/src/ogl/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21924 2024-01-17 19:01:50.000000 ogl-2.1.31/src/ogl/preferences/OglPreferences.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/preferences/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 18:52:02.543701 ogl-2.1.31/src/ogl/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/resources/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 18:52:02.544342 ogl-2.1.31/src/ogl/resources/img/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1350 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/resources/img/Display.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1702 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/resources/img/DoNotDisplay.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2238 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/resources/img/UnSpecified.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/resources/img/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/resources/img/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 18:52:02.545028 ogl-2.1.31/src/ogl/resources/img/textdetails/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1543 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/resources/img/textdetails/DecreaseTextSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1575 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/resources/img/textdetails/IncreaseTextSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/resources/img/textdetails/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/resources/img/textdetails/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 18:52:02.546026 ogl-2.1.31/src/ogl/sd/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      791 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/sd/OglInstanceName.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6879 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/sd/OglSDInstance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6876 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/sd/OglSDMessage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/sd/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/sd/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 18:52:02.547138 ogl-2.1.31/src/ogl/ui/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      657 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/ui/BaseOglPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4001 2024-01-12 00:19:17.000000 ogl-2.1.31/src/ogl/ui/DefaultValuesPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12232 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/ui/DiagramPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11862 2024-01-14 15:43:14.000000 ogl-2.1.31/src/ogl/ui/OglClassMenuHandler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/ui/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/ui/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 18:52:02.548185 ogl-2.1.31/src/ogl/ui/valuecontrols/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2279 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/ui/valuecontrols/AssociationAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6507 2024-02-19 14:44:08.000000 ogl-2.1.31/src/ogl/ui/valuecontrols/ClassAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2987 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/ui/valuecontrols/DefaultNamesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1952 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/ui/valuecontrols/NoteAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2697 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/ui/valuecontrols/SDAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5322 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/ui/valuecontrols/TextAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.31/src/ogl/ui/valuecontrols/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 18:52:02.548315 ogl-2.1.31/src/ogl.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2391 2024-04-28 18:52:02.000000 ogl-2.1.31/src/ogl.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2934 2024-04-28 18:52:02.000000 ogl-2.1.31/src/ogl.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2024-04-28 18:52:02.000000 ogl-2.1.31/src/ogl.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       80 2024-04-28 18:52:02.000000 ogl-2.1.31/src/ogl.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2024-04-28 18:52:02.000000 ogl-2.1.31/src/ogl.egg-info/top_level.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-01-17 19:09:25.211936 ogl-2.1.5/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-07-05 13:40:50.000000 ogl-2.1.5/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2390 2024-01-17 19:09:25.211739 ogl-2.1.5/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1812 2023-09-18 19:13:40.000000 ogl-2.1.5/README.md
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      885 2024-01-17 18:58:26.000000 ogl-2.1.5/pyproject.toml
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2024-01-17 19:09:25.211979 ogl-2.1.5/setup.cfg
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-01-17 19:09:25.198295 ogl-2.1.5/src/
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-01-17 19:09:25.202737 ogl-2.1.5/src/miniogl/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5038 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/AnchorPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3100 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       87 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/Constants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1365 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/ControlPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3743 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/Diagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    41005 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/DiagramFrame.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4713 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/DlgDebugDiagramFrame.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1669 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/LinePoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13685 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/LineShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3606 2024-01-11 17:39:29.000000 ogl-2.1.5/src/miniogl/LollipopLine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1747 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/MiniOglColorEnum.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1684 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/MiniOglPenStyle.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      170 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/MiniOglUtils.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2771 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/PointShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10767 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/RectangleShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1076 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/RectangleShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4772 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/RotatableShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2176 2024-01-11 17:37:44.000000 ogl-2.1.5/src/miniogl/SelectAnchorPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21669 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/Shape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2336 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/ShapeEventHandler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1632 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/ShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1452 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/SizerShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7511 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/TextShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      649 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/TextShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5650 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/VShapes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/miniogl/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-01-17 19:09:25.206341 ogl-2.1.5/src/ogl/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1457 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/EventEngineMixin.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      126 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/IllegalOperationException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4648 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglActor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1463 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglAggregation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13189 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglAssociation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1085 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglAssociationLabel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    17671 2024-01-12 21:10:07.000000 ogl-2.1.5/src/ogl/OglClass.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1411 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglComposition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      647 2024-01-12 21:20:02.000000 ogl-2.1.5/src/ogl/OglConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      717 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglDimensions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1464 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglInheritance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3538 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6213 2024-01-11 15:42:53.000000 ogl-2.1.5/src/ogl/OglInterface2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15757 2024-01-11 17:41:50.000000 ogl-2.1.5/src/ogl/OglLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3091 2024-01-17 19:03:51.000000 ogl-2.1.5/src/ogl/OglLinkFactory.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2695 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1183 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglNoteLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4936 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglObject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      474 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglPosition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8636 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglText.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      226 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglTextFontFamily.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2201 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglUseCase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4349 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/OglUtils.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       37 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       22 2024-01-17 18:53:00.000000 ogl-2.1.5/src/ogl/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-01-17 19:09:25.207808 ogl-2.1.5/src/ogl/events/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      546 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/events/IOglEventEngine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/events/InvalidKeywordException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4573 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/events/OglEventEngine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      792 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/events/OglEvents.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      239 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/events/ShapeSelectedEventData.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/events/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/events/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-01-17 19:09:25.208160 ogl-2.1.5/src/ogl/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21924 2024-01-17 19:01:50.000000 ogl-2.1.5/src/ogl/preferences/OglPreferences.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/preferences/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-01-17 19:09:25.208269 ogl-2.1.5/src/ogl/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/resources/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-01-17 19:09:25.208872 ogl-2.1.5/src/ogl/resources/img/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1350 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/resources/img/Display.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1702 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/resources/img/DoNotDisplay.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2238 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/resources/img/UnSpecified.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/resources/img/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/resources/img/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-01-17 19:09:25.209332 ogl-2.1.5/src/ogl/resources/img/textdetails/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1543 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/resources/img/textdetails/DecreaseTextSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1575 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/resources/img/textdetails/IncreaseTextSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/resources/img/textdetails/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/resources/img/textdetails/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-01-17 19:09:25.209877 ogl-2.1.5/src/ogl/sd/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      791 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/sd/OglInstanceName.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6879 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/sd/OglSDInstance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6876 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/sd/OglSDMessage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/sd/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/sd/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-01-17 19:09:25.210549 ogl-2.1.5/src/ogl/ui/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      657 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/ui/BaseOglPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4001 2024-01-12 00:19:17.000000 ogl-2.1.5/src/ogl/ui/DefaultValuesPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12232 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/ui/DiagramPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11862 2024-01-14 15:43:14.000000 ogl-2.1.5/src/ogl/ui/OglClassMenuHandler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/ui/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/ui/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-01-17 19:09:25.211404 ogl-2.1.5/src/ogl/ui/valuecontrols/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2279 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/ui/valuecontrols/AssociationAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6502 2024-01-12 00:33:03.000000 ogl-2.1.5/src/ogl/ui/valuecontrols/ClassAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2987 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/ui/valuecontrols/DefaultNamesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1952 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/ui/valuecontrols/NoteAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2697 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/ui/valuecontrols/SDAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5322 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/ui/valuecontrols/TextAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:11:32.000000 ogl-2.1.5/src/ogl/ui/valuecontrols/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-01-17 19:09:25.211541 ogl-2.1.5/src/ogl.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2390 2024-01-17 19:09:25.000000 ogl-2.1.5/src/ogl.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2934 2024-01-17 19:09:25.000000 ogl-2.1.5/src/ogl.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2024-01-17 19:09:25.000000 ogl-2.1.5/src/ogl.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       80 2024-01-17 19:09:25.000000 ogl-2.1.5/src/ogl.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2024-01-17 19:09:25.000000 ogl-2.1.5/src/ogl.egg-info/top_level.txt
```

### Comparing `ogl-2.1.31/LICENSE` & `ogl-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/PKG-INFO` & `ogl-2.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ogl
-Version: 2.1.31
+Version: 2.1.5
 Summary: External Pyut Graphical Shapes
 Author-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 Maintainer-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Project-URL: Repository, https://github.com/hasii2011/ogl
 Keywords: pyut,graphical shapes,python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wxPython~=4.2.1
-Requires-Dist: codeallybasic>=1.3.0
-Requires-Dist: codeallyadvanced>=1.3.1
-Requires-Dist: pyutmodelv2>=2.1.5
+Requires-Dist: codeallybasic>=1.1.0
+Requires-Dist: codeallyadvanced>=1.1.0
+Requires-Dist: pyutmodelv2==2.1.0
 
 ![](https://github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-badge-version-2-256x48.png "AGPL")
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/ogl/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/ogl/tree/master)
 [![PyPI version](https://badge.fury.io/py/ogl.svg)](https://badge.fury.io/py/ogl)
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: ogl Version: 2.1.31 Summary: External Pyut
-Graphical Shapes Author-email: "Humberto A. Sanchez II"
+Metadata-Version: 2.1 Name: ogl Version: 2.1.5 Summary: External Pyut Graphical
+Shapes Author-email: "Humberto A. Sanchez II"
 gmail.com> Maintainer-email: "Humberto A. Sanchez II"
 gmail.com> License: GNU AFFERO GENERAL PUBLIC LICENSE Project-URL: Repository,
 https://github.com/hasii2011/ogl Keywords: pyut,graphical shapes,python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-wxPython~=4.2.1 Requires-Dist: codeallybasic>=1.3.0 Requires-Dist:
-codeallyadvanced>=1.3.1 Requires-Dist: pyutmodelv2>=2.1.5 ![](https://
+wxPython~=4.2.1 Requires-Dist: codeallybasic>=1.1.0 Requires-Dist:
+codeallyadvanced>=1.1.0 Requires-Dist: pyutmodelv2==2.1.0 ![](https://
 github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-
 badge-version-2-256x48.png "AGPL") [![Maintenance](https://img.shields.io/
 badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/
 graphs/commit-activity) [![CircleCI](https://dl.circleci.com/status-badge/img/
 gh/hasii2011/ogl/tree/master.svg?style=shield)](https://dl.circleci.com/status-
 badge/redirect/gh/hasii2011/ogl/tree/master) [![PyPI version](https://
 badge.fury.io/py/ogl.svg)](https://badge.fury.io/py/ogl) ð ð¨ ð¤ ð£
```

### Comparing `ogl-2.1.31/README.md` & `ogl-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/pyproject.toml` & `ogl-2.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 license     = {text = 'GNU AFFERO GENERAL PUBLIC LICENSE'}
 authors     = [{name = 'Humberto A. Sanchez II', email = 'Humbert.A.Sanchez.II@gmail.com'}]
 maintainers = [{name = 'Humberto A. Sanchez II', email = 'Humbert.A.Sanchez.II@gmail.com'}]
 keywords    = ['pyut', 'graphical shapes', 'python',]
 
 dependencies = [
   'wxPython~=4.2.1',
-  'codeallybasic>=1.3.0',
-  'codeallyadvanced>=1.3.1',
-  'pyutmodelv2>=2.1.5',
+  'codeallybasic>=1.1.0',
+  'codeallyadvanced>=1.1.0',
+  'pyutmodelv2==2.1.0',
 ]
 
 [project.urls]
 Repository = 'https://github.com/hasii2011/ogl'
 
 
 [tool.setuptools.packages.find]
```

### Comparing `ogl-2.1.31/src/miniogl/AnchorPoint.py` & `ogl-2.1.5/src/miniogl/AnchorPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/Common.py` & `ogl-2.1.5/src/miniogl/Common.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/ControlPoint.py` & `ogl-2.1.5/src/miniogl/ControlPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/Diagram.py` & `ogl-2.1.5/src/miniogl/Diagram.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/DiagramFrame.py` & `ogl-2.1.5/src/miniogl/DiagramFrame.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         self._minLevelZoom:  int = 0
         self._zoomLevel:     int = 0           # number of zoom factors applied
         self._maxZoomFactor: float = 6         # can zoom in beyond 600%
         self._minZoomFactor: float = 0.2       # can zoom out beyond 20%
 
         self._defaultZoomFactor: float = 1.5   # used when only a point is selected
 
-        # margins define a perimeter around the work area that must remain
+        # margins define a perimeter around the work area that must remains
         # blank and hidden. if we scroll beyond the limits, the diagram is
         # resized.
         # self._leftMargin   = DEFAULT_MARGIN_VALUE
         # self._rightMargin  = DEFAULT_MARGIN_VALUE
         # self._topMargin    = DEFAULT_MARGIN_VALUE
         # self._bottomMargin = DEFAULT_MARGIN_VALUE
         self._isInfinite = False    # to know if the frame is infinite or not
@@ -501,14 +501,16 @@
     def Refresh(self, eraseBackground: bool = True, rect: Rect = None):
         """
         not used
         Args:
             eraseBackground:    if False, the stored background is used
             rect:               not used
         """
+
+        # self.clsLogger.warning(f'Refresh - {eraseBackground=}')
         if eraseBackground:
             self.Redraw()
         else:
             self.RedrawWithBackground()
 
     def SaveBackground(self, dc: DC):
         """
@@ -556,24 +558,23 @@
         dc.Clear()
         dc.SelectObject(NullBitmap)
 
     def CreateDC(self, loadBackground: bool, w: int, h: int) -> DC:
         """
         Create a DC, load the background on demand.
 
-        Args:
-            loadBackground:
-            w: width of the frame.
-            h: height of the frame.
+        @param loadBackground
+        @param w : width of the frame.
+        @param h :  height of the frame.
 
-        Returns:  A device context
+        @return DC
         """
         dc = MemoryDC()
         bm = self.__workingBitmap
-        # cache the bitmap, to avoid creating a new one at each refresh.
+        # cache the bitmap, to avoid creating a new at each refresh.
         # only recreate it if the size of the window has changed
         if (bm.GetWidth(), bm.GetHeight()) != (w, h):
             bm = self.__workingBitmap = Bitmap(w, h)
         dc.SelectObject(bm)
         if loadBackground:
             self.LoadBackground(dc, w, h)
         else:
@@ -615,28 +616,28 @@
 
         dc.SetFont(self._defaultFont)
 
         shapes = self._diagram.GetShapes()
         if full:
             # first time, need to create the background
             if saveBackground:
-                # first, draw every non-moving shape
+                # first, draw every non-moving shapes
                 for shape in shapes:
                     if not shape.IsMoving():
                         shape.Draw(dc)
                 # save the background
                 self.SaveBackground(dc)
                 # draw every moving shape
                 for shape in shapes:
                     if shape.IsMoving():
                         shape.Draw(dc)
 
             # x, y = self.CalcUnScrolledPosition(0, 0)
             if useBackground:
-                # draw every moving shape
+                # draw every moving shapes
                 for shape in shapes:
                     if shape.IsMoving():
                         shape.Draw(dc)
                 # TODO: This code belongs in OnPaint
                 # if self._prefs.backgroundGridEnabled is True:
                 #     self._drawGrid(memDC=dc, width=w, height=h, startX=x, startY=y)
             else:  # don't use background
@@ -656,27 +657,28 @@
 
             x, y = self.CalcUnscrolledPosition(0, 0)
             client.Blit(0, 0, w, h, dc, x, y)
 
     # noinspection PyUnusedLocal
     def OnPaint(self, event: PaintEvent):
         """
-        Refresh the screen when the system issues a paint event.
+        Refresh the screen when a paint event is issued by the system.
 
         Args:
             event:
         """
         dc = PaintDC(self)
         w, h = self.GetSize()
         mem = self.CreateDC(False, w, h)
         mem.SetBackground(Brush(self.GetBackgroundColour()))
         mem.Clear()
 
         x, y = self.CalcUnscrolledPosition(0, 0)
         #
+        # self.clsLogger.warning(f'OnPaint - {w=}, {h=} {x=} {y=}')
         # Paint events don't seem to be generated when Pyut is built for deployment;  So code duplicated in .Redraw()
         #
         if self._prefs.backgroundGridEnabled is True:
             self._drawGrid(memDC=mem, width=w, height=h, startX=x, startY=y)
         self.Redraw(mem)
 
         dc.Blit(0, 0, w, h, mem, x, y)
@@ -685,36 +687,36 @@
         """
         Do the "zoom in" fitted on the selected area or with a default factor
         and the clicked point as central point of the zoom.
         The maximal zoom that can be reached is :
 
             self.GetMaxLevelZoom() * self.GetDefaultZoomFactor()
 
-        If the maximal zoom level is reached, then the shapes are centered
+        If the maximal zoom level is reached, then the shapes are just centered
         on the selected area or on the clicked point.
 
 
         Args:
             ax:     abscissa of the upper left corner of the selected
                             area or abscissa of the central point of the zoom
             ay:     ordinate of the upper left corner of the selected
                             area or ordinate of the central point of the zoom
             width:  width of the selected area for the zoom
             height: height of the selected area for the zoom
         """
         # number of pixels per unit of scrolling
         xUnit, yUnit = self.GetScrollPixelsPerUnit()
 
-        # This is the position of the client area upper left corner.
+        # position of the upper left corner of the client area
         # (work area that is visible) in scroll units.
         viewStartX, viewStartY = self.GetViewStart()
 
-        # Get the client and virtual work area size.
-        # The client size is the size of the work area that is visible.
-        # The virtual is the whole work area's size.
+        # Get the client and virtual size of the work area, where
+        # the client size is the size of the work area that is
+        # visible and the virtual is the whole work area's size.
         clientWidth, clientHeight = self.GetClientSize()
         virtualWidth, virtualHeight = self.GetVirtualSize()
 
         # maximal zoom factor that can be applied
         # maxZoomFactor = self.GetMaxLevelZoom() * self.GetDefaultZoomFactor()
         maxZoomFactor = self.maxZoomFactor
 
@@ -736,97 +738,95 @@
             y = y - height
 
         # init the zoom's offsets and factor
         # zoomFactor = 1
         # dx = 0
         # dy = 0
 
-        # If there is no selected area but a clicked point, a default
-        # zoom is performed with the clicked point as its center.
+        # if there is no selected area but a clicked point, a default
+        # zoom is performed with the clicked point as center.
         if width == 0 or height == 0:
             zoomFactor = self.GetDefaultZoomFactor()
-            # Check if the zoom factor that we are to apply combined with the
+            # check if the zoom factor that we are to apply combined with the
             # previous ones won't be beyond the maximal zoom. If it's the case,
             # we proceed to the calculation of the zoom factor that allows to
             # exactly reach the maximal zoom.
             maxZoomReached = maxZoomFactor <= (self.GetCurrentZoom() * zoomFactor)
             if maxZoomReached:
                 zoomFactor = maxZoomFactor/self.GetCurrentZoom()
-            # if the view is reduced, we eliminate the
+            # if the view is reduced, we just eliminate the
             # last zoom out performed
             if self._zoomLevel < 0:
                 self._zoomStack.pop()
                 self._zoomLevel += 1
             else:
                 if zoomFactor > 1.0:
                     self._zoomStack.append(zoomFactor)
                     self._zoomLevel += 1
 
-            # Calculate the zoom area upper-left corner.
-            # The size is half of the diagram frame.
-            # It is centred on the clicked point.
-            # This calculation is done in a way to
+            # calculation of the upper-left corner of a zoom area whose
+            # size is the half of the diagram frame and which is centred
+            # on the clicked point. This calculation is done in the way to
             # get the zoom area centred in the middle of the virtual screen.
             dx = virtualWidth/2 - x
             dy = virtualHeight/2 - y
 
         else:
             # to be sure to get all the shapes in the selected zoom area
             if width > height:
                 zoomFactor = clientWidth / abs(width)
             else:
                 zoomFactor = clientHeight / abs(height)
 
-            # Check if the zoom factor that we are to apply combined with the
+            # check if the zoom factor that we are to apply combined with the
             # previous ones won't be beyond the maximal zoom. If it's the case,
             # we proceed to the calculation of the zoom factor that allows to
             # exactly reach the maximal zoom.
             maxZoomReached = maxZoomFactor <= self.currentZoom * zoomFactor
             if maxZoomReached:
                 zoomFactor = maxZoomFactor/self.GetCurrentZoom()
 
-            # Calculate the zoom area upper-left corner.
-            # The size is the half of the diagram frame and is centred
-            # on the clicked point.
-            # This calculation is done in a way to
-            # get the zoom area centered in the middle of the virtual screen.
+            # calculation of the upper-left corner of a zoom area whose
+            # size is the half of the diagram frame and which is centred
+            # on the clicked point. This calculation is done in the way to
+            # get the zoom area centred in the middle of the virtual screen.
             dx = virtualWidth/2 - x - (clientWidth / zoomFactor / 2.0)
             dy = virtualHeight/2 - y - (clientHeight / zoomFactor / 2.0)
 
-            # We have to check if the "zoom in" on a reduced view produces
+            # we have to check if the "zoom in" on a reduced view produces
             # another less reduced view or an enlarged view. For this, we
             # get the global current zoom, multiply by the zoom factor to
             # obtain only one zoom factor.
             if self._zoomLevel < 0:
 
                 globalFactor = zoomFactor * self.currentZoom
                 self._zoomStack = []
                 self._zoomStack.append(globalFactor)
 
                 if globalFactor < 1.0:
                     self._zoomLevel = -1    # the view is still reduced
                 elif globalFactor > 1.0:
                     self._zoomLevel = 1     # the view is enlarged
                 else:
-                    self._zoomLevel = 0     # the zoom in is  equal to all the zoom out previously applied
+                    self._zoomLevel = 0     # the zoom in is just equal to all the zoom out previously applied
             else:
                 if zoomFactor > 1.0:
                     self._zoomStack.append(zoomFactor)
                     self._zoomLevel += 1
 
         # set the offsets between the model and the view
         self.xOffSet = (self.xOffSet + dx) * zoomFactor
         self.yOffSet = (self.yOffSet + dy) * zoomFactor
 
         # updates the shapes (view) position and dimensions from
         # their models in the light of the new zoom factor and offsets.
         for shape in self.diagram.GetShapes():
             shape.UpdateFromModel()
 
-        # resize the virtual screen to match with the zoom
+        # resize the virtual screen in order to match with the zoom
         virtualWidth  = round(virtualWidth * zoomFactor)
         virtualHeight = round(virtualHeight * zoomFactor)
 
         virtualSize:   Size = Size(virtualWidth, virtualHeight)
         self.SetVirtualSize(virtualSize)
 
         # perform the scrolling in the way to have the zoom area visible
@@ -835,60 +835,59 @@
         scrollY = (virtualHeight - clientHeight) / 2 / yUnit
         self.Scroll(round(scrollX), round(scrollY))
 
     def DoZoomOut(self, ax: int, ay: int):
         """
         Do the 'zoom out' in the way to have the clicked point (ax, ay) as
         the central point of new view.
-        If one or many of 'zoom in' operations where performed before, then we suppress the
+        If one or many 'zoom in' where performed before, then we just suppress the
         last one from the zoom stack.
         Else, we add the default inverted zoom factor to the stack.
 
         Args:
             ax: abscissa of the clicked point
             ay: ordinate of the clicked point
         """
         # number of pixels per unit of scrolling
         xUnit, yUnit = self.GetScrollPixelsPerUnit()
 
-        # Position of the client area upper-left corner.
+        # position of the upper left corner of the client area
         # (work area that is visible) in scroll units.
         viewStartX, viewStartY = self.GetViewStart()
 
-        # Get the work area client and virtual size.
-        # The client size is the size of the work area that is visible.
-        # The virtual size is the whole work area's size.
+        # Get the client and virtual size of the work area, where
+        # the client size is the size of the work area that is
+        # visible and the virtual is the whole work area's size.
         clientWidth, clientHeight = self.GetClientSize()
         virtualWidth, virtualHeight = self.GetVirtualSize()
 
-        # Transform event coordinates to get them relative to the upper left corner of
+        # transform event coordinates to get them relative to the upper left corner of
         # the virtual screen (avoid the case where that corner is on a shape and
         # get its coordinates relative to the shape).
         if ax >= viewStartX * xUnit and ay >= viewStartY * yUnit:
             x = ax
             y = ay
         else:
             x = ax + viewStartX * xUnit
             y = ay + viewStartY * yUnit
 
-        # Calculate the upper-left corner of a zoom area whose
+        # calculation of the upper-left corner of a zoom area whose
         # size is the half of the diagram frame and which is centred
-        # on the clicked point.
-        # This calculation is done to
+        # on the clicked point. This calculation is done in the way to
         # get the zoom area centred in the middle of the virtual screen.
         dx: int = virtualWidth // 2 - x
         dy: int = virtualHeight // 2 - y
 
         # minZoomFactor = self.GetMinZoomFactor()
         minZoomFactor: float = self.minZoomFactor
         # minZoomReached = False        not used
 
-        # If the view is enlarged, then we remove the last
-        # zoom-in factor that has been applied.
-        # Else, we apply the default one in inverted.
+        # if the view is enlarged, then we just remove the last
+        # zoom in factor that has been applied. Else, we apply
+        # the default one in inverted.
         if self._zoomLevel > 0:
             zoomFactor = 1/self._zoomStack.pop()
             self._zoomLevel -= 1
         else:
             # zoomFactor = 1/self.GetDefaultZoomFactor()
             zoomFactor = 1 / self.defaultZoomFactor
             # check if minimal zoom has been reached
@@ -912,15 +911,15 @@
 
         # updates the shapes (view) position and dimensions from
         # their model in the light of the new zoom factor and offsets.
         # for shape in self.GetDiagram().GetShapes():
         for shape in self.diagram.GetShapes():
             shape.UpdateFromModel()
 
-        # resize the virtual screen to match with the zoom
+        # resize the virtual screen in order to match with the zoom
         virtualWidth  = round(virtualWidth * zoomFactor)
         virtualHeight = round(virtualHeight * zoomFactor)
 
         virtualSize:   Size = Size(virtualWidth, virtualHeight)
         self.SetVirtualSize(virtualSize)
 
         # perform the scrolling in the way to have the zoom area visible
@@ -946,15 +945,15 @@
         if infinite is True:
             # place all the shapes in an area centered on the infinite work area
             vWidth, vHeight = self.GetVirtualSize()
             cWidth, cHeight = self.GetClientSize()
             # get the number of pixels per scroll unit
             xUnit, yUnit = self.GetScrollPixelsPerUnit()
 
-            # get the scroll units
+            # get the number of scroll unit
             noUnitX = (vWidth-cWidth) / xUnit
             noUnitY = (vHeight-cHeight) / yUnit
 
             if self._prefs.centerDiagram is True:
                 self.Scroll(noUnitX / 2, noUnitY / 2)   # set the scrollbars position in the middle of their scale
             else:
                 self.Scroll(0, 0)
@@ -1147,14 +1146,15 @@
     def _drawHorizontalLines(self, memDC: DC, width: int, height: int, startX: int, startY: int):
 
         x1:   int = 0
         x2:   int = startX + width
         stop: int = height + startY
         step: int = self._prefs.backgroundGridInterval
         for movingY in range(startY, stop, step):
+            # self.clsLogger.info(f'{x1=} {movingY=} - {x2=} {movingY=}')
             memDC.DrawLine(x1, movingY, x2, movingY)
 
     def _drawVerticalLines(self, memDC: DC, width: int, height: int, startX: int, startY: int):
 
         y1:   int = 0
         y2:   int = startY + height
         stop: int = width + startX
```

### Comparing `ogl-2.1.31/src/miniogl/DlgDebugDiagramFrame.py` & `ogl-2.1.5/src/miniogl/DlgDebugDiagramFrame.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/LinePoint.py` & `ogl-2.1.5/src/miniogl/LinePoint.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/LineShape.py` & `ogl-2.1.5/src/miniogl/LineShape.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/LollipopLine.py` & `ogl-2.1.5/src/miniogl/LollipopLine.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/MiniOglColorEnum.py` & `ogl-2.1.5/src/miniogl/MiniOglColorEnum.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from wx import Colour
 from wx import ColourDatabase
 
 
 class MiniOglColorEnum(Enum):
     """
     The purpose of this enumeration is to keep wxPython types from getting into
-    the user visible portions of the preference dialog
+    the user visible portions of the preferences dialog
     Custom colors came from:
         https://www.rapidtables.com/web/color/RGB_Color.html
     """
 
     BLACK             = 'Black'
     CORNFLOWER_BLUE   = 'Cornflower Blue'
     WHITE             = 'White'
```

### Comparing `ogl-2.1.31/src/miniogl/MiniOglPenStyle.py` & `ogl-2.1.5/src/miniogl/MiniOglPenStyle.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/PointShape.py` & `ogl-2.1.5/src/miniogl/PointShape.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/RectangleShape.py` & `ogl-2.1.5/src/miniogl/RectangleShape.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/RectangleShapeModel.py` & `ogl-2.1.5/src/miniogl/RectangleShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/RotatableShape.py` & `ogl-2.1.5/src/miniogl/RotatableShape.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/SelectAnchorPoint.py` & `ogl-2.1.5/src/miniogl/SelectAnchorPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/Shape.py` & `ogl-2.1.5/src/miniogl/Shape.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/ShapeEventHandler.py` & `ogl-2.1.5/src/miniogl/ShapeEventHandler.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/ShapeModel.py` & `ogl-2.1.5/src/miniogl/ShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/SizerShape.py` & `ogl-2.1.5/src/miniogl/SizerShape.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/TextShape.py` & `ogl-2.1.5/src/miniogl/TextShape.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/TextShapeModel.py` & `ogl-2.1.5/src/miniogl/TextShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/miniogl/VShapes.py` & `ogl-2.1.5/src/miniogl/VShapes.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/EventEngineMixin.py` & `ogl-2.1.5/src/ogl/EventEngineMixin.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/OglActor.py` & `ogl-2.1.5/src/ogl/OglActor.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/OglAggregation.py` & `ogl-2.1.5/src/ogl/OglAggregation.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/OglAssociation.py` & `ogl-2.1.5/src/ogl/OglAssociation.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from wx import FONTWEIGHT_NORMAL
 from wx import WHITE_BRUSH
 
 from wx import Font
 
 from pyutmodelv2.PyutLink import PyutLink
 
+from miniogl.Diagram import Diagram
 from miniogl.LineShape import Segments
 
 from ogl.OglAssociationLabel import OglAssociationLabel
 from ogl.OglLink import OglLink
 from ogl.OglPosition import OglPosition
 
 from ogl.preferences.OglPreferences import OglPreferences
@@ -57,42 +58,43 @@
     def __init__(self, srcShape, pyutLink, dstShape, srcPos=None, dstPos=None):
         """
 
         Args:
             srcShape:   Source shape
             pyutLink:   Conceptual links associated with the graphical links.
             dstShape:   Destination shape
-            srcPos:     Source position  Override location of input source
-            dstPos:     Destination position Override location of input destination
+            srcPos:     Position of source      Override location of input source
+            dstPos:     Position of destination Override location of input destination
         """
         self.oglAssociationLogger: Logger         = getLogger(__name__)
         self._preferences:         OglPreferences = OglPreferences()
 
         super().__init__(srcShape, pyutLink, dstShape, srcPos=srcPos, dstPos=dstPos)
 
         self._defaultFont: Font = Font(self._preferences.associationTextFontSize, FONTFAMILY_DEFAULT, FONTSTYLE_NORMAL, FONTWEIGHT_NORMAL)
 
         self._associationName:        OglAssociationLabel = cast(OglAssociationLabel, None)
         self._sourceCardinality:      OglAssociationLabel = cast(OglAssociationLabel, None)
         self._destinationCardinality: OglAssociationLabel = cast(OglAssociationLabel, None)
 
         self.SetDrawArrow(False)
+        self._labelsAdded: bool = False
 
     @property
     def pyutObject(self) -> PyutLink:
         """
         Override
         Returns:  The data model
         """
         return self._link
 
     @pyutObject.setter
     def pyutObject(self, pyutLink: PyutLink):
         """
-
+        Override in order to update the UI
         Args:
             pyutLink:
         """
         self.oglAssociationLogger.debug(f'{pyutLink=}')
         self._link = pyutLink
         self.centerLabel.text            = pyutLink.name
         self.sourceCardinality.text      = pyutLink.sourceCardinality
@@ -120,14 +122,31 @@
     def destinationCardinality(self) -> OglAssociationLabel:
         return self._destinationCardinality
 
     @destinationCardinality.setter
     def destinationCardinality(self, newValue: OglAssociationLabel):
         self._destinationCardinality = newValue
 
+    def addLabelsToDiagram(self):
+        """
+        This method should only be called once.   It should only
+        be called once the OglAssociation shape itself has been
+        added to the diagram
+        """
+        assert self._labelsAdded is False, 'Developer error:  Labels should only be added once'
+        diagram: Diagram = self._diagram
+        if self.centerLabel is not None:
+            diagram.AddShape(self.centerLabel, withModelUpdate=True)
+        if self._sourceCardinality is not None:
+            diagram.AddShape(self.sourceCardinality, withModelUpdate=True)
+        if self._destinationCardinality is not None:
+            diagram.AddShape(self._destinationCardinality, withModelUpdate=True)
+
+        self._labelsAdded = True
+
     def Draw(self, dc: DC, withChildren: bool = True):
         """
         Called to draw the link content.
         We are going to draw all of our stuff, cardinality, Link name, etc.
 
         Args:
             dc:     Device context
@@ -263,15 +282,15 @@
 
         oglAssociationLabel.draggable = True
         return oglAssociationLabel
 
     @staticmethod
     def calculateDiamondPoints(lineSegments: Segments) -> DiamondPoints:
         """
-        Made static so that we can unit test it;  Only instance variables needed
+        Made static so that we can unit test it;  Please the only instance variables needed
         are passed in
 
         Args:
             lineSegments:  The line where we are putting the diamondPoints
 
         Returns:  The diamond points that define the diamond polygon
         """
```

### Comparing `ogl-2.1.31/src/ogl/OglAssociationLabel.py` & `ogl-2.1.5/src/ogl/OglAssociationLabel.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/OglClass.py` & `ogl-2.1.5/src/ogl/OglClass.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,33 +26,27 @@
 from pyutmodelv2.PyutMethod import PyutMethod
 from pyutmodelv2.PyutObject import PyutObject
 from pyutmodelv2.PyutClass import PyutClass
 
 from miniogl.MiniOglColorEnum import MiniOglColorEnum
 from miniogl.SelectAnchorPoint import SelectAnchorPoint
 
-from ogl.OglDimensions import OglDimensions
 from ogl.OglObject import OglObject
 from ogl.OglObject import DEFAULT_FONT_SIZE
 
 from ogl.events.OglEvents import OglEventType
 
 from ogl.preferences.OglPreferences import OglPreferences
 
 from ogl.ui.OglClassMenuHandler import OglClassMenuHandler
 
 DUNDER_METHOD_INDICATOR: str = '__'
 CONSTRUCTOR_NAME:        str = '__init__'
 
 MARGIN: int = 10
-#
-#  When I added optional display of constructor and dunder methods, I introduced this bug
-#  I'll fix this later
-#
-HACK_FIX_AUTO_RESIZE: bool = True   # TODO:  This should be a debug flag
 
 
 @dataclass
 class ClickedOnSelectAnchorPointData:
     clicked:           bool             = False
     selectAnchorPoint: SelectAnchorPoint = cast(SelectAnchorPoint, None)
 
@@ -60,15 +54,15 @@
 class OglClass(OglObject):
     """
     OGL object that represents a modeling class in class diagrams.
     This Python class defines a graphical object that represents a specific UML class.
     You instantiate an OGL class and add it to the diagram.
     Links, resizing, are managed by parent class `OglObject`.
 
-    For more instructions about how to create an OGL object, refer
+    For more instructions about how to create an OGL object, please refer
     to the `OglObject` class.
     """
     def __init__(self, pyutClass: PyutClass | None, w: int = 0, h: int = 0):
         """
 
         Args:
             pyutClass: a PyutClass object
@@ -202,32 +196,21 @@
             y = methodY + methodH
         else:
             methodW, methodH = 0, 0
 
         w = max(headerW, fieldsW, methodW)
         h = y - headerY
         w += 2 * MARGIN
-
-        minDimensions: OglDimensions = self._oglPreferences.classDimensions
-        if w < minDimensions.width:
-            w = minDimensions.width
-        if h < minDimensions.height:
-            h = minDimensions.height
-
-        if HACK_FIX_AUTO_RESIZE is True:
-            w = w - 20      # Hack keeps growing
         self.SetSize(w, h)
 
         # to automatically replace the sizer objects at a correct place
         if self.selected is True:
             self.selected = False
             self.selected = True
 
-        self.eventEngine.sendEvent(OglEventType.DiagramFrameModified)
-
     def OnRightDown(self, event: MouseEvent):
         """
         Callback for right clicks
         """
         if self._menuHandler is None:
             self._menuHandler = OglClassMenuHandler(oglClass=self, eventEngine=self.eventEngine)
 
@@ -287,15 +270,15 @@
             calcWidth:
 
         Returns: tuple (x, y, w, h) = position and size of the header
         """
         # Init
         dc.SetFont(self._defaultFont)
         dc.SetTextForeground(self._textColor)
-
+        # pyutObject = self.getPyutObject()
         x, y = self.GetPosition()
         if initialX is not None:
             x = initialX
         if initialY is not None:
             y = initialY
         w = self._width
         h = 0
```

### Comparing `ogl-2.1.31/src/ogl/OglComposition.py` & `ogl-2.1.5/src/ogl/OglComposition.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/OglConstants.py` & `ogl-2.1.5/src/ogl/OglConstants.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/OglDimensions.py` & `ogl-2.1.5/src/ogl/OglDimensions.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/OglInheritance.py` & `ogl-2.1.5/src/ogl/OglInheritance.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/OglInterface.py` & `ogl-2.1.5/src/ogl/OglInterface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 
 from logging import Logger
 from logging import getLogger
 
-from deprecated import deprecated
-
 from wx import DC
 from wx import Pen
 
 from wx import PENSTYLE_SHORT_DASH
 from wx import PENSTYLE_LONG_DASH
 from wx import RED_PEN
 from wx import BLACK_PEN
@@ -16,23 +14,27 @@
 from pyutmodelv2.PyutLink import PyutLink
 
 from miniogl.TextShape import TextShape
 
 from ogl.OglLink import OglLink
 from ogl.OglClass import OglClass
 
+# Kind of labels
+[CENTER] = list(range(1))
+
 
 class OglInterface(OglLink):
+
+    clsLogger: Logger = getLogger(__name__)
+
     """
     Graphical OGL representation of an interface link.
     This class provide the methods for drawing an interface link between
     two classes of an UML diagram. Add labels to an OglLink.
     """
-    clsLogger: Logger = getLogger(__name__)
-
     def __init__(self, srcShape: OglClass, pyutLink: PyutLink, dstShape: OglClass, srcPos=None, dstPos=None):
 
         """
 
         Args:
             srcShape:  Source shape
             pyutLink:  Conceptual links associated with the graphical links.
@@ -41,25 +43,20 @@
             dstPos:    Position of destination Override location of input destination
 
         """
         super().__init__(srcShape, pyutLink, dstShape, srcPos=srcPos, dstPos=dstPos)
 
         self.SetPen(Pen("BLACK", 1, PENSTYLE_LONG_DASH))
         self.SetBrush(WHITE_BRUSH)
-
-        self._label: TextShape = self.AddText(0, 0, "")
+        self._labels = {CENTER: self.AddText(0, 0, "")}
 
         # Initialize labels objects
         self.updateLabels()
         self.SetDrawArrow(True)
 
-    @property
-    def label(self) -> TextShape:
-        return self._label
-
     def updateLabels(self):
         """
         Update the labels according to the link.
         """
         def prepareLabel(textShape: TextShape, text):
             # If label should be drawn
             if text.strip() != "":
@@ -68,23 +65,26 @@
                 # textShape.Show(True)
                 textShape.SetVisible(True)
             else:
                 # textShape.Show(False)
                 textShape.SetVisible(False)
 
         # Prepares labels
-        prepareLabel(self._label, self._link.name)
+        prepareLabel(self._labels[CENTER], self._link.name)
 
-    @deprecated(reason='Use property .label')
     def getLabels(self):
         """
+        Get the labels.
+
+        @return TextShape []
+        @since 1.0
         """
-        return self._label
+        return self._labels
 
-    def Draw(self, dc: DC, withChildren: bool = True):
+    def Draw(self, dc: DC, withChildren: bool = False):
         """
         Called for drawing of interface links.
         OglLink drew regular lines
         I need dashed lines for an interface
 
         Args:
             dc: Device context
```

### Comparing `ogl-2.1.31/src/ogl/OglInterface2.py` & `ogl-2.1.5/src/ogl/OglInterface2.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/OglLink.py` & `ogl-2.1.5/src/ogl/OglLink.py`

 * *Files 1% similar despite different names*

```diff
@@ -434,15 +434,15 @@
         dstId:    int   = dstShape.id
 
         return f'from: id: {sourceId} {srcShape} to id: {dstId} {dstShape}'
 
     def _avoidCrossedLines(self, dstShape, dstX: int, dstY: int, orient, srcShape, srcX: int, srcY: int):
         """
         Avoid over-lining
-        Added by: C. Dutoit (still experimental in 2024
+        Added by: C. Dutoit (still experimental in 2024 🤪)
 
         Args:
             dstShape:
             dstX:
             dstY:
             orient:
             srcShape:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ogl-2.1.31/src/ogl/OglLinkFactory.py` & `ogl-2.1.5/src/ogl/OglLinkFactory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 
-from typing import cast
-
 from logging import Logger
 from logging import getLogger
 
 from codeallybasic.SingletonV3 import SingletonV3
 
 from pyutmodelv2.enumerations.PyutLinkType import PyutLinkType
 
@@ -25,35 +23,32 @@
     return OglLinkFactory()
 
 
 def getLinkType(link: OglAssociation) -> PyutLinkType:
     """
 
     Args:
-        link:   The OglLink object
+        link:   The enumeration OglLinkType
 
     Returns:  The OglLinkType
 
     """
-    match link:
-        case OglAggregation():
-            return PyutLinkType.AGGREGATION
-        case OglComposition():
-            return PyutLinkType.COMPOSITION
-        case OglInheritance():
-            return PyutLinkType.INHERITANCE
-        case OglAssociation():
-            return PyutLinkType.ASSOCIATION
-        case OglInterface():
-            return PyutLinkType.INTERFACE
-        case OglNoteLink():
-            return PyutLinkType.NOTELINK
-        case _:
-            print(f"Unknown OglLink: {link}")
-            return cast(PyutLinkType, None)
+
+    if isinstance(link, OglAggregation):
+        return PyutLinkType.AGGREGATION
+    elif isinstance(link, OglComposition):
+        return PyutLinkType.COMPOSITION
+    elif isinstance(link, OglInheritance):
+        return PyutLinkType.INHERITANCE
+    elif isinstance(link, OglAssociation):
+        return PyutLinkType.ASSOCIATION
+    elif isinstance(link, OglInterface):
+        return PyutLinkType.INTERFACE
+    elif isinstance(link, OglNoteLink):
+        return PyutLinkType.NOTELINK
 
 
 class OglLinkFactory(metaclass=SingletonV3):
     """
     This class is a factory to produce `OglLink` objects.
     It works under the Factory Design Pattern model. Ask for a link
     from this object, and it will return an instance of request link.
@@ -70,37 +65,30 @@
             srcShape:   Source shape
             pyutLink:   Conceptual links associated with the graphical links.
             destShape:  Destination shape
             linkType:   The linkType of the link (OGL_INHERITANCE, ...)
 
         Returns:  The requested link
         """
-        match linkType:
-            case PyutLinkType.AGGREGATION:
-                oglAggregation: OglAggregation = OglAggregation(srcShape, pyutLink, destShape)
-                oglAggregation.createDefaultAssociationLabels()
-                return oglAggregation
-
-            case PyutLinkType.COMPOSITION:
-                oglComposition: OglComposition = OglComposition(srcShape, pyutLink, destShape)
-                oglComposition.createDefaultAssociationLabels()
-                return oglComposition
-
-            case PyutLinkType.INHERITANCE:
-                return OglInheritance(srcShape, pyutLink, destShape)
-
-            case PyutLinkType.ASSOCIATION:
-                oglAssociation: OglAssociation = OglAssociation(srcShape, pyutLink, destShape)
-                oglAssociation.createDefaultAssociationLabels()
-                return oglAssociation
-
-            case PyutLinkType.INTERFACE:
-                return OglInterface(srcShape, pyutLink, destShape)
-
-            case PyutLinkType.NOTELINK:
-                return OglNoteLink(srcShape, pyutLink, destShape)
-
-            case PyutLinkType.SD_MESSAGE:
-                return OglSDMessage(srcSDInstance=srcShape, pyutSDMessage=pyutLink, dstSDInstance=destShape)
-            case _:
-                self.logger.error(f"Unknown PyutLinkType: {linkType}")
-                return None
+        if linkType == PyutLinkType.AGGREGATION:
+            return OglAggregation(srcShape, pyutLink, destShape)
+
+        elif linkType == PyutLinkType.COMPOSITION:
+            return OglComposition(srcShape, pyutLink, destShape)
+
+        elif linkType == PyutLinkType.INHERITANCE:
+            return OglInheritance(srcShape, pyutLink, destShape)
+
+        elif linkType == PyutLinkType.ASSOCIATION:
+            return OglAssociation(srcShape, pyutLink, destShape)
+
+        elif linkType == PyutLinkType.INTERFACE:
+            return OglInterface(srcShape, pyutLink, destShape)
+
+        elif linkType == PyutLinkType.NOTELINK:
+            return OglNoteLink(srcShape, pyutLink, destShape)
+
+        elif linkType == PyutLinkType.SD_MESSAGE:
+            return OglSDMessage(srcSDInstance=srcShape, pyutSDMessage=pyutLink, dstSDInstance=destShape)
+        else:
+            self.logger.error(f"Unknown OglLinkType: {linkType}")
+            return None
```

### Comparing `ogl-2.1.31/src/ogl/OglNote.py` & `ogl-2.1.5/src/ogl/OglNote.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/OglNoteLink.py` & `ogl-2.1.5/src/ogl/OglNoteLink.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/OglObject.py` & `ogl-2.1.5/src/ogl/OglObject.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/OglText.py` & `ogl-2.1.5/src/ogl/OglText.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/OglUseCase.py` & `ogl-2.1.5/src/ogl/OglUseCase.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/OglUtils.py` & `ogl-2.1.5/src/ogl/OglUtils.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/events/IOglEventEngine.py` & `ogl-2.1.5/src/ogl/events/IOglEventEngine.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/events/OglEventEngine.py` & `ogl-2.1.5/src/ogl/events/OglEventEngine.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/events/OglEvents.py` & `ogl-2.1.5/src/ogl/events/OglEvents.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from enum import Enum
 
 from wx.lib.newevent import NewEvent
 
 #
-# The constructor returns a tuple; The first entry is the event,  The second is the binder
+# Constructor returns a tuple; First is the event,  The second is the binder
 #
 ShapeSelectedEvent,        EVT_SHAPE_SELECTED         = NewEvent()
 CutOglClassEvent,          EVT_CUT_OGL_CLASS          = NewEvent()
 DiagramFrameModifiedEvent, EVT_DIAGRAM_FRAME_MODIFIED = NewEvent()
 
 RequestLollipopLocationEvent, EVT_REQUEST_LOLLIPOP_LOCATION = NewEvent()
 CreateLollipopInterfaceEvent, EVT_CREATE_LOLLIPOP_INTERFACE = NewEvent()
```

### Comparing `ogl-2.1.31/src/ogl/preferences/OglPreferences.py` & `ogl-2.1.5/src/ogl/preferences/OglPreferences.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/resources/img/Display.py` & `ogl-2.1.5/src/ogl/resources/img/Display.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/resources/img/DoNotDisplay.py` & `ogl-2.1.5/src/ogl/resources/img/DoNotDisplay.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/resources/img/UnSpecified.py` & `ogl-2.1.5/src/ogl/resources/img/UnSpecified.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/resources/img/textdetails/DecreaseTextSize.py` & `ogl-2.1.5/src/ogl/resources/img/textdetails/DecreaseTextSize.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/resources/img/textdetails/IncreaseTextSize.py` & `ogl-2.1.5/src/ogl/resources/img/textdetails/IncreaseTextSize.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/sd/OglInstanceName.py` & `ogl-2.1.5/src/ogl/sd/OglInstanceName.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/sd/OglSDInstance.py` & `ogl-2.1.5/src/ogl/sd/OglSDInstance.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/sd/OglSDMessage.py` & `ogl-2.1.5/src/ogl/sd/OglSDMessage.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/ui/BaseOglPreferencesPage.py` & `ogl-2.1.5/src/ogl/ui/BaseOglPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/ui/DefaultValuesPreferencesPage.py` & `ogl-2.1.5/src/ogl/ui/DefaultValuesPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/ui/DiagramPreferencesPage.py` & `ogl-2.1.5/src/ogl/ui/DiagramPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/ui/OglClassMenuHandler.py` & `ogl-2.1.5/src/ogl/ui/OglClassMenuHandler.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/ui/valuecontrols/AssociationAttributesControl.py` & `ogl-2.1.5/src/ogl/ui/valuecontrols/AssociationAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/ui/valuecontrols/ClassAttributesControl.py` & `ogl-2.1.5/src/ogl/ui/valuecontrols/ClassAttributesControl.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         self._displayConstructor   = CheckBox(parent=methodDisplayPanel, label='Display Constructor')
 
     def _setControlValues(self):
         """
         """
         self._classDimensions.dimensions = self._preferences.classDimensions
 
-        oglColors:      List[str] = self._classBackgroundColor.GetItems()
+        oglColors: List[str] = self._classBackgroundColor.GetItems()
         bgColorSelIdx:  int       = oglColors.index(self._preferences.classBackgroundColor.value)
         self._classBackgroundColor.SetSelection(bgColorSelIdx)
 
         txtColorSelIdx: int = oglColors.index(self._preferences.classTextColor.value)
         self._classTextColor.SetSelection(txtColorSelIdx)
 
         self._displayDunderMethods.SetValue(self._preferences.displayDunderMethods)
```

### Comparing `ogl-2.1.31/src/ogl/ui/valuecontrols/DefaultNamesControl.py` & `ogl-2.1.5/src/ogl/ui/valuecontrols/DefaultNamesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/ui/valuecontrols/NoteAttributesControl.py` & `ogl-2.1.5/src/ogl/ui/valuecontrols/NoteAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/ui/valuecontrols/SDAttributesControl.py` & `ogl-2.1.5/src/ogl/ui/valuecontrols/SDAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl/ui/valuecontrols/TextAttributesControl.py` & `ogl-2.1.5/src/ogl/ui/valuecontrols/TextAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-2.1.31/src/ogl.egg-info/PKG-INFO` & `ogl-2.1.5/src/ogl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ogl
-Version: 2.1.31
+Version: 2.1.5
 Summary: External Pyut Graphical Shapes
 Author-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 Maintainer-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Project-URL: Repository, https://github.com/hasii2011/ogl
 Keywords: pyut,graphical shapes,python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wxPython~=4.2.1
-Requires-Dist: codeallybasic>=1.3.0
-Requires-Dist: codeallyadvanced>=1.3.1
-Requires-Dist: pyutmodelv2>=2.1.5
+Requires-Dist: codeallybasic>=1.1.0
+Requires-Dist: codeallyadvanced>=1.1.0
+Requires-Dist: pyutmodelv2==2.1.0
 
 ![](https://github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-badge-version-2-256x48.png "AGPL")
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/ogl/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/ogl/tree/master)
 [![PyPI version](https://badge.fury.io/py/ogl.svg)](https://badge.fury.io/py/ogl)
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: ogl Version: 2.1.31 Summary: External Pyut
-Graphical Shapes Author-email: "Humberto A. Sanchez II"
+Metadata-Version: 2.1 Name: ogl Version: 2.1.5 Summary: External Pyut Graphical
+Shapes Author-email: "Humberto A. Sanchez II"
 gmail.com> Maintainer-email: "Humberto A. Sanchez II"
 gmail.com> License: GNU AFFERO GENERAL PUBLIC LICENSE Project-URL: Repository,
 https://github.com/hasii2011/ogl Keywords: pyut,graphical shapes,python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-wxPython~=4.2.1 Requires-Dist: codeallybasic>=1.3.0 Requires-Dist:
-codeallyadvanced>=1.3.1 Requires-Dist: pyutmodelv2>=2.1.5 ![](https://
+wxPython~=4.2.1 Requires-Dist: codeallybasic>=1.1.0 Requires-Dist:
+codeallyadvanced>=1.1.0 Requires-Dist: pyutmodelv2==2.1.0 ![](https://
 github.com/hasii2011/code-ally-basic/blob/master/developer/agpl-license-web-
 badge-version-2-256x48.png "AGPL") [![Maintenance](https://img.shields.io/
 badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/
 graphs/commit-activity) [![CircleCI](https://dl.circleci.com/status-badge/img/
 gh/hasii2011/ogl/tree/master.svg?style=shield)](https://dl.circleci.com/status-
 badge/redirect/gh/hasii2011/ogl/tree/master) [![PyPI version](https://
 badge.fury.io/py/ogl.svg)](https://badge.fury.io/py/ogl) ð ð¨ ð¤ ð£
```

### Comparing `ogl-2.1.31/src/ogl.egg-info/SOURCES.txt` & `ogl-2.1.5/src/ogl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

