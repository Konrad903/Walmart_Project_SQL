# Walmart Sales Data Analysis

## About
This project aims to explore the Walmart Sales data to understand top-performing branches and products, sales trends of different products, and customer behavior. The goal is to study how sales strategies can be improved and optimized. The dataset was obtained from the Kaggle Walmart Sales Forecasting Competition.

## Purposes Of The Project
The major aim of this project is to gain insight into the sales data of Walmart to understand the different factors that affect sales across different branches.

## About Data
The dataset contains sales transactions from three different branches of Walmart, located in Mandalay, Yangon, and Naypyitaw. The data contains 17 columns and 1,000 rows.

## Analysis List
1. **Product Analysis**: Conduct analysis on the data to understand the different product lines, the product lines performing best, and the product lines that need improvement.
2. **Sales Analysis**: This analysis aims to answer questions regarding product sales trends to help measure the effectiveness of sales strategies and identify necessary modifications.
3. **Customer Analysis**: This analysis aims to uncover different customer segments, purchase trends, and the profitability of each segment.

## Approach Used
1. **Data Wrangling**: 
   - Build a database.
   - Create tables and insert data.
   - Inspect data for NULL or missing values (fields were set with `NOT NULL` during creation to filter out missing values).
2. **Feature Engineering**: Generate new columns from existing ones:
   - `time_of_day`: Insights into sales during Morning, Afternoon, and Evening.
   - `day_name`: Extracted days of the week when transactions took place (Mon-Fri).
   - `month_name`: Extracted months of the year (Jan-Mar).
3. **Exploratory Data Analysis (EDA)**: Conducted to answer the business questions and project aims.

## Business Questions To Answer

### Generic Questions
* How many unique cities does the data have?
* In which city is each branch?

### Product
* How many unique product lines does the data have?
* What is the most common payment method?
* What is the most selling product line?
* What is the total revenue by month?
* What month had the largest COGS?
* What product line had the largest revenue?
* What is the city with the largest revenue?
* What product line had the largest VAT?
* Fetch each product line and add a column showing "Good" or "Bad" (Good if greater than average sales).
* Which branch sold more products than the average product sold?
* What is the most common product line by gender?
* What is the average rating of each product line?

### Sales
* Number of sales made in each time of the day per weekday.
* Which of the customer types brings the most revenue?
* Which city has the largest tax percent / VAT (Value Added Tax)?
* Which customer type pays the most in VAT?

### Customer
* How many unique customer types does the data have?
* How many unique payment methods does the data have?
* What is the most common customer type?
* Which customer type buys the most?
* What is the gender of most of the customers?
* What is the gender distribution per branch?
* Which time of the day do customers give the most ratings?
* Which time of the day do customers give the most ratings per branch?
* Which day of the week has the best average ratings?
* Which day of the week has the best average ratings per branch?

## Revenue And Profit Calculations
* $COGS = \text{unitPrice} \times \text{quantity}$
* $VAT = 5\% \times COGS$
* $\text{total (gross\_sales)} = VAT + COGS$
* $\text{grossProfit (grossIncome)} = \text{total (gross\_sales)} - COGS$
* $\text{Gross Margin} = \frac{\text{gross income}}{\text{total revenue}}$
