# Comparing `tmp/glook-0.1.5-py3-none-any.whl.zip` & `tmp/glook-0.1.5b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,20 @@
-Zip file size: 17536 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat     3200 b- defN 24-Apr-16 17:28 glook/GLook.py
+Zip file size: 54246 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat     3200 b- defN 24-Apr-24 16:04 glook/GLook.py
 -rw-rw-rw-  2.0 fat       51 b- defN 24-Mar-25 17:39 glook/__init__.py
 -rw-rw-rw-  2.0 fat      339 b- defN 24-Mar-25 18:24 glook/cli.py
--rw-rw-rw-  2.0 fat     3698 b- defN 24-Apr-14 17:22 glook/pages/1_General_Data_Insights.py
--rw-rw-rw-  2.0 fat    17728 b- defN 24-Apr-14 15:18 glook/pages/2_Univariate_Analysis.py
--rw-rw-rw-  2.0 fat     7813 b- defN 24-Apr-16 16:59 glook/pages/3_Bivariate_Analysis.py
--rw-rw-rw-  2.0 fat     7647 b- defN 24-Apr-16 17:15 glook/pages/4_Trivariate_Analysis.py
--rw-rw-rw-  2.0 fat     7139 b- defN 24-Apr-26 19:08 glook-0.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-26 19:08 glook-0.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       38 b- defN 24-Apr-26 19:08 glook-0.1.5.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-26 19:08 glook-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      967 b- defN 24-Apr-26 19:08 glook-0.1.5.dist-info/RECORD
-12 files, 48718 bytes uncompressed, 15910 bytes compressed:  67.3%
+-rw-rw-rw-  2.0 fat    25002 b- defN 24-Apr-10 10:33 glook/pages/10_Unsupervised_learning.py
+-rw-rw-rw-  2.0 fat    96985 b- defN 24-Apr-27 21:03 glook/pages/11_Custom_Model_Training.py
+-rw-rw-rw-  2.0 fat     5875 b- defN 24-Apr-27 19:48 glook/pages/1_General_Data_Insights.py
+-rw-rw-rw-  2.0 fat    19725 b- defN 24-Apr-27 19:10 glook/pages/2_Univariate_Analysis.py
+-rw-rw-rw-  2.0 fat     7813 b- defN 24-Apr-24 16:05 glook/pages/3_Bivariate_Analysis.py
+-rw-rw-rw-  2.0 fat     7647 b- defN 24-Apr-24 16:05 glook/pages/4_Trivariate_Analysis.py
+-rw-rw-rw-  2.0 fat   130608 b- defN 24-Apr-27 20:33 glook/pages/5_Pre_Processing.py
+-rw-rw-rw-  2.0 fat     3315 b- defN 24-Apr-27 20:41 glook/pages/6_Split_Data.py
+-rw-rw-rw-  2.0 fat     4588 b- defN 24-Apr-11 19:05 glook/pages/7_Dimensionality_Reduction.py
+-rw-rw-rw-  2.0 fat    59951 b- defN 24-Apr-27 20:43 glook/pages/8_Supervised_Learning.py
+-rw-rw-rw-  2.0 fat     7141 b- defN 24-Apr-27 21:14 glook-0.1.5b1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-27 21:14 glook-0.1.5b1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       38 b- defN 24-Apr-27 21:14 glook-0.1.5b1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-27 21:14 glook-0.1.5b1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1537 b- defN 24-Apr-27 21:14 glook-0.1.5b1.dist-info/RECORD
+18 files, 373913 bytes uncompressed, 51718 bytes compressed:  86.2%
```

## zipnote {}

```diff
@@ -3,35 +3,53 @@
 
 Filename: glook/__init__.py
 Comment: 
 
 Filename: glook/cli.py
 Comment: 
 
+Filename: glook/pages/10_Unsupervised_learning.py
+Comment: 
+
+Filename: glook/pages/11_Custom_Model_Training.py
+Comment: 
+
 Filename: glook/pages/1_General_Data_Insights.py
 Comment: 
 
 Filename: glook/pages/2_Univariate_Analysis.py
 Comment: 
 
 Filename: glook/pages/3_Bivariate_Analysis.py
 Comment: 
 
 Filename: glook/pages/4_Trivariate_Analysis.py
 Comment: 
 
-Filename: glook-0.1.5.dist-info/METADATA
+Filename: glook/pages/5_Pre_Processing.py
+Comment: 
+
+Filename: glook/pages/6_Split_Data.py
+Comment: 
+
+Filename: glook/pages/7_Dimensionality_Reduction.py
+Comment: 
+
+Filename: glook/pages/8_Supervised_Learning.py
+Comment: 
+
+Filename: glook-0.1.5b1.dist-info/METADATA
 Comment: 
 
