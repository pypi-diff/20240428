# Comparing `tmp/EcoStock-0.1.tar.gz` & `tmp/EcoStock-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EcoStock-0.1.tar", last modified: Tue Apr 23 15:18:34 2024, max compression
+gzip compressed data, was "EcoStock-0.2.tar", last modified: Sat Apr 27 17:33:54 2024, max compression
```

## Comparing `EcoStock-0.1.tar` & `EcoStock-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 15:18:34.792025 EcoStock-0.1/
-drwxrwxrwx   0        0        0        0 2024-04-23 15:18:34.758043 EcoStock-0.1/EcoStock/
--rw-rw-rw-   0        0        0      799 2024-04-23 14:37:00.000000 EcoStock-0.1/EcoStock/__init__.py
--rw-rw-rw-   0        0        0     5281 2024-04-23 14:54:21.000000 EcoStock-0.1/EcoStock/api.py
--rw-rw-rw-   0        0        0     8565 2024-04-23 14:54:35.000000 EcoStock-0.1/EcoStock/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-23 15:18:34.782029 EcoStock-0.1/EcoStock.egg-info/
--rw-rw-rw-   0        0        0     1737 2024-04-23 15:18:33.000000 EcoStock-0.1/EcoStock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-04-23 15:18:34.000000 EcoStock-0.1/EcoStock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 15:18:33.000000 EcoStock-0.1/EcoStock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2024-04-23 15:18:33.000000 EcoStock-0.1/EcoStock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-23 15:18:34.000000 EcoStock-0.1/EcoStock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2024-04-20 17:30:29.000000 EcoStock-0.1/LICENSE.md
--rw-rw-rw-   0        0        0     1737 2024-04-23 15:18:34.788027 EcoStock-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1125 2024-04-23 14:38:58.000000 EcoStock-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 15:18:34.792025 EcoStock-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1205 2024-04-23 15:18:24.000000 EcoStock-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 17:33:54.925283 EcoStock-0.2/
+drwxrwxrwx   0        0        0        0 2024-04-27 17:33:54.920299 EcoStock-0.2/EcoStock/
+-rw-rw-rw-   0        0        0      869 2024-04-27 17:05:18.000000 EcoStock-0.2/EcoStock/__init__.py
+-rw-rw-rw-   0        0        0     8646 2024-04-27 16:48:18.000000 EcoStock-0.2/EcoStock/api.py
+-rw-rw-rw-   0        0        0    13738 2024-04-27 16:45:22.000000 EcoStock-0.2/EcoStock/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-27 17:33:54.924318 EcoStock-0.2/EcoStock.egg-info/
+-rw-rw-rw-   0        0        0     1737 2024-04-27 17:33:54.000000 EcoStock-0.2/EcoStock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-04-27 17:33:54.000000 EcoStock-0.2/EcoStock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 17:33:54.000000 EcoStock-0.2/EcoStock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2024-04-27 17:33:54.000000 EcoStock-0.2/EcoStock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-27 17:33:54.000000 EcoStock-0.2/EcoStock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2024-04-20 17:30:30.000000 EcoStock-0.2/LICENSE.md
+-rw-rw-rw-   0        0        0     1737 2024-04-27 17:33:54.925283 EcoStock-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1125 2024-04-23 14:39:00.000000 EcoStock-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 17:33:54.925283 EcoStock-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1205 2024-04-27 17:04:08.000000 EcoStock-0.2/setup.py
```

### Comparing `EcoStock-0.1/EcoStock/__init__.py` & `EcoStock-0.2/EcoStock/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 
 """
 Economic-Finance Correlation Package
 
 A Python package for investigating the correlation between economic and financial data.
 """
 
-__version__ = "0.1"
+__version__ = "0.2"
 
 from .api import app
 from .functions import (
     get_stock_data,
     plot_candlestick,
-    avg_stock_data,
+    moving_avg_stock_data,
     get_world_bank_data,
-    calculate_correlation,
     plot_correlation,
-    generate_text,
+    plot_bollinger_bands,
+    get_news,
+    plot_indicator_for_countries,
+    compare_indicators_countries
 )
 
 
 # Questo file fornisce una breve descrizione del pacchetto e definisce la versione. 
 # Infine, importa tutte le funzioni dal modulo functions.py in modo che siano disponibili quando importi il tuo pacchetto.
