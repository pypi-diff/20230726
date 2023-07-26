# Comparing `tmp/ThermalNetwork-0.1.1.tar.gz` & `tmp/ThermalNetwork-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ThermalNetwork-0.1.1.tar", last modified: Thu Jul 20 17:35:11 2023, max compression
+gzip compressed data, was "ThermalNetwork-0.2.tar", last modified: Wed Jul 26 17:02:45 2023, max compression
```

## Comparing `ThermalNetwork-0.1.1.tar` & `ThermalNetwork-0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 17:35:11.662903 ThermalNetwork-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-07-20 17:35:11.662903 ThermalNetwork-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 17:35:11.662903 ThermalNetwork-0.1.1/ThermalNetwork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-07-20 17:35:11.000000 ThermalNetwork-0.1.1/ThermalNetwork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-20 17:35:11.000000 ThermalNetwork-0.1.1/ThermalNetwork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 17:35:11.000000 ThermalNetwork-0.1.1/ThermalNetwork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-20 17:35:11.000000 ThermalNetwork-0.1.1/ThermalNetwork.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-20 17:35:11.000000 ThermalNetwork-0.1.1/ThermalNetwork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-20 17:35:11.000000 ThermalNetwork-0.1.1/ThermalNetwork.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-20 17:35:11.662903 ThermalNetwork-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 17:35:11.662903 ThermalNetwork-0.1.1/thermalnetwork/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/base_component.py
--rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/energy_transfer_station.py
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)      533 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/fan.py
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/ground_heat_exchanger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/heat_pump.py
--rw-r--r--   0 runner    (1001) docker     (122)    23849 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/network.py
--rw-r--r--   0 runner    (1001) docker     (122)      901 2023-07-20 17:35:08.000000 ThermalNetwork-0.1.1/thermalnetwork/pump.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 17:02:45.646352 ThermalNetwork-0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-07-26 17:02:45.646352 ThermalNetwork-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 17:02:45.642352 ThermalNetwork-0.2/ThermalNetwork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-07-26 17:02:45.000000 ThermalNetwork-0.2/ThermalNetwork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-26 17:02:45.000000 ThermalNetwork-0.2/ThermalNetwork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 17:02:45.000000 ThermalNetwork-0.2/ThermalNetwork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-26 17:02:45.000000 ThermalNetwork-0.2/ThermalNetwork.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-26 17:02:45.000000 ThermalNetwork-0.2/ThermalNetwork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-26 17:02:45.000000 ThermalNetwork-0.2/ThermalNetwork.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-26 17:02:45.646352 ThermalNetwork-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 17:02:45.646352 ThermalNetwork-0.2/thermalnetwork/
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/base_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/energy_transfer_station.py
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/fan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/ground_heat_exchanger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/heat_pump.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24151 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/network.py
+-rw-r--r--   0 runner    (1001) docker     (122)      901 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/pump.py
```

### Comparing `ThermalNetwork-0.1.1/LICENSE` & `ThermalNetwork-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.1.1/PKG-INFO` & `ThermalNetwork-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ThermalNetwork
-Version: 0.1.1
+Version: 0.2
 Summary: A thermal network solver for GHE sizing.
 Home-page: https://github.com/mitchute/ThermalNetwork
 Author: Matt Mitchell
 Author-email: mitchute@gmail.com
 License: BSD-3
 Description: # ThermalNetwork
```

### Comparing `ThermalNetwork-0.1.1/ThermalNetwork.egg-info/PKG-INFO` & `ThermalNetwork-0.2/ThermalNetwork.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ThermalNetwork
-Version: 0.1.1
+Version: 0.2
 Summary: A thermal network solver for GHE sizing.
 Home-page: https://github.com/mitchute/ThermalNetwork
 Author: Matt Mitchell
 Author-email: mitchute@gmail.com
 License: BSD-3
 Description: # ThermalNetwork
```

### Comparing `ThermalNetwork-0.1.1/ThermalNetwork.egg-info/SOURCES.txt` & `ThermalNetwork-0.2/ThermalNetwork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.1.1/setup.py` & `ThermalNetwork-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.1.1/thermalnetwork/energy_transfer_station.py` & `ThermalNetwork-0.2/thermalnetwork/energy_transfer_station.py`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.1.1/thermalnetwork/fan.py` & `ThermalNetwork-0.2/thermalnetwork/fan.py`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.1.1/thermalnetwork/ground_heat_exchanger.py` & `ThermalNetwork-0.2/thermalnetwork/ground_heat_exchanger.py`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.1.1/thermalnetwork/heat_pump.py` & `ThermalNetwork-0.2/thermalnetwork/heat_pump.py`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.1.1/thermalnetwork/network.py` & `ThermalNetwork-0.2/thermalnetwork/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -430,41 +430,39 @@
         """
 
         # This is being done in the GHE sizer call.  Should those dirs get moved somewhere else?
 
         pass
 
 
-def run_sizer_from_cli_worker(geojson_file_path: Path, scenario_directory_path: Path,
+def run_sizer_from_cli_worker(system_parameter_path: Path, scenario_directory_path: Path, geojson_file_path: Path,
                               output_directory_path: Path) -> int:
     """
     Sizing worker function. Worker is called by tests, and thus not wrapped by `click`.
 
     :param geojson_file_path: path to GeoJSON file