-Filename: glook-0.1.5.dist-info/WHEEL
+Filename: glook-0.1.5b1.dist-info/WHEEL
 Comment: 
 
-Filename: glook-0.1.5.dist-info/entry_points.txt
+Filename: glook-0.1.5b1.dist-info/entry_points.txt
 Comment: 
 
-Filename: glook-0.1.5.dist-info/top_level.txt
+Filename: glook-0.1.5b1.dist-info/top_level.txt
 Comment: 
 
-Filename: glook-0.1.5.dist-info/RECORD
+Filename: glook-0.1.5b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## glook/pages/1_General_Data_Insights.py

```diff
@@ -1,10 +1,11 @@
 import streamlit as st
 import pandas as pd
 import plotly.graph_objects as go
+from io import StringIO
 st.set_page_config(page_title="GLook", layout="wide")
 st.write("Session State:->", st.session_state["shared"])
 
 
 if "df" in st.session_state and st.session_state.df is not None:
 	df = st.session_state.df
 	# Get number of rows
@@ -30,45 +31,100 @@
 	
 	# st.dataframe(df)
 	# Exclude non-numeric columns
 	numeric_df = df.select_dtypes(include='number')
 
 	# Convert non-numeric values to NaN
 	numeric_df = numeric_df.apply(pd.to_numeric, errors='coerce')
-	st.header(":green[Correlation Coefficient Heatmap]")
+	st.header("Correlation Coefficient :green[Heatmap]")
 	# Calculate the correlation matrix
 	correlation_matrix = numeric_df.corr()
 	# Define the list of colorscales
 	# colorscales = ['aggrnyl', 'agsunset', 'algae', 'amp', 'armyrose', 'balance', 'blackbody', 'bluered', 'blues', 'blugrn', 'bluyl', 'brbg', 'brwnyl', 'bugn', 'bupu', 'burg', 'burgyl', 'cividis', 'curl', 'darkmint', 'deep', 'delta', 'dense', 'earth', 'edge', 'electric', 'emrld', 'fall', 'geyser', 'gnbu', 'gray', 'greens', 'greys', 'haline', 'hot', 'hsv', 'ice', 'icefire', 'inferno', 'jet', 'magenta', 'magma', 'matter', 'mint', 'mrybm', 'mygbm', 'oranges', 'orrd', 'oryel', 'oxy', 'peach', 'phase', 'picnic', 'pinkyl', 'piyg', 'plasma', 'plotly3', 'portland', 'prgn', 'pubu', 'pubugn', 'puor', 'purd', 'purp', 'purples', 'purpor', 'rainbow', 'rdbu', 'rdgy', 'rdpu', 'rdylbu', 'rdylgn', 'redor', 'reds', 'solar', 'spectral', 'speed', 'sunset', 'sunsetdark', 'teal', 'tealgrn', 'tealrose', 'tempo', 'temps', 'thermal', 'tropic', 'turbid', 'turbo', 'twilight', 'viridis', 'ylgn', 'ylgnbu', 'ylorbr', 'ylorrd']
 	# Number input for selecting the colorscale index
 	# colorscale_index = st.number_input('Select a colorscale index:', min_value=0, max_value=len(colorscales)-1, value=0)
 	# st.write(colorscales[colorscale_index])
 	# Create the heatmap plot
+
 	fig = go.Figure(data=go.Heatmap(
 		z=correlation_matrix.values,
 		x=correlation_matrix.columns,
 		y=correlation_matrix.index,
 		# colorscale=colorscales[colorscale_index],  # You can choose any colorscale
-		colorscale='aggrnyl'
+		colorscale='aggrnyl',
+		text=correlation_matrix.values,  # Values to display
+		texttemplate='%{text:.2f}',  # Format for displaying values
+		showscale=True  # Display the color scale on the side
 	))
 
 	# Add title and axis labels
 	fig.update_layout(
 		title='Correlation Coefficient Heatmap',
 		xaxis=dict(title='Columns'),
 		yaxis=dict(title='Columns'),
 		width=700,  # Adjust width
 		height=700,  # Adjust height
+
 	)
 
 	# Show the plot
 	st.plotly_chart(fig)
 
-	st.data_editor(df)
-	
+	st.header(":green[Edit Data] to Suit Your Needs:")
+	df = st.data_editor(df)
+
+
+	# Capture the output of df.info()
+	info_buffer = StringIO()
+	df.info(buf=info_buffer)
+	info_str = info_buffer.getvalue()
+
+	# Display the info in Streamlit
+	st.subheader("DataFrame :green[Info:]")
+	st.code(info_str, language="neon")
+
+
+
+	st.header("Numerical :green[Data Overview]")
+	# df_info = df.describe().T
+	# styled_df_info = df_info.style.highlight_max(axis=0).highlight_min(axis=0).format("{:.2f}")
+	df_info = (
+		df.describe().T.style.set_table_styles(
+			[
+				{'selector': 'th', 'props': 'background-color: lightgreen; color: black;'},  # Table headers
+				{'selector': 'td', 'props': 'background-color: lightblue; border: 1px solid black;'},  # Table cells
+				{'selector': 'tr', 'props': 'border: 1px solid black;'}  # Table rows
+			]
+		)
+		.highlight_max(axis=0, props='background-color: darkgreen; color: white;')  # Highlight max values with specific color
+		.highlight_min(axis=0, props='background-color: yellowgreen; color: black;')  # Highlight min values with another color
+		.format("{:.2f}")
+	)
+	st.dataframe(df_info)
+
+	st.header("Categorical :green[Data Overview]")
+
+	df_info1 = df.select_dtypes(include=['object']).describe().T
+
+	# Style to highlight the most frequent category
+	styled_df_info1 = (
+    df_info1.style.set_table_styles(
+			[
+				{'selector': 'th', 'props': 'background-color: lightgreen; color: black;'},  # Table headers
+				{'selector': 'td', 'props': 'background-color: lightblue; border: 1px solid black;'},  # Table cells
+				{'selector': 'tr', 'props': 'border: 1px solid black;'}  # Table rows
+			]
+		)
+		.highlight_max(axis=0, props='background-color: darkgreen; color: white;')  # Highlight max values with specific color
+		.highlight_min(axis=0, props='background-color: yellowgreen; color: black;')  # Highlight min values with another color
+		# .format("{:.2f}")
+	)
+
+	st.dataframe(styled_df_info1, width = 720)
+
 	# Display the insights
 	st.subheader(f"Data dimensions: :green[{num_rows} rows, {num_columns} columns]")
 	st.subheader(f"Number of rows: :green[{num_rows}]")
 	st.subheader(f"Number of duplicates: :green[{num_duplicates}]")
 	st.subheader(f"Memory usage: :green[{memory_usage:.5f} KB]")
 	st.subheader(f"Number of features: :green[{num_features}]")
 	st.subheader(f"Number of categorical features: :green[{num_categorical}]")
```

