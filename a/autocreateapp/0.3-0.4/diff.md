# Comparing `tmp/autocreateapp-0.3.tar.gz` & `tmp/autocreateapp-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocreateapp-0.3.tar", last modified: Wed Jul 26 09:31:12 2023, max compression
+gzip compressed data, was "autocreateapp-0.4.tar", last modified: Wed Jul 26 10:10:18 2023, max compression
```

## Comparing `autocreateapp-0.3.tar` & `autocreateapp-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 asc       (1000) asc       (1000)        0 2023-07-26 09:31:12.081260 autocreateapp-0.3/
--rw-rw-r--   0 asc       (1000) asc       (1000)     3552 2023-07-26 09:31:12.081260 autocreateapp-0.3/PKG-INFO
--rw-rw-r--   0 asc       (1000) asc       (1000)     2836 2023-07-26 09:30:19.000000 autocreateapp-0.3/README.md
-drwxrwxr-x   0 asc       (1000) asc       (1000)        0 2023-07-26 09:31:12.077260 autocreateapp-0.3/autocreateapp/
--rw-rw-r--   0 asc       (1000) asc       (1000)        0 2023-07-26 08:44:37.000000 autocreateapp-0.3/autocreateapp/__init__.py
--rw-rw-r--   0 asc       (1000) asc       (1000)     2488 2023-07-26 08:55:05.000000 autocreateapp-0.3/autocreateapp/create_project.py
-drwxrwxr-x   0 asc       (1000) asc       (1000)        0 2023-07-26 09:31:12.081260 autocreateapp-0.3/autocreateapp.egg-info/
--rw-rw-r--   0 asc       (1000) asc       (1000)     3552 2023-07-26 09:31:11.000000 autocreateapp-0.3/autocreateapp.egg-info/PKG-INFO
--rw-rw-r--   0 asc       (1000) asc       (1000)      300 2023-07-26 09:31:12.000000 autocreateapp-0.3/autocreateapp.egg-info/SOURCES.txt
--rw-rw-r--   0 asc       (1000) asc       (1000)        1 2023-07-26 09:31:11.000000 autocreateapp-0.3/autocreateapp.egg-info/dependency_links.txt
--rw-rw-r--   0 asc       (1000) asc       (1000)       86 2023-07-26 09:31:11.000000 autocreateapp-0.3/autocreateapp.egg-info/entry_points.txt
--rw-rw-r--   0 asc       (1000) asc       (1000)        7 2023-07-26 09:31:11.000000 autocreateapp-0.3/autocreateapp.egg-info/requires.txt
--rw-rw-r--   0 asc       (1000) asc       (1000)       14 2023-07-26 09:31:11.000000 autocreateapp-0.3/autocreateapp.egg-info/top_level.txt
--rw-rw-r--   0 asc       (1000) asc       (1000)       38 2023-07-26 09:31:12.081260 autocreateapp-0.3/setup.cfg
--rw-rw-r--   0 asc       (1000) asc       (1000)      610 2023-07-26 09:30:54.000000 autocreateapp-0.3/setup.py
+drwxrwxr-x   0 asc       (1000) asc       (1000)        0 2023-07-26 10:10:18.053030 autocreateapp-0.4/
+-rw-rw-r--   0 asc       (1000) asc       (1000)     3130 2023-07-26 10:10:18.049030 autocreateapp-0.4/PKG-INFO
+-rw-rw-r--   0 asc       (1000) asc       (1000)     2454 2023-07-26 10:09:03.000000 autocreateapp-0.4/README.md
+drwxrwxr-x   0 asc       (1000) asc       (1000)        0 2023-07-26 10:10:18.049030 autocreateapp-0.4/autocreateapp/
+-rw-rw-r--   0 asc       (1000) asc       (1000)        0 2023-07-26 08:44:37.000000 autocreateapp-0.4/autocreateapp/__init__.py
+-rw-rw-r--   0 asc       (1000) asc       (1000)     2488 2023-07-26 08:55:05.000000 autocreateapp-0.4/autocreateapp/create_project.py
+drwxrwxr-x   0 asc       (1000) asc       (1000)        0 2023-07-26 10:10:18.049030 autocreateapp-0.4/autocreateapp.egg-info/
+-rw-rw-r--   0 asc       (1000) asc       (1000)     3130 2023-07-26 10:10:17.000000 autocreateapp-0.4/autocreateapp.egg-info/PKG-INFO
+-rw-rw-r--   0 asc       (1000) asc       (1000)      300 2023-07-26 10:10:18.000000 autocreateapp-0.4/autocreateapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 asc       (1000) asc       (1000)        1 2023-07-26 10:10:17.000000 autocreateapp-0.4/autocreateapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 asc       (1000) asc       (1000)       86 2023-07-26 10:10:17.000000 autocreateapp-0.4/autocreateapp.egg-info/entry_points.txt
+-rw-rw-r--   0 asc       (1000) asc       (1000)        7 2023-07-26 10:10:17.000000 autocreateapp-0.4/autocreateapp.egg-info/requires.txt
+-rw-rw-r--   0 asc       (1000) asc       (1000)       14 2023-07-26 10:10:17.000000 autocreateapp-0.4/autocreateapp.egg-info/top_level.txt
+-rw-rw-r--   0 asc       (1000) asc       (1000)       38 2023-07-26 10:10:18.053030 autocreateapp-0.4/setup.cfg
+-rw-rw-r--   0 asc       (1000) asc       (1000)      610 2023-07-26 10:09:06.000000 autocreateapp-0.4/setup.py
```

### Comparing `autocreateapp-0.3/PKG-INFO` & `autocreateapp-0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,63 @@
-Metadata-Version: 2.1
-Name: autocreateapp
-Version: 0.3
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Description: # AutoCreateApp - Django Project Automation
-        
-        ![AutoCreateApp Logo](https://your-domain.com/path/to/your/logo.png)
-        
-        AutoCreateApp is a Python package that automates the process of creating Django projects with multiple apps and models based on user input. With this tool, you can quickly set up Django projects without manually creating apps, models, and migration files.
-        
-        ## Installation
-        
-        You can install AutoCreateApp via pip:
-        
-        ```bash
-        pip install autocreateapp
-        ```
-        
-        ## Usage
-        
-        Once AutoCreateApp is installed, you can use the `autocreateapp` command to create your Django project interactively.
-        
-        ```bash
-        autocreateapp
-        ```
-        
-        Follow the prompts to provide the project name, the number of apps to create, app names, model names, and model fields. The package will automatically generate the necessary files and set up the Django project with your specified apps and models.
-        
-        ## How It Works
-        
-        AutoCreateApp uses Python's built-in `os` module to create and navigate directories, and it utilizes Django's command-line tools (`django-admin` and `manage.py`) to create projects, apps, and migration files.
-        
-        The `add_app_to_installed_apps` function ensures that the newly created apps are added to the `INSTALLED_APPS` list in the Django project's `settings.py` file.
-        
-        The package also supports interactive model creation, allowing you to specify model names and their respective fields, such as strings (`CharField`) or integers (`IntegerField`).
-        
-        ## Example
-        
-        Here's a simple example of how to use AutoCreateApp:
-        
-        ```bash
-        # Create a new Django project with two apps and models
-        autocreateapp
-        Enter the name of your Django project: myproject
-        How many apps do you want to create? 2
-        
-        Enter the name of your app: app1
-        Enter the name of your app: app2
-        
-        Enter the name of your first model in app1: MyModel
-        Enter model fields (comma-separated, e.g., name:str, age:int): name:str, age:int
-        
-        Enter the name of your first model in app2: AnotherModel
-        Enter model fields (comma-separated, e.g., title:str, description:str): title:str, description:str
-        ```
-        
-        After the above steps, you'll have a new Django project called `myproject`, with two apps (`app1` and `app2`), each containing one model (`MyModel` and `AnotherModel`) with the specified fields.
-        
-        ## License
-        
-        AutoCreateApp is distributed under the MIT License. See the [LICENSE](LICENSE) file for more information.
-        
-        ## Contributions
-        
-        Contributions are welcome! If you have any suggestions, bug reports, or improvements, please open an issue or submit a pull request.
-        
-        ---
-        
-        Happy coding! 🚀
-        ```
-        
-        Please replace the logo image URL and the license information as per your requirements. Make sure to replace any placeholders with relevant information about your package. This `README.md` file will provide a clear and concise overview of your package's functionality and how users can get started with it.
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# AutoCreateApp - Django Project Automation
+
+AutoCreateApp is a Python package that automates the process of creating Django projects with multiple apps and models based on user input. With this tool, you can quickly set up Django projects without manually creating apps, models, and migration files.
+
+## Installation
+
+You can install AutoCreateApp via pip:
+
+```bash
+pip install autocreateapp
+```
+
+## Usage
+
+Once AutoCreateApp is installed, you can use the `autocreateapp` command to create your Django project interactively.
+
+```bash
+autocreateapp
+```
+
+Follow the prompts to provide the project name, the number of apps to create, app names, model names, and model fields. The package will automatically generate the necessary files and set up the Django project with your specified apps and models.
+
+## How It Works
+
+AutoCreateApp uses Python's built-in `os` module to create and navigate directories, and it utilizes Django's command-line tools (`django-admin` and `manage.py`) to create projects, apps, and migration files.
+
+The `add_app_to_installed_apps` function ensures that the newly created apps are added to the `INSTALLED_APPS` list in the Django project's `settings.py` file.
+
+The package also supports interactive model creation, allowing you to specify model names and their respective fields, such as strings (`CharField`) or integers (`IntegerField`).
+
+## Example
+
+Here's a simple example of how to use AutoCreateApp:
+
+```bash
+# Create a new Django project with two apps and models
+autocreateapp
+Enter the name of your Django project: myproject
+How many apps do you want to create? 2
+
+Enter the name of your app: app1
+Enter the name of your app: app2
+
+Enter the name of your first model in app1: MyModel
+Enter model fields (comma-separated, e.g., name:str, age:int): name:str, age:int
+
+Enter the name of your first model in app2: AnotherModel
+Enter model fields (comma-separated, e.g., title:str, description:str): title:str, description:str
+```
+
+After the above steps, you'll have a new Django project called `myproject`, with two apps (`app1` and `app2`), each containing one model (`MyModel` and `AnotherModel`) with the specified fields.
+
+## License
+
+AutoCreateApp is distributed under the MIT License. See the [LICENSE](LICENSE) file for more information.
+
+## Contributions
+
+Contributions are welcome! If you have any suggestions, bug reports, or improvements, please open an issue or submit a pull request.
+
+---
+
+Happy coding! 🚀
```

### Comparing `autocreateapp-0.3/README.md` & `autocreateapp-0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,71 @@
-# AutoCreateApp - Django Project Automation
-
-![AutoCreateApp Logo](https://your-domain.com/path/to/your/logo.png)
-
-AutoCreateApp is a Python package that automates the process of creating Django projects with multiple apps and models based on user input. With this tool, you can quickly set up Django projects without manually creating apps, models, and migration files.
-
-## Installation
-
-You can install AutoCreateApp via pip:
-
-```bash
-pip install autocreateapp
-```
-
-## Usage
-
-Once AutoCreateApp is installed, you can use the `autocreateapp` command to create your Django project interactively.
-
-```bash
-autocreateapp
-```
-
-Follow the prompts to provide the project name, the number of apps to create, app names, model names, and model fields. The package will automatically generate the necessary files and set up the Django project with your specified apps and models.
-
-## How It Works
-
-AutoCreateApp uses Python's built-in `os` module to create and navigate directories, and it utilizes Django's command-line tools (`django-admin` and `manage.py`) to create projects, apps, and migration files.
-
-The `add_app_to_installed_apps` function ensures that the newly created apps are added to the `INSTALLED_APPS` list in the Django project's `settings.py` file.
-
-The package also supports interactive model creation, allowing you to specify model names and their respective fields, such as strings (`CharField`) or integers (`IntegerField`).
-
-## Example
-
-Here's a simple example of how to use AutoCreateApp:
-
-```bash
-# Create a new Django project with two apps and models
-autocreateapp
-Enter the name of your Django project: myproject
-How many apps do you want to create? 2
-
-Enter the name of your app: app1
-Enter the name of your app: app2
-
-Enter the name of your first model in app1: MyModel
-Enter model fields (comma-separated, e.g., name:str, age:int): name:str, age:int
-
-Enter the name of your first model in app2: AnotherModel
-Enter model fields (comma-separated, e.g., title:str, description:str): title:str, description:str
-```
-
-After the above steps, you'll have a new Django project called `myproject`, with two apps (`app1` and `app2`), each containing one model (`MyModel` and `AnotherModel`) with the specified fields.
-
-## License
-
-AutoCreateApp is distributed under the MIT License. See the [LICENSE](LICENSE) file for more information.
-
-## Contributions
-
-Contributions are welcome! If you have any suggestions, bug reports, or improvements, please open an issue or submit a pull request.
-
----
-
-Happy coding! 🚀
-```
-
-Please replace the logo image URL and the license information as per your requirements. Make sure to replace any placeholders with relevant information about your package. This `README.md` file will provide a clear and concise overview of your package's functionality and how users can get started with it.
+Metadata-Version: 2.1
+Name: autocreateapp
+Version: 0.4
+Summary: UNKNOWN
+Home-page: UNKNOWN
+License: UNKNOWN
+Description: # AutoCreateApp - Django Project Automation
+        
+        AutoCreateApp is a Python package that automates the process of creating Django projects with multiple apps and models based on user input. With this tool, you can quickly set up Django projects without manually creating apps, models, and migration files.
+        
+        ## Installation
+        
+        You can install AutoCreateApp via pip:
+        
+        ```bash
+        pip install autocreateapp
+        ```
+        
+        ## Usage
+        
+        Once AutoCreateApp is installed, you can use the `autocreateapp` command to create your Django project interactively.
+        
+        ```bash
+        autocreateapp
+        ```
+        
+        Follow the prompts to provide the project name, the number of apps to create, app names, model names, and model fields. The package will automatically generate the necessary files and set up the Django project with your specified apps and models.
+        
+        ## How It Works
+        
+        AutoCreateApp uses Python's built-in `os` module to create and navigate directories, and it utilizes Django's command-line tools (`django-admin` and `manage.py`) to create projects, apps, and migration files.
+        
+        The `add_app_to_installed_apps` function ensures that the newly created apps are added to the `INSTALLED_APPS` list in the Django project's `settings.py` file.
+        
+        The package also supports interactive model creation, allowing you to specify model names and their respective fields, such as strings (`CharField`) or integers (`IntegerField`).
+        
+        ## Example
+        
+        Here's a simple example of how to use AutoCreateApp:
+        
+        ```bash
+        # Create a new Django project with two apps and models
+        autocreateapp
+        Enter the name of your Django project: myproject
+        How many apps do you want to create? 2
+        
+        Enter the name of your app: app1
+        Enter the name of your app: app2
+        
+        Enter the name of your first model in app1: MyModel
+        Enter model fields (comma-separated, e.g., name:str, age:int): name:str, age:int
+        
+        Enter the name of your first model in app2: AnotherModel
+        Enter model fields (comma-separated, e.g., title:str, description:str): title:str, description:str
+        ```
+        
+        After the above steps, you'll have a new Django project called `myproject`, with two apps (`app1` and `app2`), each containing one model (`MyModel` and `AnotherModel`) with the specified fields.
+        
+        ## License
+        
+        AutoCreateApp is distributed under the MIT License. See the [LICENSE](LICENSE) file for more information.
+        
+        ## Contributions
+        
+        Contributions are welcome! If you have any suggestions, bug reports, or improvements, please open an issue or submit a pull request.
+        
+        ---
+        
+        Happy coding! 🚀
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `autocreateapp-0.3/autocreateapp/create_project.py` & `autocreateapp-0.4/autocreateapp/create_project.py`

 * *Files identical despite different names*

### Comparing `autocreateapp-0.3/autocreateapp.egg-info/PKG-INFO` & `autocreateapp-0.4/autocreateapp.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: autocreateapp
-Version: 0.3
+Version: 0.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # AutoCreateApp - Django Project Automation
         
-        ![AutoCreateApp Logo](https://your-domain.com/path/to/your/logo.png)
-        
         AutoCreateApp is a Python package that automates the process of creating Django projects with multiple apps and models based on user input. With this tool, you can quickly set up Django projects without manually creating apps, models, and migration files.
         
         ## Installation
         
         You can install AutoCreateApp via pip:
         
         ```bash
@@ -65,12 +63,9 @@
         ## Contributions
         
         Contributions are welcome! If you have any suggestions, bug reports, or improvements, please open an issue or submit a pull request.
         
         ---
         
         Happy coding! 🚀
-        ```
-        
-        Please replace the logo image URL and the license information as per your requirements. Make sure to replace any placeholders with relevant information about your package. This `README.md` file will provide a clear and concise overview of your package's functionality and how users can get started with it.
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `autocreateapp-0.3/setup.py` & `autocreateapp-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='autocreateapp',
-    version='0.3',  # Update the version number to 0.2 (or any desired version)
+    version='0.4',  # Update the version number to 0.2 (or any desired version)
     packages=find_packages(),
     install_requires=[
         'Django',
     ],
     entry_points={
         'console_scripts': [
             'autocreateapp=autocreateapp.create_project:create_django_project',
```

