# 📱 Mobile-IQ — Sales Intelligence Dashboard

> A Power BI dashboard for analyzing mobile phone sales across brands, regions, customer segments, and sales channels.

---

## 📊 Dashboard Preview

## Overview 
<img width="1198" height="674" alt="Screenshot 2026-02-21 060854" src="https://github.com/user-attachments/assets/eaa9f95e-f0aa-499b-9e13-f4bc93bc8fb4" />

## Product Analysis 
 <img width="1198" height="675" alt="Screenshot 2026-02-21 060912" src="https://github.com/user-attachments/assets/88d70827-64da-4fdd-8491-2c5b04e1165a" />
 
## Customer Insights
<img width="1201" height="672" alt="Screenshot 2026-02-21 060944" src="https://github.com/user-attachments/assets/f748f747-5453-4c9b-8724-17f2b1a469b1" />

## Channel Performance
 <img width="1199" height="675" alt="Screenshot 2026-02-21 061000" src="https://github.com/user-attachments/assets/f0e2360e-1d2a-4f55-8905-3de246c504cf" />

## Summary
<img width="1201" height="674" alt="Screenshot 2026-02-21 061024" src="https://github.com/user-attachments/assets/6d352db5-a22a-49ec-b7ac-fbcf285f3b9d" />

---

## 🗂️ Pages & Features

### 🏠 Overview
High-level snapshot of the business performance.
- **KPI Cards** — Total Revenue (GH₵14.53M), Average Revenue (GH₵39.69K), Total Units Sold (19K), Average Price (GH₵784.73)
- **Revenue by Month** — Line chart tracking monthly revenue trends (Jan–Dec)
- **Revenue by Brand** — Donut chart showing brand market share (Samsung 23.97%, OnePlus 20.84%, Apple 25.08%, Google 17.58%, Xiaomi 12.53%)
- **Revenue by Channel** — Horizontal bar: Online, Retail Store, Partner
- **Revenue by Model (Top 5)** — Z Fold 6, Galaxy S25 Ultra, Pixel 9 Pro, OnePlus 12 Pro, OnePlus 11R

---

### 📦 Product Analysis
Deep-dive into product-level performance.
- **Product Table** — All 19 models with Sum of Price and Total Revenue per brand
- **KPI Cards** — Total Models (19), Average Unit Price (GH₵784.73), Total Units Sold
- **Revenue by Storage Size** — 128GB (34.93%), 256GB (32.62%), 64GB (32.45%)
- **Revenue by Color** — Ranked bar chart: White, Black, Green, Blue, Red

---

### 👥 Customer Insights
Understanding who is buying and how.
- **KPI Cards** — Avg Customer Age (38.69), Female Customers (191), Male Customers (143), Others (32)
- **Revenue by Age Group** — Column chart across 6 brackets (26–33 leads)
- **Revenue by Gender** — Donut: Female 49.55%, Male 42.09%, Other 8.36%
- **Revenue by Country** — Bing map with bubble markers (India, Turkey, Bangladesh, Pakistan)
- **Age Group by Payment Type** — Grouped bar: EMI, Cash, Credit Card, UPI
- **Age Group by Average Spending** — Horizontal bar ranked by age bracket

---

### 📡 Channel Performance
Sales channel and payment breakdown.
- **Revenue by Sales Channel** — Donut: Online 62.32%, Retail Store 25.63%, Partner 12.05%
- **Unit Sold by Channel** — Horizontal bar chart
- **Total Revenue by Brand** — Clustered bar across months
- **Total Revenue by Month** — 100% stacked bar split by channel (Online / Partner / Retail Store)
- **Revenue % by Country** — 100% stacked bar (India, Turkey, Bangladesh, Pakistan)

---

### 📋 Summary
Cross-dimensional breakdown for strategic review.
- **Total Revenue by Brand and Age Group** — Matrix visual showing channel (Online / Retail / Partner) split per age group across all brands

---

## 🎛️ Global Filters

All pages include the following slicer filters:
| Filter | Options |
|---|---|
| Filter by Country | All / India / Turkey / Bangladesh / Pakistan |
| Filter by Brand | All / Apple / Google / OnePlus / Samsung / Xiaomi |
| Operating System | All / Android / iOS |

---

## 📁 Dataset Overview

| Column | Description |
|---|---|
| `Transaction_ID` | Unique transaction identifier |
| `Transaction_Date` | Date of sale |
| `End of Month` | Month-end date for time grouping |
| `Mobile_Model` | Phone model name |
| `Brand` | Manufacturer brand |
| `Storage_Size` | 64GB / 128GB / 256GB |
| `Color` | Device color |
| `Operating_System` | Android or iOS |
| `Price` | Unit selling price (GH₵) |
| `Units_Sold` | Number of units in transaction |
| `Total_Revenue` | Price × Units Sold |
| `Sales_Channel` | Online / Retail Store / Partner |
| `Payment_Type` | Cash / Credit Card / EMI / UPI |
| `Customer_Age` | Buyer's age |
| `Customer_Age_Group` | Age bracket (18-25 through 58-65) |
| `Customer_Gender` | Male / Female / Other |
| `Country` | Country of sale |
| `City` | City of sale |
| `Latitude` / `Longitude` | Coordinates for map visuals |

**Records:** 366 transactions | **Period:** Jan 1 – Dec 31, 2024 | **Markets:** 5 countries, 22 cities

---

## 🚀 Getting Started

### Prerequisites
- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/mobile-iq-dashboard.git
   cd mobile-iq-dashboard
   ```

2. **Open the report**
   - Launch Power BI Desktop
   - Open `Mobile-IQ.pbix`

3. **Load your data**
   - The dashboard uses the CSV dataset in `/data/mobile_sales_2024.csv`
   - If prompted, update the data source path via **Home → Transform Data → Data Source Settings**

4. **Refresh**
   - Click **Refresh** in the Home ribbon to reload data

---

## 🗃️ Project Structure

```
Retails-analysis/
│
├── pdf-file
    ├── Mobile-IQ.pdf
├── powerBi
    ├── Mobile-IQ.pbix              # Power BI report file
├── README.md                   # This file
│
├── data/
│   └── mobile_sales_2024.csv   # Raw transaction dataset
│
└── screenshots/
    ├── overview.png
    ├── product.png
    ├── customer.png
    ├── channel.png
    └── summary.png
```

---

## 🛠️ Built With

- [Power BI Desktop](https://powerbi.microsoft.com/) — Report authoring
- [Microsoft Bing Maps](https://www.microsoft.com/en-us/maps) — Geographic visuals
- DAX — Calculated measures and KPIs

---

## 📌 Key Metrics (2024)

| Metric | Value |
|---|---|
| Total Revenue | GH₵14.53M |
| Total Units Sold | ~19,000 |
| Average Price | GH₵784.73 |
| Top Brand | Apple (25.08%) |
| Top Model | Z Fold 6 |
| Top Channel | Online (62.32%) |
| Top Market | India |
| Top Age Group | 26–33 |

---

## 📄 License

This project is for educational and portfolio purposes. Dataset is synthetic.

---

*Built with Power BI · Mobile-IQ Sales Intelligence · 2024*
