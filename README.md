# Market-Basket-Analysis-on-Grocery-Data-Report
#### Introduction
Market Basket Analysis (MBA) is an analytical technique used to discover relationships between items frequently purchased together in transactional data.
In this project, Market Basket Analysis was applied to a grocery dataset to identify frequent item combinations in supermarket purchases.

##### Dataset Overview
Dataset Name: Groceries Dataset

Number of Rows: 38,765

Number of Columns: 3 (Member_number, Date, itemDescription)

Unique Items: 167

## Key Steps
`Data Loading:`

The dataset was loaded from a CSV file containing purchase information, including member number, date, and item description.

`Data Cleaning:`

The "Date" column was converted to a datetime format.

Duplicate rows were identified and removed.

The most purchased items were identified.

`Data Preprocessing:`

Data was grouped by member number and date to create transaction baskets.

Data was transformed into a binary matrix (One-Hot Encoding) where each column represents an item and each row represents a transaction.

`Applying the Apriori Algorithm:`

The Apriori algorithm was applied to find frequent itemsets with a minimum support of 0.001.

Association rules were generated based on confidence and lift.

`Visualizing Results:`

Results were visualized using network graphs to display relationships between items.

A recommendation function was created to suggest products based on association rules.

`Key Findings`

Most Purchased Items:

Whole milk: 2,502 purchases

Other vegetables: 1,898 purchases

Rolls/buns: 1,716 purchases

Strongest Association Rules:

(sausage) → (whole milk, yogurt): lift = 2.18

(whole milk, yogurt) → (sausage): lift = 2.18

(whole milk, sausage) → (yogurt): lift = 1.91

Product Recommendations:

For "sausage", the recommended products are "whole milk" and "yogurt".

`Visualizations`

Number of Purchases Over Time:

A line chart was used to visualize the number of purchases over time.

Top 10 Most Purchased Items:

A bar chart was used to visualize the top 10 most purchased items.

Association Rules Network Graph:

A network graph was used to visualize the relationships between items, highlighting the strongest association rules.

`Conclusion`

Market Basket Analysis provides valuable insights into customer behavior and can help improve marketing strategies and product placement in stores. Through this analysis, frequently co-purchased items were identified, enabling the store to offer effective promotions and enhance the customer experience.

`Future Steps`

Refine support and confidence thresholds to obtain more accurate rules.

Apply the analysis to specific time periods to discover seasonal changes in purchasing behavior.

Incorporate additional data, such as pricing, for a more comprehensive analysis.
