# Comparing `tmp/pyBCV-1.0.7-py3-none-any.whl.zip` & `tmp/pyBCV-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6253 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       25 b- defN 23-Apr-27 21:59 pyBCV/__init__.py
--rw-rw-rw-  2.0 fat     6498 b- defN 23-Apr-27 21:59 pyBCV/pyBCV.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-27 21:56 pyBCV/core/__init__.py
--rw-rw-rw-  2.0 fat      856 b- defN 23-Apr-27 20:51 pyBCV/core/requests.py
--rw-rw-rw-  2.0 fat     1094 b- defN 23-Apr-28 01:43 pyBCV-1.0.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4177 b- defN 23-Apr-28 01:43 pyBCV-1.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 01:43 pyBCV-1.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-28 01:43 pyBCV-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      672 b- defN 23-Apr-28 01:43 pyBCV-1.0.7.dist-info/RECORD
-9 files, 13420 bytes uncompressed, 5099 bytes compressed:  62.0%
+Zip file size: 5790 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       38 b- defN 23-Jul-25 06:44 pyBCV/__init__.py
+-rw-rw-rw-  2.0 fat     5049 b- defN 23-Jul-25 06:43 pyBCV/pyBCV.py
+-rw-rw-rw-  2.0 fat      449 b- defN 23-Jul-25 05:18 pyBCV/requests.py
+-rw-rw-rw-  2.0 fat      135 b- defN 23-Jul-25 05:16 pyBCV/util.py
+-rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-25 07:05 pyBCV-1.0.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3677 b- defN 23-Jul-25 07:05 pyBCV-1.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-25 07:05 pyBCV-1.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-25 07:05 pyBCV-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      660 b- defN 23-Jul-25 07:05 pyBCV-1.0.8.dist-info/RECORD
+9 files, 11200 bytes uncompressed, 4664 bytes compressed:  58.4%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: pyBCV/__init__.py
 Comment: 
 
 Filename: pyBCV/pyBCV.py
 Comment: 
 
-Filename: pyBCV/core/__init__.py
+Filename: pyBCV/requests.py
 Comment: 
 
-Filename: pyBCV/core/requests.py
+Filename: pyBCV/util.py
 Comment: 
 
-Filename: pyBCV-1.0.7.dist-info/LICENSE
+Filename: pyBCV-1.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: pyBCV-1.0.7.dist-info/METADATA
+Filename: pyBCV-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: pyBCV-1.0.7.dist-info/WHEEL
+Filename: pyBCV-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: pyBCV-1.0.7.dist-info/top_level.txt
+Filename: pyBCV-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: pyBCV-1.0.7.dist-info/RECORD
+Filename: pyBCV-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyBCV/__init__.py

```diff
@@ -1 +1 @@
-from pyBCV.pyBCV import *
+from pyBCV.pyBCV import Currency, Bank
```

## pyBCV/pyBCV.py

