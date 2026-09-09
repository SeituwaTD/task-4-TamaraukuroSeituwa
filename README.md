Sales Performance & Customer Insights Dashboard — Power BI

📊 Project Overview

This project transforms a cleaned e-commerce sales dataset into an interactive Power BI dashboard designed to uncover sales performance, product trends, customer behaviour, order patterns, and revenue drivers.

The project was completed as part of my Decode Labs Data Analytics internship, following earlier stages of data cleaning, exploration, and querying with Python/SQL.

The final dashboard brings the analysis together in three main areas:

Overview — executive-level KPIs and high-level sales trends.

Product & Customers — product performance, customer spending, referral sources, and the relationship between basket activity and revenue.

Time, Orders & Behaviour — time-based performance, order status, payment methods, and coupon performance.

🎯 Project Objectives

The main objectives were to:

Measure overall revenue and sales performance.

Identify the best- and worst-performing products.

Analyse revenue trends across 2023–2025.

Understand customer purchasing behaviour.

Identify the strongest referral, payment, and coupon sources.

Analyse order-status performance.

Examine daily and monthly revenue patterns.

Identify high-value customers.

Build an interactive dashboard that communicates business insights clearly.

Translate the analysis into practical recommendations for decision-making.

🛠️ Tools & Technologies

Tool

Purpose

Python

Data cleaning, preprocessing and exploratory analysis

Pandas

Data manipulation and transformation

SQL / MySQL

Data querying and analytical questions

Power BI

Interactive dashboard development and visualization

DAX

Measures and KPI calculations

Power Query

Data transformation inside Power BI

GitHub

Project documentation and portfolio presentation

Key Power BI/DAX Measures

Examples of measures used in the dashboard include:

Total Revenue = SUM(Sheet1[totalprice])

Total Quantity = SUM(Sheet1[quantity])

Total Orders = DISTINCTCOUNT(Sheet1[orderid])

Total Customers = DISTINCTCOUNT(Sheet1[customerid])

Average Order Value =
DIVIDE([Total Revenue], [Total Orders])

The dashboard also uses calculated date attributes such as Year, Month Name, Month Number, and Day Name to support time-based analysis.

📌 Dataset

The sales dataset contains transaction-level information including:

Order ID

Date

Customer ID

Product

Quantity

Unit Price

Shipping Address

Payment Method

Order Status

Tracking Number

Items in Cart

Coupon Code

Referral Source

Total Price

📈 Dashboard KPIs

The dashboard reports the following headline figures:

KPI

Result

Total Revenue

£1.26M

Total Orders

1,200

Total Quantity Sold

3,535

Total Customers

1,189

Average Order Value

£1.05K

A notable observation is that the number of unique customers is very close to the number of orders. If the customer IDs are reliable, this suggests that repeat purchasing may be relatively low, creating an opportunity to investigate customer retention and repeat-order behaviour.

🔎 Key Business Insights

1. Overall Revenue Performance

The business generated approximately £1.26 million in total revenue from 1,200 orders, with an average order value of approximately £1.05K.

However, the dashboard indicates an overall decline in annual revenue as the years progress from 2023 to 2025.

Business implication

The decline should be investigated rather than viewed only as a reporting trend. Possible areas to investigate include:

Changes in product demand.

Changes in order volume.

Changes in average order value.

Product availability.

Customer retention.

Pricing.

Promotions and coupon effectiveness.

Referral-source performance.

📅 2. Monthly Revenue Trends

The highest-revenue month differs by year:

2023: June

2024: July

2025: June

This suggests that the business experiences a recurring period of stronger performance around June/July.

However, the repeated peak does not by itself prove that the business operates on a July–June fiscal year. The pattern should be validated against the company's actual financial calendar before adopting a fiscal-year interpretation.

🪑 3. Product Performance

Chair was the strongest overall product in terms of quantity sold and revenue/profit contribution in the dashboard.

Phone was the weakest overall product in terms of quantity sold and profit contribution.

This creates a clear contrast between a high-performing product category and a product that may require further investigation.

Possible actions

Investigate why Chair performs strongly.

Identify the characteristics of high-performing Chair purchases.

Review Phone pricing, demand, promotion, and customer interest.

Consider whether low-performing products should be repositioned, discounted, bundled, or reduced.

📦 4. Product Demand Changed Across Years

Product leadership changed from year to year:

Year

Highest Quantity/Product

