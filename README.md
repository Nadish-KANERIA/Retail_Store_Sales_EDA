# Retail Store Sales: Exploratory Data Analysis

An exploratory analysis of retail-store transaction data, focused on spending behavior, high-value purchases, and sales patterns over time.

## Data dictionary

| Column | Description |
| --- | --- |
| `Transaction ID` | Unique identifier for each transaction. |
| `Customer ID` | Identifier for the customer who made the purchase. |
| `Category` | Product category associated with the transaction. |
| `Item` | Specific item purchased. |
| `Price Per Unit` | Price of one unit of the item. |
| `Quantity` | Number of units purchased. |
| `Total Spent` | Total value of the transaction. |
| `Payment Method` | Method used to pay for the transaction. |
| `Location` | Whether the purchase was made online or in-store. |
| `Transaction Date` | Date on which the transaction occurred. |
| `Discount Applied` | Indicates whether a discount was applied to the transaction. |

## Project goals

- Clean and prepare the transaction data for analysis.
- Describe the distribution of transaction spending and identify outliers.
- Explore the categories represented in high-spending transactions.
- Track monthly sales totals over the available time period.
- Compare the total quantity purchased online and in-store.

## Tools used

- Python
- Pandas and NumPy
- Matplotlib and Seaborn

## Repository contents

| File | Description |
| --- | --- |
| `Data_Cleaning.ipynb` | Data-cleaning process and preparation steps. |
| `Data_Analysis.ipynb` | Descriptive analysis and visualizations. |
| `retail_store_sales.csv` | Original transaction dataset. |
| `cleaned_data.pkl` | Cleaned dataset used by the analysis notebook. |
| `visualizations/` | PNG versions of the key charts. |

## Key findings

- The average transaction spend is **$129.65**, while the median is **$108.50**, indicating a right-skewed spending distribution.
- Using the 1.5 x IQR rule, transactions above **$403.50** are high-spending outliers; there are **60** such transactions.
- Food appears most often among high-spending transactions (**12 transactions**), followed by Beverages and Butchers (**11 each**).
- Monthly sales fluctuate rather than following a consistent upward trend. January 2025 is incomplete and should not be compared directly with full months.
- Online purchases total **33,731 units**, **1,186** more than in-store purchases (**32,545 units**).

## Visualizations

### Total spending distribution

![Box plot of total spending per transaction](visualizations/total_spent_boxplot.png)

### Categories of high-spending transactions

![Count plot of categories represented in high-spending transactions](visualizations/high_spending_categories.png)

### Monthly sales trend

![Line chart of monthly total sales](visualizations/monthly_sales_trend.png)

### Quantity purchased by location

![Bar chart comparing total quantity purchased online and in-store](visualizations/location_quantity_purchases.png)

## How to run

1. Clone this repository.
2. Install the required Python libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scipy
   ```

3. Open and run `Data_Cleaning.ipynb` before `Data_Analysis.ipynb`.