```diff
@@ -1,195 +1,106 @@
-import locale
-from decimal import Decimal
-from typing import Any, Callable
-from datetime import datetime, timedelta
-
 from bs4 import BeautifulSoup
 
-from pyBCV.core.requests import BCVRequests
-
-def _extract_timestamp(soup: BeautifulSoup) -> datetime:
-    try:
-        return datetime.fromisoformat(
-            soup.find("span", "date-display-single").get("content")
-        )
-    except:
-        return None
-
-def _formatted_date(soup: BeautifulSoup) -> str:
-    locale.setlocale(locale.LC_TIME, 'es_MX.UTF-8')
-    current_date = _extract_timestamp(soup)
-    day_weekday = current_date.weekday()
-
-    day_name = (
-        'Lunes' if day_weekday == 0 else
-        'Martes' if day_weekday == 1 else
-        'Miercoles' if day_weekday == 2 else
-        'Jueves' if day_weekday == 3 else
-        'Viernes'
-    )
-
-    if current_date is not None:
-        return current_date.strftime(f'{day_name}, %d %B del %Y')
-
-def _get_rate_by_id(tag_id: str, soup: BeautifulSoup) -> Decimal:
-    try:
-        rate_value = soup.find(id=tag_id).find("strong").text.strip().replace(",", ".")
-        rate_value = Decimal(rate_value)
-    except:
-        rate_value = None
+from pyBCV.requests import get_content_page
+from pyBCV.util import (
+    TASAS_INFORMATIVAS_URL,
+    PAGINA_PRINCIPAL_URL
+)
+
+def _get_rate_by_id(tag_id: str, soup: BeautifulSoup):
+    return soup.find(id=tag_id).find("strong").text.strip().replace(',', '.')
 
-    return rate_value
+def _get_time(soup: BeautifulSoup):
+    return soup.find("span", "date-display-single").text.strip()
 
+def _get_rates_with_for(soup: BeautifulSoup, name: str = "td", attrs: str = None):
+    return [str(x.text).strip() for x in soup.find_all(name, attrs)]
 
-class Currency:
+class Currency(object):
     """
-    `pyBCV.Currency()`. Es la instancia principal para obtener los datos de tipo de cambio del BCV.\n
-    https://github.com/fcoagz/pyBCV#uso
-
-    ```py
+    La clase Currency se utiliza para obtener los precios de los tipos de cambio \
+    proporcionados por el Banco Central de Venezuela (BCV). \n
+    - El método _load se encarga de obtener los datos de la página web y almacenarlos en el diccionario self.rates. \n
+    - El método get_rate se utiliza para obtener los datos almacenados en el diccionario self.rates. Si se proporciona un código de moneda, devolverá el valor correspondiente para esa moneda. \n\n
+    ```python
     import pyBCV
 
-    bcv = pyBCV.Currency()
-    bcv.get_rate(currency_code='USD')
+    currency = pyBCV.Currency()
+
+    # Obtener todos los datos almacenados en el diccionario
+    all_rates = currency.get_rate()
+    print(all_rates)
+
+    # Obtener el tipo de cambio para USD sin símbolo de moneda
+    usd_rate = currency.get_rate(currency_code='USD', prettify=False)
+    print(usd_rate)
+
+    # Obtener la fecha de la última actualización
+    last_update = currency.get_rate(currency_code='Fecha')
+    print(last_update)
     ```
     """
-
-    def __init__(
-        self,
-        refresh_period: timedelta = timedelta(hours=1),
-        lazy_load: bool = False,
-    ):
-        self.refresh_period = refresh_period
-        self.rates = {}
-        self.loaded = False
-        self.last_request_timestamp = None
-        self.lazy_load = lazy_load
-        if not self.lazy_load:
-            self._load()
-
-    def _load(self):
-        self.loaded = False
-        if (
-            self.last_request_timestamp
-            and (datetime.now() - self.last_request_timestamp) < self.refresh_period
-        ):
-            return
-
-        soup = BeautifulSoup(BCVRequests.get_main_page(), "html.parser")
-        section_tipo_de_cambio_oficial = soup.find(
-            "div", "view-tipo-de-cambio-oficial-del-bcv"
-        )
+    def _load(self) -> None:
+        soup = BeautifulSoup(get_content_page(PAGINA_PRINCIPAL_URL), "html.parser")
+        section_tipo_de_cambio_oficial = soup.find("div", "view-tipo-de-cambio-oficial-del-bcv")
 
         self.rates = {
             "EUR": _get_rate_by_id("euro", section_tipo_de_cambio_oficial),
             "CNY": _get_rate_by_id("yuan", section_tipo_de_cambio_oficial),
             "TRY": _get_rate_by_id("lira", section_tipo_de_cambio_oficial),
             "RUB": _get_rate_by_id("rublo", section_tipo_de_cambio_oficial),
             "USD": _get_rate_by_id("dolar", section_tipo_de_cambio_oficial),
-            "Fecha": [_extract_timestamp(section_tipo_de_cambio_oficial), _formatted_date(section_tipo_de_cambio_oficial)]
-        }
-        self.loaded = True
-        self.last_request_timestamp = datetime.now()
-
-    def _pretty_rates(self) -> dict[str, str]:
-        return {
-            k: (f"Bs {value}" if k != "Fecha" else value.isoformat())
-            for k, value in self.rates.items()
+            "Fecha": _get_time(section_tipo_de_cambio_oficial)
         }
 
-    def get_rate(
-        self, currency_code: str = None, prettify: bool = False, date_format: bool = True
-    ) -> dict[str, str] | str | dict[str, float] | float:
-        """
-        El módulo `get_rate()` acepta un código de moneda como argumento y devuelve
-        la tasa de cambio actual de esa moneda.
-        """
-
-        if (
-            not self.last_request_timestamp
-            or (datetime.now() - self.last_request_timestamp) >= self.refresh_period
-        ):
-            self._load()
-
-        if currency_code == 'Fecha':
-            return self.rates[currency_code][0] if not date_format else self.rates[currency_code][1]
+    def get_rate(self, currency_code: str = None, prettify: bool = True):
+        self._load()
 
         if not currency_code:
-            return self.rates if not prettify else self._pretty_rates()
-
-        return (
-            self.rates[currency_code]
-            if not prettify
-            else f"Bs. {self.rates[currency_code]}"
-        )
-
+            return self.rates
+        if currency_code not in self.rates:
+            raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pyBCV")
+        
+        return (self.rates[currency_code] if currency_code == "Fecha" 
+                else f"Bs. {self.rates[currency_code]}" if prettify 
+                else self.rates[currency_code])
 
-class Bank:
+class Bank(object):
     """
