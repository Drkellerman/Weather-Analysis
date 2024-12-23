#Objective: Analyze temperature data for 04-01-2006.

#Data Source: Kaggle Weather Data: https://www.kaggle.com/datasets/muthuj7/weather-dataset/data

#Example: This data source displays temperatures, precipiation, pressure, and other related items.

#Data Collection and Cleaning
#Importing Data


import pandas as pd

import matplotlib.pyplot as plt

import sys

import pandas as pd

# Replace 'your_file.csv' with the actual file path
df = pd.read_csv('weatherHistory.csv') 

# Print the DataFrame
print(df)

#install openPyXl
import openpyxl
from openpyxl import Workbook, load_workbook
# load in your workbook

# Select specific rows and columns using loc
#df.loc[1:25, ['Summary', 'Precip Type']]

# Select the first 25 rows and first 2 columns
subset_df = df.iloc[:26, :5]

# Print the output
print(subset_df)

# Outputs the first twenty five rows of data for 2006-04-01 only, and first four columns.

import pandas as pd

df = pd.DataFrame({'D': [9.472222222,
9.355555556,
9.377777778,
8.288888889,
8.755555556,
9.222222222,
7.733333333,
8.772222222,
10.82222222,
13.77222222,
16.01666667,
17.14444444,
17.33333333,
18.87777778,
18.91111111,
15.38888889,
14.25555556,
13.14444444,
11.18333333,
10.11666667]})



# Round to two decimal places
df = df.round(2) 
print(df)
# Temperature Output is in degrees Celsius, rounded to two decimal places. 

#Handle Missing Values: Choose how to handle missing values (drop, fill, or leave as is).
#Explain why you did this drop, fill, etc. 
#No Missing values, left as is. 

import pandas as pd

# Dataframe is named 'df' and the date column is named 'Formatted Date' and the temp column is named 'Temperature (C)'
df = pd.read_csv('weatherHistory.csv') 

df['Formatted Date'] = pd.to_datetime(df['Formatted Date'])
df['Temperature (C)'] = pd.to_numeric(df['Temperature (C)'], errors='coerce') 

print(df)

#Descriptive Statistics: Provide summary statistics (mean, median, min, max) for numerical columns.
#Data Visualizations:
#Required: One visualization (e.g., line plot) if time-series data is relevant.
#Optional: Additional visuals like bar charts for comparisons, histograms for distributions, or scatter plots for relationships.

import pandas as pd

df = pd.read_csv('weatherHistory.csv')

df= pd.DataFrame({
    'D': [9.472222222,
9.355555556,
9.377777778,
8.288888889,
8.755555556,
9.222222222,
7.733333333,
8.772222222,
10.82222222,
13.77222222,
16.01666667,
17.14444444,
17.8,
17.33333333,
18.87777778,
18.91111111,
15.38888889,
15.55,
14.25555556,
13.14444444,
11.55,
11.18333333,
10.11666667,
10.2
]
})

# Calculate summary statistics for numerical columns
summary_stats = df.describe()

# Extract mean, median, min, and max
mean = summary_stats.loc['mean']
median = summary_stats.loc['50%']
min_val = summary_stats.loc['min']
max_val = summary_stats.loc['max']

print("Mean:", mean)
print("Median:", median)
print("Min:", min_val)
print("Max:", max_val)

#summary_stats = df.agg(['mean', 'median', 'min', 'max'])
#print(summary_stats)

#Analysis and Insights
#Findings: Summarize any patterns observed and address the main project question.
#Supporting Data: Reference specific statistics or plot features to back up findings.

#Data Visualizations:
#Required: One visualization (e.g., line plot) if time-series data is relevant.
#Optional: Additional visuals like bar charts for comparisons, histograms for distributions, or scatter plots for relationships.

import pandas as pd
import matplotlib.pyplot as plt
#octal_string = '0o10' 


# Sample data For 10 data points for date/time and temperature
df = pd.read_csv('weatherHistory.csv')

