# 📊 E-Commerce Sales Data Analysis

## 🎯 Project Overview
This project focuses on analyzing 12 months of sales data for an electronics store. The goal is to clean the raw data, perform exploratory data analysis (EDA), and answer key business questions to help the marketing and sales teams optimize their strategies, improve advertising campaigns, and increase overall revenue.

## 🛠️ Tools & Technologies Used
* **Python** (Core language)
* **Pandas** (Data manipulation, merging, and cleaning)
* **Matplotlib & Seaborn** (Data visualization)
* **Jupyter Notebook** (Development environment)

## 🧹 Data Cleaning & Preprocessing
Before analyzing the data, extensive cleaning and preprocessing were performed to ensure data integrity:
1. **Data Consolidation:** Merged 12 individual monthly CSV files into a single master Pandas DataFrame.
2. **Datetime Parsing:** Converted the combined 'Order Date' column into a true `datetime` format. Extracted specific 'Date' and 'Time' properties into separate columns using `.dt` accessors for time-series analysis.
3. **Data Type Casting:** Converted string-formatted numeric columns (Quantity Ordered, Price Each) into appropriate numeric data types.
4. **Feature Engineering:** * Split the 'Purchase Address' into four distinct columns: `Street`, `City`, `State`, and `Zip Code` for geographical analysis.
   * Created a new `Sales` column by multiplying `Quantity Ordered` by `Price Each`.

## 📈 Business Questions Answered
Through this analysis, actionable insights were extracted by answering the following business questions:

1. **What was the best month for sales? How much was earned that month?**
   * *Identified peak purchasing seasons to help allocate inventory.*
2. **What city had the highest number of sales?**
   * *Pinpointed geographical hotspots for targeted regional marketing.*
3. **What time should we display advertisements to maximize the likelihood of a customer's buying product?**
   * *Analyzed order hours to recommend optimal ad-spend schedules (e.g., targeting the 11 AM and 7 PM peaks).*
4. **What products are most often sold together?**
   * *Utilized `itertools` and `collections` to find product combinations, providing opportunities for cross-selling and bundling strategies.*
5. **What product sold the most? Why do you think it sold the most?**
   * *Overlaid quantity ordered with average price charts to demonstrate the correlation between lower prices and higher sales volumes.*

---
*This project demonstrates hands-on experience in data wrangling, problem-solving, and communicating data-driven business insights.*