## glook/pages/2_Univariate_Analysis.py

```diff
@@ -297,17 +297,47 @@
 							st.write(df[column].head())
 
 					with tab2:
 						# Prepare data for donut chart
 						data = limit_unique_values(df[column]).value_counts().reset_index()
 						data.columns = [column, 'count']
 
+						# fig = px.pie(data, values='count', names=column, hole=0.4)
+
+						# Create a pie chart with a donut style (hole)
+						# Create a pie chart with a donut style (hole)
 						fig = px.pie(data, values='count', names=column, hole=0.5)
-						fig.update_traces(textposition='inside', textinfo='percent+label')
-						fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1))
+
+						# Customize the traces
+						fig.update_traces(
+							textposition='inside',  # Place labels inside pie slices
+							textinfo='percent+label',  # Show percentage and label
+							marker=dict(
+								line=dict(color='black', width=3.5)  # Black border for contrast
+							),
+							pull=0.05,  # Pull segments outward slightly when hovered
+							hoverinfo='label+percent+name',  # Display information on hover
+							hoverlabel=dict(bgcolor='white', font_size=12, font_color='black')  # Customize hover label appearance
+						)
+
+						# Customize the layout with proper legend position and margins
+						fig.update_layout(
+							title=f'Category Distribution for {str(column)}',  # Title of the pie chart
+							legend=dict(
+								orientation="v",  # Vertical legend
+								yanchor="top",  # Anchor to the top
+								y=1,  # Position along y-axis
+								xanchor="left",  # Anchor to the left
+								x=-0.35  # Left position (x-axis) to ensure it's away from the plot
+							),
+							width=600,  # Adjust the width
+							height=600,  # Adjust the height
+							margin=dict(l=50, r=50, t=50, b=50),  # Increase left margin for more space
+							showlegend=True  # Display the legend
+						)
 						st.plotly_chart(fig)
 						print("j")
 						# st.header("An owl")
 						# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
 
 					# with tab3:
 					# 	# Concatenate all values of the column into a single string
@@ -425,15 +455,32 @@
 							# st.write(f"**Interquartile range:** {insights.get('Interquartile range', 'N/A')}")
 							st.write(f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]")
 							st.write(f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]")
 							st.write(f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]")
 						
 
 					with tab2:
-						fig = px.box(df, y=column)
+						fig = px.box(df, y=column, title=str(column))
+						# Center the title by setting title_x to 0.5
+					# Customize the box plot with trace-specific properties
+						fig.update_traces(
+							marker=dict(color='forestgreen'), #yellowgreen # Set the color to yellow-green
+							boxmean=True,  # Display the mean as a line in the box plot
+						)
+
+						# Set the plot title, center it, and adjust the height
+						fig.update_layout(
+							title={
+								'text': f'Box Plot for {column}',
+								'x': 0.5,  # Center the title
+								'xanchor': 'center',  # Title alignment to be centered
+								'yanchor': 'top'  # Title anchor point
+							},
+							height=500,  # Set the plot height
+						)
 						st.plotly_chart(fig)
 
 					with tab3:
 						plt.figure(figsize=(10, 6))  # Adjust figure size
 
 						# Generate QQ plot
 						qqplot_data = sm.qqplot(df[column], line='s').gca().lines
@@ -441,48 +488,45 @@
 						fig = go.Figure()
 						fig.add_trace({
 							'type': 'scatter',
 							'x': qqplot_data[0].get_xdata(),
 							'y': qqplot_data[0].get_ydata(),
 							'mode': 'markers',
 							'marker': {
-								'color': '#19d3f3'
-							}
+								'color': '#1f77b4' # Blue color #1f77b4  # blue
+							},
+							'name': 'Sample Data Points',
 						})
 
 						fig.add_trace({
 							'type': 'scatter',
 							'x': qqplot_data[1].get_xdata(),
 							'y': qqplot_data[1].get_ydata(),
 							'mode': 'lines',
 							'line': {
-								'color': '#636efa'
-							}
+								'color': 'red' # Bright green
+							},
+							'name': 'Theoretical Line',
 						})
 
 						# Add reference line (identity line)
 						x_min = min(qqplot_data[0].get_xdata())
 						x_max = max(qqplot_data[0].get_xdata())
 						y_min = min(qqplot_data[0].get_ydata())
 						y_max = max(qqplot_data[0].get_ydata())
-						fig.add_trace(go.Scatter(x=[x_min, x_max], y=[y_min, y_max], mode='lines', line=dict(color='red', width=2), name='Identity Line'))
+						fig.add_trace(go.Scatter(x=[x_min, x_max], y=[y_min, y_max], mode='lines', line=dict(color='#00ff00', width=2), name='Identity Line'))
 
-						fig.update_layout({
-							'title': f'QQ Plot for {column}',
-							'xaxis': {
-								'title': 'Theoretical Quantiles',
-								'zeroline': False
-							},
-							'yaxis': {
-								'title': 'Sample Quantiles'
-							},
-							'showlegend': False,
-							'width': 800,
-							'height': 700,
-						})
+						fig.update_layout(
+							title=f'QQ Plot for {column}',
+							xaxis=dict(title='Theoretical Quantiles', zeroline=False),
+							yaxis=dict(title='Sample Quantiles'),
+							showlegend=True,  # Now shows the legend
+							width=800,
+							height=700
+						)
 
 						st.plotly_chart(fig)
 		# st.text("hi")
 		# et = time.time()
 		# tt = et - s
 		# st.text(tt)
 			# st.write("hehe")
```