data= df[['Formatted Date', 'Temperature (C)']]

weather = pd.DataFrame({'Formatted Date':[
"2006-4-1 12:00:00",
"2006-4-1 1:00:00",
"2006-4-1 2:00:00",
"2006-4-1 3:00:00",
"2006-4-1 4:00:00",
"2006-4-1 5:00:00",
"2006-4-1 6:00:00",
"2006-4-1 7:00:00",
"2006-4-1 8:00:00",
"2006-4-1 9:00:00"],

'Temperature (C)': [9.472222222,
9.355555556,
9.377777778,
8.288888889,
8.755555556,
9.222222222,
7.733333333,
8.772222222,
10.82222222,
13.77222222
]})

# Create a DataFrame
df = pd.DataFrame(data)

# Create the line plot
weather.plot(x= 'Formatted Date', y= 'Temperature (C)', kind = 'line')
# Rotate the x-axis labels
plt.xticks(rotation=45)
weather.plot(figsize=(20,4))
# Reduce the number of ticks
plt.xticks(range(0, 10, 2))
# Adjust figure size
plt.figure(figsize=(10, 6))
plt.show()


# Create a bar graph
weather.plot.bar(x='Formatted Date', y= 'Temperature (C)', title= 'Bar Graph')
# Rotate the x-axis labels
plt.xticks(rotation=45)
weather.plot(figsize=(20,4))
# Reduce the number of ticks
plt.xticks(range(0, 10, 2))
# Adjust figure size
plt.figure(figsize=(10, 6))
plt.show()


# Create a scatter plot
weather.plot.scatter(x='Formatted Date', y= 'Temperature (C)', title= 'Scatter Plot')
# Rotate the x-axis labels
plt.xticks(rotation=45)
weather.plot(figsize=(20,4))
# Reduce the number of ticks
plt.xticks(range(0, 10, 2))
# Adjust figure size
plt.figure(figsize=(10, 6))
plt.show()


#df.plot(x='Formatted Date', y='Temperature (C)', kind='line')

# Put On title and labels
#plt.title('Temperature Change Over One Day In Ten Hours')
#plt.xlabel('Formatted Date')
#plt.ylabel('Temperature (C)')



# Rotate x-axis labels for readability


# Show the plot
#plt.tight_layout()
#plt.show()



# Display the plot
#plt.show()

# Analysis and Insights 
# Findings: Summarize any patterns observed and address the main project question. 
# Supporting Data: Reference specific statistics or plot features to back up findings. 

# The analysis of the data shows a plot of temperatures for a ten hour period. The pattern of falling temperatures continue through
#  the overnight hours leading up to sunrise, with the coolest temperature observered right before sunrise at around 6 AM at 8 degrees Celsuis.
# In meteorology, the temperatures cool at night due to radiational cooling, and is also dependent on cloud cover and wind speeds.

# This appears to be a warmer weather pattern as the temperatures still rise quickly after sunrise even with cloud cover and rain.
# As mentioned, the temperatures generally decrease between midnight through most of the night, but features a sudden drop between
# after 5:00 AM, with the minimum being reached at 6:00 AM per the Line Graph, Bar Graph, and Scatter Plot Graphs. 

# Conclusion and Recommendations (10 points) 
# Summarize: Present the main conclusions drawn from the analysis. 
# Recommendations: Based on findings, suggest actions or further analysis. 

# The main summary and conclusions from the weather data indicate that temperatures were dropping during the overnight hours with moderate
# winds along with partly cloudy conditions. The lowest temperature was reached at 6:00 AM, and the temperature rapidly warmed during the
# early morning hours- with wind speeds continuing to be elevated- meaning warmer air aloft was mixing down to the surface, heating the
# ground with partly cloudy conditions. 

# I want to further study the data to find further trends regarding wind speeds at night, cloud cover, and overnight low temperatures.
# This may involve consulting other sources of recorded data pertaining to this time period to confirm information or add to it. 

