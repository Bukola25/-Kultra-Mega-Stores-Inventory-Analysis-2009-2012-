# -Kultra-Mega-Stores-Inventory-Analysis-2009-2012

##  Overview

This project analyzes historical sales and shipping data for Kultra Mega Stores (KMS), a Nigerian-based office and furniture supplier. The focus is on identifying top-performing product categories, customer segments, shipping strategies, and opportunities to boost profitability using SQL-based exploratory analysis.

---

##  Tools Used
- SQL Server (T-SQL)
- Microsoft Excel (for final dashboards)

---

##  Dataset Details

- Orders data from: 2009 to 2012
- Key fields: `Product_Category`, `Sales`, `Region`, `Customer_Segment`, `Ship_Mode`, `Order_Quantity`, `Profit`, etc.

---

##  SQL Analysis Breakdown

### Scenario I – Sales & Operations

1. **Highest Sales Product Category**  
   → Summed `Sales` per category and ordered descending.

2. **Top 3 and Bottom 3 Regions by Sales**  
   → Grouped `Region` by `Sales` and sorted both ways.

3. **Sales of Appliances in Ontario**  
   → Filtered `Product_Sub_Category = 'Appliances'` and `Region = 'Ontario'`.

4. **Bottom 10 Customers by Revenue**  
   → Summed `Sales × Order Quantity` and advised management to upsell or offer loyalty programs.

5. **Highest Shipping Cost by Method**  
   → Summed `Shipping_Cost` by `Ship_Mode`.

---

###  Scenario II – Customer Insight & Logistics

6. **Top 10 Most Valuable Customers & Their Purchases**  
   → Revenue = `Sales × Order Quantity`, grouped by customer and product category.

7. **Top Small Business Customer by Sales**  
   → Filtered `Customer_Segment = 'Small Business'`, summed `Sales`.

8. **Top Corporate Customer by Orders (2009–2012)**  
   → Counted `Order_ID` and filtered by segment and year.

9. **Most Profitable Consumer Customer**  
   → Summed `Profit` for `Customer_Segment = 'Consumer'`.

10. **Customers Who Returned Items**  
   → (Note: Query not implemented – recommend joining with a return dataset if available).

11. **Shipping Cost vs Order Priority**  
   → Analyzed `Shipping Cost` by `Order_Priority` and `Ship_Mode` to evaluate misuse of Express Air for low-priority orders.

---

##  Recommendations

- Expand stock in top-performing categories (e.g., Chairs, Office Desks).
- Review shipping policies: Express Air is overused for non-urgent orders.
- Focus upsell strategies on Small Business and Corporate customers with high lifetime value.
- Offer incentives to low-performing customers (bottom 10) to increase loyalty.
- Ensure shipping method matches order urgency to reduce costs.