```

### Comparing `EcoStock-0.1/EcoStock/functions.py` & `EcoStock-0.2/EcoStock/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,244 +1,216 @@
-# Nel file functions.py, includeremo tutte le funzioni per ottenere i dati finanziari e economici ecc...
-# ESEMPIO:
-# EcoStock/functions.py
-
-import pandas as pd
-import numpy as np
-import requests
-import yfinance as yf
-import plotly.graph_objects as go
-import matplotlib.pyplot as plt
-import matplotlib.ticker as mticker
-import openai
-from openai import OpenAI
+from fastapi import FastAPI, HTTPException, Depends
+from fastapi.responses import JSONResponse, HTMLResponse, FileResponse
+from fastapi.staticfiles import StaticFiles
 import os
-import base64
-import io
-
-# Define the get_stock_data function
-def get_stock_data(ticker, start_date, end_date):
-    """
-    Fetch stock data from Yahoo Finance.
-
-    Parameters:
-    ticker (str): Ticker symbol of the stock.
-    start_date (str): Start date in 'YYYY-MM-DD' format.
-    end_date (str): End date in 'YYYY-MM-DD' format.
-
-    Returns:
-    pandas.DataFrame: DataFrame containing the stock data.
-    """
-    return yf.download(ticker, start=start_date, end=end_date)
-
-# Plotting the stock data
-def plot_candlestick(stock_data, ticker):
-    """
-    Plot the stock data as a candlestick chart.
-
-    Parameters:
-    stock_data (pandas.DataFrame): DataFrame containing the stock data.
-    ticker (str): Ticker symbol of the stock.
-    """
-    # Create a candlestick chart
-    fig = go.Figure(data=[go.Candlestick(x=stock_data.index,
-                                         open=stock_data['Open'],
-                                         high=stock_data['High'],
-                                         low=stock_data['Low'],
-                                         close=stock_data['Close'])])
-
-    # Add volume bars
-    fig.add_trace(go.Bar(x=stock_data.index, y=stock_data['Volume'], marker=dict(color=np.where(stock_data['Close'] >= stock_data['Open'], 'green', 'red')), yaxis='y2'))
-
-    # Add range slider
-    fig.update_layout(
-        title=f'{ticker} Stock Price',
-        yaxis_title='Stock Price (USD)',
-        shapes = [dict(x0='2022-01-01', x1='2022-12-31', y0=0, y1=1, xref='x', yref='paper', line_width=2)],
-        xaxis=dict(
-            rangeselector=dict(
-                buttons=list([
-                    dict(count=1, label="1m", step="month", stepmode="backward"),
-                    dict(count=6, label="6m", step="month", stepmode="backward"),
-                    dict(count=1, label="YTD", step="year", stepmode="todate"),
-                    dict(count=1, label="1y", step="year", stepmode="backward"),
-                    dict(step="all")
-                ])
-            ),
-            rangeslider=dict(visible=True),
-            type="date"
-        ),
-        yaxis2=dict(domain=[0, 0.2], anchor='x', title='Volume')
-    )
-
-    return fig
-
-# Annual average stock data
-def avg_stock_data(ticker, start_year, end_year):
-    """
-    Fetch stock data from Yahoo Finance and resample to annual frequency.
-
-    Parameters:
-    ticker (str): Ticker symbol of the stock.
-    start_year (str): Start year in 'YYYY' format.
-    end_year (str): End year in 'YYYY' format.
-
-    Returns:
-    pandas.DataFrame: DataFrame containing the annual average stock data.
-    """
-    # Format the years as 'YYYY-MM-DD'
-    start_date = f'{start_year}-01-01'
-    end_date = f'{end_year}-12-31'
-
-    # Fetch the daily stock data
-    df = yf.download(ticker, start=start_date, end=end_date)
-
-    # Resample to annual frequency, calculating the mean of each year
-    df = df.resample('A').mean()
-
-    # Modify the index to only include the year
-    df.index = df.index.year
-
-    return df
-
-# World Bank data
-def get_world_bank_data(indicator, country, start_date, end_date):
-    """
-    Fetch economic data from the World Bank.
-
-    Parameters:
-    indicator (str): The indicator of interest.
-    country (str): The country of interest.
-    start_date (str): The start date for the data.
-    end_date (str): The end date for the data.
-
-    Returns:
-    pandas.DataFrame: DataFrame containing the economic data.
-    """
-    # Define the API URL
-    url = f"http://api.worldbank.org/v2/country/{country}/indicator/{indicator}?date={start_date}:{end_date}&format=json"
-
-    # Send the HTTP request and get the response
-    response = requests.get(url)
-
-    # Check if the request was successful
-    if response.status_code == 200:
-        # Get the data from the response
-        data = response.json()
-
-        # Check if the data has at least two elements
-        if len(data) < 2:
-            print("Error: No data available for the given parameters")
-            return pd.DataFrame()
-
-        # Convert the data to a DataFrame and set the date as the index
-        df = pd.DataFrame(data[1])
-        df['date'] = pd.to_datetime(df['date']).dt.year
-        df.set_index('date', inplace=True)
-
-        # Extract the name of the indicator and the country
-        df['indicator'] = df['indicator'].apply(lambda x: x['value'])
-        df['country'] = df['country'].apply(lambda x: x['value'])
-
-        return df
-    else:
-        print(f"Error: HTTP request failed with status code {response.status_code}")
-        return pd.DataFrame()
-
-# Calculate correlation
-def calculate_correlation(stock_data, econ_data):
-    """
-    Calculate the correlation coefficient between stock and economic data.
-
-    Parameters:
-    stock_data (pandas.DataFrame): DataFrame containing the stock data.
-    econ_data (pandas.DataFrame): DataFrame containing the economic data.
-
-    Returns:
-    float: Correlation coefficient.
-    """
-    # Check if 'Close' column exists in stock_data
-    if 'Close' not in stock_data.columns:
-        print("Error: 'Close' column not found in stock_data")
-        return None
-
-    # Merge the data
-    merged_data = pd.merge(stock_data, econ_data, how='inner', left_index=True, right_index=True)
-
-    # Check if merged_data is empty
-    if merged_data.empty:
-        print("Error: No matching data found for stock_data and econ_data")
-        return None
-
-    return merged_data['Close'].corr(merged_data['value'])
-
-# Plotting correlation
-def plot_correlation(stock_data, econ_data, stock_label, econ_label):
-    """
-    Plot the correlation between stock and economic data over time.
-
-    Parameters:
-    stock_data (pandas.DataFrame): DataFrame containing the stock data.
-    econ_data (pandas.DataFrame): DataFrame containing the economic data.
-    stock_label (str): Label for the stock data.
-    econ_label (str): Label for the economic data.
-    """
-    # Check if 'Close' column exists in stock_data
-    if 'Close' not in stock_data.columns:
-        print("Error: 'Close' column not found in stock_data")
-        return None
-
-    # Merge the data
-    merged_data = pd.merge(stock_data, econ_data, how='inner', left_index=True, right_index=True)
-
-    # Check if merged_data is empty
-    if merged_data.empty:
-        print("Error: No matching data found for stock_data and econ_data")
-        return None
-
-    # Calculate the correlation
-    correlation = merged_data['Close'].corr(merged_data['value'])
-
-    # Create the plot
-    fig, ax1 = plt.subplots(figsize=(10, 6))  # Increase the size of the plot
-
-    color = 'tab:red'
-    ax1.set_xlabel('Date')
-    ax1.set_ylabel(stock_label, color=color)
-    ax1.plot(stock_data.index, stock_data['Close'], color=color)
-    ax1.tick_params(axis='y', labelcolor=color)
-
-    ax2 = ax1.twinx()
-    color = 'tab:blue'
-    ax2.set_ylabel(econ_label, color=color)
-    ax2.plot(econ_data.index, econ_data['value'], color=color)
-    ax2.tick_params(axis='y', labelcolor=color)
-
-    # Format the y-tick labels to include a dollar sign and display in terms of billions or trillions
-    def human_format(num):
-        magnitude = 0
-        while abs(num) >= 1000:
-            magnitude += 1
-            num /= 1000.0
-        return '${:.1f}{}'.format(num, ['', 'K', 'M', 'B', 'T'][magnitude])
-
-    formatter = mticker.FuncFormatter(lambda x, pos: human_format(x))
-    ax2.yaxis.set_major_formatter(formatter)
-
-    plt.title(f'Correlation between {stock_label} and {econ_label}: {correlation:.2f}')
-    plt.grid(True)
-    fig.tight_layout()
+import plotly.io as pio
+import traceback
+import argparse
+import sys
+import uvicorn
+from typing import List
+from typing import Optional
+from EcoStock.functions import (
+    get_stock_data,
+    plot_candlestick,
+    moving_avg_stock_data,
+    get_world_bank_data,
+    plot_correlation,
+    plot_bollinger_bands,
+    get_news,
+    plot_indicator_for_countries,
+    compare_indicators_countries
+)
+
+app = FastAPI()
+
+@app.get("/")
+async def read_root():
+    return {"results": {
+    "message": "Welcome to EcoStock API!"
+  }}
+
+@app.get("/stock_data/{ticker}/{start_date}/{end_date}")
+async def get_stock_data_api(ticker: str, start_date: str, end_date: str):
+    try:
+        data = get_stock_data(ticker, start_date, end_date).to_dict(orient='records')
+        return JSONResponse(content={
+            "status": "success",
+            "message": "Stock data fetched successfully",
+            "ticker": ticker,
+            "start_date": start_date,
+            "end_date": end_date,
+            "results": data
+        })
+    except Exception as e:
+        return JSONResponse(content={
+            "status": "error",
+            "message": str(e),
+        }, status_code=400)
+
+# Mount the static directory to serve static files
+app.mount("/static", StaticFiles(directory="static"), name="static")
+
+def ensure_static_dir():
+    # Create the 'static' directory if it doesn't exist
+    if not os.path.exists('static'):
+        os.makedirs('static')
+
+@app.get("/plot_candlestick/{ticker}/{start_date}/{end_date}")
+async def plot_candlestick_api(ticker: str, start_date: str, end_date: str):
+    try:
+        # Generate the plot
+        fig = plot_candlestick(ticker, start_date, end_date)
+
+        # Create the 'static' directory if it doesn't exist
+        if not os.path.exists('static'):
+            os.makedirs('static')
+
+        # Save the figure as a PNG image
+        image_path = f"static/{ticker}_{start_date}_{end_date}.png"
+        pio.write_image(fig, image_path)
+
+        # Return the image URL
+        return {"url": f"https://ecofin-496487b9809a.herokuapp.com/{image_path}"}
+    except Exception as e:
+        raise HTTPException(status_code=400, detail=str(e))
+
+@app.get("/moving_avg_stock_data/{ticker}/{start_year}/{end_year}")
+async def moving_avg_stock_data_api(ticker: str, start_year: str, end_year: str):
+    try:
+        # Call the moving_avg_stock_data function
+        df = moving_avg_stock_data(ticker, start_year, end_year)
+
+        # Convert the DataFrame to a dictionary and return it as a JSON response
+        return JSONResponse(content={
+            "status": "success",
+            "message": "Moving average stock data fetched successfully",
+            "ticker": ticker,
+            "start_year": start_year,
+            "end_year": end_year,
+            "results": df.to_dict(orient='records')
+        })
+    except Exception as e:
+        raise HTTPException(status_code=400, detail=str(e))
+
+@app.get("/world_bank_data/{indicator}/{country}/{start_date}/{end_date}")
+async def world_bank_data_api(indicator: str, country: str, start_date: str, end_date: str):
+    try:
+        # Call the get_world_bank_data function
+        df = get_world_bank_data(indicator, country, start_date, end_date)
+
+        # Convert the DataFrame to a dictionary and return it as a JSON response
+        return JSONResponse(content={
+            "status": "success",
+            "message": "World Bank data fetched successfully",
+            "indicator": indicator,
+            "country": country,
+            "start_date": start_date,
+            "end_date": end_date,
+            "results": df.to_dict(orient='records')
+        })
+    except Exception as e:
+        raise HTTPException(status_code=400, detail=str(e))
+    
+@app.get("/plot_correlation/{ticker}/{start_year}/{end_year}/{indicator}/{country}/{start_date}/{end_date}/{econ_label}/{econ_format}")
+async def plot_correlation_api(ticker: str, start_year: str, end_year: str, indicator: str, country: str, start_date: str, end_date: str, econ_label: str, econ_format: str = None):
+    try:
+        # Call the plot_correlation function
+        plot_correlation(ticker, start_year, end_year, indicator, country, start_date, end_date, econ_label, econ_format)
+
+        # Create the 'static' directory if it doesn't exist
+        if not os.path.exists('static'):
+            os.makedirs('static')
+
+        # Save the current figure as an image file in the 'static' directory
+        image_path = f"static/{ticker}_{indicator}.png"
+        plt.savefig(image_path)
+
+        # Close the current figure to free up memory
+        plt.close()
+
+        # Return the image URL
+        return {"url": f"https://ecofin-496487b9809a.herokuapp.com/{image_path}"}
+    except Exception as e:
+        raise HTTPException(status_code=400, detail=str(e))
+
+@app.get("/plot_bollinger_bands/{ticker}/{start_date}/{end_date}/{window_size}/{num_of_std}")
+async def plot_bollinger_bands_api(ticker: str, start_date: str, end_date: str, window_size: int, num_of_std: int):
+    try:
+        # Call the plot_bollinger_bands function
+        fig = plot_bollinger_bands(ticker, start_date, end_date, window_size, num_of_std)
+
+        # Create the 'static' directory if it doesn't exist
+        if not os.path.exists('static'):
+            os.makedirs('static')
+
+        # Save the current figure as an image file in the 'static' directory
+        image_path = f"static/{ticker}_bollinger_bands.png"
+        fig.write_image(image_path)
+
+        # Return the image URL
+        return {"url": f"https://ecofin-496487b9809a.herokuapp.com/{image_path}"}
+    except Exception as e:
+        raise HTTPException(status_code=400, detail=str(e))
+
+@app.get("/get_news/{symbol}")
+async def get_news_api(symbol: str):
+    try:
+        # Call the get_news function
+        data = get_news(symbol)
+
+        # Check if data is None (an error occurred)
+        if data is None:
+            raise HTTPException(status_code=400, detail="Error fetching news data")
+
+        # Return the news data
+        return data
+    except Exception as e:
+        raise HTTPException(status_code=400, detail=str(e))
+
+@app.get("/plot_indicator_for_countries/{indicator}/{start_date}/{end_date}")
+async def plot_indicator_for_countries_api(indicator: str, countries: List[str], start_date: str, end_date: str):
+    try:
+        # Call the plot_indicator_for_countries function
+        fig = plot_indicator_for_countries(indicator, countries, start_date, end_date)
+
+        # Create the 'static' directory if it doesn't exist
+        if not os.path.exists('static'):
+            os.makedirs('static')
+
+        # Save the current figure as an image file in the 'static' directory
+        image_path = f"static/{indicator}_for_countries.png"
+        fig.write_image(image_path)
+
+        # Return the image URL
+        return {"url": f"https://ecofin-496487b9809a.herokuapp.com/{image_path}"}
+    except Exception as e:
+        raise HTTPException(status_code=400, detail=str(e))
+
+@app.get("/compare_indicators_countries/{start_date}/{end_date}")
+async def compare_indicators_countries_api(indicators: List[str], countries: List[str], start_date: str, end_date: str):
+    try:
+        # Call the compare_indicators_countries function
+        fig = compare_indicators_countries(indicators, countries, start_date, end_date)
+
+        # Create the 'static' directory if it doesn't exist
+        if not os.path.exists('static'):
+            os.makedirs('static')
+
+        # Save the current figure as an image file in the 'static' directory
+        image_path = f"static/compare_indicators_countries.png"
+        fig.write_image(image_path)
+
+        # Return the image URL
+        return {"url": f"https://ecofin-496487b9809a.herokuapp.com/{image_path}"}
+    except Exception as e:
+        raise HTTPException(status_code=400, detail=str(e))
     
