# Comparing `tmp/pyDolarVenezuela-1.0.6-py3-none-any.whl.zip` & `tmp/pyDolarVenezuela-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 4997 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       68 b- defN 23-Jul-14 18:45 pyDolarVenezuela/__init__.py
--rw-rw-rw-  2.0 fat      216 b- defN 23-Jul-14 18:45 pyDolarVenezuela/request.py
--rw-rw-rw-  2.0 fat     1597 b- defN 23-Jul-14 18:58 pyDolarVenezuela/scraping_bcv.py
--rw-rw-rw-  2.0 fat     1351 b- defN 23-Jul-14 18:56 pyDolarVenezuela/scraping_monitor.py
--rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-14 19:00 pyDolarVenezuela-1.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2579 b- defN 23-Jul-14 19:00 pyDolarVenezuela-1.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 19:00 pyDolarVenezuela-1.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-14 19:00 pyDolarVenezuela-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      779 b- defN 23-Jul-14 19:00 pyDolarVenezuela-1.0.6.dist-info/RECORD
-9 files, 7793 bytes uncompressed, 3637 bytes compressed:  53.3%
+Zip file size: 5951 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat       98 b- defN 23-Jul-26 05:29 pyDolarVenezuela/__init__.py
+-rw-rw-rw-  2.0 fat      389 b- defN 23-Jul-26 03:29 pyDolarVenezuela/module_bcv.py
+-rw-rw-rw-  2.0 fat      573 b- defN 23-Jul-26 04:17 pyDolarVenezuela/request.py
+-rw-rw-rw-  2.0 fat     2584 b- defN 23-Jul-26 06:02 pyDolarVenezuela/scraping_monitor.py
+-rw-rw-rw-  2.0 fat       81 b- defN 23-Jul-26 04:18 pyDolarVenezuela/util.py
+-rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-26 06:24 pyDolarVenezuela-1.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3533 b- defN 23-Jul-26 06:24 pyDolarVenezuela-1.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-26 06:24 pyDolarVenezuela-1.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-26 06:24 pyDolarVenezuela-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      855 b- defN 23-Jul-26 06:24 pyDolarVenezuela-1.0.7.dist-info/RECORD
+10 files, 9316 bytes uncompressed, 4471 bytes compressed:  52.0%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: pyDolarVenezuela/__init__.py
 Comment: 
 
-Filename: pyDolarVenezuela/request.py
+Filename: pyDolarVenezuela/module_bcv.py
 Comment: 
 
-Filename: pyDolarVenezuela/scraping_bcv.py
+Filename: pyDolarVenezuela/request.py
 Comment: 
 
 Filename: pyDolarVenezuela/scraping_monitor.py
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.6.dist-info/LICENSE
+Filename: pyDolarVenezuela/util.py
+Comment: 
+
+Filename: pyDolarVenezuela-1.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.6.dist-info/METADATA
+Filename: pyDolarVenezuela-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.6.dist-info/WHEEL
+Filename: pyDolarVenezuela-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.6.dist-info/top_level.txt
+Filename: pyDolarVenezuela-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.6.dist-info/RECORD
+Filename: pyDolarVenezuela-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyDolarVenezuela/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .scraping_bcv import Bcv
-from .scraping_monitor import Monitor
+from pyDolarVenezuela.module_bcv import Bcv
+from pyDolarVenezuela.scraping_monitor import Monitor
```

## pyDolarVenezuela/request.py

```diff
@@ -1,6 +1,14 @@
 import requests
+from requests import Response
 
-def _get_response_content(response: requests.Response):
+# headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3'}
+
+def ensure_200_and_return_content(response: Response) -> bytes:
     if not response.status_code == requests.codes.ok:
-        raise ValueError("Connection error on the page")
-    return response.content
+        raise ValueError("Error de comunicación Alcambio. Codigo: {0}".format(response.status_code))
+    return response.content
+
+def get_content_page(url: str) -> bytes:
+    return ensure_200_and_return_content(
+        requests.get(url=url)
+    )
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## pyDolarVenezuela/scraping_monitor.py