-    `pyBCV.Bank()`. Es la segunda instancia para obtener los datos del sistema bancario del BCV.\n
-    https://github.com/fcoagz/pyBCV#uso
-
+    La clase Bank en la librería pyBCV se utiliza para obtener información sobre los tipos de cambio de compra y venta de moneda extranjera \
+    para los bancos disponibles en el sistema bancario del Banco Central de Venezuela (BCV). \n
+    - La función _load de la clase Bank utiliza el módulo BeautifulSoup para extraer la información de las tasas informativas oficiales del BCV y almacenarla en un diccionario. \n
+    - El método get_by_bank se utiliza para obtener la información de compra y venta de moneda extranjera para un banco específico o para todos los bancos disponibles. \n\n
     ```py
     import pyBCV
 
     bcv = pyBCV.Bank()
-    bcv.get_by_bank(bank_code='Banesco', rate_or_sale='Compra')
+    bank_info = bcv.get_by_bank()
+    print(bank_info)
     ```
     """
+    def _load(self):
+        section_tasas_informativas_oficial = BeautifulSoup(get_content_page(TASAS_INFORMATIVAS_URL), "html.parser")
 
-    def get_by_bank(
-        self, bank_code=None, rate_or_sale=None
-    ) -> dict[Any, dict[str, str]] | str | dict[str, str]:
-        """
-        El módulo `get_by_bank()` acepta el nombre de un banco como argumento y devuelve la fecha vigente y el sistema cambiario de compra y venta de moneda extranjera para ese banco.
-        """
-
-        soup = BeautifulSoup(BCVRequests.get_tasas_bancos(), "html.parser")
-
-        date_indicator = []
-        title_bank = []
-        rate_buys = []
-        rate_sales = []
-
-        for i in soup.find_all(
-            "td", "views-field views-field-field-fecha-del-indicador"
-        ):
-            date_indicator.append(i.text.strip())
-        for j in soup.find_all("td", "views-field views-field-views-conditional"):
-            title_bank.append(j.text.strip())
-        for k in soup.find_all("td", "views-field views-field-field-tasa-compra"):
-            rate_buys.append(k.text.strip().replace(",", "."))
-        for e in soup.find_all("td", "views-field views-field-field-tasa-venta"):
-            rate_sales.append(e.text.strip().replace(",", "."))
-
-        bank = {
-            title_bank[0]: {
-                "Fecha": date_indicator[0],
-                "Compra": f"Bs. {rate_buys[0]}",
-                "Venta": f"Bs. {rate_sales[0]}",
-            },
-            title_bank[1]: {
-                "Fecha": date_indicator[1],
-                "Compra": f"Bs. {rate_buys[1]}",
-                "Venta": f"Bs. {rate_sales[1]}",
-            },
-            title_bank[2]: {
-                "Fecha": date_indicator[2],
-                "Compra": f"Bs. {rate_buys[2]}",
-                "Venta": f"Bs. {rate_sales[2]}",
-            },
-            title_bank[3]: {
-                "Fecha": date_indicator[2],
-                "Compra": f"Bs. {rate_buys[2]}",
-                "Venta": f"Bs. {rate_sales[3]}",
-            },
-        }
-
-        if not bank_code:
-            return bank
+        date_indicator = _get_rates_with_for(section_tasas_informativas_oficial, attrs = "views-field views-field-field-fecha-del-indicador")
+        title_bank = _get_rates_with_for(section_tasas_informativas_oficial, attrs = "views-field views-field-views-conditional")
+        rate_buys = _get_rates_with_for(section_tasas_informativas_oficial, attrs = "views-field views-field-field-tasa-compra")
+        rate_sales = _get_rates_with_for(section_tasas_informativas_oficial, attrs = "views-field views-field-field-tasa-venta")
+
+        self.banks = {}
+        for i in range(10): # results: 10
+            bank = {
+                "Fecha": date_indicator[i],
+                "Compra": f"Bs. {rate_buys[i]}",
+                "Venta": f"Bs. {rate_sales[i]}",
+            }
+            self.banks[title_bank[i]] = bank
 
-        elif rate_or_sale in bank[bank_code]:
-            return bank[bank_code][rate_or_sale]
+    def get_by_bank(self, bank_code=None, rate_or_sale=None):
+        self._load()
 
-        elif bank_code in bank:
-            return bank[bank_code]
+        if not bank_code:
+            return self.banks
+        if bank_code not in self.banks:
+            raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pyBCV")
+        
+        return self.banks[bank_code][rate_or_sale] if rate_or_sale in self.banks[bank_code] else self.banks[bank_code]
```

## Comparing `pyBCV-1.0.7.dist-info/LICENSE` & `pyBCV-1.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyBCV-1.0.7.dist-info/METADATA` & `pyBCV-1.0.8.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBCV
-Version: 1.0.7
+Version: 1.0.8
 Summary: PyBCV es una librería desarrollada en el lenguaje de programación Python que se utiliza para recopilar los precios de los tipos de cambio y las tasas informativas proporcionados por el Banco Central de Venezuela (BCV).
 Home-page: https://github.com/fcoagz/pyBCV
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fcoagz/pyBCV
 Project-URL: Bug Tracker, https://github.com/fcoagz/pyBCV/issues
@@ -20,58 +20,45 @@
 Requires-Dist: beautifulsoup4
 
  <p align="center">
  <img width="300" height="170" src="pyBCV/pybcv-preview.png">
 </p>
 
 # pyBCV
-PyBCV es una librería desarrollada en el lenguaje de programación Python que se utiliza para recopilar los precios de los tipos de cambio y la tasas informativas del sistema bancario proporcionados por el Banco Central de Venezuela (BCV). Esta librería se centra específicamente en la obtención de los datos de tipos de cambio y las tasas informativas del BCV y los convierte en un formato fácilmente utilizable en Python.
+pyBCV es una librería de Python que simplifica la obtención de los precios de los tipos de cambio y las tasas informativas del sistema bancario proporcionados por el Banco Central de Venezuela (BCV) convirtiéndolos en un formato fácilmente utilizable en Python.
 
 ## Instalación
 Para instalar esta librería, puedes utilizar el siguiente comando:
 ```py
 pip install pyBCV
 ```
 Para actualizar esta librería, puedes utilizar el siguiente comando:
 ```py
 pip install pyBCV --upgrade
 ```
 ## Uso
-La clase `pyBCV.Currency` tiene los siguiente métodos:
-- `refresh_period`: Inicializa la clase Currency con un período de actualización. Por defecto `timedelta = timedelta(hours=1)`.
-- `lazy_load`: Indicador de carga. Matendra la tasa de cambio guardado en cache si vuelve a preguntar por la tasa nuevamente. por defecto `bool = False`.
-
-El método `pyBCV.Currency().get_rate()` tiene los siguiente parametros:
-- `currency_code`: Acepta un código de moneda o fecha como argumento.
-- `prettify`: Acepta un valor booleano si desea que el valor de la moneda salga junto con el simbolo de Bolivares. `Bs. [VALOR]`
-- `date_format`: Acepta un valor booleano si desea que la fecha extraiga la fecha y hora de la página web del Banco Central de Venezuela (BCV) o Formatea la fecha extraída en una cadena de texto legible. Por defecto `bool = True`. Extrae la fecha en una cadena de texto.
+La librería pyBCV proporciona dos clases, `Currency` y `Bank`, para obtener tasas de cambio e informativas de bancos del Banco Central de Venezuela.
 
-### Ejemplo:
-```python
+La clase `Currency` obtiene tasas de cambio para varias monedas y las devuelve en formato de diccionario. También proporciona métodos para obtener una tasa de cambio específica o la hora de la última actualización.
+```py
 import pyBCV
 
-bcv = pyBCV.Currency(lazy_load=True)
-
-get_value_usd = bcv.get_rate(currency_code='USD')
-get_in_bs_eur = bcv.get_rate(currency_code='EUR', prettify=True)
-get_date_valid = bcv.get_rate(currency_code='Fecha', date_format=True)
+currency = pyBCV.Currency()
+all_rates = currency.get_rate() # obtener todas las tasas de cambio de moneda
+usd_rate = currency.get_rate(currency_code='USD', prettify=False) # obtener la tasa de cambio del dólar estadounidense sin símbolo de moneda
+last_update = currency.get_rate(currency_code='Fecha') # obtener la hora de la última actualización
 ```
-Para obtener una estructura tipo JSON de las monedas disponibles en pyBCV, utilizamos la función `pyBCV.Currency().get_rate()` sin argumentos, el cual devuelve un diccionario.
 
-La clase `pyBCV.Bank` tiene el siguiente método:
-- `pyBCV.Bank().get_by_bank()`: Devuelve el sistema cambiario de compra y venta de moneda extranjera para un banco específico o todos los bancos disponibles.
-### Ejemplo:
-```python
+La clase `Bank` obtiene tasas informativas proporcionadas por varios bancos en Venezuela y las devuelve en formato de diccionario. Proporciona métodos para obtener información sobre un banco específico o todos los bancos disponibles.
+```py
 import pyBCV
 
 bcv = pyBCV.Bank()
-
-get_bank = bcv.get_by_bank(bank_code='Banesco') # Devolvera un diccionario con los valores de compra y venta de moneda extranjera y su fecha valida.
-specific_bank = bcv.get_by_bank(bank_code='Banesco', rate_or_sale='Compra') # Decolvera el valor de compra de moneda extranjera.
+bank_info = bcv.get_by_bank() # obtener todas las tasas de cambio informativas de los bancos disponibles
+bnc_buy_rate = bcv.get_by_bank(bank_code='Banco Nacional de Crédito', rate_or_sale='Compra') # obtener la tasa de compra del Banco Nacional de Crédito
 ```
-
 ## Colaboradores
 
 | [<img src="https://avatars.githubusercontent.com/u/103836660?v=4" width=115><br><sub>Francisco Griman</sub>](https://github.com/fcoagz) |  [<img src="https://avatars.githubusercontent.com/u/12820150?v=4" width=115><br><sub>Jesús Alfredo Reyes Vargas</sub>](https://github.com/jesusareyesv) |
 | :---: | :---: |
 ## Propósito de pyBCV
-El objetivo principal de PyBCV es proporcionar una forma fácil y rápida de acceder a los datos de tipos de cambio y tasas informativas del BCV en un formato que sea fácil de usar y manipular en Python. 
+Esta librería está diseñada específicamente para recopilar y convertir estos datos en un formato fácilmente utilizable en Python, lo que permite a los desarrolladores acceder a ellos y utilizarlos en sus aplicaciones con facilidad. Con pyBCV, los usuarios pueden obtener información actualizada sobre las tasas de cambio y las tasas informativas de los bancos de manera rápida y sencilla, haciendo que el proceso de obtener estos datos sea más eficiente y conveniente.
```

