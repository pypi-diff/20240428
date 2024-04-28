# Comparing `tmp/indipyclient-0.0.8.tar.gz` & `tmp/indipyclient-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipyclient-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipyclient-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipyclient-0.0.8.tar` & `indipyclient-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.0.8/LICENSE
--rw-r--r--   0        0        0     2646 2024-04-13 20:38:26.000000 indipyclient-0.0.8/README.md
--rw-r--r--   0        0        0      291 2024-04-27 09:31:27.000000 indipyclient-0.0.8/indipyclient/__init__.py
--rw-r--r--   0        0        0     3089 2024-04-03 21:43:04.000000 indipyclient-0.0.8/indipyclient/__main__.py
--rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.0.8/indipyclient/console/__init__.py
--rw-r--r--   0        0        0    19759 2024-04-04 21:35:51.000000 indipyclient-0.0.8/indipyclient/console/consoleclient.py
--rw-r--r--   0        0        0    48364 2024-04-05 12:12:41.000000 indipyclient-0.0.8/indipyclient/console/widgets.py
--rw-r--r--   0        0        0   144085 2024-04-25 16:29:53.000000 indipyclient-0.0.8/indipyclient/console/windows.py
--rw-r--r--   0        0        0      192 2023-09-20 21:15:05.000000 indipyclient-0.0.8/indipyclient/error.py
--rw-r--r--   0        0        0    25043 2024-04-26 19:21:44.000000 indipyclient-0.0.8/indipyclient/events.py
--rw-r--r--   0        0        0    34733 2024-04-27 09:30:24.000000 indipyclient-0.0.8/indipyclient/ipyclient.py
--rw-r--r--   0        0        0    16066 2024-04-27 09:28:41.000000 indipyclient-0.0.8/indipyclient/propertymembers.py
--rw-r--r--   0        0        0    27590 2024-04-13 18:00:12.000000 indipyclient-0.0.8/indipyclient/propertyvectors.py
--rw-r--r--   0        0        0      935 2024-04-27 09:31:13.000000 indipyclient-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 indipyclient-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2646 2024-04-13 20:38:26.000000 indipyclient-0.0.9/README.md
+-rw-r--r--   0        0        0      330 2024-04-28 19:27:59.000000 indipyclient-0.0.9/indipyclient/__init__.py
+-rw-r--r--   0        0        0     3089 2024-04-03 21:43:04.000000 indipyclient-0.0.9/indipyclient/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.0.9/indipyclient/console/__init__.py
+-rw-r--r--   0        0        0    19759 2024-04-28 18:10:23.000000 indipyclient-0.0.9/indipyclient/console/consoleclient.py
+-rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.0.9/indipyclient/console/widgets.py
+-rw-r--r--   0        0        0   144085 2024-04-28 18:17:36.000000 indipyclient-0.0.9/indipyclient/console/windows.py
+-rw-r--r--   0        0        0      192 2023-09-20 21:15:05.000000 indipyclient-0.0.9/indipyclient/error.py
+-rw-r--r--   0        0        0    26765 2024-04-28 19:07:19.000000 indipyclient-0.0.9/indipyclient/events.py
+-rw-r--r--   0        0        0    34733 2024-04-28 18:01:26.000000 indipyclient-0.0.9/indipyclient/ipyclient.py
+-rw-r--r--   0        0        0    16189 2024-04-28 19:10:31.000000 indipyclient-0.0.9/indipyclient/propertymembers.py
+-rw-r--r--   0        0        0    27645 2024-04-28 18:21:13.000000 indipyclient-0.0.9/indipyclient/propertyvectors.py
+-rw-r--r--   0        0        0      935 2024-04-28 19:27:49.000000 indipyclient-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 indipyclient-0.0.9/PKG-INFO
```

### Comparing `indipyclient-0.0.8/LICENSE` & `indipyclient-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.8/README.md` & `indipyclient-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.8/indipyclient/__main__.py` & `indipyclient-0.0.9/indipyclient/__main__.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.8/indipyclient/console/consoleclient.py` & `indipyclient-0.0.9/indipyclient/console/consoleclient.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.8/indipyclient/console/widgets.py` & `indipyclient-0.0.9/indipyclient/console/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 
 import asyncio, curses, sys, pathlib, time
 
 from decimal import Decimal
 
 from curses import ascii
 
+from ..propertymembers import getfloat
+
 def shorten(text, width=0, placeholder="..."):
     "Shorten text"
     txt = text.replace("\n", " ")
     if not width:
         return txt
     if len(txt)<=width:
         return txt
