# Pre Product Launch Analysis | Adventure Works

End-to-end business intelligence project simulating real-world analytics workflows for a global bicycle manufacturing company.


## Context
Adventure Works, a multinational bicycle and accessories manufacturer, is preparing to launch a new product line next quarter.

The leadership team requested a data-driven analysis of historical sales performance and customer purchasing behavior to guide pricing, marketing strategy, product positioning, and launch priorities.

This project uses Power BI to transform raw sales data into executive insights and launch recommendations.


## Business Objective

Use historical sales data to answer:

- Which product categories perform best?
- What customer preferences can inform the launch?
- Which products show strongest demand trends?
- What pricing signals can guide the new line?
- What should sales and marketing prioritize?


## Dataset Limitations

While the analysis provides meaningful business insights, several dataset constraints should be considered when interpreting the results:

- **Limited time range**: The dataset covers only two months of activity (February–March), which restricts long-term trend analysis and seasonality detection.
- **No customer retention patterns**: All customer IDs are unique, meaning there is no observable repeat purchase behavior. This limits customer lifetime value and loyalty analysis.
- **Order cancellations impact**: A significant portion of orders (13%) were cancelled, which can distort raw revenue and product performance if not properly filtered.
- **Product scope constraints**: The dataset focuses exclusively on bicycle sales, without accessories or complementary product lines, limiting cross-sell or basket expansion analysis.
- **Simplified operational data**: External factors such as marketing spend, inventory constraints, and customer demographics are not included, which limits deeper causal analysis.


## Data Preparation
- Removed duplicates
- Standardized product categories
- Fixed formatting inconsistencies
- Validated date types
- Checked null values
- Created calculated KPIs


## Case Study
### 1. Sales Performance Analysis
In order to understand revenue growth, product mix, and order quality across the two-month period. I focused on key performance indicators such as total revenue, average order value (AOV), product category distribution, and cancellation rates.

![Executive Summary](/assets/1-executive-summary.png)

#### Key Insights
- March outperformed February significantly. Revenue more than doubled, growing from $36500 to $80400. An increase of 120% month-over-month.
- Growth was driven by higher order volume. While AOV incresed sightly, it was not the main driver of growth.
- Mountain Bikes dominate revenue with 43% of fullfilled orders.
- Touring Bikes take second place with 22% of revenue share.
- Third place is constested between Road Bikes and E-Bikes.
- 13% of orders were cancelled during the period, which is a significant factor to consider when evaluating raw revenue and product performance.



### 2. Customer Behaviour Analysis
In this regard the limitations of the dataset are notable. To identify patterns in customer purchasing behavior and order composition, I analyzed average order value by customer, product size preferences and product category performance. Payment method distribution was also available for analysis, but customer segmentation and retention patterns were not possible due to no repeating customer IDs and lack of demographic data.

![Customer Analysis](/assets/2-customer-insights.png)

#### Key Insights
- 100% unique customers. No repeat customers were identified in the available period, suggesting a high-ticket / low-frequency purchase model centered on bicycles.This creates an opportunity to expand recurring revenue through accessories, maintenance plans, and replacement parts.
- Product size distribution is skewed toward M and L. Small-size low sales may indicate either lower demand or unmet market reach, requiring further investigation.
- Regarding payment methods, the data was split 60-40 between credit card and PayPal, with no significant differences in order value or product category preference between the two groups. This suggests that payment method may not be a strong differentiator for customer segments in this dataset. This is why a visualization of payment method distribution was not included in the final report.


### 3. Product Performance Analysis

The objective was to identify top-selling products and evaluate revenue concentration risk. I analyzed revenue contribution by product, and pricing patterns across product categories. 

![Product Performance](/assets/3-product-performance.png)

#### Key Insights
- The analysis revealed a significant concentration of revenue in the top 3 products. This indicates a potential risk if demand shifts away from these key products, but also highlights clear opportunities for targeted marketing and inventory prioritization around these high performers.
- Lower reliance on a single product can be a positive sign of a diversified product portfolio, but it also means that the company may need to invest in marketing and inventory management across multiple products to maintain overall performance.
- From the price vs revenue distribution analysis, it was observed that the highest priced products still generated significant revenue, suggesting that there is a strong demand for premium offerings in the market (no ceiling appears to be met).
- Mid-priced products also showed solid performance, indicating that there is a healthy demand across different price points. This suggests that a tiered pricing strategy could be effective for the new product line, catering to both budget-conscious customers and those seeking premium features.
- Lower-priced products had low revenue contribution, indicating that the majority of customers are willing to invest in higher-priced bicycles. This could inform the product mix and marketing strategy for the launch, emphasizing the value and features of mid to high-end products.


## Conclusion
The analysis of historical sales data for Adventure Works provided valuable insights into sales performance, customer behavior, and product performance. The significant revenue growth in March, driven by higher order volume, highlights the importance of understanding market demand and optimizing inventory management. The concentration of revenue in a few key products suggests both opportunities and risks that should be carefully managed. Additionally, the customer behavior analysis indicates potential areas for growth through expansion to accessories and maintenance plans. Overall, these insights can inform strategic decisions for the upcoming product launch and help guide marketing and sales efforts to maximize success.


## Tools Used
- Power BI Desktop (data modeling and visualization)
- DAX (metrics and KPIs)
- Excel (for data cleaning and preparation)

