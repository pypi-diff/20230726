# Comparing `tmp/quant-alchemy-0.1.2.tar.gz` & `tmp/quant-alchemy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant-alchemy-0.1.2.tar", last modified: Wed Jul 26 18:54:28 2023, max compression
+gzip compressed data, was "quant-alchemy-0.1.3.tar", last modified: Wed Jul 26 21:50:32 2023, max compression
```

## Comparing `quant-alchemy-0.1.2.tar` & `quant-alchemy-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 18:54:28.861735 quant-alchemy-0.1.2/
--rw-rw-rw-   0        0        0      400 2023-07-26 18:54:28.861735 quant-alchemy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-07-07 18:15:03.000000 quant-alchemy-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 18:54:28.855736 quant-alchemy-0.1.2/quant_alchemy/
--rw-rw-rw-   0        0        0       94 2023-07-26 18:53:42.000000 quant-alchemy-0.1.2/quant_alchemy/__init__.py
--rw-rw-rw-   0        0        0     3572 2023-07-12 19:45:17.000000 quant-alchemy-0.1.2/quant_alchemy/portfolio.py
--rw-rw-rw-   0        0        0    14526 2023-07-12 19:18:04.000000 quant-alchemy-0.1.2/quant_alchemy/timeseries.py
-drwxrwxrwx   0        0        0        0 2023-07-26 18:54:28.860736 quant-alchemy-0.1.2/quant_alchemy.egg-info/
--rw-rw-rw-   0        0        0      400 2023-07-26 18:54:28.000000 quant-alchemy-0.1.2/quant_alchemy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-07-26 18:54:28.000000 quant-alchemy-0.1.2/quant_alchemy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 18:54:28.000000 quant-alchemy-0.1.2/quant_alchemy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-26 18:54:28.000000 quant-alchemy-0.1.2/quant_alchemy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-26 18:54:28.000000 quant-alchemy-0.1.2/quant_alchemy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 18:54:28.861735 quant-alchemy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-07-26 18:54:23.000000 quant-alchemy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 21:50:32.930703 quant-alchemy-0.1.3/
+-rw-rw-rw-   0        0        0      400 2023-07-26 21:50:32.930703 quant-alchemy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-07-07 18:15:03.000000 quant-alchemy-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 21:50:32.923478 quant-alchemy-0.1.3/quant_alchemy/
+-rw-rw-rw-   0        0        0       94 2023-07-26 18:55:50.000000 quant-alchemy-0.1.3/quant_alchemy/__init__.py
+-rw-rw-rw-   0        0        0     3572 2023-07-12 19:45:17.000000 quant-alchemy-0.1.3/quant_alchemy/portfolio.py
+-rw-rw-rw-   0        0        0    14668 2023-07-26 21:49:51.000000 quant-alchemy-0.1.3/quant_alchemy/timeseries.py
+drwxrwxrwx   0        0        0        0 2023-07-26 21:50:32.928704 quant-alchemy-0.1.3/quant_alchemy.egg-info/
+-rw-rw-rw-   0        0        0      400 2023-07-26 21:50:32.000000 quant-alchemy-0.1.3/quant_alchemy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-07-26 21:50:32.000000 quant-alchemy-0.1.3/quant_alchemy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 21:50:32.000000 quant-alchemy-0.1.3/quant_alchemy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-26 21:50:32.000000 quant-alchemy-0.1.3/quant_alchemy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 21:50:32.000000 quant-alchemy-0.1.3/quant_alchemy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 21:50:32.931705 quant-alchemy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-07-26 21:49:59.000000 quant-alchemy-0.1.3/setup.py
```

### Comparing `quant-alchemy-0.1.2/quant_alchemy/portfolio.py` & `quant-alchemy-0.1.3/quant_alchemy/portfolio.py`

 * *Files identical despite different names*

### Comparing `quant-alchemy-0.1.2/quant_alchemy/timeseries.py` & `quant-alchemy-0.1.3/quant_alchemy/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,24 +142,30 @@
 
         Returns:
             float: The compounded return.
         """
         returns = self.returns()
         return np.expm1(np.log1p(returns).sum())
     
-    def max_drawdown(self):        
+    def max_drawdown(self):
         """
         This method calculates and returns the maximum drawdown of the time series data.
         
         The drawdown is the percentage loss from the highest point to the lowest point.
         
         Returns:
             float: The maximum drawdown of the time series data.
         """
-        return (self.prices / self.prices.cummax()).min() - 1
+        drawdown = self.drawdown()
+        max_drawdowns = {}
+
+        for col, df in drawdown.items():
+            max_drawdowns[col] = df['Drawdown'].min()
+
+        return pd.Series(max_drawdowns)
     
     def drawdown(self):
         """
         This method calculates and returns a DataFrame containing the return series,
         cumulative return series, previous peak in the cumulative returns, 
         and the drawdown series.
 
