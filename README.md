# 📈 Superstore Sales Analysis

---

## ℹ️ Project Description

This project provides a comprehensive analysis of sales data from a fictional Superstore. The main goal is to uncover key trends, patterns, and insights that can inform business decisions and optimize strategies in sales, marketing, and supply chain management.

---

## 📊 Data

The `train.csv` dataset contains information about various orders, including customer details, product specifications, shipping methods, and sales amounts.

**Important Note:** This specific dataset does not include columns for `Profit` or `Quantity`, so the analysis has focused exclusively on `Sales` and other available features.

---

## 🎯 Analysis Objectives

The primary objectives of this analysis are:

* To understand sales trends over time (yearly, monthly).
* To identify top-performing product categories and sub-categories based on sales.
* To recognize the most profitable geographical regions in terms of sales.
* To determine the most significant shipping modes.
* To identify customer segments that contribute most to sales.
* To recognize top customers and top products.

---

## 🛠️ Methodology

The analysis was implemented using the Python programming language and the following libraries: Pandas for data manipulation, Matplotlib and Seaborn for visualization.

### 🧹 Data Cleaning

1.  **Missing Values:** 11 missing values were identified in the `Postal Code` column. Given that all transactions are within the United States and the number of missing values is negligible (approximately 0.11% of the total), these rows were removed.
2.  **Duplicate Rows:** A check for duplicate rows was performed, and no entirely duplicate entries were found.

### ⚙️ Preprocessing & Feature Engineering

1.  **Data Type Conversion:** The `Order Date` and `Ship Date` columns were converted to datetime format for temporal calculations. The `Postal Code` column converted to an integer.
2.  **New Feature Creation:**
    * `Order_Year`: The year of the order.
    * `Order_Month`: The month of the order.
    * `Order_Day`: The day of the order.
    * `Shipping_Duration_Days`: The shipping duration in days (Ship Date - Order Date).

### 📊 Exploratory Data Analysis (EDA) & Visualization

A series of visualizations were created to reveal trends and patterns in the sales data. Charts include:

* Total Sales by Year 
* Average Monthly Sales 
* Average Monthly Sales Per Year 
* Total Sales by Product Category 
* Total Sales by Product Sub-Category 
* Total Sales by Ship Mode 
* Total Sales by Region 
* Total Sales by Customer Segment 
* Top 10 Customers by Total Sales 


---

## 💡 Key Findings & Business Insights

The analysis of the data revealed the following significant findings:

* **Sales Trend:** Total sales show a clear upward trend over the years, especially after 2016. Notable growth was observed in 2017 and 2018, where sales increased significantly, reaching their highest point in 2018.

* **Seasonality:** Sales exhibit clear seasonality. On average, sales are usually higher in March, January, and October, while they are lower in February, April, June, and July. The monthly sales pattern shows some variations across the years, with specific months exhibiting unusually high or low sales in different years (e.g., December 2018 was unusually low compared to previous years, while January and August 2018 were very strong).

* **Product Categories:** The Technology category dominates sales ($825,856.11), followed by Furniture ($723,538.48) and Office Supplies ($703,212.82). The pie chart shows that 

**Technology** accounts for approximately 36.7% of total sales, with Furniture and Office Supplies following with 32.1% and 31.2% respectively. This indicates a relatively balanced sales distribution among the three main categories.

* **Product Sub-Categories:** Among sub-categories, Phones ($326,487.70) and Chairs ($322,107.53) are the top performers in sales, indicating strong demand for these specific products. Other significant sub-categories include Storage ($217,779.10) and Tables ($202,810.63). Specifically, Phones account for 14.5% and Chairs for 14.3% of total sales.

* **Shipping Modes:** The Standard Class shipping mode is the most frequently used and contributes the most to sales ($1,332,617), followed by Second Class ($449,199) and First Class ($345,572).

* **Geographical Regions:** The West region is the strongest in sales ($710,219.68), followed by East ($660,589.36) and Central ($492,646.91). The South region has the lowest sales ($389,151.46).

* **Customer Segments:** The Consumer segment contributes the largest share of sales ($1,146,708), indicating that marketing efforts should further focus on this audience. Corporate ($682,211.8) and Home Office ($423,687.4) segments follow.

* **Top Customers & Products:**
    * Customers such as Sean Miller ($25,043.05), Tamara Chand ($19,052.22), and Raymond Buch ($15,117.34) are the top contributors to total sales.
    * Products like Canon imageCLASS 2200 Advanced Copier and Fellowes PB500 Electric Punch Plastic Comb Binding Machine are major sales drivers, demonstrating very high individual sales.

---

## 📈 Conclusions & Recommendations

Based on the above findings, the following recommendations can be made:

1.  **Leverage Seasonality:** The Superstore can capitalize on high-sales months with targeted promotional activities and adequate product availability. Conversely, during low-sales months, special offers or campaigns can be launched to stimulate demand. The analysis of monthly sales by year indicates that seasonality may vary slightly, requiring flexible planning.

2.  **Focus on Top Categories/Sub-Categories:** Continue to invest in and promote products within the top categories such as Technology, Furniture, Office Supplies, and sub-categories like Phones and Chairs. Explore opportunities for expanding product offerings in these successful categories.

3.  **Targeted Marketing:** Strengthen marketing efforts towards the Consumer customer segment and in the West and East geographical regions, given their high sales contribution. Simultaneously, explore ways to boost sales in lower-performing regions or segments.

4.  **Customer Management:** Implement loyalty programs or special offers for top customers to maintain their loyalty and encourage repeat purchases.

5.  **Shipping Optimization:** Given the dominance of the Standard Class shipping mode, optimize processes for this method to ensure efficiency and customer satisfaction.

---

## 💻 Tools & Libraries

* **Python** 
* **Jupyter Notebook**
* **Pandas** 
* **NumPy** 
* **Matplotlib**
* **Seaborn** 

---

## 🚀 How to Run the Project

Follow the steps below to reproduce the analysis:

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/YourUsername/Superstore-Sales-Analysis.git](https://github.com/YourUsername/Superstore-Sales-Analysis.git)
    cd Superstore-Sales-Analysis
    ```
2.  **Create a Virtual Environment (recommended):**
    ```bash
    python -m venv venv
    ```
3.  **Activate the Virtual Environment:**
    * **Windows:** `.\venv\Scripts\activate`
    * **macOS/Linux:** `source venv/bin/activate`
4.  **Install Required Libraries:**
    ```bash
    pip install -r requirements.txt
    ```
5.  **Run the Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
    Open the `superstore_sales_analysis.ipynb` file and execute the cells in order.

---