@@ -856,33 +858,33 @@
             curses.doupdate()
         curses.curs_set(0)
 
     def checknumber(self):
         "set self._newvalue, limiting it to correct range"
         # self._newvalue is the new value input
         try:
-            newfloat = self.member.getfloat(self._newvalue)
+            newfloat = getfloat(self._newvalue)
         except (ValueError, TypeError):
             # reset self._newvalue
             self._newvalue = self.member.getformattedvalue()
             return
         # check step, and round newfloat to nearest step value
-        stepvalue = self.member.getfloat(self.member.step)
-        minvalue = self.member.getfloat(self.member.min)
+        stepvalue = getfloat(self.member.step)
+        minvalue = getfloat(self.member.min)
         if stepvalue:
             stepvalue = Decimal(str(stepvalue))
             difference = newfloat - minvalue
             newfloat = minvalue + float(int(Decimal(str(difference)) / stepvalue) * stepvalue)
         # check not less than minimum
         if newfloat < minvalue:
             # reset self._newvalue to be the minimum, and accept this
             self._newvalue = self.member.getformattedstring(minvalue)
             return
         if self.member.max != self.member.min:
-            maxvalue = self.member.getfloat(self.member.max)
+            maxvalue = getfloat(self.member.max)
             if newfloat > maxvalue:
                 # reset self._newvalue to be the maximum, and accept this
                 self._newvalue = self.member.getformattedstring(maxvalue)
                 return
         # reset self._newvalue to the correct format, and accept this
         self._newvalue = self.member.getformattedstring(newfloat)
```

### Comparing `indipyclient-0.0.8/indipyclient/console/windows.py` & `indipyclient-0.0.9/indipyclient/console/windows.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.8/indipyclient/events.py` & `indipyclient-0.0.9/indipyclient/events.py`

 * *Files 5% similar despite different names*

```diff
@@ -347,27 +347,27 @@
         # create object dictionary of member name to value
         # and another dictionary of self.memberlabels with key member name and value being label
         self.memberlabels = {}
         for member in root:
             if member.tag == "defLight":
                 membername = member.get("name")
                 if not membername:
-                    raise ParseException
+                    raise ParseException("No name given in defLight")
                 label = member.get("label", membername)
                 self.memberlabels[membername] = label
                 if not member.text:
-                    raise ParseException
+                    raise ParseException("No value given in defLight")
                 value = member.text.strip()
                 if not value in ('Idle','Ok','Busy','Alert'):
-                    raise ParseException
+                    raise ParseException("Invalid value given in defLight")
                 self.data[membername] = value
             else:
-                raise ParseException
+                raise ParseException("No members of defLight present")
         if not self.data:
-            raise ParseException
+            raise ParseException("No member values present")
 
 
         # properties is a dictionary of property name to propertyvector this device owns
         # This method updates a property vector and sets it into properties
         properties = device.data
 
         # does this vector already exist
