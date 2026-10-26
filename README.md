#  Apple (AAPL) Stock Data Analysis Using Python

##  Project Overview

This project focuses on understanding, cleaning, analyzing, and visualizing Apple (AAPL) stock market data using Python. It explores historical stock prices, daily price changes, percentage returns, trading volume trends, and unusual trading activities.

The project uses Python libraries such as Pandas, NumPy, and Matplotlib to perform data preprocessing, statistical calculations, and data visualization. It helps identify patterns in stock market data and understand daily stock price movements through graphical representations.

##  Project Objectives

The main objectives of this project are:

- To load and explore Apple stock market data.
- To inspect dataset structure, column names, data types, and missing values.
- To clean and preprocess stock market data.
- To calculate daily price changes using opening and closing prices.
- To calculate daily percentage returns.
- To analyze historical trading volume trends.
- To identify unusual trading volume using statistical methods.
- To visualize daily stock returns and trading volume.
- To calculate the mean, variance, and standard deviation of stock returns.
- To save the cleaned dataset for further analysis.

##  Technologies Used

The following tools and technologies are used in this project:

- **Python:** Main programming language for data analysis.
- **Pandas:** Used for loading, cleaning, manipulating, and analyzing data.
- **NumPy:** Supports numerical operations and statistical analysis.
- **Matplotlib:** Used to create charts and visualize stock market trends.
- **Google Colab:** Cloud-based environment for running Python code.
- **Jupyter Notebook:** Used to organize and execute analysis step by step.

##  Dataset Description

The project uses an Apple stock market dataset named `AAPL.csv.xls`.

The dataset contains the following attributes:

| Column | Description |
|---|---|
| Date | Date of the stock market record |
| Open | Stock price at the beginning of the trading period |
| High | Highest stock price during the trading period |
| Low | Lowest stock price during the trading period |
| Close | Stock price at the end of the trading period |
| Volume | Number of shares traded during the period |

These attributes are used to study stock price movements, trading activity, and return distributions.

##  Project Implementation

### 1. Data Loading and Exploration

The dataset is loaded using Pandas. Initial exploration is performed using functions such as `head()`, `info()`, `describe()`, and `shape`.

This step helps understand the dataset's structure, identify available columns, inspect data types, and check for missing values.

### 2. Data Cleaning and Preprocessing

The dataset is prepared for analysis by performing the following operations:

- Converting the Date column into datetime format.
- Converting stock price and volume columns into numeric values.
- Handling invalid or missing values in important numerical columns.
- Sorting records by date.
- Selecting the required columns for analysis.

These steps help improve data consistency and prepare the dataset for further calculations.

### 3. Daily Price Change Calculation

The daily price change is calculated by subtracting the opening price from the closing price.

**Formula:**

`Price Delta = Close - Open`

A positive value indicates that the closing price is higher than the opening price, while a negative value indicates that the closing price is lower.

This calculation helps examine daily stock price movements.

### 4. Daily Percentage Return Analysis

The daily percentage return is calculated to understand the relative change between the opening and closing prices.

**Formula:**

`Daily Return (%) = ((Close - Open) / Open) × 100`

This value expresses the daily price change as a percentage, making it easier to compare movements across different price levels.

### 5. Trading Volume Trend Analysis

Matplotlib is used to create a line chart showing trading volume over time.

This visualization helps identify changes in trading activity and periods with unusually high trading volumes.

The average trading volume is also calculated to provide a reference point for understanding trading activity.

### 6. Anomalous Trading Day Detection

The project identifies unusually high trading volumes using the mean and standard deviation.

**Formula:**

`Anomaly Limit = Mean Volume + (2 × Standard Deviation)`

Trading days with volumes above this threshold are classified as anomalous for this analysis.

A chart displays trading volume alongside the anomaly threshold, helping visualize periods of unusually high trading activity.

**Note:** These observations indicate unusual trading volume, but they do not establish the cause of the activity or predict future stock movements.

### 7. Stock Return Distribution

A histogram is created to visualize the distribution of daily percentage returns.

This chart helps examine how frequently different return values occur and understand the general pattern of daily price movements.

### 8. Statistical Analysis

The project calculates three statistical measures for daily percentage returns:

- **Mean:** Represents the average daily percentage return.
- **Variance:** Measures the spread of daily returns around their mean.
- **Standard Deviation:** Measures the typical dispersion of daily returns around their mean.

These measures help summarize the characteristics and variability of the observed daily returns.

### 9. Exporting the Cleaned Dataset

After completing the analysis, the processed dataset is saved as `AAPL_cleaned.csv`.

This file contains the cleaned stock data along with the calculated price delta and daily return columns.

The exported dataset can be reused for further data analysis and visualization projects.

##  Visualizations

The project generates the following visualizations:

1. **Trading Volume Trend:** Displays trading volume changes over time.
2. **Trading Volume with Anomaly Limit:** Highlights trading days with unusually high volumes.
3. **Daily Return Distribution:** Shows the distribution of daily percentage returns.

These visualizations make the results easier to interpret and understand.

##  Project Structure

```text
Apple-Stock-Data-Analysis/
│
├── AAPL.csv.xls
├── AAPL_cleaned.csv
├── DV_TASK_3.ipynb
├── dv_task_3.py
└── README.md
```

*Note: `AAPL_cleaned.csv` is generated after running the notebook or Python script.*

##  How to Run the Project

Follow these steps to run the project:

1. Clone or download the GitHub repository.
2. Open `DV_TASK_3.ipynb` in Google Colab or Jupyter Notebook.
3. Upload the Apple stock dataset.
4. Update the dataset path in the code according to your environment.
5. Install the required Python libraries if they are not already available.
6. Execute the notebook cells in order.
7. Review the generated charts and statistical results.
8. Access the cleaned dataset saved as `AAPL_cleaned.csv`.

### Required Libraries

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
```

##  Key Learning Outcomes

Through this project, I developed practical knowledge of:

- Loading and exploring real-world stock market data.
- Cleaning and preprocessing datasets using Pandas.
- Performing numerical calculations with Python.
- Calculating daily price changes and percentage returns.
- Analyzing trading volume trends.
- Applying statistical thresholds to identify unusual observations.
- Creating meaningful data visualizations.
- Calculating statistical measures such as mean, variance, and standard deviation.
- Exporting cleaned datasets for future use.

##  Future Enhancements

The project can be extended with the following features:

- Compare Apple stock performance with other technology companies.
- Create interactive charts using Plotly.
- Analyze moving averages and longer-term price trends.
- Explore relationships between trading volume and price changes.
- Add additional statistical methods for detecting unusual observations.
- Develop a dashboard for exploring stock market data interactively.

##  Conclusion

The Apple Stock Data Analysis project demonstrates how Python can be used to clean, analyze, and visualize financial datasets. By calculating daily price changes, percentage returns, trading volume trends, and statistical measures, the project provides a structured overview of historical stock market activity.

The project also demonstrates the importance of data preprocessing and visualization in exploratory data analysis. It serves as a practical learning project for developing Python programming, data analysis, statistical analysis, and data visualization skills.

##  Author

**Gnana Yoshua**

Aspiring Data Analyst | Python Programmer | Data Visualization Enthusiast

This project was developed to gain practical experience in Python-based data analysis and visualization.

---

⭐ If you find this project useful, consider giving the repository a star!
