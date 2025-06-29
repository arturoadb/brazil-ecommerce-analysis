# Sales Performance and Delivery Insights for Brazilian E-Commerce

**Author:** Arturo Alejandro Díaz Barbosa  | LinkedIn: [Arturo Díaz Barbosa](https://www.linkedin.com/in/arturo-díaz-barbosa)  
**Date:** June 2025

**Data Source:**  
Brazilian E-Commerce Public Dataset by Olist  
[https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

---

## Dataset Description

This project leverages the Olist Brazilian e-commerce dataset, which contains over 100,000 orders recorded between September 2016 and August 2018 across multiple marketplaces in Brazil. Key tables include:

- `customer_data`, `orders_data`, `order_items_data`, `order_payments_data`, `order_reviews_data`, `products_data`, `sellers_data`, `geolocation_data`, and `product_translation`

These tables allow multi-dimensional analysis of sales, customer behavior, delivery times, payment methods, and product reviews.

---

## Objective

Provide actionable insights into Olist’s business by analyzing:

1. Overall sales growth and seasonality  
2. Top product categories by revenue and order volume  
3. Customer satisfaction patterns via review analysis  
4. Regional performance in terms of sales volume, revenue, and delivery efficiency  
5. Payment method preferences and their impact  
6. Customer retention and cohort behavior  
7. Order status dynamics and cancellation hotspots

---

## Key Findings

- **Robust Growth Trajectory:** 99,440 orders and \$1.26M in revenue between Sep 2016 and Aug 2018, with revenue rising from \$49.8K in 2016 to \$6.17M in 2017 and \$7.39M in 2018.  
- **Seasonal Peaks:** Significant spikes in May (Health & Beauty for Mother’s Day) and November (Watches & Gifts for Black Friday) drove higher order volumes.  
- **Top Product Categories:** Health & Beauty leads revenue (~\$1.26M), while Bed & Bath Table leads order volume (11,115 orders, 15.5%), followed by Sports & Leisure, Furniture Decor, and Computer Accessories.  
- **Customer Satisfaction Patterns:** 75% positive vs. 25% negative reviews; Bed & Bath Table stands out with both the most positive (7,916) and negative (3,221) reviews.  
- **Regional Concentration:** São Paulo accounts for 41K orders (\$5.20M), followed by Rio de Janeiro and Minas Gerais; Roraima shows minimal sales (7,829).  
- **Delivery Performance Gaps:** Average delivery is 18.8 days to customers, 15.2 days seller dispatch; São Paulo excels (8.8/12.3 days), Bahia shows a 5-day difference between seller and customer.  
- **Payment Preferences:** Credit card is dominant (73.9%), followed by boleto (19%), voucher (5.6%), and debit card (1.5%).  
- **Low Repeat Purchases:** 96.9% of customers only buy once, 2.9% make a second order, with extremely low third purchases.  
- **Order Status Insights:** Highest cancellations are in São Paulo (140), Rio de Janeiro (48), and Belo Horizonte (17), consistent with their order volume.

---

## Repository Structure

```
brazil-ecommerce-analysis/
│
├── data/
│   ├── *.csv                                         # Raw Olist dataset
│   └── results_sql/                                  # Exported CSVs for Power BI
│
├── notebook/
│   └── brazilian-ecommerce-analysis.ipynb            # Jupyter notebook with data loading, SQL queries, and exports
│
├── dashboard/
│   ├── brazilian-ecommerce-dashboard.pbix            # Interactive Power BI dashboard
│   └── brazilian-ecommerce-dashboard.pdf             # PDF version of the dashboard
│
├── docs/
│   └── brazilian-ecommerce-analysis.html             # HTML version of the dashboard or documentation
│
├── .env.example                                      # Example environment variables
├── requirements.txt                                  # Python dependencies
├── README.md                                         # This project overview
└── .gitignore                                        # Ignore credentials and outputs


```

---

## Technologies & Libraries

- **Python**
  - pandas
  - SQLAlchemy
  - python-dotenv
- **PostgreSQL** (via psycopg2)
- **Power BI**
- **Git / GitHub**

---

## Installation

1. **Clone the repository**

```bash
git clone https://github.com/arturoadb/brazil-ecommerce-analysis.git
cd brazil-ecommerce-analysis
```

2. **Configure environment variables**

```bash
cp .env.example .env
# Edit .env with your DB_USER, DB_PASSWORD, DB_HOST, DB_PORT, DB_NAME
```

3. **Install dependencies**

```bash
pip install -r requirements.txt
```

4. **Run the analysis notebook**

- Launch Jupyter and open `notebooks/brazilian-ecommerce-analysis.ipynb`
- Execute all cells to load CSVs into SQL, run the queries, and export CSVs for Power BI

5. **Open Power BI Dashboard**

- Open `powerbi/brazilian-ecommerce-dashboard.pbix` in Power BI Desktop to explore the interactive visuals

---

## Requirements (`requirements.txt`)

```
pandas
SQLAlchemy
psycopg2-binary
python-dotenv
```

---

## Conclusions and Strategic Insights

The following conclusions are based on the data exploration, SQL queries, and visual analysis through the accompanying Power BI dashboard:

1. **Growth Opportunities**  
   Solid growth with 99K+ orders and \$1.26M in revenue, but the high rate of one-time purchases suggests investing in loyalty and retention programs.

2. **Seasonality Awareness**  
   Demand spikes in May (Mother’s Day) and November (Black Friday) highlight the potential of targeted seasonal promotions.

3. **Category Leaders**  
   Health & Beauty dominates revenue, while Bed & Bath Table dominates order counts. Bundling strategies and cross-selling higher-margin products could help.

4. **Regional Strategy**  
   Heavy concentration in São Paulo; consider expanding fulfillment and marketing efforts in under-served states like Roraima.

5. **Delivery Optimization**  
   Reduce average delivery times, particularly in states where a large gap exists between seller dispatch and customer reception (e.g., Bahia).

6. **Payment Methods**  
   Credit card dominates, but supporting installments or “buy now, pay later” for boleto users could improve conversions.

7. **Cohort Retention**  
   Very low repeat rates (96% purchase only once); retention campaigns, loyalty programs, and re-engagement initiatives are critical.

8. **Order Status Trends**  
   Cancellations mirror higher-volume areas; deeper investigation of cancellation reasons could improve fulfillment processes.

---

By combining Python for data orchestration (ETL + SQL) with Power BI dashboards, this project demonstrates a robust, end-to-end data analysis workflow applicable to real-world business environments.


![1](https://github.com/user-attachments/assets/dce2662c-f3d6-48ec-9a02-0a1efa0f03a3)

![2](https://github.com/user-attachments/assets/b7ab189d-0f45-4c02-99ce-70224cc59153)

![3](https://github.com/user-attachments/assets/7f8c4e6f-cbab-4993-9f12-6e68c92027ec)

![4](https://github.com/user-attachments/assets/f33811f9-c3b0-4c83-a57d-34df679db8b4)




