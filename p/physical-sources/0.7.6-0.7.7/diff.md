# Comparing `tmp/physical_sources-0.7.6.tar.gz` & `tmp/physical_sources-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physical_sources-0.7.6.tar", last modified: Wed Jul 26 16:39:10 2023, max compression
+gzip compressed data, was "physical_sources-0.7.7.tar", last modified: Wed Jul 26 19:59:43 2023, max compression
```

## Comparing `physical_sources-0.7.6.tar` & `physical_sources-0.7.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 16:39:10.031713 physical_sources-0.7.6/
--rw-rw-rw-   0        0        0     1246 2023-07-11 17:45:55.000000 physical_sources-0.7.6/LICENSE.txt
--rw-rw-rw-   0        0        0     5896 2023-07-26 16:39:10.025713 physical_sources-0.7.6/PKG-INFO
--rw-rw-rw-   0        0        0     4416 2023-07-26 16:35:56.000000 physical_sources-0.7.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-26 16:39:10.032710 physical_sources-0.7.6/setup.cfg
--rw-rw-rw-   0        0        0     1018 2023-07-26 12:43:45.000000 physical_sources-0.7.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:39:09.863709 physical_sources-0.7.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 16:39:09.906710 physical_sources-0.7.6/src/physical_sources/
--rw-rw-rw-   0        0        0        0 2023-07-07 16:01:14.000000 physical_sources-0.7.6/src/physical_sources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:39:09.995713 physical_sources-0.7.6/src/physical_sources/acoustic/
--rw-rw-rw-   0        0        0      909 2023-07-26 15:15:47.000000 physical_sources-0.7.6/src/physical_sources/acoustic/INoiseSource.py
--rw-rw-rw-   0        0        0        0 2023-07-07 16:01:14.000000 physical_sources-0.7.6/src/physical_sources/acoustic/__init__.py
--rw-rw-rw-   0        0        0     4078 2023-07-26 15:15:48.000000 physical_sources-0.7.6/src/physical_sources/acoustic/analytic_source.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:39:10.019713 physical_sources-0.7.6/src/physical_sources/acoustic/line_source/
--rw-rw-rw-   0        0        0        0 2023-07-26 12:31:58.000000 physical_sources-0.7.6/src/physical_sources/acoustic/line_source/__init__.py
--rw-rw-rw-   0        0        0    22182 2023-07-26 15:41:18.000000 physical_sources-0.7.6/src/physical_sources/acoustic/point_source.py
--rw-rw-rw-   0        0        0    54940 2023-07-26 15:15:48.000000 physical_sources-0.7.6/src/physical_sources/acoustic/sphere_source.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:39:09.949710 physical_sources-0.7.6/src/physical_sources.egg-info/
--rw-rw-rw-   0        0        0     5896 2023-07-26 16:39:05.000000 physical_sources-0.7.6/src/physical_sources.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2023-07-26 16:39:05.000000 physical_sources-0.7.6/src/physical_sources.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 16:39:05.000000 physical_sources-0.7.6/src/physical_sources.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-07-26 16:39:05.000000 physical_sources-0.7.6/src/physical_sources.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 16:39:05.000000 physical_sources-0.7.6/src/physical_sources.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 19:59:43.387848 physical_sources-0.7.7/
+-rw-rw-rw-   0        0        0     1246 2023-07-11 17:45:55.000000 physical_sources-0.7.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     1863 2023-07-26 19:59:43.382883 physical_sources-0.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-07-26 17:25:21.000000 physical_sources-0.7.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-26 19:59:43.387848 physical_sources-0.7.7/setup.cfg
+-rw-rw-rw-   0        0        0     1018 2023-07-26 19:59:14.000000 physical_sources-0.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:59:43.274288 physical_sources-0.7.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 19:59:43.300290 physical_sources-0.7.7/src/physical_sources/
+-rw-rw-rw-   0        0        0        0 2023-07-07 16:01:14.000000 physical_sources-0.7.7/src/physical_sources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:59:43.367849 physical_sources-0.7.7/src/physical_sources/acoustic/
+-rw-rw-rw-   0        0        0      909 2023-07-26 18:01:31.000000 physical_sources-0.7.7/src/physical_sources/acoustic/INoiseSource.py
+-rw-rw-rw-   0        0        0        0 2023-07-07 16:01:14.000000 physical_sources-0.7.7/src/physical_sources/acoustic/__init__.py
+-rw-rw-rw-   0        0        0     4078 2023-07-26 15:15:48.000000 physical_sources-0.7.7/src/physical_sources/acoustic/analytic_source.py
+-rw-rw-rw-   0        0        0    25196 2023-07-26 19:53:14.000000 physical_sources-0.7.7/src/physical_sources/acoustic/point_source.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:59:43.378858 physical_sources-0.7.7/src/physical_sources/acoustic/source_definitions/
+-rw-rw-rw-   0        0        0        0 2023-07-26 18:13:37.000000 physical_sources-0.7.7/src/physical_sources/acoustic/source_definitions/__init__.py
+-rw-rw-rw-   0        0        0     2439 2023-07-26 19:31:26.000000 physical_sources-0.7.7/src/physical_sources/acoustic/source_definitions/noisefile.py
+-rw-rw-rw-   0        0        0    54940 2023-07-26 15:15:48.000000 physical_sources-0.7.7/src/physical_sources/acoustic/sphere_source.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:59:43.338286 physical_sources-0.7.7/src/physical_sources.egg-info/
+-rw-rw-rw-   0        0        0     1863 2023-07-26 19:59:41.000000 physical_sources-0.7.7/src/physical_sources.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      681 2023-07-26 19:59:42.000000 physical_sources-0.7.7/src/physical_sources.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 19:59:41.000000 physical_sources-0.7.7/src/physical_sources.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-07-26 19:59:41.000000 physical_sources-0.7.7/src/physical_sources.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 19:59:41.000000 physical_sources-0.7.7/src/physical_sources.egg-info/top_level.txt
```

### Comparing `physical_sources-0.7.6/LICENSE.txt` & `physical_sources-0.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `physical_sources-0.7.6/setup.py` & `physical_sources-0.7.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
     with open('HISTORY.md') as history_file:
         HISTORY = history_file.read()
 
 setup(
     name='physical_sources',
-    version='0.7.6',
+    version='0.7.7',
     packages=find_packages('src', exclude=['test*.py']),
     license='',
     author='Dr. Frank Mobley',
     author_email='frank.mobley.1@afrl.af.mil',
     description="A collection of classes that can be used to build acoustic sources from the NOISEFILE format. It "
                 "also contains classes to read the binary representations born from the author's dissertation",
     package_dir={'': 'src'},
```