@@ -391,53 +391,53 @@
        However this class does not have an object mapping of member name to value, since
        values are not given in defBLOBVectors"""
 
     def __init__(self, root, device, client):
         Event.__init__(self, root, device, client)
         self.eventtype = "DefineBLOB"
         if self.devicename is None:
-            raise ParseException
+            raise ParseException("No device name given in defBLOBVector")
         self.vectorname = root.get("name")
         if self.vectorname is None:
-            raise ParseException
+            raise ParseException("No vector name given in defBLOBVector")
         self.label = root.get("label", self.vectorname)
         self.group = root.get("group", "DEFAULT GROUP")
         state = root.get("state")
         if not state:
-            raise ParseException
+            raise ParseException("No state given in defBLOBVector")
         if not state in ('Idle','Ok','Busy','Alert'):
-            raise ParseException
+            raise ParseException("Invalid state given in defBLOBVector")
         self.state = state
         self.message = root.get("message", "")
         self.perm = root.get("perm")
         if self.perm is None:
-            raise ParseException
+            raise ParseException("No perm given in defBLOBVector")
         if self.perm not in ('ro', 'wo', 'rw'):
-            raise ParseException
+            raise ParseException("Invalid perm given in defBLOBVector")
         try:
             timeout = root.get("timeout")
             if not self.timeout:
                 self.timeout = 0.0
             else:
                 self.timeout = float(timeout)
         except:
             self.timeout = 0.0
         # create a dictionary of self.memberlabels with key member name and value being label
         self.memberlabels = {}
         for member in root:
             if member.tag == "defBLOB":
                 membername = member.get("name")
                 if not membername:
-                    raise ParseException
+                    raise ParseException("Missing member name in defBLOB")
                 label = member.get("label", membername)
                 self.memberlabels[membername] = label
             else:
                 raise ParseException(f"Invalid child tag {member.tag} of defBLOBVector received")
         if not self.memberlabels:
-            raise ParseException
+            raise ParseException("No labels given in defBLOBVector")
 
         # properties is a dictionary of property name to propertyvector this device owns
         # This method updates a property vector and sets it into properties
         properties = device.data
 
         # does this vector already exist
         if self.vectorname in properties:
@@ -455,26 +455,26 @@
 class setVector(Event, UserDict):
     "Parent to set vectors, adds dictionary"
     def __init__(self, root, device, client):
         Event.__init__(self, root, device, client)
         UserDict.__init__(self)
         self.eventtype = "Set"
         if self.devicename is None:
-            raise ParseException
+            raise ParseException("Missing device name in set vector")
         self.vectorname = root.get("name")
         if self.vectorname is None:
-            raise ParseException
+            raise ParseException("Missing vector name in set vector")
         # This vector must already exist, and be enabled
         self.timeout = None
         if self.vectorname in self.device:
             vector = self.device[self.vectorname]
             if not vector.enable:
-                raise ParseException
+                raise ParseException("Set vector ignored as vector deleted")
         else:
-            raise ParseException
+            raise ParseException("Set vector ignored as vector is unknown")
         state = root.get("state")
         if state and (state in ('Idle','Ok','Busy','Alert')):
             self.state = state
         else:
             self.state = None
         self.message = root.get("message", "")
 
@@ -497,26 +497,26 @@
             # dont update
             pass
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneSwitch":
                 membername = member.get("name")
                 if not membername:
-                    raise ParseException
+                    raise ParseException("Missing name in oneSwitch")
                 if not member.text:
-                    raise ParseException
+                    raise ParseException("Missing value in oneSwitch")
                 value = member.text.strip()
                 if value == "On":
                     self.data[membername] = "On"
                 elif value == "Off":
                     self.data[membername] = "Off"
                 else:
-                    raise ParseException
+                    raise ParseException("Invalid value in oneSwitch")
             else:
-                raise ParseException
+                raise ParseException("Invalid child tag of setSwitchVector")
         properties = device.data
         self.vector = properties[self.vectorname]
         # set changed values into self.vector
         self.vector._setvector(self)
 
 
 class setTextVector(setVector):
@@ -534,22 +534,22 @@
             # dont update
             pass
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneText":
                 membername = member.get("name")
                 if not membername:
-                    raise ParseException
+                    raise ParseException("Missing name in oneText")
                 if not member.text:
                     value = ""
                 else:
                     value = member.text.strip()
                 self.data[membername] = value
             else:
-                raise ParseException
+                raise ParseException("Invalid child tag of setTextVector")
         properties = device.data
         self.vector = properties[self.vectorname]
         # set changed values into self.vector
         self.vector._setvector(self)
 
 
 class setNumberVector(setVector):
@@ -568,20 +568,28 @@
             # dont update
             pass
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneNumber":
                 membername = member.get("name")
                 if not membername:
-                    raise ParseException
+                    raise ParseException("Missing name in oneNumber")
                 if not member.text:
-                    raise ParseException
-                self.data[membername] = member.text.strip()
+                    raise ParseException("Missing value in oneNumber")
+                membervalue = member.text.strip()
+                if not membervalue:
+                    raise ParseException("Missing value in oneNumber")
+                # test membervalue ok
+                try:
+                    memberfloat = propertymembers.getfloat(membervalue)
+                except TypeError:
+                    raise ParseException("Invalid number in setNumberVector")
+                self.data[membername] = membervalue
             else:
-                raise ParseException
+                raise ParseException("Invalid child tag of setNumberVector")
         properties = device.data
         self.vector = properties[self.vectorname]
         # set changed values into self.vector
         self.vector._setvector(self)
 
 
 class setLightVector(setVector):
@@ -593,23 +601,23 @@
     def __init__(self, root, device, client):
         setVector.__init__(self, root, device, client)
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneLight":
                 membername = member.get("name")
                 if not membername:
-                    raise ParseException
+                    raise ParseException("Missing name in oneLight")
                 if not member.text:
-                    raise ParseException
+                    raise ParseException("Missing value in oneLight")
                 value = member.text.strip()
                 if not value in ('Idle','Ok','Busy','Alert'):
-                    raise ParseException
+                    raise ParseException("Invalid value in oneLight")
                 self.data[membername] = value
             else:
-                raise ParseException
+                raise ParseException("Invalid child tag of setLightVector")
         properties = device.data
         self.vector = properties[self.vectorname]
         # set changed values into self.vector
         self.vector._setvector(self)
 
 
 class setBLOBVector(setVector):
@@ -636,27 +644,30 @@
         # and dictionary sizeformat
         # with key member name and value being a tuple of size, format
         self.sizeformat = {}
         for member in root:
             if member.tag == "oneBLOB":
                 membername = member.get("name")
                 if not membername:
-                    raise ParseException
+                    raise ParseException("Missing name in oneBLOB")
                 membersize = member.get("size")
                 if not membersize:
-                    raise ParseException
+                    raise ParseException("Missing size in oneBLOB")
+                try:
+                    memberize = int(membersize)
+                except:
+                    raise ParseException("Invalid size in oneBLOB")
                 memberformat = member.get("format")
                 if not memberformat:
-                    raise ParseException
+                    raise ParseException("Missing format in oneBLOB")
                 if not member.text:
-                    raise ParseException
+                    raise ParseException("Missing value in oneBLOB")
                 try:
                     self.data[membername] = standard_b64decode(member.text.encode('ascii'))
-                    memberize = int(membersize)
                 except:
-                    raise ParseException
+                    raise ParseException("Unable to decode oneBLOB contents")
                 self.sizeformat[membername] = (membersize, memberformat)
             else:
-                raise ParseException
+                raise ParseException("Invalid child tag of setBLOBVector")
         self.vector = device[self.vectorname]
         # set changed values into self.vector
         self.vector._setvector(self)
```

### Comparing `indipyclient-0.0.8/indipyclient/ipyclient.py` & `indipyclient-0.0.9/indipyclient/ipyclient.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.8/indipyclient/propertymembers.py` & `indipyclient-0.0.9/indipyclient/propertymembers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,61 @@
 import xml.etree.ElementTree as ET
 
 import sys, pathlib
 
 from .error import ParseException
 
 
+def getfloat(value):
+    """The INDI spec allows a number of different number formats, given a number,
+       this returns a float.
+       If an error occurs while parsing the number, a TypeError exception is raised."""
+    try:
+        if isinstance(value, float):
+            return value
+        if isinstance(value, int):
+            return float(value)
+        if not isinstance(value, str):
+            raise TypeError
+        # negative is True, if the value is negative
+        value = value.strip()
+        negative = value.startswith("-")
+        if negative:
+            value = value.lstrip("-")
+        # Is the number provided in sexagesimal form?
+        if value == "":
+            parts = ["0", "0", "0"]
+        elif " " in value:
+            parts = value.split(" ")
+        elif ":" in value:
+            parts = value.split(":")
+        elif ";" in value:
+            parts = value.split(";")
+        else:
+            # not sexagesimal
+            parts = [value, "0", "0"]
+        if len(parts) > 3:
+            raise TypeError
+        # Any missing parts should have zero
+        if len(parts) == 1:
+            parts.append("0")
+            parts.append("0")
+        if len(parts) == 2:
+            parts.append("0")
+        assert len(parts) == 3
+        # a part could be empty string, ie if 2:5: is given
+        numbers = list(float(x) if x else 0.0 for x in parts)
+        floatvalue = numbers[0] + (numbers[1]/60) + (numbers[2]/3600)
+        if negative:
+            floatvalue = -1 * floatvalue
+    except:
+        raise TypeError("Unable to parse number value")
+    return floatvalue
+
+
 class Member():
 
     """This class is the parent of further member classes.
        Should you use the ipyclient.snapshot method to create a snapshot,
        the snapshot vectors for Switch, Light and Text will contain objects
        of this Member class."""
 
@@ -140,77 +187,37 @@
     def __init__(self, name, label=None, format='', min='0', max='0', step='0', membervalue='0'):
         super().__init__(name, label, membervalue)
         self.format = format
         self.min = min
         self.max = max
         self.step = step
 
-    def getfloatvalue(self):
+    def getfloat(self, value):
         """The INDI spec allows a number of different number formats, this method returns