@@ -264,35 +270,35 @@
                 The method uses a degrees of freedom (ddof) value of 1, implying that the function
                 computes sample standard deviation which is an unbiased estimator of the population 
                 standard deviation.
         """
         returns = self.returns()
         return returns[returns < threshold].std(ddof=1)
 
-def var_historic(self, level=5):
-    """
-    This method calculates and returns the historic Value at Risk (VaR) at a specified level.
-
-    VaR is a statistical technique used to measure and quantify the level of financial risk within a firm or investment portfolio over a specific time frame.
-
-    Parameters:
-        level: (float, optional)
-            The percentile level at which to calculate VaR. This is the level below which the returns would fall with the given level of probability. Defaults to 5.
-
-    Raises:
-        ValueError: If the given level is not a valid percentile (i.e., not between 0 and 100).
-
-    Returns:
-        float: The historic VaR at the specified level. This is the return value such that 'level' percent of returns fall below this number and (100 - level) percent of returns fall above this number.
-    """
-    if not 0 <= level <= 100:
-        raise ValueError("The 'level' should be a percentile, i.e., between 0 and 100.")
-    
-    returns = self.returns()
-    return np.percentile(returns, level)
+    def var_historic(self, level=5):
+        """
+        This method calculates and returns the historic Value at Risk (VaR) at a specified level.
+
+        VaR is a statistical technique used to measure and quantify the level of financial risk within a firm or investment portfolio over a specific time frame.
+
+        Parameters:
+            level: (float, optional)
+                The percentile level at which to calculate VaR. This is the level below which the returns would fall with the given level of probability. Defaults to 5.
+
+        Raises:
+            ValueError: If the given level is not a valid percentile (i.e., not between 0 and 100).
+
+        Returns:
+            float: The historic VaR at the specified level. This is the return value such that 'level' percent of returns fall below this number and (100 - level) percent of returns fall above this number.
+        """
+        if not 0 <= level <= 100:
+            raise ValueError("The 'level' should be a percentile, i.e., between 0 and 100.")
+        
+        returns = self.returns()
+        return np.percentile(returns, level)
 
     def cvar_historic(self, level=5):
         """
         Calculates the historic Conditional Value at Risk (CVaR), also known as Expected Shortfall (ES),
         at a specified level. CVaR quantifies the expected value of loss given that a certain level of 
         loss threshold (VaR) has been exceeded.
 
@@ -331,9 +337,8 @@
             float: The Gaussian VaR at the specified level. This is the return value such that 'level' percent of 
                     returns fall below this number, assuming returns follow a Gaussian distribution.
         """
         if not 0 <= level <= 100:
             raise ValueError("The 'level' should be a percentile, i.e., between 0 and 100.")
         
         returns = self.returns()
-        # Using 'ppf' function to find the percentile point
         return -norm.ppf(level/100, loc=returns.mean(), scale=returns.std(ddof=1))
```

### Comparing `quant-alchemy-0.1.2/setup.py` & `quant-alchemy-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 setuptools.setup(
     name="quant-alchemy",
-    version="0.1.2",
+    version="0.1.3",
     author="Eladio Rocha Vizcaino",
     author_email="eladio.rocha99@gmail.com",
     description="Package for quantitative finance.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/EladioRocha/quant-alchemy",
     project_urls={
```