### Comparing `physical_sources-0.7.6/src/physical_sources/acoustic/INoiseSource.py` & `physical_sources-0.7.7/src/physical_sources/acoustic/INoiseSource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 from PythonCoordinates.coordinates.coordinate_representations import SphericalCoordinate
 from PythonCoordinates.measurables.physical_quantities import Length
 
 
 class INoiseSource:
-    @abs.abstractmethod
+    @abc.abstractmethod
     def predict(self, location: SphericalCoordinate):
         """
         This function will utilize the information within the class to predict the acoustic metric at the specific
         emission location on the surface of the definition.
 
         :param location:
             This is the emission location. It is defined on the surface of a sphere inscribed around the source.
```

### Comparing `physical_sources-0.7.6/src/physical_sources/acoustic/analytic_source.py` & `physical_sources-0.7.7/src/physical_sources/acoustic/analytic_source.py`

 * *Files identical despite different names*

### Comparing `physical_sources-0.7.6/src/physical_sources/acoustic/point_source.py` & `physical_sources-0.7.7/src/physical_sources/acoustic/point_source.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,122 +1,225 @@
 import abc
+import copy
 from enum import Enum
 import numpy as np
 from PythonCoordinates.measurables.physical_quantities import Length, Angle, Speed, Temperature, Humidity, Pressure
 from PythonCoordinates.coordinates.coordinate_representations import SphericalCoordinate
 from physical_sources.acoustic.inoisesource import INoiseSource
 
 
 class AircraftType(Enum):
+    """
+    Within the NOISEFILE source description there is an ability to represent the acoustic emissions from both military
+    and civilian aircraft. This is an enumeration to define which type of aircraft is represented by a specific source
+    description.
+    """
     Military = 0, 'Military'
     Civilian = 1, 'Civilan'
 
 
 class DataCollectionType(Enum):
+    """
+    The NOISEFILE dataset permits the definition of acoustic source emissions through estimating the acoustic levels.
+    The desired method is to measure the source levels. This determines what type of data is being represented in the
+    source.
+    """
     Measured = 0, 'Measured'
     Estimated = 1, 'Estimated'
 
 
 class InterpolationCode(Enum):
+    """
+    Inside the Omega10 program (which reads the NOISEFILE Dataset) there are three methods available for interpolation
+    of the acoustic levels. The first is fixed and will return an error if the user attempts to interpolat this levels
+    as part of the calculation of new levels. The parallel method assumes that there is a linear relationship between
+    the data, but this point defines an offset point parallel to that linear relationship. The final method is variable
+    which defines the linear relationship between all points marked with the variable label.
+    """
     Fixed = 0, 'Fixed'
     Parallel = 1, 'Parallel'
     Variable = 2, 'Variable'
 
 
-class NoiseFilePowerSetting:
+class PowerSetting:
+    """
+    This class contains the information that is present in the source definition that relates to the power setting of
+    the aircraft. It contains an average, minimum, and maximum value for this description and the associated units.
+    """
     def __init__(self):
-        self.value = 0.0
-        self.units = ''
-        self.upper_limit = 0.0
-        self.lower_limit = 0.0
+        self._value = 0.0
+        self._units = ''
+        self._upper_limit = 0.0
+        self._lower_limit = 0.0
+
+    @property
+    def power_setting_value(self) -> float:
+        return self._value
+
+    @power_setting_value.setter
+    def power_setting_value(self, value):
+        self._value = value
+
+    @property
+    def units(self) -> str:
+        return self._units
+
+    @units.setter
+    def units(self, value):
+        self._units = value
+
+    @property
+    def lower_limit(self) -> float:
+        return self._lower_limit
+
+    @lower_limit.setter
+    def lower_limit(self, value):
+        self._lower_limit = value
+
+    @property
+    def upper_limit(self) -> float:
+        return self._upper_limit
+
+    @upper_limit.setter
+    def upper_limit(self, value):
+        self._vupper_limit = value
 
 
 class IPointSource(INoiseSource):
+    """
+    Older models of acoustic source
+    """
     def __init__(self):
-        pass
+        super().__init__()
+
+        self._vehicle_type = None
+        self._interpolation_code = None
+        self._id = None
+        self._operational_power_code = None
+        self._reference_distance = None
+        self._reference_temperature = None
+        self._reference_humidity = None
+        self._source = None
+        self._engine_name = None
+        self._engine_count = None
+        self._collection_date = None
+        self._power_settings = []
+        self._power_setting_description = None
 
     @abc.abstractmethod
     def predict(self, location: SphericalCoordinate):
         raise NotImplementedError
 
+    @property
+    def vehicle_type(self) -> AircraftType:
+        return self._vehicle_type
+
+    @property
+    def interpolation_code(self) -> InterpolationCode:
+        return self._interpolation_code
 
-class NoiseFileAcousticSource(IPointSource):
+    @property
+    def aircraft_id(self) -> int:
+        return self._id
+
+    @property
+    def operational_power_code(self) -> int:
+        return self._operational_power_code
+
+    @property
+    def reference_distance(self):
+        return self._reference_distance
+
+    @property
+    def reference_temperature(self):
+        return self._reference_temperature
+
+    @property
+    def reference_humidity(self):
+        return self._reference_humidity
+
+    @property
+    def source(self):
+        return self._source
+
+    @property
+    def engine_name(self):
+        return self._engine_name
+
+    @property
+    def engine_count(self):
+        return self._engine_count
+
+    @property
+    def collection_date(self):
+        return self._collection_date
+
+    @property
+    def data_collection_type(self) -> DataCollectionType:
+        return self._data_collection_type
+
+    @property
+    def power_settings(self):
+        return self._power_settings
+
+    @staticmethod
+    def source_type():
+        return 'Unknown'
+
+
+    @property
+    def power_setting_description(self):
+        return self._power_setting_description
+
+
+class FlightPointSource(IPointSource):
 
     def __init__(self, filename=None):
         super().__init__()
-        # in the C# code this is an observable collection. Not sure why...
-        self._power_settings = []
-
-        self._vehicle_type = None
-        self._interpolation_code = None
-        self._data_collection_type = None
         self._microphone_count = None
         self._directivity_angle = None
         self._perceived_noise_level = None
         self._tone_corrected_perceived_noise_level = None
         self._la = None
         self._lat = None
         self._effective_perceived_noise_level = None
         self._sound_exposure_level = None
         self._tone_corrected_sound_exposure_level = None
         self._tone_correction = None
-        self._id = None
-        self._operational_power_code = None
         self._operational_type_code = None
-        self._engine_name = None
-        self._engine_count = None
         self._drag_configuration = None
-        self._source = None
-        self._collection_date = None
-        self._reference_distance = None
         self._reference_speed = None
-        self._reference_temperature = None
-        self._reference_humidity = None
         self._power_setting_description = None
         self._sound_pressure_levels = []
         self._frequency_resolution = 3
         self._minimum_frequency_band = 10
         self._maximum_frequency_band = 40
 
         if filename is not None:
             self.filename = filename
             f = open(self.filename)
             contents = f.readlines()
             f.close()
             self._load_data(contents, 0)
 
-    @staticmethod
-    def source_type():
-        return 'FLIGHT'
+
 
     @property
     def frequency_resolution(self):
         return self._frequency_resolution
 
     @property
     def minimum_frequency_band(self):
         return self._minimum_frequency_band
 
     @property
     def maximum_frequency_band(self):
         return self._maximum_frequency_band
 
     @property
-    def vehicle_type(self) -> AircraftType:
-        return self._vehicle_type
-
-    @property
-    def interpolation_code(self) -> InterpolationCode:
-        return self._interpolation_code
-
-    @property
-    def data_collection_type(self) -> DataCollectionType:
-        return self._data_collection_type
-
-    @property
     def number_microphone_in_average(self):
         return self._microphone_count
 
     @property
     def directivity_angle(self):
         return self._directivity_angle
 
@@ -149,73 +252,40 @@
         return self._effective_perceived_noise_level
 
     @property
     def tone_correction(self):
         return self._tone_correction
 
     @property
-    def aircraft_id(self):
-        return self._id
-
-    @property
-    def operational_power_code(self):
-        return self._operational_power_code
-
-    @property
     def operational_type_code(self):
         return self._operational_type_code
 
     @property
-    def engine_name(self):
-        return self._engine_name
-
-    @property
-    def engine_count(self):
-        return self._engine_count
-
-    @property
     def drag_configuration(self):
         return self._drag_configuration
 
     @property
-    def source(self):
-        return self._source
-
-    @property
-    def collection_date(self):
-        return self._collection_date
-    #
-    # @property
-    # def reference_distance(self):
-    #     return self._reference_distance
-
-    @property
     def reference_speed(self):
         return self._reference_speed
 
-    @property
-    def reference_temperature(self):
-        return self._reference_temperature
-
-    @property
-    def reference_humidity(self):
-        return self._reference_humidity
-
-    @property
-    def power_setting_description(self):
-        return self._power_setting_description
-
-    @property
-    def power_settings(self):
-        return self._power_settings
-
     def predict(self, location):
         return self._sound_pressure_levels
 
+    @staticmethod
+    def source_type():
+        return 'FLIGHT'
+
     def write_data(self, file):
+        """
+        This function will write the data from the class into a formatted file that is the same format as the current
+        representation of the NOISEFILE dataset.
+
+        :param file:
+            This is the file writer that receives the bytes to write to the file.
+        """
         if self.vehicle_type == AircraftType.Military:
             record1 = 'MILITARY FM{:5d}{:2d}{:1d}'.format(self.aircraft_id, self.operational_power_code,
                                                           self.operational_type_code)
         else:
             record1 = 'CIVILIAN FC{:5d}{:2d}{:1d}'.format(self.aircraft_id, self.operational_power_code,
                                                           self.operational_type_code)
 
@@ -259,15 +329,26 @@
 
         file.write(record1 + '\n')
         file.write(record2 + '\n')
         file.write(record3 + '\n')
         file.write(record4 + '\n')
         file.write(record5 + '\n')
 
-    def _load_data(self, contents, start_index):
+    def _load_data(self, contents, start_index: int = 0):
+        """
+        This function loads the information for this description from the contents of a file. In the case where this may
+        represent multiple point source definitions in a single file, the second parameter tells the function where to
+        begin looking for the start of the source definition.
+        :param contents:
+            This list of rows from a file that contain the source definitions
+        :param start_index:
+            An index within the contents list/array for where we will start processing the information for this
+            definition.
+        """
+
         record1 = contents[start_index].rstrip()
         start_index += 1
         record2 = contents[start_index].rstrip()
         start_index += 1
         record3 = contents[start_index].rstrip()
         start_index += 1
         record4 = contents[start_index].rstrip()
@@ -303,15 +384,15 @@
             self._reference_speed = Speed(float(record2[109:109 + 5]), Speed.Units.Knots)
             self._reference_temperature = Temperature(float(record2[120:120 + 3]), Temperature.Units.Fahrenheit)
             self._reference_humidity = Humidity(float(record2[127:127 + 3]), Humidity.Units.Percentage)
             if len(record3) > 0:
                 self._power_setting_description = record3[0:20].strip()
                 record3 = record3[20:]
                 while len(record3) > 0:
-                    temp = NoiseFilePowerSetting()
+                    temp = PowerSetting()
                     temp.value = float(record3[0:9].strip())
                     temp.units = record3[10:10 + 10].strip()
                     temp.lower_limit = float(record3[20:20 + 9].strip())
                     temp.upper_limit = float(record3[30:30 + 9].strip())
                     self._power_settings.append(temp)
                     record3 = record3[39:]
             self._microphone_count = int(record4[0:4].strip())
@@ -329,38 +410,42 @@
                 self._sound_pressure_levels.append(float(record5[index:index + 4].strip()) / 10.0)
         except Exception as e:
             raise ValueError('An error ocurred in the NOISEFILE formatted file at index = ' + str(
                 start_index) + ' - error message: ' + str(e))
         return start_index
 
 
-class NoiseFileStaticAcousticSource(NoiseFileAcousticSource):
+class GroundPointSource(IPointSource):
     def __init__(self, filename=None):
+
+        super().__init__()
         self.noise_suppression_system = ''
         self._reference_pressure = Pressure()
 
         if filename is None:
-            super().__init__()
             self.polar_sound_pressure_levels = {}
         else:
             self.filename = filename
-            self._power_settings = []
             self.polar_sound_pressure_levels = {}
             with open(filename, 'r') as file:
                 contents = file.readlines()
                 self._load_data(contents, 0)
 
     @property
-    def measurement_count(self):
-        return self.polar_sound_pressure_levels.shape[0]
-
-    @property
     def reference_pressure(self):
         return self._reference_pressure
 
+    @property
+    def angle_count(self) -> int:
+        return len(self.polar_sound_pressure_levels)
+
+    @staticmethod
+    def source_type():
+        return 'GROUND'
+
     def _load_data(self, contents, start_index):
         record1 = contents[start_index].rstrip()
         start_index += 1
         try:
             #   Record or line 1
             if record1[0:8] == 'MILITARY':
                 self._vehicle_type = AircraftType.Military
@@ -395,18 +480,18 @@
             start_index += 1
             self._power_setting_description = record3[0:20].strip()
             for i in range(0, 3, 1):
                 substring = record3[20 + (i * 20): 20 + (i * 20) + 21]
                 try:
                     power_setting_value = float(substring[0:9])
                     power_setting_units = substring[10:10 + 10].strip()
-                    power_setting = NoiseFilePowerSetting()
+                    power_setting = PowerSetting()
                     power_setting.value = power_setting_value
                     power_setting.units = power_setting_units
-                    self.power_settings.append(power_setting)
+                    self._power_settings.append(power_setting)
                 except Exception as ee:
                     print('FAILURE: {}'.format(str(ee)))
                     break
 
             self._reference_distance = Length(float(record3[80:80 + 5]), Length.Units.Feet)
             self._reference_speed = Speed()
             self._reference_temperature = Temperature(float(record3[89:89 + 3]), Temperature.Units.Fahrenheit)
@@ -477,65 +562,62 @@
 
     def predict(self, location: SphericalCoordinate) -> list:
         if isinstance(location, SphericalCoordinate):
             return self.__sound_pressure_level__(location.azimuthal)
         else:
             raise ValueError("You must use the PythonCoordinates module to define the location on the source")
 
-    def __sound_pressure_level__(self, polar) -> list:
-        if isinstance(polar, Angle):
-            angle = polar.normalized.degrees
+    def __sound_pressure_level__(self, azimuthal) -> list:
+        if isinstance(azimuthal, Angle):
+            angle = azimuthal.normalized.degrees
             if angle > 180:
                 angle = 360 - angle
             degree_angle_key = int(np.floor(angle / 10))
             return self.polar_sound_pressure_levels[degree_angle_key]
         else:
             raise ValueError("You must use the PythonCoordinates module to define the location on the source")
 
 
-class FlightNoiseFileDatabase:
-    def __init__(self, filename):
+class InterpolatedPointSource(IPointSource):
+    """
+    This class provides a method of representing the noise power distance curve that is used by NoiseMap to determine
+    the acoustic levels as a function of power setting. The power settings are described as individual IPointNoise
+    sources. The interpolation is then defined in accordance with the Omega 10 interpolation schema.
+    """
+
+    def __init__(self, a: list):
         """
