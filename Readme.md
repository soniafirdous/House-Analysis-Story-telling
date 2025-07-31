🏠 Housing Data Analysis

This project explores and analyzes a housing dataset to uncover insights into pricing, area, bedroom distribution, and more. The analysis includes detailed univariate and multivariate statistics, visualizations, and data storytelling to help understand the key factors that influence housing prices.

📁 Dataset

Filename: Housing.csv

Location: /content/Housing.csv

Description: Contains details of houses including price, area, number of bedrooms, bathrooms, and more.

📦 Libraries Used

import numpy as np  
import pandas as pd  
import matplotlib.pyplot as plt  
import seaborn as sns  
%matplotlib inline is used for inline plotting in Jupyter notebooks.

🔍 Project Workflow

1. Data Loading and Overview
Load CSV using pandas.

Use .head(), .tail(), .info(), .describe() to inspect the data.

Checked for null/missing values.

2. Feature Classification
Numerical Columns: Identified using select_dtypes.

Categorical Columns: Extracted for further EDA.

📊 Exploratory Data Analysis (EDA)

🔢 Numerical Analysis

Computed statistics for each numerical column:

Mean, Median, Mode

Standard Deviation, Variance

Skewness, Kurtosis

Min, Max

Visualizations:

Histograms

Boxplots (for outlier detection)

📈 Univariate Analysis
🏷 Price
Right-skewed distribution.

High variability with significant outliers.

Prices range from ₹1.75M to ₹13.3M.

Coefficient of Variation: ~39%

📐 Area
Also right-skewed with large spread.

Area ranges from 1,650 to 16,200 sq.ft.

Coefficient of Variation: ~42%

🛏 Bedrooms
Most common: 3 bedrooms.

Mild right skew due to 5-6 bedroom homes.

Low variability, IQR = 1.

🔁 Multivariate Analysis

💰 Price vs Area
Positive correlation: larger houses tend to cost more.

Heavier tails in area distribution indicate extreme values.

Dense clustering in mid-sized homes (2,500–6,000 sq.ft).

💰 Price vs Bathrooms
Price increases with more bathrooms (up to 5), then drops slightly.

Median is more stable than mean due to outliers.

📚 Insights & Storytelling

Most homes cluster in the middle market with mid-sized houses and mid-range prices.
Mean prices are skewed by a few luxury homes, so median is more representative of central tendency.
Bedroom count alone doesn’t fully explain price variance—additional features like location, furnishing, and access to main roads matter.
Both buyers and sellers should analyze median prices of similarly featured homes for a realistic market view.


📈 Sample Plots

Distribution of Price and Area

Boxplots for detecting outliers

Countplot for Bedrooms

Scatter plot: Price vs Area

📌 Future Improvements

Build predictive models (e.g., linear regression)

Include location-based filtering

Add categorical feature analysis (furnishing, main road access, etc.)

Interactive dashboards using Plotly or Streamlit

👨‍💻 Author
SONIA FIRDOUS