```diff
@@ -1,31 +1,48 @@
-import requests
 from bs4 import BeautifulSoup
 
-from .request import _get_response_content
+from pyDolarVenezuela.request import get_content_page
+from pyDolarVenezuela.util import PAGINA_PRINCIPAL_EXCHANGE_MONITOR
 
-class Monitor:
-    def __init__(self) -> None:
-        self.website = 'https://monitordolarvenezuela.com/'
+def _get_values_monitors(soup: BeautifulSoup):
+    return [value for value in soup]
 
-    def _get_content(self, url: str):
-        return _get_response_content(requests.get(url))
-    
-    def _get_results_price(self, soup: BeautifulSoup):
-        return [str(x.find('p').text).split(' ')[-1].replace(',', '.') for x in soup.find_all('div', 'col-12 col-sm-4 col-md-2 col-lg-2')]
-    
-    def get_value_monitors(self, monitor_code: str = None, prettify: bool = False):
-        page = self._get_content(self.website)
-        soup = BeautifulSoup(page, features='html.parser')
+class Monitor(object):
+    """
+    La clase Monitor permite consultar los precios del dólar en diversos monitores en Venezuela. \n
+    El método `_load` carga los datos de los monitores a través del scraping de la página web de referencia, donde los datos son almacenados en un diccionario. \ 
+    El método `get_value_monitors` permite acceder a los datos almacenados en el diccionario.
+    """
+    def _load(self):
+        soup = BeautifulSoup(get_content_page(PAGINA_PRINCIPAL_EXCHANGE_MONITOR), "html.parser")
+        section_dolar_venezuela = soup.find_all("div", "col-xs-12 col-sm-6 col-md-4 col-tabla")
+        all_monitors = _get_values_monitors(section_dolar_venezuela)
 
-        results = {
-            'enparalelovzla': self._get_results_price(soup)[1],
-            'monitordolarweb': self._get_results_price(soup)[3],
-            'enparalelovzlavip': self._get_results_price(soup)[4],
-            'binance': self._get_results_price(soup)[5]
-        }
+        self.all_monitors = {}
+        i: int = 0
+        for monitor in all_monitors:
+            monitor = monitor.find("div", "module-table module-table-fecha")
+            data = {
+                "name": monitor.find('h6', 'nombre').text,
+                "unit": monitor.find('p', 'unidad').text,
+                "price": str(monitor.find('p', 'precio').text).replace(',', '.'),
+                "last_update": monitor.find('p', 'fecha').text
+            }
+            self.all_monitors[i] = data
+            i += 1
+    
+    def get_value_monitors(self, monitor_code: int = None, name_property: str = None, prettify: bool = False):
+        """
+        El parámetro `monitor_code` indica el código del monitor del cual se desea obtener información, \
+        mientras que el parámetro `prettify` permite mostrar los precios en formato de moneda con el símbolo de Bolívares. \
+        Si se proporciona un nombre de propiedad válido, se devolverá el valor correspondiente para ese monitor.
+        """
+        self._load()
 
         if not monitor_code:
-            return results
-        if monitor_code not in results:
-            raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pydolarvenezuela")
-        return results[monitor_code] if not prettify else f'Bs. {results[monitor_code]}'
+            return self.all_monitors
+        if monitor_code not in self.all_monitors:
+            raise ValueError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pyDolarVenezuela")
+        
+        return (f"Bs. {self.all_monitors[monitor_code][name_property]}" if prettify and name_property == "price"
+                else self.all_monitors[monitor_code][name_property] if name_property in self.all_monitors[monitor_code]
+                else self.all_monitors[monitor_code])
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `pyDolarVenezuela-1.0.6.dist-info/LICENSE` & `pyDolarVenezuela-1.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