-    return  plt.show()
 
-# Generate text using OpenAI GPT-3
-def generate_text(prompt):
-    os.environ['OPENAI_API_KEY'] = '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'
-    openai.api_key = os.getenv('OPENAI_API_KEY')
-    client_openai = OpenAI()
-    response = client_openai.completions.create(
-        model="gpt-3.5-turbo-instruct",
-        prompt=prompt,
-        max_tokens=150
-    )
+if __name__ == "__main__":
+    
+    parser = argparse.ArgumentParser(description="Run the FastAPI application.")
+    parser.add_argument("-p", "--port", type=int, default=8000, help="The port to bind.")
+    parser.add_argument("-r", "--reload", action="store_true", help="Enable hot reloading.")
+    args = parser.parse_args()
 
-    return response.choices[0].text.strip()
+    uvicorn.run("api:app", host="127.0.0.1", port=args.port, reload=args.reload)
```

### Comparing `EcoStock-0.1/EcoStock.egg-info/PKG-INFO` & `EcoStock-0.2/EcoStock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.1
+Version: 0.2
 Summary: A Python package for investigating the correlation between economic and financial data.
 Home-page: https://github.com/Tonij10/fastapi-project
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo
 Author-email: antoniopaparo@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EcoStock-0.1/LICENSE.md` & `EcoStock-0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `EcoStock-0.1/PKG-INFO` & `EcoStock-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.1
+Version: 0.2
 Summary: A Python package for investigating the correlation between economic and financial data.
 Home-page: https://github.com/Tonij10/fastapi-project
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo
 Author-email: antoniopaparo@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EcoStock-0.1/README.md` & `EcoStock-0.2/README.md`

 * *Files identical despite different names*

### Comparing `EcoStock-0.1/setup.py` & `EcoStock-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='EcoStock',
-    version='0.1',
+    version='0.2',
     author="Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo",
     author_email="antoniopaparo@outlook.com",
     description='A Python package for investigating the correlation between economic and financial data.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tonij10/fastapi-project",
     packages=find_packages(),
```