Lowest Quantity/Product

2023

Printer

Desk

2024

Chair

Desk

2025

Desk

Chair

The movement is particularly interesting in 2025 because Desk became the strongest product while Chair became the weakest by quantity.

This does not automatically prove an ongoing preference for desks over chairs. Instead, it indicates a change in product demand that deserves further investigation.

Possible explanations include:

Changing customer needs.

Pricing changes.

Product availability.

Promotions.

Seasonal demand.

Changes in customer segments.

🚚 5. Order Status Requires Attention

The dashboard shows that Cancelled and Returned orders form a significant portion of order statuses.

This is potentially concerning because cancellations and returns can reduce realized revenue and increase operational costs.

Product-specific findings

Chair recorded the highest number of cancelled orders.

Tablet recorded the highest number of returned orders.

Recommended investigation

Management should investigate:

Reasons for cancellations.

Reasons for returns.

Product quality.

Product descriptions and customer expectations.

Delivery performance.

Pricing.

Stock availability.

Whether certain products have disproportionately high cancellation/return rates.

Importantly, high counts should be compared with total orders for each product. A product with many orders will naturally have more cancellations/returns, so a cancellation or return rate would provide a stronger performance measure than raw counts alone.

💰 6. Laptop Has the Highest Average Order Value

Laptop recorded the highest average order value among the products analysed.

This suggests that Laptop purchases tend to generate higher-value transactions.

Business opportunity

The business could investigate whether Laptop customers are suitable targets for:

Accessories.

Bundles.

Extended product offerings.

Cross-selling.

Premium upgrades.

👤 7. Highest-Value Customer

Customer C38840 generated the highest recorded revenue, spending approximately:

£5,723.23

This customer represents an example of a high-value customer segment that could be analysed further.

Useful follow-up questions include:

What products did the customer purchase?

How many orders did the customer make?

Which payment method was used?

Which referral source brought the customer?

Did the customer use coupons?

What was the customer's average order value?

📱 8. Referral Source Performance

Instagram generated the highest revenue among the referral sources analysed.

Referral generated the lowest revenue.

This suggests that Instagram may be an important acquisition channel for the business.

Recommendation

Marketing teams should investigate:

Instagram campaign performance.

Conversion rates.

Customer acquisition cost.

Product categories purchased by Instagram customers.

Average order value by referral source.

Revenue alone should not be used to determine marketing ROI because a high-revenue channel may also have high acquisition costs.

💳 9. Payment Method Performance

Credit Card generated the highest revenue.

Debit Card generated the lowest revenue.

This indicates that credit-card customers contributed more revenue within this dataset.

However, this should not automatically be interpreted as credit cards being more effective. The difference may be influenced by:

Number of transactions.

Customer demographics.

Order value.

Product mix.

Customer preference.

A useful next step would be to compare revenue, order count, and average order value by payment method.

🎟️ 10. Coupon Code Performance

FREESHIP generated the highest revenue among the coupon codes analysed.

SAVE10 generated the lowest revenue.

This suggests that free-shipping incentives may have been associated with higher sales value in this dataset.

However, revenue alone does not establish that FREESHIP was the most profitable promotion.

A stronger promotional analysis would compare:

Revenue.

Number of orders.

Average order value.

Discount cost.

Gross profit.

Profit margin.

📆 11. Revenue by Day of the Week

Sunday generated the highest revenue.

Wednesday generated the lowest revenue, followed by Saturday.

This is an interesting finding because the highest revenue day was not a conventional weekday.

The result suggests that customer purchasing behaviour may vary significantly throughout the week.

Recommendation

Consider analysing:

Order volume by day.

Average order value by day.

Product preference by day.

Marketing campaigns by day.

Whether Sunday performance is driven by a small number of unusually large orders.

📊 12. Quantity and Revenue Relationship

The dashboard includes a scatter plot examining the relationship between basket activity and revenue.

Important dashboard validation: in the current PBIX file, the scatter visual is configured with itemsincart on the X-axis and Total Revenue on the Y-axis, with product as the series. Therefore, the safer interpretation is:

There is a positive relationship between the number of items in the cart and revenue in the visual.

If the intended analysis was specifically Quantity vs Revenue, the scatter plot should be reconfigured with Total Quantity on the X-axis before making that claim.

A positive relationship would be expected because larger baskets can naturally produce higher transaction values, but correlation does not prove that increasing quantity causes revenue to increase.

