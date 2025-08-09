# Zepto SQL Data Analysis

## Project Overview
This project performs **data cleaning, exploration, and analysis** on a dataset from Zepto (an Indian online grocery platform) using **PostgreSQL**.  
It simulates real-world retail analytics to extract insights about product pricing, discounts, stock status, and revenue.

---

## Tech Stack
- **Database:** PostgreSQL 17
- **Language:** SQL (DDL, DML, Aggregations, CASE statements)
- **Tools:** psql CLI

---

##Dataset Description
The dataset contains product-level details such as:
- **Category** – Product category (e.g., Fruits & Vegetables)
- **Name** – Product name
- **MRP** – Maximum Retail Price
- **Discount Percent** – % discount on MRP
- **Available Quantity** – Units in stock
- **Discounted Selling Price** – Price after discount
- **Weight in gms** – Product weight
- **Out of Stock** – Boolean indicating stock status
- **Quantity** – Package quantity
- **SKU ID** – Unique identifier (auto-generated)

---

## 📊 Steps Performed
### 1. **Data Import**
- Created a PostgreSQL table schema.
- Imported CSV data using `\copy`.

### 2. **Data Exploration**
- Counted total rows and sampled data.
- Checked for NULL values and duplicate product names.
- Reviewed distinct categories and stock status distribution.

### 3. **Data Cleaning**
- Removed invalid rows with MRP = 0.
- Converted prices from paise to rupees.
- Ensured column data types matched the intended usage.

### 4. **Data Analysis Queries**
- **Q1:** Top 10 products with the highest discount.
- **Q2:** High-MRP products that are out of stock.
- **Q3:** Estimated revenue by category.
- **Q4:** Products with MRP > ₹500 and discount < 10%.
- **Q5:** Top 5 categories with highest average discount.
- **Q6:** Price per gram analysis for products > 100g.
- **Q7:** Categorization into Low/Medium/Bulk weight classes.
- **Q8:** Total inventory weight per category.

---

## Insights
- Certain categories offer higher discounts, which can be used for marketing.
- Some high-value products are frequently out of stock, indicating supply chain gaps.
- Price per gram analysis helps in competitive pricing.

---