+    :param system_parameter_path: path to System Parameter File
     :param scenario_directory_path: path to scenario directory
     :param output_directory_path: path to output directory
     """
 
     # load geojson_file file
     if not geojson_file_path.exists():
         print(f"No input file found at {geojson_file_path}, aborting.", file=stderr)
         return 1
 
     geojson_data = json.loads(geojson_file_path.read_text())
     # print(f"geojson_data: {geojson_data}")
 
-    # load system_parameters file from the scenario directory path
-    system_parameters_path = scenario_directory_path.joinpath("ghe_dir", "system_parameter.json")
-
     # Check if the file exists
-    if not system_parameters_path.exists():
-        print(f"No system_parameter.json file found at {system_parameters_path}, aborting.", file=stderr)
+    if not system_parameter_path.exists():
+        print(f"No system_parameter.json file found at {system_parameter_path}, aborting.", file=stderr)
         return 1
 
-    system_parameters_data = json.loads(system_parameters_path.read_text())
+    system_parameters_data = json.loads(system_parameter_path.read_text())
     # print(f"system_parameters_data: {system_parameters_data}")
 
     # load all input data
     version: int = system_parameters_data["district_system"]["fifth_generation"]["ghe_parameters"]["version"]
     if version != VERSION:
         print("Mismatched versions, could be a problem", file=stderr)
         return 1
@@ -518,63 +516,69 @@
     network.size(output_directory_path)
     # network.write_outputs(output_path)
 
     return 0
 
 
 @click.command(name="ThermalNetworkCommandLine")
-@click.option("-f", "--geojson_file", type=click.Path(exists=True), metavar="GEOJSON_FILE", help="Path to GeoJSON file")
+@click.option("-y", "--sys_param_file", type=click.Path(exists=True), metavar="SYS_PARAM_PATH", help="Path to System Parameter file")
 @click.option("-s", "--scenario_directory", type=click.Path(exists=True), metavar="SCENARIO_DIRECTORY",
               help="Path to scenario directory")
+@click.option("-f", "--geojson_file", type=click.Path(exists=True), metavar="GEOJSON_FILE", help="Path to GeoJSON file")
 @click.option("-o", "--output_directory", type=click.Path(), metavar="OUTPUT_DIRECTORY",
               help="Path to output directory")
 @click.version_option(VERSION)
 # @click.option(
 #     "--validate",
 #     default=False,
 #     is_flag=True,
 #     show_default=False,
 #     help="Validate input and exit."
 # )
-def run_sizer_from_cli(geojson_file, scenario_directory, output_directory):
+def run_sizer_from_cli(system_parameter_file, scenario_directory, geojson_file, output_directory):
     """
     CLI entrypoint for sizing runner.
 
+    :param system_parameter_file: path to system parameter file
     :param geojson_file: path to GeoJSON file
-    :param scenario_directory: path to scenario directory
     :param output_directory: path to output directory    :param validate: flag for input schema validation
     """
 
-    print("GeoJSON file:", geojson_file)
+    print("System Parameter File:", system_parameter_file)
     print("Scenario directory:", scenario_directory)
+    print("GeoJSON file:", geojson_file)
     print("Output directory:", output_directory)
 
-    geojson_file_path = Path(geojson_file).resolve()
-    print(f"geojson_file path: {geojson_file_path}\n")
     # if validate:
     #    try:
     #        validate_input_file(input_path)
     #        print("Valid input file.")
     #        return 0
     #    except ValidationError:
     #        print("Schema validation error. See previous error message(s) for details.", file=stderr)
     #        return 1
     # calling the worker function here
 
+    system_parameter_path = Path(system_parameter_file).resolve()
+    print(f"scenario_directory path: {system_parameter_path}\n")
+
     scenario_directory_path = Path(scenario_directory).resolve()
     print(f"scenario_directory path: {scenario_directory_path}\n")
 
+    geojson_file_path = Path(geojson_file).resolve()
+    print(f"geojson_file path: {geojson_file_path}\n")
+
     output_directory_path = Path(output_directory)
     print(f"Output path: {output_directory_path}\n")
     if not output_directory_path.exists():
         print("Output path does not exist. attempting to create")  # Add this line
         try:
             output_directory_path.mkdir(parents=True, exist_ok=True)
         except Exception as e:
             print(f"Failed to create directory: {e}")
 
     output_directory_path = output_directory_path.resolve()
-    return run_sizer_from_cli_worker(geojson_file_path, scenario_directory_path, output_directory_path)
+    return run_sizer_from_cli_worker(system_parameter_path, scenario_directory_path, geojson_file_path, output_directory_path)
 
 
 if __name__ == "__main__":
     exit(run_sizer_from_cli())
```

### Comparing `ThermalNetwork-0.1.1/thermalnetwork/pump.py` & `ThermalNetwork-0.2/thermalnetwork/pump.py`

 * *Files identical despite different names*

