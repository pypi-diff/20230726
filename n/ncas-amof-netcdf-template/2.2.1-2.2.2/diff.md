# Comparing `tmp/ncas_amof_netcdf_template-2.2.1.tar.gz` & `tmp/ncas_amof_netcdf_template-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncas_amof_netcdf_template-2.2.1.tar", last modified: Wed Jun 28 08:47:00 2023, max compression
+gzip compressed data, was "ncas_amof_netcdf_template-2.2.2.tar", last modified: Wed Jul 26 13:02:54 2023, max compression
```

## Comparing `ncas_amof_netcdf_template-2.2.1.tar` & `ncas_amof_netcdf_template-2.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:47:00.698795 ncas_amof_netcdf_template-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-28 08:46:50.000000 ncas_amof_netcdf_template-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-28 08:47:00.698795 ncas_amof_netcdf_template-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-28 08:46:50.000000 ncas_amof_netcdf_template-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-28 08:46:50.000000 ncas_amof_netcdf_template-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 08:47:00.698795 ncas_amof_netcdf_template-2.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:47:00.694795 ncas_amof_netcdf_template-2.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:47:00.698795 ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-28 08:46:50.000000 ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22463 2023-06-28 08:46:50.000000 ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template/create_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-28 08:46:50.000000 ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template/remove_empty_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-06-28 08:46:50.000000 ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template/tsv2dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-28 08:46:50.000000 ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-28 08:46:50.000000 ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template/values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:47:00.698795 ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-28 08:47:00.000000 ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-28 08:47:00.000000 ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 08:47:00.000000 ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-28 08:47:00.000000 ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-28 08:47:00.000000 ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 08:47:00.698795 ncas_amof_netcdf_template-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-28 08:46:50.000000 ncas_amof_netcdf_template-2.2.1/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-28 08:46:50.000000 ncas_amof_netcdf_template-2.2.1/tests/test_create_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-28 08:46:50.000000 ncas_amof_netcdf_template-2.2.1/tests/test_tsv2dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-28 08:46:50.000000 ncas_amof_netcdf_template-2.2.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:02:54.635084 ncas_amof_netcdf_template-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-26 13:02:43.000000 ncas_amof_netcdf_template-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-26 13:02:54.635084 ncas_amof_netcdf_template-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-26 13:02:43.000000 ncas_amof_netcdf_template-2.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-26 13:02:43.000000 ncas_amof_netcdf_template-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:02:54.635084 ncas_amof_netcdf_template-2.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:02:54.631084 ncas_amof_netcdf_template-2.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:02:54.635084 ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-26 13:02:43.000000 ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23485 2023-07-26 13:02:43.000000 ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template/create_netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-26 13:02:43.000000 ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template/remove_empty_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-26 13:02:43.000000 ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template/tsv2dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-26 13:02:43.000000 ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-07-26 13:02:43.000000 ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:02:54.635084 ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-26 13:02:54.000000 ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-26 13:02:54.000000 ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:02:54.000000 ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-26 13:02:54.000000 ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-26 13:02:54.000000 ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:02:54.635084 ncas_amof_netcdf_template-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-26 13:02:43.000000 ncas_amof_netcdf_template-2.2.2/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-26 13:02:43.000000 ncas_amof_netcdf_template-2.2.2/tests/test_create_netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-26 13:02:43.000000 ncas_amof_netcdf_template-2.2.2/tests/test_tsv2dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-26 13:02:43.000000 ncas_amof_netcdf_template-2.2.2/tests/test_util.py
```

### Comparing `ncas_amof_netcdf_template-2.2.1/LICENSE` & `ncas_amof_netcdf_template-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ncas_amof_netcdf_template-2.2.1/PKG-INFO` & `ncas_amof_netcdf_template-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncas_amof_netcdf_template
-Version: 2.2.1
+Version: 2.2.2
 Summary: Package to create NCAS AMOF netCDF files.
 Author-email: "Joshua M. Ralph-Hampton" <joshua.hampton@ncas.ac.uk>
 License: MIT License
         
         Copyright (c) 2023 Joshua Hampton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ncas_amof_netcdf_template-2.2.1/README.md` & `ncas_amof_netcdf_template-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ncas_amof_netcdf_template-2.2.1/pyproject.toml` & `ncas_amof_netcdf_template-2.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ncas_amof_netcdf_template"
-version = "2.2.1"
+version = "2.2.2"
 authors = [
   { name="Joshua M. Ralph-Hampton", email="joshua.hampton@ncas.ac.uk" },
 ]
 description = "Package to create NCAS AMOF netCDF files."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7, <4"
