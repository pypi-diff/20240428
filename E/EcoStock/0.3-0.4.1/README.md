# Comparing `tmp/EcoStock-0.3.tar.gz` & `tmp/EcoStock-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EcoStock-0.3.tar", last modified: Sun Apr 28 10:32:28 2024, max compression
+gzip compressed data, was "EcoStock-0.4.1.tar", last modified: Sun Apr 28 12:13:07 2024, max compression
```

## Comparing `EcoStock-0.3.tar` & `EcoStock-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 10:32:28.381217 EcoStock-0.3/
-drwxrwxrwx   0        0        0        0 2024-04-28 10:32:28.365621 EcoStock-0.3/EcoStock/
--rw-rw-rw-   0        0        0      854 2024-04-28 10:30:11.000000 EcoStock-0.3/EcoStock/__init__.py
--rw-rw-rw-   0        0        0     8646 2024-04-27 16:48:18.000000 EcoStock-0.3/EcoStock/api.py
--rw-rw-rw-   0        0        0    12900 2024-04-28 10:29:49.000000 EcoStock-0.3/EcoStock/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-28 10:32:28.381217 EcoStock-0.3/EcoStock.egg-info/
--rw-rw-rw-   0        0        0     1737 2024-04-28 10:32:28.000000 EcoStock-0.3/EcoStock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-04-28 10:32:28.000000 EcoStock-0.3/EcoStock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 10:32:28.000000 EcoStock-0.3/EcoStock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2024-04-28 10:32:28.000000 EcoStock-0.3/EcoStock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-28 10:32:28.000000 EcoStock-0.3/EcoStock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2024-04-20 17:30:30.000000 EcoStock-0.3/LICENSE.md
--rw-rw-rw-   0        0        0     1737 2024-04-28 10:32:28.381217 EcoStock-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1125 2024-04-23 14:39:00.000000 EcoStock-0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 10:32:28.381217 EcoStock-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1205 2024-04-28 10:27:54.000000 EcoStock-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 12:13:07.571614 EcoStock-0.4.1/
+drwxrwxrwx   0        0        0        0 2024-04-28 12:13:07.567053 EcoStock-0.4.1/EcoStock/
+-rw-rw-rw-   0        0        0     1003 2024-04-28 12:03:02.000000 EcoStock-0.4.1/EcoStock/__init__.py
+-rw-rw-rw-   0        0        0     6366 2024-04-28 11:55:39.000000 EcoStock-0.4.1/EcoStock/adalo.py
+-rw-rw-rw-   0        0        0     8328 2024-04-28 11:55:37.000000 EcoStock-0.4.1/EcoStock/api.py
+-rw-rw-rw-   0        0        0    12892 2024-04-28 11:55:35.000000 EcoStock-0.4.1/EcoStock/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-28 12:13:07.570615 EcoStock-0.4.1/EcoStock.egg-info/
+-rw-rw-rw-   0        0        0     1739 2024-04-28 12:13:07.000000 EcoStock-0.4.1/EcoStock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-28 12:13:07.000000 EcoStock-0.4.1/EcoStock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 12:13:07.000000 EcoStock-0.4.1/EcoStock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-04-28 12:13:07.000000 EcoStock-0.4.1/EcoStock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-28 12:13:07.000000 EcoStock-0.4.1/EcoStock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2024-04-28 11:55:32.000000 EcoStock-0.4.1/LICENSE.md
+-rw-rw-rw-   0        0        0     1739 2024-04-28 12:13:07.571614 EcoStock-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1125 2024-04-28 11:55:28.000000 EcoStock-0.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-28 12:13:07.571614 EcoStock-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2024-04-28 12:12:23.000000 EcoStock-0.4.1/setup.py
```

### Comparing `EcoStock-0.3/EcoStock/__init__.py` & `EcoStock-0.4.1/EcoStock/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,24 @@
 
 """
 Economic-Finance Correlation Package
 
 A Python package for investigating the correlation between economic and financial data.
 """
 
-__version__ = "0.3"
+__version__ = "0.4.1"
 
 from .api import app