🏆 13. Product Revenue Ranking

The dashboard ranks products by total revenue.

Chair appears as the strongest overall product, while Phone appears as the weakest among the products analysed.

This ranking provides management with a quick view of where revenue is concentrated and which products may need further investigation.

🧩 Dashboard Structure

Page 1 — Overview

The Overview page focuses on executive-level performance:

Total Revenue

Total Orders

Total Quantity

Total Customers

Average Order Value

Revenue by Product

Revenue trend by month/year

Order-status distribution

Page 2 — Product & Customers

This page focuses on:

Product performance

Customer revenue ranking

Referral-source revenue

Product revenue and quantity

Customer/product relationships

High-value customers

Page 3 — Time, Orders & Behaviour

This page focuses on:

Day-of-week revenue

Payment-method revenue

Payment-method order distribution

Coupon performance

Average Order Value

Basket activity vs revenue

Time-based and order behaviour

🎨 Visualization Techniques

The dashboard uses several Power BI visual types to communicate different analytical questions:

Cards — KPI reporting.

Bar charts — product and category ranking.

Column charts — comparisons between categorical groups.

Line charts — monthly revenue trends across years.

Donut charts — order/payment-status composition.

Scatter plots — relationship between numerical variables.

Funnel chart — customer/revenue ranking exploration.

Tables — detailed product and coupon performance.

Slicers — interactive filtering by dimensions such as year and other attributes.

The dashboard also uses sorting to rank categories in descending order where appropriate.

🧮 Data & Date Transformation

During the Power BI transformation stage, date-related fields were prepared for time-based analysis.

Key fields include:

Date

Year

Month Name

Month Number

Day Name

A major issue encountered was that Month Name is a text field, while the actual Date field must remain a date data type.

The Month Name field was therefore treated as text and sorted using Month Number to ensure chronological ordering:

January → February → March → ... → December

This prevents Power BI from incorrectly sorting months alphabetically.

🚧 Challenges / Pain Points & Solutions

1. Refreshing DAX Knowledge

Challenge

After working mainly with Python and SQL, remembering DAX syntax and understanding how measures work in Power BI was initially challenging.

Solution

I refreshed core DAX concepts and applied measures directly to the dashboard, including:

SUM

AVERAGE

DISTINCTCOUNT

CALCULATE

DIVIDE

SAMEPERIODLASTYEAR

This helped me move from simply creating visuals to building reusable analytical measures.

2. Creating Previous-Year Revenue

Challenge

Understanding how to calculate revenue for the previous year for comparison.

Solution

A previous-year measure can be created using:

Previous Year Revenue =
CALCULATE(
    [Total Revenue],
    SAMEPERIODLASTYEAR('Date'[Date])
)

This supports year-over-year analysis when a proper Date table is available.

3. Understanding Previous Period

Challenge

The meaning of "previous period" was initially unclear because it depends on the selected time context.

Solution

I learned that:

For yearly analysis, previous period can mean previous year.

For monthly analysis, previous period can mean previous month.

The correct interpretation depends on the business question and filter context.

4. Month Name Being Treated as a Date

Challenge

Power BI produced an error similar to:

Cannot convert value 'March' of type Text to type Date.

Solution

I identified that March is a month name, not a date.

The solution was to keep Month Name as Text and create/use a numeric Month Number field for sorting.

Example:

Month Number = MONTH(Sheet1[date])

Month Name = FORMAT(Sheet1[date], "MMMM")

Then:

Month Name → Sort by column → Month Number

5. Month Ordering on the Line Chart

Challenge

The monthly line chart did not initially behave as expected and appeared to start from July.

Solution

I learned that the visual's starting month does not automatically prove that the business uses a July–June financial year.

I therefore separated two concepts:

Calendar year: January–December.

Fiscal year: depends on the organization's reporting calendar.

The correct approach is to verify the business reporting calendar before creating a fiscal-year model.

6. Sorting Bar Charts

Challenge

Ranking products and categories correctly in Power BI required understanding how visual-level sorting works.

Solution

For a bar chart:

Three dots (...) → Sort by → Measure → Descending

For example:

Product → Total Revenue → Descending

This ensures the highest-revenue product appears at the top of the ranking.

7. Creating Top 10 Products

Challenge

The dashboard required identifying the highest-performing products rather than displaying every product equally.

Solution

Power BI's Top N filter was used:

Filters → Product → Top N → Top 10 → By value → Total Revenue → Apply filter

This creates a focused Top 10 product analysis.

8. Combining Multiple Measures in a Visual

Challenge

Understanding how to display multiple measures such as Revenue, Quantity Sold, and Orders in a single visual was initially confusing.

Solution

I learned the difference between:

Clustered column/bar charts for side-by-side measures.

Line and clustered column charts when one measure is better represented as a line.

Secondary axes when measures have substantially different scales.

This helped me avoid misleading or unreadable comparisons.

💡 Recommendations

Based on the dashboard findings, the following areas deserve further investigation:

1. Investigate revenue decline

Break annual revenue into:

Revenue = Number of Orders × Average Order Value

This can help determine whether the decline is caused primarily by fewer orders, lower order values, or both.

2. Reduce cancellations and returns

Analyse cancellation/return rates, not only counts.

For example:

Cancellation Rate =
Cancelled Orders / Total Orders

and:

Return Rate =
Returned Orders / Total Orders

Calculate these by product to identify products with unusually high rates.

3. Improve customer retention

With 1,189 customers and 1,200 orders, repeat-purchase behaviour should be investigated.

Useful metrics include:

Repeat customer rate.

Orders per customer.

Customer lifetime value.

First-order vs repeat-order revenue.

4. Investigate product demand changes

The shift from Printer → Chair → Desk across the years suggests changing demand.

Further analysis should examine whether this is caused by:

Pricing.

Promotions.

Product availability.

Customer segments.

Seasonality.

5. Evaluate marketing channels using profitability

Instagram generated the highest revenue, but revenue alone does not measure marketing efficiency.

Compare:

Revenue + Orders + AOV + Acquisition Cost + Profit

by referral source.

6. Evaluate coupon profitability

FREESHIP generated the most revenue, but promotional success should ultimately be measured using profit/margin rather than revenue alone.

📚 Key Learning Outcomes

This project strengthened my ability to:

Transform raw data into business-ready analytical datasets.

Build Power BI dashboards from cleaned data.

Create and use DAX measures.

Work with date dimensions and chronological sorting.

Design KPI cards.

Build interactive visualizations.

Apply Top N filters.

Rank products and customers.

Analyse trends across multiple years.

Interpret categorical and numerical relationships.

Translate visual findings into business recommendations.

Validate insights instead of assuming that a visual automatically proves causation.

Document an end-to-end analytics project for portfolio presentation.

🚀 Future Improvements

Potential future versions of this dashboard could include:

Profit margin analysis.

Customer retention dashboard.

Customer segmentation.

RFM analysis.

Cancellation and return rates.

Product-level profitability.

Year-over-year growth measures.

Monthly and quarterly forecasts.

Marketing ROI analysis.

Customer lifetime value.

Drill-through pages for individual customers/products.

A dedicated calendar/date table for more advanced time intelligence.

📁 Project Workflow

Raw Sales Dataset
       ↓
Data Cleaning with Python/Pandas
       ↓
Exploratory Data Analysis
       ↓
SQL Analysis & Business Questions
       ↓
Power BI Data Transformation
       ↓
DAX Measures
       ↓
Interactive Visualizations
       ↓
Dashboard
       ↓
Business Insights & Recommendations

🏁 Conclusion

This project demonstrates how raw sales data can be transformed into an interactive business intelligence solution.

The analysis identified several important patterns, including £1.26M in revenue, product performance differences, changing yearly product demand, revenue decline over time, high-value customers, significant cancellation/return activity, and differences in revenue across referral sources, payment methods, coupon codes, and days of the week.

More importantly, the project reinforced an important principle of data analytics:

A dashboard should not only show what happened; it should help explain why it happened and what should be investigated next.

The next stage would be to move from descriptive analysis toward diagnostic and predictive analytics by investigating the drivers of revenue decline, customer retention, product returns, and profitability.

👨‍💻 Author

Seituwa Tamaraukuro Dominic

Medical Laboratory Scientist | Data Analyst | Data Science Enthusiast

Skills demonstrated

Python Pandas SQL MySQL Power BI DAX Data Cleaning EDA Data Visualization Business Intelligence

⭐ Project Status

Completed — Power BI Visualization & Business Insights

This project forms part of my continued transition from Medical Laboratory Science into Data Analytics and Data Science, combining domain experience with analytical and business intelligence skills.