```

### Comparing `ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template/create_netcdf.py` & `ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template/create_netcdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,92 +108,106 @@
                                 tsv2dict.isntrument_dict.
         product (str): name of data product.
         verbose (int): level of additional info to print. At the moment,
                        there is only 1 additional level. Default 0.
     """
     for obj in [product, "common"]:
         for key, value in instrument_dict[obj]["variables"].items():
-            # therefore, value is instrument_dict[obj]['variables'][key]
-            # want to pop certain things here, but not for ever, so make tmp_value
-            tmp_value = copy.copy(value)
-
-            # error, there are some variables with dimensions
-            # missing, error in spreadsheet
-            # if we encounter one, we're going to print out an error
-            # and forget about that variable
-            if "dimension" not in tmp_value.keys():
-                print(f"ERROR: Missing dimensions for variable {key} in product {obj}")
-                print("Variable not added file")
+            # make sure variable doesn't already exist, warn if it does
+            if key in ncfile.variables.keys():
+                print(f"WARN: variable {key} defined multiple times.")
             else:
-                var_dims = tmp_value.pop("dimension")
-                # there was an error somewhere meaning 2 dimensions
-                # had a '.' instead of ',' between them
-                var_dims = var_dims.replace(".", ",")
-                var_dims = tuple(x.strip() for x in var_dims.split(","))
-
-                datatype = tmp_value.pop("type")
-
-                if "_FillValue" in tmp_value:
-                    fill_value = float(tmp_value.pop("_FillValue"))
-                else:
-                    fill_value = ""
-
-                if fill_value != "":
-                    var = ncfile.createVariable(
-                        key, datatype, var_dims, fill_value=fill_value
+                # therefore, value is instrument_dict[obj]['variables'][key]
+                # want to pop certain things here, but not for ever, so make tmp_value
+                tmp_value = copy.copy(value)
+
+                # error, there are some variables with dimensions
+                # missing, error in spreadsheet
+                # if we encounter one, we're going to print out an error
+                # and forget about that variable
+                if "dimension" not in tmp_value.keys():
+                    print(
+                        f"ERROR: Missing dimensions for variable {key} in product {obj}"
                     )
+                    print("Variable not added file")
                 else:
-                    var = ncfile.createVariable(key, datatype, var_dims)
-
-                for mdatkey, mdatvalue in tmp_value.items():
-                    # flag meanings in the tsv files are separated by '|',
-                    # should be space separated
-                    if "|" in mdatvalue and "flag_meaning" in mdatkey:
-                        mdatvalue = " ".join([i.strip() for i in mdatvalue.split("|")])
-                    # flag values are bytes, can't add byte array
-                    # into NETCDF4_CLASSIC so have to muddle a bit
-                    if "flag_value" in mdatkey and "qc" in key and var.dtype == np.int8:
-                        # turn string like "0b,1b..." into list of ints like [0,1...]
-                        mdatvalue = mdatvalue.strip(",")
-                        newmdatvalue = [int(i.strip("b")) for i in mdatvalue.split(",")]
-                        # turn list into array with int8 type
-                        mdatvalue = np.array(newmdatvalue, dtype=np.int8)
-                    # print warning for example values,
-                    # and don't add example values for standard_name
-                    if (
-                        mdatkey == "standard_name"
-                        and ("EXAMPLE" in mdatvalue or mdatvalue == "")
-                        and verbose >= 1
-                    ):
-                        print(
-                            f"WARN: No standard name for variable {key}, "
-                            "standard_name attribute not added"
-                        )
-                    elif "EXAMPLE" in mdatvalue and verbose >= 1:
-                        print(
-                            "WARN: example value for attribute "
-                            f"{mdatkey} for variable {key}"
+                    var_dims = tmp_value.pop("dimension")
+                    # there was an error somewhere meaning 2 dimensions
+                    # had a '.' instead of ',' between them
+                    var_dims = var_dims.replace(".", ",")
+                    var_dims = tuple(x.strip() for x in var_dims.split(","))
+
+                    datatype = tmp_value.pop("type")
+
+                    if "_FillValue" in tmp_value:
+                        fill_value = float(tmp_value.pop("_FillValue"))
+                    else:
+                        fill_value = ""
+
+                    if fill_value != "":
+                        var = ncfile.createVariable(
+                            key, datatype, var_dims, fill_value=fill_value
                         )
-                    # don't add EXAMPLE standard name
-                    if not (
-                        mdatkey == "standard_name"
-                        and ("EXAMPLE" in mdatvalue or mdatvalue == "")
-                    ):
-                        # don't add empty attributes
+                    else:
+                        var = ncfile.createVariable(key, datatype, var_dims)
+
+                    for mdatkey, mdatvalue in tmp_value.items():
+                        # flag meanings in the tsv files are separated by '|',
+                        # should be space separated
+                        if "|" in mdatvalue and "flag_meaning" in mdatkey:
+                            mdatvalue = " ".join(
+                                [i.strip() for i in mdatvalue.split("|")]
+                            )
+                        # flag values are bytes, can't add byte array
+                        # into NETCDF4_CLASSIC so have to muddle a bit
+                        if (
+                            "flag_value" in mdatkey
+                            and "qc" in key
+                            and var.dtype == np.int8
+                        ):
+                            # turn string "0b,1b..." into list of ints [0,1...]
+                            mdatvalue = mdatvalue.strip(",")
+                            newmdatvalue = [
+                                int(i.strip("b")) for i in mdatvalue.split(",")
+                            ]
+                            # turn list into array with int8 type
+                            mdatvalue = np.array(newmdatvalue, dtype=np.int8)
+                        # print warning for example values,
+                        # and don't add example values for standard_name
                         if (
-                            isinstance(mdatvalue, str)
-                            and mdatvalue == ""
+                            mdatkey == "standard_name"
+                            and ("EXAMPLE" in mdatvalue or mdatvalue == "")
                             and verbose >= 1
                         ):
                             print(
-                                f"WARN: No value for attribute {mdatkey} "
-                                "for variable {key}, attribute not added"
+                                f"WARN: No standard name for variable {key}, "
+                                "standard_name attribute not added"
+                            )
+                        elif "EXAMPLE" in mdatvalue and verbose >= 1:
+                            print(
+                                "WARN: example value for attribute "
+                                f"{mdatkey} for variable {key}"
                             )
-                        else:
-                            var.setncattr(mdatkey, mdatvalue)
+                        # don't add EXAMPLE standard name
+                        if not (
+                            mdatkey == "standard_name"
+                            and ("EXAMPLE" in mdatvalue or mdatvalue == "")
+                        ):
+                            # don't add empty attributes
+                            if (
+                                isinstance(mdatvalue, str)
+                                and mdatvalue == ""
+                                and verbose >= 1
+                            ):
+                                print(
+                                    f"WARN: No value for attribute {mdatkey} "
+                                    "for variable {key}, attribute not added"
+                                )
+                            else:
+                                var.setncattr(mdatkey, mdatvalue)
 
 
 def make_netcdf(
     instrument,
     product,
     time,
     instrument_dict,
@@ -328,15 +342,18 @@
     all_dimensions = []
     dimlengths = {}
     for key, val in product_dict.items():
         if "dimensions" in val.keys() and (key == product or key == "common"):
             for dim in list(val["dimensions"].keys()):
                 if dim not in all_dimensions:
                     all_dimensions.append(dim)
-                    if "<" not in val["dimensions"][dim]["Length"]:
+                    if (
+                        isinstance(val["dimensions"][dim]["Length"], int)
+                        or "<" not in val["dimensions"][dim]["Length"]
+                    ):
                         dimlengths[dim] = int(val["dimensions"][dim]["Length"])
     for key, value in dimension_lengths.items():
         if key not in dimlengths.keys():
             dimlengths[key] = value
     for dim in all_dimensions:
         if dim not in dimlengths.keys():
             length = input(f"Enter length for dimension {dim}: ")
@@ -427,15 +444,18 @@
     all_dimensions = []
     dimlengths = {}
     for key, val in instrument_dict.items():
         if "dimensions" in val.keys() and (key in products or key == "common"):
             for dim in list(val["dimensions"].keys()):
                 if dim not in all_dimensions:
                     all_dimensions.append(dim)
-                    if "<" not in val["dimensions"][dim]["Length"]:
+                    if (
+                        isinstance(val["dimensions"][dim]["Length"], int)
+                        or "<" not in val["dimensions"][dim]["Length"]
+                    ):
                         dimlengths[dim] = int(val["dimensions"][dim]["Length"])
     for key, value in dimension_lengths.items():
         if key not in dimlengths.keys():
             dimlengths[key] = value
     for dim in all_dimensions:
         if dim not in dimlengths.keys():
             length = input(f"Enter length for dimension {dim}: ")
```

### Comparing `ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template/remove_empty_variables.py` & `ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template/remove_empty_variables.py`

 * *Files identical despite different names*

### Comparing `ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template/tsv2dict.py` & `ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template/tsv2dict.py`

 * *Files identical despite different names*

### Comparing `ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template/util.py` & `ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template/util.py`

 * *Files identical despite different names*

### Comparing `ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template/values.py` & `ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template/values.py`

 * *Files identical despite different names*

### Comparing `ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template.egg-info/PKG-INFO` & `ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncas-amof-netcdf-template
-Version: 2.2.1
+Version: 2.2.2
 Summary: Package to create NCAS AMOF netCDF files.
 Author-email: "Joshua M. Ralph-Hampton" <joshua.hampton@ncas.ac.uk>
 License: MIT License
         
         Copyright (c) 2023 Joshua Hampton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ncas_amof_netcdf_template-2.2.1/src/ncas_amof_netcdf_template.egg-info/SOURCES.txt` & `ncas_amof_netcdf_template-2.2.2/src/ncas_amof_netcdf_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ncas_amof_netcdf_template-2.2.1/tests/test_create_netcdf.py` & `ncas_amof_netcdf_template-2.2.2/tests/test_create_netcdf.py`

 * *Files identical despite different names*

