# 🚕 Taxi-Trip-Data-Analysis-Using-Python

## 📌 Project Overview

This project focuses on analyzing taxi trip data using Python to identify patterns, relationships, distributions, and trends in taxi trips. The analysis explores important variables such as distance, fare, tip, tolls, total amount, payment method, and pickup borough.
The project uses Pandas, NumPy, Matplotlib, and Seaborn to perform data cleaning, exploratory data analysis (EDA), statistical analysis, and data visualization.

## 🎯 Objective

Taxi trip datasets contain information about trip distance, fares, tips, tolls, payment methods, and pickup locations. Analyzing these variables can help identify common trip patterns and understand the factors associated with taxi fares and total trip charges.
This project aims to clean and explore the taxi dataset and use different statistical and visualization techniques to discover meaningful patterns, relationships, distributions, and unusual observations.

## ❓ Problem Statement

- Analyze taxi trip data to understand overall trip patterns.
- Identify the distribution of trip distances, fares, tips, tolls, and total amounts.
- Examine the relationship between trip distance and fare.
- Compare taxi activity across different pickup boroughs.
- Analyze payment method preferences.
- Identify correlations among important numerical variables.
- Detect potential outliers in distance, fare, tip, toll, and total amounts.
- Generate meaningful insights through different visualizations.

## 🛠️ Technologies & Libraries

- Python  
- Pandas – Data manipulation and analysis  
- NumPy – Numerical operations  
- Matplotlib – Data visualization  
- Seaborn – Statistical visualization  
- Google Colab / Jupyter Notebook – Development environment

## 📂 Dataset

The dataset is loaded directly from the Seaborn built-in datasets:
import seaborn as snsdf = sns.load_dataset("taxis")

The dataset contains information related to taxi trips, including:

- Pickup and drop-off timestamps  
- Passenger count  
- Trip distance  
- Fare  
- Tip  
- Tolls  
- Total amount  
- Payment method  
- Pickup and drop-off locations  
- Pickup and drop-off boroughs  
- Pickup and drop-off zones
  
## 🧹 Data Cleaning & Preprocessing

The following preprocessing steps were performed:
- Checked the dataset structure and data types.
- Identified missing values in different columns.
- Analyzed missing values based on column type and importance.
- Applied appropriate imputation techniques where reasonable.
- Removed records where missing values could not be reasonably handled.
- Converted the pickup column into datetime format for time-based analysis.
- Examined numerical variables for unusual values and potential outliers.

## 📊 Data Visualizations

Matplotlib / Pandas Visualizations

1. Line Chart – Fare Over Time

Analyzed fare values over time using the pickup timestamp.
**Insight:** Fare values fluctuate over time, but there is no clear overall upward or downward trend. Most fares remain relatively low, with occasional high-fare trips.

2. Bar Chart – Total Fare by Pickup Borough
   
Compared the total fare generated from different pickup boroughs.
Pickup Borough	Total Fare
Bronx	          $2,078.91
Brooklyn	      $6,327.48
Manhattan	      $59,426.42
Queens	        $16,382.06
**Insight:** Manhattan generated the highest total fare among the recorded pickup boroughs. However, total fare is influenced by the number of trips as well as fare amounts.

3. Pie Chart – Payment Method
   
Analyzed the distribution of trips by payment method.
- Credit Card: 4,621 trips (~71.8%)  
- Cash: 1,812 trips (~28.2%)  
**Insight:** Credit card was the dominant payment method in the dataset.
  
4. Histogram – Trip Distance
   
Analyzed the distribution of taxi trip distances.
**Insight:** Most trips are short-distance trips, while fewer long-distance trips create a right-skewed distribution. The maximum observed distance is approximately 36.7 miles.

6. Box Plot – Tip by Pickup Borough

Compared tip distributions across pickup boroughs.
**Insight:** Most tip amounts are concentrated at lower values, while some higher-value tips appear as outliers.

## 📈 Seaborn Visualizations

8. Count Plot – Pickup Borough
   
Analyzed the number of trips recorded for each pickup borough.
**Insight:** Manhattan is the most frequent pickup borough, accounting for the majority of recorded pickup locations in this dataset.

9. Scatter Plot – Distance vs Fare
 
Examined the relationship between trip distance and fare.
**Insight:** There is a strong positive relationship between distance and fare. The correlation between distance and fare is approximately 0.920, indicating that longer trips generally have higher fares.

10. Heatmap – Correlation Analysis

Analyzed relationships among numerical variables.
Relationship	Correlation
Fare – Total	0.974
Distance – Fare	0.920
Distance – Total	0.905
Tolls – Total	0.683
Tip – Total	0.646
Distance – Tip	0.453
**Insight:** Fare and total have the strongest relationship, followed by distance and fare. Distance and total also show a strong positive relationship.

11. Pair Plot

Explored pairwise relationships between:
- Distance
- Fare
- Tip
- Total
**Insight:** The pair plot visually confirms strong relationships among distance, fare, and total, while tip has comparatively weaker relationships with the other variables.
  
12. Violin Plot – Fare by Payment Method

Compared fare distributions for cash and credit-card transactions.
**Insight:** The violin plot shows the distribution, concentration, and spread of fares across payment methods and helps identify the presence of higher-fare trips.

# 🔍 Key Insights
- Most taxi trips are short-distance trips.  
- Distance distribution is right-skewed, with a small number of long-distance trips.  
- Fare, tip, and total amounts also show right-skewed distributions.  
- Several high-value outliers are present in distance, fare, tip, and total.  
- Approximately 94.56% of trips have zero toll charges, making toll payments relatively uncommon.  
- Distance and fare have a strong positive correlation of approximately 0.920.  
- Fare and total have the strongest correlation at approximately 0.974.  
- Manhattan has the highest total fare and the largest number of recorded pickup trips.  
- Credit card is the most common payment method, accounting for approximately 71.8% of recorded trips.  
- Most tip amounts are low, with a smaller number of high-tip observations.  
- Fare values fluctuate over time without a clear overall increasing or decreasing trend.
  
## 💡 Overall Conclusion

The Taxi Trip Data Analysis project demonstrates how Python can be used to explore and understand real-world transportation data. The analysis shows that taxi trips are predominantly short-distance, while a smaller number of longer trips contribute to right-skewed distributions and high-value outliers.
Distance has a strong relationship with fare and total trip amount, while toll charges are relatively uncommon. Manhattan represents a major concentration of taxi activity in the dataset, and credit card payments are more frequently recorded than cash payments.
Overall, the project demonstrates the use of data cleaning, exploratory data analysis, statistical analysis, and visualization to transform raw taxi trip data into meaningful and interpretable insights.

## 🚀 Future Scope
- Analyze taxi demand by hour, day, and month.  
- Study peak and off-peak travel patterns.  
- Analyze average fare and distance by pickup and drop-off locations.  
- Investigate factors influencing tip amounts.  
- Develop an interactive dashboard using Power BI.  
- Build a machine learning model to predict taxi fares.  
- Analyze unusual trips and potential data-quality issues in greater detail.
  
### 👩‍💻 Author

Shanthini
Aspiring Data Analyst
Skills: Python | Pandas | NumPy | Matplotlib | Seaborn | Exploratory Data Analysis | Data Visualization
