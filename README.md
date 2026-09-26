# Olist Business Discovery - HVIA Task 01

This project analyzes the public Olist Brazilian E-Commerce dataset for HVIA Data & AI Solutions Internship Task 01.

## Objective

The goal is to understand Olist's business ecosystem, explore the dataset, identify business patterns/frictions, and propose a realistic data-driven solution HVIA could offer.

## Tools Used

- Python
- pandas
- numpy
- matplotlib
- Jupyter Notebook

## Project Structure

```text
olist_business_discovery_hvia/
├── notebooks/
│   ├── olist_business_discovery.ipynb
│   └── olist_business_discovery.py
├── outputs/
│   ├── charts/
│   ├── summary_metrics.csv
│   ├── category_summary.csv
│   ├── late_vs_ontime_summary.csv
│   └── state_delivery_summary.csv
├── report/
│   └── Olist_Business_Discovery_Report.pdf
├── data/
│   └── README_place_csv_files_here.txt
├── README.md
├── requirements.txt
└── .gitignore
```

## Dataset

Data source: Olist Brazilian E-Commerce Public Dataset.

The raw CSV files are not included in this repository. To run the notebook locally, place the CSV files inside a folder named `data/`.

Required files:

- `olist_orders_dataset.csv`
- `olist_customers_dataset.csv`
- `olist_order_items_dataset.csv`
- `olist_products_dataset.csv`
- `olist_sellers_dataset.csv`
- `olist_order_payments_dataset.csv`
- `olist_order_reviews_dataset.csv`
- `olist_geolocation_dataset.csv`
- `product_category_name_translation.csv`

## Main Focus

The analysis focuses on:

- dataset row-level understanding
- safe joins and aggregation before merging
- order volume and status
- customer and seller locations
- category performance
- delivery performance
- review scores and customer satisfaction
- freight burden
- possible HVIA solution opportunities

## Key Findings

- The dataset contains 99,441 orders, with 96,478 delivered orders.
- Delivery performance is strongly connected with customer satisfaction: late delivered orders had an average review score of about 2.57, compared with about 4.29 for on-time/early delivered orders.
- Demand is concentrated in a few states, especially SP, RJ, and MG.
- Some categories have much higher freight burden relative to item revenue.
- Repeat-customer rate is low in this dataset, so customer experience is important.

## Proposed HVIA Solution

The proposed solution is a Logistics & Customer Satisfaction Intelligence Dashboard.

It would monitor:

- late delivery rate
- average delivery days
- review score impact
- seller performance
- state/location delivery performance
- category freight burden
- risky seller/category/location combinations

## How to Run

1. Clone the repo.
2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Place the Olist CSV files inside a folder named `data/`.
4. Open and run:

```text
notebooks/olist_business_discovery.ipynb
```