-        This constructor will load the entire noise database from the flight01.dat file that is passed to the
-        constructor
-        :param filename: str - the path to the NOISEFILE database which we want to load
+        This constructs the collection of sources and provides the methods for interpolating the levels as a function
+        of the desired power setting
         """
-        self.filename = filename
-        self.sources = []
-        with open(filename, 'r') as f:
-            contents = f.readlines()
-        line_index = 0
-        while line_index < len(contents):
-            src_data = NoiseFileAcousticSource()
-            try:
-                line_index = src_data._load_data(contents, line_index)
-            except Exception as eee:
-                raise ValueError('An incorrect formatted NOISEFILE entry found at index {}: {}'.format(
-                    line_index, str(eee)))
-            self.sources.append(src_data)
 
+        super().__init__()
 
-class GroundNoiseFileDatabase:
-    def __init__(self, path):
-        """
-        This will read a file with multiple NOISEFILE_Static_AcousticSource definition in a single file and place the
-        elements into an internal array
-        """
+        self._sources = copy.deepcopy(a)
 
-        self.filename = path
-        self.sources = []
+        self._desired_power_setting = a[0].power_setting[0]
 
-        with open(self.filename, 'rt') as f:
-            contents = f.readlines()
+    @property
+    def desired_power_setting(self) -> PowerSetting:
+        return self._desired_power_setting
+
+    @desired_power_setting.setter
+    def desired_power_setting(self, value: PowerSetting):
+        self._desired_power_setting = value
+
+    @property
+    def sources(self):
+        return self._sources
 
-        line_index = 0
+    def predict(self, location: SphericalCoordinate):
+        """
+        This function will take the value in the desired_power_setting function and determine the interpolated value at
+        this location in accordance with the NoiseMap program called Omega10.
+        :param location:
+            The spherical location were we want to evaluate the source levels for the desired_power_setting
+        :returns:
+            A list or array of the sound pressure levels at this location and desired_power_setting
+        """
+
+        raise NotImplementedError
 
-        while line_index < len(contents):
-            src_data = NoiseFileStaticAcousticSource()
-            try:
-                line_index = src_data._load_data(contents, line_index)
-            except Exception as eee:
-                raise ValueError("An incorrect formatted NOISEFILE entry found at index {}: {}".format(
-                    line_index, str(eee)
-                ))
 
-            self.sources.append(src_data)
```

### Comparing `physical_sources-0.7.6/src/physical_sources/acoustic/sphere_source.py` & `physical_sources-0.7.7/src/physical_sources/acoustic/sphere_source.py`

 * *Files identical despite different names*

### Comparing `physical_sources-0.7.6/src/physical_sources.egg-info/SOURCES.txt` & `physical_sources-0.7.7/src/physical_sources.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 src/physical_sources.egg-info/top_level.txt
 src/physical_sources/acoustic/INoiseSource.py
 src/physical_sources/acoustic/__init__.py
 src/physical_sources/acoustic/analytic_source.py
 src/physical_sources/acoustic/inoisesource.py
 src/physical_sources/acoustic/point_source.py
 src/physical_sources/acoustic/sphere_source.py
-src/physical_sources/acoustic/line_source/__init__.py
+src/physical_sources/acoustic/source_definitions/__init__.py
+src/physical_sources/acoustic/source_definitions/noisefile.py
```

