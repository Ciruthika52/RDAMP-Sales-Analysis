# RDAMP-Sales-Analysis

## Project Description
ACE Super Store Sales Analaysis was completed as part of Realcare Tech Mark Limited Data Analyst Mendorship Program.  
This project provides experience working with real-world data, helping to gain hands-on skills and develop attractive dashboards. 

## Objectives Of this Project
1. **Identify sales trends and revenue distribution** across regions and customer segments to highlight growth opportunities and regional gaps.
2. **Understand customer purchasing behavior** (e.g., online vs in-store sales) to tailor marketing and sales strategies.
3. **Spot top-performing and underperforming products** to focus efforts on high-impact items and reconsider low performers.
4. **Determine the most and least profitable product categories**

## Dataset And Tools Used
**Dataset:**
1. Ace Super Store Sales Dataset: Order ID	Order Date	Order Mode	Customer ID	City	Postal Code	Country	Region	Product ID	Product Name	Category	Sub-Category	Sales	Cost Price	Quantity	Discount
2. Store Locations Dataset: City	Postal Code	Country	Region

**Tool:** Power BI

## Data Pre Processing
1. Performed Extract, Transform, and Load (ETL) using Power BI Power Query.
2. Created new groups in Power Query and duplicated the original dataset, moving the duplicate to the new group. This way, the original dataset remains as raw data for future clarifications or double-checking.
3. Removed duplicates from Location dataset.
4. Removed Region,country and city from sales dataset. Kept postcode to connect sales and location dataset.
5. The Product table was generated from sales table and product name, category,sub-category were removed from sales table.
6. In product table segment column was generated based on category column for further analysis.
7. Removed negative values from sales and cost column : Negative Sales and Cost Price typically represent returns or refunds, which should correspond with negative Quantity as products are returned to inventory. Having a positive Quantity contradicts this logic, indicating a likely data entry or system error.
8. Date table was generated to have analysis based on trend.
9. Total Sales,Total Cost,Total Revenue,Profit columns were generated for analysis purpose.
10. Checked and corrected data types across all datasets to resolve any mismatches.

## Relationship between datasets
1. Sales ↔ Location: Many-to-One via [Postal Code]
2. Sales ↔ Product: Many-to-One via [Product ID]
3. Sales ↔ Date: Many-to-One via [Order Date] = [Date]

## Data Visualisation
1. Cards: Total Sales, Total Cost, Total Revenue, Profit,Units Sold,Total Orders
2. Clustered Bar Chart: Best Selling Products By Revenue , Under performing Products By Revenue, Profit By Category, Total Cost,Sales,Revenue By Region
3. Donut Chart: Total Sales By Order Mode, Customer Behaviour By Order Mode
4. Line Chart: Total Revenue By Order Mode
5. Treemap: Sales By Category
6. Matrix: Sales Summary By Region and Segment
   
## Key Insights
1. **Overall Performance**
     * Total Sales stand at £3.17M, with a Profit of £1.64M, indicating a healthy margin and efficient cost management (£1.04M total cost).
     * 115K units sold across 10.95K orders reflects strong customer engagement and transaction volume.
2. **Product Performance**
     * The best-selling products by revenue include Portable Solar Generator, Portable Refrigerator Freezer, and Electric Bike, suggesting high demand in outdoor and tech-related segments.
     * Underperforming products such as Instant Mashed Potatoes and Paprika indicate potential issues with these SKUs, either due to low demand, pricing, or competition.
 3. **Sales Distribution by Order Mode**
     * The revenue and customer counts are relatively balanced between Online and In-Store channels.
     * Both order modes contribute significantly, with slight dominance by the Online channel in revenue.
 4. **Trends Over Time**
     * Sales revenue shows monthly fluctuations with peaks, indicating possible seasonality or promotional effects.
 5. **Category Performance**
     * The largest sales contribution comes from Outdoor, Kitchen, and Clothing categories.
     * A broad range of smaller categories contributes to total sales, but with less impact individually.
     
  ## Recommendations
  1. **Focus on High-Performing Products and Categories**
      * Allocate marketing and inventory resources to best-selling products such as Portable Solar Generator and Electric Bike to maximize revenue growth.
      * Explore cross-selling opportunities within strong categories (Outdoor, Kitchen, Clothing).
  2. **Address Underperforming Products**
      * Review pricing, placement, and promotion strategies for products like Instant Mashed Potatoes and Paprika.
  3. **Enhance Online and In-Store Integration**
      * Since both sales channels contribute significantly, develop strategies to provide a seamless customer experience across Online and In-Store.
  4. **Leverage Seasonality Trends**
      * Analyze peak sales months further to identify drivers (holidays, campaigns) and plan future promotions accordingly.
    
   ## Screenshots

   ![Screenshot](/Ciruthika_Nithusyanthan_Visualisation01.png)

    ![Screenshot](/Ciruthika_Nithusyanthan_Visualisation02.png)

     ![Screenshot](/Ciruthika_Nithusyanthan_Datarelationship.png)

   
              
  
     
      