-           this members value as a float.
+           the given value as a float.
            If an error occurs while parsing the number, a TypeError exception is raised."""
-        return self.getfloat(self._membervalue)
+        return getfloat(value)
 
 
-    def getfloat(self, value):
-        """The INDI spec allows a number of different number formats, given a number,
-           this returns a float.
+    def getfloatvalue(self):
+        """The INDI spec allows a number of different number formats, this method returns
+           this members value as a float.
            If an error occurs while parsing the number, a TypeError exception is raised."""
-        try:
-            if isinstance(value, float):
-                return value
-            if isinstance(value, int):
-                return float(value)
-            if not isinstance(value, str):
-                raise TypeError
-            # negative is True, if the value is negative
-            value = value.strip()
-            negative = value.startswith("-")
-            if negative:
-                value = value.lstrip("-")
-            # Is the number provided in sexagesimal form?
-            if value == "":
-                parts = ["0", "0", "0"]
-            elif " " in value:
-                parts = value.split(" ")
-            elif ":" in value:
-                parts = value.split(":")
-            elif ";" in value:
-                parts = value.split(";")
-            else:
-                # not sexagesimal
-                parts = [value, "0", "0"]
-            if len(parts) > 3:
-                raise TypeError
-            # Any missing parts should have zero
-            if len(parts) == 1:
-                parts.append("0")
-                parts.append("0")
-            if len(parts) == 2:
-                parts.append("0")
-            assert len(parts) == 3
-            # a part could be empty string, ie if 2:5: is given
-            numbers = list(float(x) if x else 0.0 for x in parts)
-            floatvalue = numbers[0] + (numbers[1]/60) + (numbers[2]/3600)
-            if negative:
-                floatvalue = -1 * floatvalue
-        except:
-            raise TypeError("Unable to parse number value")
-        return floatvalue
+        return getfloat(self._membervalue)
 
 
     def getformattedvalue(self):
         """This method returns this members value as a formatted string."""
         return self.getformattedstring(self._membervalue)
 
 
     def getformattedstring(self, value):
         """Given a number this returns a formatted string"""
         try:
