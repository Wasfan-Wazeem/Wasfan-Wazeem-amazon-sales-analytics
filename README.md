# 📊 Amazon Sales Strategy Analysis

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Library-Pandas-orange)
![Seaborn](https://img.shields.io/badge/Visualization-Seaborn-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 📖 Project Overview
This project analyzes over **1,400 Amazon product listings** to investigate the relationship between **discount strategies** and **customer satisfaction (ratings)**. 

The primary business question addressed is:
> *"Does offering deeper discounts lead to higher customer ratings, or do users rate products based on quality regardless of price?"*

## 📂 Dataset
- **Source:** [Kaggle - Amazon Sales Dataset](https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset)
- **File:** `amazon.csv`
- **Size:** 1,465 rows, 16 columns.
- **Key Features:** `discounted_price`, `actual_price`, `discount_percentage`, `rating`, `rating_count`, `category`.

## 🛠️ Methodology
The analysis followed a structured data science pipeline:

1.  **Data Cleaning:** - Handled missing values in the `rating` column.
    - Removed currency symbols (`₹`) and percentage signs (`%`) from numerical columns.
    - Converted string objects to `float` and `int` types for analysis.
2.  **Exploratory Data Analysis (EDA):**
    - Visualized the distribution of ratings (Histograms).
    - Analyzed the relationship between Discount % and Rating (Scatter Plots).
3.  **Statistical Analysis:**
    - Calculated **Pearson Correlation Coefficients** to quantify relationships.
    - Grouped data by `category` to find the highest-discounted product types.

## 📊 Key Findings
1.  **Positivity Bias:** The majority of products on Amazon are rated between **3.8 and 4.5**.
2.  **Discount vs. Rating:** There is **no significant linear correlation** (~0.01) between the percentage of discount offered and the customer rating. Deep discounts do not guarantee better reviews.
3.  **Category Insight:** The **Electronics** category has the highest average discount percentage, likely due to rapid depreciation cycles.

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/YOUR-USERNAME/amazon-sales-analytics.git](https://github.com/YOUR-USERNAME/amazon-sales-analytics.git)