## Comparing `glook-0.1.5.dist-info/METADATA` & `glook-0.1.5b1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glook
-Version: 0.1.5
+Version: 0.1.5b1
 Summary: Auto EDA.
 Home-page: https://github.com/gaurang157/glook
 Author: Gaurang Ingle
 Author-email: gaurang.ingle@gmail.com
 Maintainer: Gaurang Ingle, Sharat Chandra Manikonda
 Maintainer-email: manikondasharat@gmail.com
 License: MIT
```

### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: glook Version: 0.1.5 Summary: Auto EDA. Home-page:
-https://github.com/gaurang157/glook Author: Gaurang Ingle Author-email:
+Metadata-Version: 2.1 Name: glook Version: 0.1.5b1 Summary: Auto EDA. Home-
+page: https://github.com/gaurang157/glook Author: Gaurang Ingle Author-email:
 gaurang.ingle@gmail.com Maintainer: Gaurang Ingle, Sharat Chandra Manikonda
 Maintainer-email: manikondasharat@gmail.com License: MIT Project-URL: Bug
 Reports, https://github.com/gaurang157/glook/issues Project-URL: Source, https:
 //github.com/gaurang157/glook Project-URL: Documentation, https://github.com/
 gaurang157/glook/blob/main/README.md Project-URL: Say Thanks!, https://
 github.com/gaurang157/glook/issues/new?assignees=&labels=&template=thanks.yml
 Keywords: AutoEDA,Exploratory Data Analysis,Data
```

