# Comparing `tmp/hellow_worldo-0.0.16.tar.gz` & `tmp/hellow_worldo-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hellow_worldo-0.0.16.tar", last modified: Wed Jul 26 17:31:35 2023, max compression
+gzip compressed data, was "hellow_worldo-0.0.17.tar", last modified: Wed Jul 26 17:34:19 2023, max compression
```

## Comparing `hellow_worldo-0.0.16.tar` & `hellow_worldo-0.0.17.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 17:31:35.773956 hellow_worldo-0.0.16/
--rw-rw-rw-   0        0        0     2576 2023-07-26 17:31:35.771824 hellow_worldo-0.0.16/PKG-INFO
--rw-rw-rw-   0        0        0     2008 2023-07-26 17:20:02.000000 hellow_worldo-0.0.16/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-26 17:31:35.720821 hellow_worldo-0.0.16/helloCode/
--rw-rw-rw-   0        0        0        0 2023-07-26 15:34:21.000000 hellow_worldo-0.0.16/helloCode/__init__.py
--rw-rw-rw-   0        0        0      256 2023-07-26 15:32:32.000000 hellow_worldo-0.0.16/helloCode/hello.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:31:35.763826 hellow_worldo-0.0.16/hellow_worldo.egg-info/
--rw-rw-rw-   0        0        0     2576 2023-07-26 17:31:35.000000 hellow_worldo-0.0.16/hellow_worldo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-07-26 17:31:35.000000 hellow_worldo-0.0.16/hellow_worldo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 17:31:35.000000 hellow_worldo-0.0.16/hellow_worldo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-26 17:31:35.000000 hellow_worldo-0.0.16/hellow_worldo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 17:31:35.775828 hellow_worldo-0.0.16/setup.cfg
--rw-rw-rw-   0        0        0      989 2023-07-26 17:30:43.000000 hellow_worldo-0.0.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:34:19.118939 hellow_worldo-0.0.17/
+-rw-rw-rw-   0        0        0     2027 2023-07-26 17:34:19.116907 hellow_worldo-0.0.17/PKG-INFO
+-rw-rw-rw-   0        0        0     1459 2023-07-26 17:33:59.000000 hellow_worldo-0.0.17/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-26 17:34:19.018908 hellow_worldo-0.0.17/helloCode/
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:34:21.000000 hellow_worldo-0.0.17/helloCode/__init__.py
+-rw-rw-rw-   0        0        0      256 2023-07-26 17:32:53.000000 hellow_worldo-0.0.17/helloCode/hello.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:34:19.108904 hellow_worldo-0.0.17/hellow_worldo.egg-info/
+-rw-rw-rw-   0        0        0     2027 2023-07-26 17:34:18.000000 hellow_worldo-0.0.17/hellow_worldo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-07-26 17:34:18.000000 hellow_worldo-0.0.17/hellow_worldo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:34:18.000000 hellow_worldo-0.0.17/hellow_worldo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-26 17:34:18.000000 hellow_worldo-0.0.17/hellow_worldo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 17:34:19.123439 hellow_worldo-0.0.17/setup.cfg
+-rw-rw-rw-   0        0        0      989 2023-07-26 17:34:03.000000 hellow_worldo-0.0.17/setup.py
```

### Comparing `hellow_worldo-0.0.16/README.rst` & `hellow_worldo-0.0.17/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,86 +1,55 @@
 My FastAPI Application
 ======================
 
-Introduction
-------------
-
-My FastAPI Application is a simple web application built using FastAPI, a modern, fast, and web-based API framework for Python. The application exposes a single endpoint that returns a greeting message.
+A simple FastAPI application that prints "Hello, World!" when accessed.
 
 Installation
 ------------
 
-1. Make sure you have Python 3.7 or later installed on your system.
-
-2. Install the required dependencies by running the following command:
-
-   .. code-block:: bash
-
-      pip install fastapi uvicorn
-
-3. Clone the repository or download the source code of the application.
+You can install the package using `pip`:
 
-4. Change into the project directory:
-
-   .. code-block:: bash
+.. code-block:: bash
 
-      cd path/to/my_fastapi_app
+   pip install hellow_worldo
 
 Usage
 -----
 
-To run the FastAPI application, execute the following command:
+Once the package is installed, you can import and use it in your Python scripts or projects.
 
-.. code-block:: bash
+Import the package in your script:
 
-   uvicorn myapp:app --host 0.0.0.0 --port 8000
+.. code-block:: python
 
-The application will start running, and you can access it by navigating to ``http://localhost:8000/`` in your web browser or using an API client like curl or Postman.
+   from hellow_worldo import print_hello
 
-Endpoints
----------
+Use the function to print the greeting:
 
-- GET `/`: Returns a greeting message.
+.. code-block:: python
 
-API Response Example
---------------------
+   response = print_hello()
+   print(response)  # Output: {'data': 'Hellow Worldo..'}
 
-.. code-block:: json
 
-   {
-       "data": "Hellow Worldo.."
-   }
+Running the Application
+-----------------------
 
-Contributing
-------------
+To run the FastAPI application, execute the following command in your terminal:
 
-If you would like to contribute to this project, please follow these steps:
-
-1. Fork the repository and create a new branch.
-
-2. Make your changes and write tests if applicable.
-
-3. Ensure that all tests pass by running:
-
-   .. code-block:: bash
+.. code-block:: bash
 
-      pytest
+   uvicorn myapp:app --host 0.0.0.0 --port 8000
 
-4. Commit your changes and push them to your fork.
+Replace ``myapp`` with the name of your Python script containing the FastAPI application (the script where you define the FastAPI app using ``app = FastAPI()``).
 
-5. Create a pull request from your branch to the main repository.
+Once the application is running, you can access it by navigating to ``http://localhost:8000/`` in your web browser or using an API client like curl or Postman.
 
-Support
--------
+Contributing
+------------
 
-If you encounter any issues or have questions about the application, feel free to open an issue on the GitHub repository.
+If you would like to contribute to this project or report any issues, please visit the GitHub repository: https://github.com/yourusername/your-repo
 
 License
 -------
 
-This project is licensed under the MIT License. See the LICENSE file for more details.
-
-Acknowledgments
----------------
-
-- FastAPI: https://fastapi.tiangolo.com
-- Uvicorn: https://www.uvicorn.org
+This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `hellow_worldo-0.0.16/setup.py` & `hellow_worldo-0.0.17/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 DESCRIPTION = 'hello world'
 LONG_DESCRIPTION = 'A package that allows showing hellow worldo.'
 
 # Setting up
 setup(
     name="hellow_worldo",
-    version="0.0.16",
+    version="0.0.17",
     author="RohitMishra (The Great DEV)",
     author_email="RKMDEV@DEV.com",
     description=DESCRIPTION,
     long_description_content_type="text/plain",  # Use text/plain for reST
     long_description=long_description,
     packages=find_packages(),
     install_requires=[],  # Replace with actual dependencies if needed
```

