# Superstore Sales Analysis – Retail Insights Project

## Overview

This project analyzes sales data from a fictional US retail company “Superstore” that sells furniture, office supplies, and technology products.  
The goal is to understand which regions, products, and customer segments drive revenue and profit, and where the business is losing money or giving too much discount.

This repository is **adapted and extended** from an original project by [WuCandice](https://github.com/WuCandice/Superstore-Sales-Analysis). I used it to learn practical data analysis for a real-world style business case.
  
## Dataset

- Source: Superstore sales dataset (2019–2022), originally from HiCounselor. :contentReference[oaicite:3]{index=3}  
- ~10K rows of transactions  
- Contains:
  - Order details (date, quantity, sales, discount, profit)
  - Customer details (segment, region, city, state)
  - Product details (category, sub-category)

The cleaned dataset is stored in the `dataset` folder in this repository. :contentReference[oaicite:4]{index=4}

## Tools & Technologies

- **Python 3**
- **Pandas** for data analysis
- **SQL** queries (see `sqlQuery.sql`) :contentReference[oaicite:5]{index=5}
- **Jupyter Notebook** (`preprocessing dataset.ipynb`)
- Basic data visualization libraries (matplotlib / seaborn etc.)

## Business Questions

Some of the main questions explored in this project:

- Which states and cities generate the highest revenue?
- Which product categories and sub-categories are most profitable?
- Which products are performing poorly or giving losses?
- Which customer segments bring the most profit?
- How do sales and profit vary across different regions and ship modes? :contentReference[oaicite:6]{index=6}

## Analysis Performed

In the notebook `preprocessing dataset.ipynb`, the following steps are carried out:

1. **Data Loading**
   - Import the CSV dataset into a Pandas DataFrame.
2. **Data Inspection**
   - Check columns, data types, duplicates, and basic statistics.
3. **Data Cleaning**
   - Remove duplicates, fix data types where needed.
4. **Exploratory Data Analysis (EDA)**
   - Region-wise and state-wise sales and profit
   - Category and sub-category performance
   - Customer segment and shipping preferences
5. **Visualizations**
   - Bar charts for sales and profit by region and category
   - Trend charts for performance over time
   - Other plots to highlight top/bottom cities and products. :contentReference[oaicite:7]{index=7}

## Key Insights (Summary)

Some important findings from the analysis (high level):

- The **West and East regions** contribute the highest revenue, with states like California, Washington, and New York performing very well.
- **Technology** is the best-performing category in both sales and profit, while some furniture sub-categories generate sales but very low or negative profit.
- A few specific products and sub-categories show **high discounts and negative profit**, indicating pricing or cost issues.
- The **Consumer** segment is the largest customer segment and Standard Class is the most preferred shipping mode. :contentReference[oaicite:8]{index=8}

*(These points are my own summary after going through the analysis.)*

## My Learning & Contribution

What I personally learned and/or modified in this project:

- Understood how to structure a business problem and convert it into data questions.
- Practiced using Pandas for cleaning, grouping, and aggregating sales data.
- Explored how to read insights from charts and pivot-style tables.
- (Optional – update this after you make a change)  
  - Added an extra analysis for:
    - Top 5 customers by profit  
    - Monthly sales trend  
    - Extra visualizations

## How to Run This Project

1. Clone or download this repository.
2. Open the Jupyter Notebook:

   ```bash
   jupyter notebook "preprocessing dataset.ipynb"
