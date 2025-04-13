# Bitcoin-Historical-Data
This repository analyzes cryptocurrency data with a focus on data processing and EDA. It includes steps for cleaning raw data, handling missing values, converting timestamps, and generating visualizations like line plots and scatter plots to explore price trends, volume patterns, and correlations.
Project Overview
The dataset contains cryptocurrency price information, with columns such as Timestamp, Open, High, Low, Close, Volume, Date, and Time. The main objective is to process the raw data and use it for generating meaningful insights through EDA.

Data Processing
Handling Missing Values:

Missing values in the datetime column are filled with a placeholder timestamp.

Other columns like Volume, Open, High, Low, Close are checked for missing values and handled appropriately.

Timestamp Conversion:

The raw dataset includes separate date and time columns. These are combined to create a single datetime column.

The datetime column is then converted to a datetime64 type for proper time series analysis.

Data Type Conversion:

Columns like Open, High, Low, Close, and Volume are converted to numeric types for accurate analysis.

The datetime column is set as the index to facilitate time-based analysis.

Resampling and Aggregation:

Data can be resampled into different time intervals, such as hourly or daily, for analysis.

Aggregation techniques like calculating the mean, sum, or other statistical measures can be applied to explore trends over time.

Exploratory Data Analysis (EDA)
Descriptive Statistics:

Basic summary statistics such as mean, median, standard deviation, and percentiles are calculated for each numerical column to understand the distribution of the data.

Correlation Analysis:

Correlations between various numerical columns (such as Open, High, Low, Close, and Volume) are examined to identify any relationships and dependencies.

Visualizations:

Time Series Plots:

Line plots are used to visualize price trends over time (e.g., Close vs. datetime).

Scatter Plots:

Scatter plots are used to visualize relationships between Open, Close, High, Low, and Volume.

Group-by Analysis:

Data is grouped by different time periods (e.g., by day, week, or month) to observe patterns in the data.

Sorted data is plotted to show trends and anomalies clearly.

Handling Outliers:

Potential outliers in the data are detected and handled using statistical methods (e.g., using z-scores or IQR for outlier detection).

Feature Engineering:

Additional columns may be derived from existing data, such as moving averages (SMA, EMA), price change percentage, or volatility measures.

Volume Analysis:

Volume is analyzed to understand trading activity and its relationship with price changes.

Visualizations
Price Trends Over Time: Line plots for Open, High, Low, and Close prices.

Volume vs Price: Scatter plots to explore the relationship between volume and price.

Moving Averages: Line plots to observe how the price smooths over different moving average periods.