+from .adalo import (
+    candlestick,
+    indicator_for_countries,
+    get_news,
+    comparison_indicators_countries,
+    bollinger_bands
+)
 from .functions import (
     get_stock_data,
     plot_candlestick,
     moving_avg_stock_data,
     get_world_bank_data,
     plot_correlation,
     plot_bollinger_bands,
```

### Comparing `EcoStock-0.3/EcoStock/api.py` & `EcoStock-0.4.1/EcoStock/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,160 +1,151 @@
-from fastapi import FastAPI, HTTPException, Depends
-from fastapi.responses import JSONResponse, HTMLResponse, FileResponse
-from fastapi.staticfiles import StaticFiles
-import os
-import plotly.io as pio
-import traceback
+from fastapi import FastAPI, HTTPException
+from fastapi.responses import JSONResponse
+from io import BytesIO
+import base64
 import argparse
-import sys
 import uvicorn
-from typing import List
-from typing import Optional
 from EcoStock.functions import (
     get_stock_data,
-    plot_candlestick,
     moving_avg_stock_data,
     get_world_bank_data,
-    plot_correlation,
-    plot_bollinger_bands,
-    get_news,
-    plot_indicator_for_countries,
-    compare_indicators_countries
+    plot_correlation
 )
+from EcoStock.adalo import (
+    candlestick, 
+    bollinger_bands, 
+    indicator_for_countries, 
+    comparison_indicators_countries, 
+    get_news)
 
 app = FastAPI()
 
 @app.get("/")
 async def read_root():
     return {"results": {
     "message": "Welcome to EcoStock API!"
   }}
 
-@app.get("/stock_data/{ticker}/{start_date}/{end_date}")
-async def get_stock_data_api(ticker: str, start_date: str, end_date: str):
-    try:
-        data = get_stock_data(ticker, start_date, end_date).to_dict(orient='records')
-        return JSONResponse(content={
-            "status": "success",
-            "message": "Stock data fetched successfully",
-            "ticker": ticker,
-            "start_date": start_date,
-            "end_date": end_date,
-            "results": data
-        })
-    except Exception as e:
-        return JSONResponse(content={
-            "status": "error",
-            "message": str(e),
-        }, status_code=400)
-
-# Mount the static directory to serve static files
-app.mount("/static", StaticFiles(directory="static"), name="static")
-
-def ensure_static_dir():
-    # Create the 'static' directory if it doesn't exist
-    if not os.path.exists('static'):
-        os.makedirs('static')
-
-@app.get("/plot_candlestick/{ticker}/{start_date}/{end_date}")
-async def plot_candlestick_api(ticker: str, start_date: str, end_date: str):
-    try:
-        # Generate the plot
-        fig = plot_candlestick(ticker, start_date, end_date)
-
-        # Create the 'static' directory if it doesn't exist
-        if not os.path.exists('static'):
-            os.makedirs('static')
-
-        # Save the figure as a PNG image
-        image_path = f"static/{ticker}_{start_date}_{end_date}.png"
-        pio.write_image(fig, image_path)
-
-        # Return the image URL
-        return {"url": f"https://ecofin-496487b9809a.herokuapp.com/{image_path}"}
+@app.get("/candlestick/{ticker}/{start_date}/{end_date}")
+async def candlestick_api(ticker: str, start_date: str, end_date: str):
+    """
+    Fetch the stock data and plot it as a simple line chart.
+
+    Parameters:
+    ticker (str): Ticker symbol of the stock.
+    start_date (str): Start date in 'YYYY-MM-DD' format.
+    end_date (str): End date in 'YYYY-MM-DD' format.
+    """
+    try:
+        # Fetch the stock data and plot
+        fig = candlestick(ticker, start_date, end_date)
+
+        # Check if fig is a Figure instance
+        if fig:
+            # Save the plot to a BytesIO object
+            buf = BytesIO()
+            fig.savefig(buf, format="png")
+            buf.seek(0)
+            
+            # Convert the buffer contents to base64 and create a data URL
+            data = base64.b64encode(buf.getbuffer()).decode("ascii")
+            return JSONResponse(content={"image": f"data:image/png;base64,{data}"})
+        else:
+            return {"error": "No data available or an error occurred"}
     except Exception as e:
-        raise HTTPException(status_code=400, detail=str(e))
-
-@app.get("/moving_avg_stock_data/{ticker}/{start_year}/{end_year}")
-async def moving_avg_stock_data_api(ticker: str, start_year: str, end_year: str):
-    try:
-        # Call the moving_avg_stock_data function
-        df = moving_avg_stock_data(ticker, start_year, end_year)
-
-        # Convert the DataFrame to a dictionary and return it as a JSON response
-        return JSONResponse(content={
-            "status": "success",
-            "message": "Moving average stock data fetched successfully",
-            "ticker": ticker,
-            "start_year": start_year,
-            "end_year": end_year,
-            "results": df.to_dict(orient='records')
-        })
-    except Exception as e:
-        raise HTTPException(status_code=400, detail=str(e))
-
-@app.get("/world_bank_data/{indicator}/{country}/{start_date}/{end_date}")
-async def world_bank_data_api(indicator: str, country: str, start_date: str, end_date: str):
-    try:
-        # Call the get_world_bank_data function
-        df = get_world_bank_data(indicator, country, start_date, end_date)
+        return {"error": f"An error occurred: {e}"}
 
-        # Convert the DataFrame to a dictionary and return it as a JSON response
-        return JSONResponse(content={
-            "status": "success",
-            "message": "World Bank data fetched successfully",
-            "indicator": indicator,
-            "country": country,
-            "start_date": start_date,
-            "end_date": end_date,
-            "results": df.to_dict(orient='records')
-        })
-    except Exception as e:
-        raise HTTPException(status_code=400, detail=str(e))
-    
 @app.get("/plot_correlation/{ticker}/{start_year}/{end_year}/{indicator}/{country}/{start_date}/{end_date}/{econ_label}/{econ_format}")
 async def plot_correlation_api(ticker: str, start_year: str, end_year: str, indicator: str, country: str, start_date: str, end_date: str, econ_label: str, econ_format: str = None):
-    try:
-        # Call the plot_correlation function
-        plot_correlation(ticker, start_year, end_year, indicator, country, start_date, end_date, econ_label, econ_format)
-
-        # Create the 'static' directory if it doesn't exist
-        if not os.path.exists('static'):
-            os.makedirs('static')
-
-        # Save the current figure as an image file in the 'static' directory
-        image_path = f"static/{ticker}_{indicator}.png"
-        plt.savefig(image_path)
-
-        # Close the current figure to free up memory
-        plt.close()
-
-        # Return the image URL
-        return {"url": f"https://ecofin-496487b9809a.herokuapp.com/{image_path}"}
+    """
+    Fetch stock data from Yahoo Finance and calculate a 1-year moving average, then fetch economic data from the World Bank, 
+    and plot the correlation between stock and economic data over time.
+
+    Parameters:
+    ticker (str): Ticker symbol of the stock.
+    start_year (str): Start year for the stock data in 'YYYY' format.
+    end_year (str): End year for the stock data in 'YYYY' format.
+    indicator (str): The indicator of interest for the World Bank data.
+    country (str): The country of interest for the World Bank data.
+    start_date (str): The start date for the World Bank data.
+    end_date (str): The end date for the World Bank data.
+    econ_label (str): Label for the economic data.
+    econ_format (str): Format of the economic data ('dollar', 'percent', or None). Default is None.
+    """
+    try:
+        # Fetch the stock data and plot
+        fig = plot_correlation(ticker, start_year, end_year, indicator, country, start_date, end_date, econ_label, econ_format)
+
+        # Check if fig is a Figure instance
+        if fig:
+            # Save the plot to a BytesIO object
+            buf = BytesIO()
+            fig.savefig(buf, format="png")
+            buf.seek(0)
+            
+            # Convert the buffer contents to base64 and create a data URL
+            data = base64.b64encode(buf.getbuffer()).decode("ascii")
+            return JSONResponse(content={"image": f"data:image/png;base64,{data}"})
+        else:
+            return {"error": "No data available or an error occurred"}
+    except Exception as e:
+        return {"error": f"An error occurred: {e}"}
+
+@app.get("/bollinger_bands/{ticker}/{start_date}/{end_date}/{window_size}/{num_of_std}")
+async def bollinger_bands_api(ticker: str, start_date: str, end_date: str, window_size: int, num_of_std: int):
+    try:
+        fig = bollinger_bands(ticker, start_date, end_date, window_size, num_of_std)
+        
+        # Check if fig is a Figure instance
+        if fig:
+            # Save the plot to a BytesIO object
+            buf = BytesIO()
+            fig.savefig(buf, format="png")
+            buf.seek(0)
+            
+            # Convert the buffer contents to base64 and create a data URL
+            data = base64.b64encode(buf.getbuffer()).decode("ascii")
+            return JSONResponse(content={"image": f"data:image/png;base64,{data}"})
+        else:
+            return {"error": "No data available or an error occurred"}
+    except Exception as e:
+        return {"error": f"An error occurred: {e}"}
+
+@app.get("/indicator_for_countries/{indicator}/{countries}/{start_date}/{end_date}")
+async def indicator_for_countries_api(indicator: str, countries: str, start_date: str, end_date: str):
+    """
+    Fetch the economic indicator data for several countries and plot it.
+
+    Parameters:
+    indicator (str): The indicator of interest.
+    countries (str): The countries of interest, separated by commas.
+    start_date (str): Start date in 'YYYY-MM-DD' format.
+    end_date (str): End date in 'YYYY-MM-DD' format.
+    """
+    try:
+        # Convert the countries string to a list
+        countries_list = countries.split(',')
+
+        # Fetch the data and plot
+        fig = indicator_for_countries(indicator, countries_list, start_date, end_date)
+
+        # Check if fig is a Figure instance
+        if fig:
+            # Save the plot to a BytesIO object
+            buf = BytesIO()
+            fig.savefig(buf, format="png")
+            buf.seek(0)
+            
+            # Convert the buffer contents to base64 and create a data URL
+            data = base64.b64encode(buf.getbuffer()).decode("ascii")
+            return JSONResponse(content={"image": f"data:image/png;base64,{data}"})
+        else:
+            return {"error": "No data available or an error occurred"}
     except Exception as e:
-        raise HTTPException(status_code=400, detail=str(e))
-
-@app.get("/plot_bollinger_bands/{ticker}/{start_date}/{end_date}/{window_size}/{num_of_std}")
-async def plot_bollinger_bands_api(ticker: str, start_date: str, end_date: str, window_size: int, num_of_std: int):
-    try:
-        # Call the plot_bollinger_bands function
-        fig = plot_bollinger_bands(ticker, start_date, end_date, window_size, num_of_std)
-
-        # Create the 'static' directory if it doesn't exist
-        if not os.path.exists('static'):
-            os.makedirs('static')
-
-        # Save the current figure as an image file in the 'static' directory
-        image_path = f"static/{ticker}_bollinger_bands.png"
-        fig.write_image(image_path)
-
-        # Return the image URL
-        return {"url": f"https://ecofin-496487b9809a.herokuapp.com/{image_path}"}
-    except Exception as e:
-        raise HTTPException(status_code=400, detail=str(e))
+        return {"error": f"An error occurred: {e}"}
 
 @app.get("/get_news/{symbol}")
 async def get_news_api(symbol: str):
     try:
         # Call the get_news function
         data = get_news(symbol)
 
@@ -163,53 +154,47 @@
             raise HTTPException(status_code=400, detail="Error fetching news data")
 
         # Return the news data
         return data
     except Exception as e:
         raise HTTPException(status_code=400, detail=str(e))
 
-@app.get("/plot_indicator_for_countries/{indicator}/{start_date}/{end_date}")
-async def plot_indicator_for_countries_api(indicator: str, countries: List[str], start_date: str, end_date: str):
-    try:
-        # Call the plot_indicator_for_countries function
-        fig = plot_indicator_for_countries(indicator, countries, start_date, end_date)
-
-        # Create the 'static' directory if it doesn't exist
-        if not os.path.exists('static'):
-            os.makedirs('static')
-
-        # Save the current figure as an image file in the 'static' directory
-        image_path = f"static/{indicator}_for_countries.png"
-        fig.write_image(image_path)
-
-        # Return the image URL
-        return {"url": f"https://ecofin-496487b9809a.herokuapp.com/{image_path}"}
+@app.get("/comparison_indicators_countries/{indicators}/{countries}/{start_date}/{end_date}")
+async def comparison_indicators_countries(indicators: str, countries: str, start_date: str, end_date: str):
+    """
+    Fetch the comparison plot for given indicators and countries.
+
+    Parameters:
+    indicators (str): The indicators of interest, separated by commas.
+    countries (str): The countries of interest, separated by commas.
+    start_date (str): The start date for the data.
+    end_date (str): The end date for the data.
+    """
+    try:
+        # Split the indicators and countries strings into lists
+        indicators_list = indicators.split(",")
+        countries_list = countries.split(",")
+
+        # Fetch the comparison plot
+        fig = comparison_indicators_countries(indicators_list, countries_list, start_date, end_date)
+        
+        if fig:
+            # Save the plot to a BytesIO object
+            buf = BytesIO()
+            fig.savefig(buf, format="png")
+            buf.seek(0)
+            
+            # Convert the buffer contents to base64 and create a data URL
+            data = base64.b64encode(buf.getbuffer()).decode("ascii")
+            return JSONResponse(content={"image": f"data:image/png;base64,{data}"})
+        else:
+            return {"error": "No data available or an error occurred"}
     except Exception as e:
-        raise HTTPException(status_code=400, detail=str(e))
-
-@app.get("/compare_indicators_countries/{start_date}/{end_date}")
-async def compare_indicators_countries_api(indicators: List[str], countries: List[str], start_date: str, end_date: str):
-    try:
-        # Call the compare_indicators_countries function
-        fig = compare_indicators_countries(indicators, countries, start_date, end_date)
-
-        # Create the 'static' directory if it doesn't exist
-        if not os.path.exists('static'):
-            os.makedirs('static')
-
-        # Save the current figure as an image file in the 'static' directory
-        image_path = f"static/compare_indicators_countries.png"
-        fig.write_image(image_path)
-
-        # Return the image URL
-        return {"url": f"https://ecofin-496487b9809a.herokuapp.com/{image_path}"}
-    except Exception as e:
-        raise HTTPException(status_code=400, detail=str(e))
+        return {"error": f"An error occurred: {e}"}
     
-
 if __name__ == "__main__":
     
     parser = argparse.ArgumentParser(description="Run the FastAPI application.")
     parser.add_argument("-p", "--port", type=int, default=8000, help="The port to bind.")
     parser.add_argument("-r", "--reload", action="store_true", help="Enable hot reloading.")
     args = parser.parse_args()
```

### Comparing `EcoStock-0.3/EcoStock/functions.py` & `EcoStock-0.4.1/EcoStock/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
     if formatter is not None:
         ax2.yaxis.set_major_formatter(formatter)
 
     fig.legend(loc="upper left", bbox_to_anchor=(0,1), bbox_transform=ax1.transAxes)
     plt.title(f'Correlation between Stock Price and {econ_label}: {correlation:.2f}')
     fig.tight_layout()
     
-    return  plt.show()
+    return fig
 
 # Plotting Bollinger Bands
 def plot_bollinger_bands(ticker, start_date, end_date, window_size, num_of_std):
     # Fetch the stock data
     data = get_stock_data(ticker, start_date, end_date)
 
     # Calculate the rolling mean of the 'Close' prices over the specified window size
```

### Comparing `EcoStock-0.3/EcoStock.egg-info/PKG-INFO` & `EcoStock-0.4.1/EcoStock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.3
+Version: 0.4.1
 Summary: A Python package for investigating the correlation between economic and financial data.
 Home-page: https://github.com/Tonij10/fastapi-project
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo
 Author-email: antoniopaparo@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EcoStock-0.3/LICENSE.md` & `EcoStock-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `EcoStock-0.3/PKG-INFO` & `EcoStock-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.3
+Version: 0.4.1
 Summary: A Python package for investigating the correlation between economic and financial data.
 Home-page: https://github.com/Tonij10/fastapi-project
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo
 Author-email: antoniopaparo@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EcoStock-0.3/README.md` & `EcoStock-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `EcoStock-0.3/setup.py` & `EcoStock-0.4.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='EcoStock',
-    version='0.3',
+    version='0.4.1',
     author="Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo",
     author_email="antoniopaparo@outlook.com",
     description='A Python package for investigating the correlation between economic and financial data.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tonij10/fastapi-project",
     packages=find_packages(),
     install_requires=[
         'fastapi',
-        'pydantic',
-        'kaleido',
         'argparse',
         'uvicorn',
         'pandas',
         'numpy',
         'matplotlib',
         'yfinance',
         'plotly',
-        'openai',
-        'requests'
+        'requests',
+        'seaborn',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
-
-
-# Assicurati di sostituire Your Name, your.email@example.com e https://github.com/yourusername/package_name con le tue informazioni.
```

