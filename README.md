# Sales & Revenue Analysis Dashboard

An 8-page Power BI dashboard built to analyze sales performance, profitability, and growth opportunities for a retail business across categories, regions, and time.

---

## Overview

This project simulates a real client engagement: a retail business with multiple product categories needed a self-service dashboard so their sales and finance teams could understand where revenue and profit were actually coming from, without waiting on custom reports for every question.

The dashboard covers category performance, revenue trends against a custom fiscal calendar, top-performing products, profit margin health, regional performance, discounting impact, and customer segment contribution.

## Business Problem

The client had transactional sales data but no way to answer basic strategic questions:
- Which categories are actually profitable, versus just high-volume?
- Is heavy discounting quietly eating into margins?
- Which regions are underperforming and need attention?
- Are we too dependent on one-time buyers instead of repeat customers?
- Which products deserve to be in the leadership deck as "hero products"?

The brief also specified the client's fiscal year starts in **July**, not January, so all trend and quarter groupings had to follow a custom fiscal calendar rather than Power BI's default date table.

## Dataset

- **7,251** transaction line items across **2,887** orders
- **850** unique customers
- Date range: **July 2023 – July 2026** (3 fiscal years)
- 5 categories (Furniture, Office Supplies, Technology, Apparel, Home & Living), each with multiple sub-categories
- Fields: Order ID, Order/Ship Date, Ship Mode, Customer, Segment, Region, State, Category, Sub-Category, Product Name, Quantity, Unit Price, Discount, Sales, Profit

> Note: this is a synthetically generated dataset built to mirror realistic retail transaction patterns (including deliberately thin margins in specific categories and a genuine discount-to-margin relationship), not scraped from a live production system.

## Key Insights

- **Technology drives the most revenue** (~$10.4M) and does so profitably, at a **26.45% margin**, making it the clear category to double down on.
- **Furniture is a volume trap.** It brings in the second-highest revenue (~$3.6M) but converts almost none of it to profit, just a **3.53% margin**, well below the client's 10% pricing-review threshold. This is exactly the kind of category that looks healthy on a revenue chart and isn't.
- **Apparel is the opposite story**, smallest revenue share (~$469K) but the highest margin of any category at **31.89%**. A strong candidate for expansion even though it currently looks "small" by revenue alone.
- **Discounting has a measurable negative relationship with margin** across the dataset, heavier discount tiers consistently show thinner profit margins, confirming the client's suspicion rather than just a gut feeling.
- Overall performance: **$15.83M** total sales, **$3.26M** total profit, **20.62%** blended margin, across 2,887 orders.

## Dashboard Pages

| Page | What it answers |
|---|---|
| **Overview** | Landing page with navigation to each analysis area | <img width="470" height="270" alt="overview" src="https://github.com/user-attachments/assets/db89e9c8-f7bb-4d60-acb1-cc8b1fb6f52a" />


| **Product & Category Performance** | Which categories/sub-categories drive sales vs. profit | <img width="638" height="367" alt="Product Performance" src="https://github.com/user-attachments/assets/fe4657b7-5fa4-4a1e-9090-9a2048a0450b" />

| **Revenue Trends & Seasonality** | Monthly/quarterly trends on a custom fiscal calendar (FY starts July) |<img width="644" height="362" alt="Revenue Trends" src="https://github.com/user-attachments/assets/5526174d-a93d-4d9b-978e-f99a75267359" />

| **Top Performing Products** | Top 10 products by revenue, units sold, and last-90-days rolling sales | <img width="643" height="366" alt="Top Products" src="https://github.com/user-attachments/assets/e1914cfc-695d-4f5d-b7de-d8de567832f2" />

| **Profit Margin Analysis** | Category margins with a below-10% threshold flag | <img width="646" height="368" alt="Profit Analysis" src="https://github.com/user-attachments/assets/ba51d383-1919-436c-96e3-943fc6e5ad08" />

| **Regional Performance** | Region/state breakdown with top/lowest performer callouts | <img width="643" height="361" alt="Regional Performance" src="https://github.com/user-attachments/assets/6e3a2893-044b-459e-af59-bde9b8aa5b3c" />

| **Discounting Impact** | Relationship between discount depth and profit erosion | <img width="642" height="370" alt="Discount Impact" src="https://github.com/user-attachments/assets/b8a0049a-5e68-45ab-a1d0-7345dbda04e4" />

| **Customer Segments** | Revenue contribution by customer segment | <img width="641" height="373" alt="Customer Segments" src="https://github.com/user-attachments/assets/f8dfb7ca-854f-4efe-84d3-c8b3df384fc5" />




## Tools Used

- **Power BI Desktop** — data modeling, DAX measures, report design
- **DAX** — custom measures (Total Sales, Profit Margin, QoQ Growth %, Sales Last 90 Days, Top N ranking logic)
- **Power Query** — data cleaning and shaping
- Custom **Fiscal Calendar** table (July fiscal-year start) built from scratch, not Power BI's default auto date-time

## What I'd Improve Next

Being upfront about current limitations rather than overselling it:
- Slicers currently only filter by Category; Sub-Category, Region, and Date Range filtering are planned additions
- Customer Segment page could use a stronger callout metric (e.g., % of revenue from one-time vs. repeat buyers) rather than a single chart

---

**Author:** Rubab Rafiq
[LinkedIn](https://linkedin.com/in/rubabrafiq) • [GitHub](https://github.com/Rubab445)