-            value = self.getfloat(value)
+            value = getfloat(value)
             if (not self.format.startswith("%")) or (not self.format.endswith("m")):
                 return self.format % value
             # sexagesimal
             # format string is of the form  %<w>.<f>m
             w,f = self.format.split(".")
             w = w.lstrip("%")
             f = f.rstrip("m")
@@ -316,17 +323,17 @@
         if not isinstance(step, str):
             raise ParseException("Number step value must be given as a string")
         self.step = step
         if not isinstance(membervalue, str):
             raise ParseException("Number value must be given as a string")
         try:
             # test a float can be created from this membervalue
-            self._floatvalue = self.getfloat(membervalue)
+            self._floatvalue = getfloat(membervalue)
         except:
-            raise ParseException("Cannot parse the number")
+            raise ParseException("Cannot parse number received.")
 
     @property
     def membervalue(self):
         return self._membervalue
 
     @membervalue.setter
     def membervalue(self, value):
@@ -334,17 +341,18 @@
             return
         if not isinstance(value, str):
             raise ParseException("Number value must be given as a string")
         if not value:
             raise ParseException("No number value given")
         try:
             # test a float can be created from this membervalue
-            self._floatvalue = self.getfloat(value)
+            # and save the float
+            self._floatvalue = getfloat(value)
         except:
-            raise ParseException("Cannot parse the number")
+            raise ParseException("Cannot parse number received")
         self._membervalue = value
 
 
     def getfloatvalue(self):
         """The INDI spec allows a number of different number formats, this method returns
            this members value as a float."""
         return self._floatvalue
```

### Comparing `indipyclient-0.0.8/indipyclient/propertyvectors.py` & `indipyclient-0.0.9/indipyclient/propertyvectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,14 @@
         raise KeyError
 
     def __getitem__(self, membername):
         return self.data[membername].membervalue
 
     def _setvector(self, event):
         "Updates this vector with new values after a set... vector has been received"
-        self._timer = False
         if not self.enable:
             # this property does not exist
             return
         if event.state:
             self.state = event.state
         if event.timestamp:
             self.timestamp = event.timestamp
@@ -158,14 +157,16 @@
         if hasattr(event, 'timeout'):
             if not self.timeout is None:
                 self.timeout = event.timeout
         for membername, membervalue in event.items():
             if membername in self.data:
                 member = self.data[membername]
                 member.membervalue = membervalue
+        # turn off timer if all updates are successful
+        self._timer = False
 
 
     def _snapshot(self):
         snapvector = Vector(self.name, self.label, self.group, self.state, self.timestamp, self.message)
         snapvector.vectortype = self.vectortype
         snapvector.devicename = self.devicename
         snapvector.enable = self.enable
```

### Comparing `indipyclient-0.0.8/pyproject.toml` & `indipyclient-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipyclient"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.0.8"
+version = "0.0.9"
 description="Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'client', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipyclient.readthedocs.io"
```

### Comparing `indipyclient-0.0.8/PKG-INFO` & `indipyclient-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipyclient
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

