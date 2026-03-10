# 🔔 Ring.com Digital Performance & Funnel Analysis — 2025

> **End-to-end e-commerce funnel analysis** of Ring.com's 2025 performance across 146K sessions, $3.33M revenue, and 8 traffic channels — built with Python, SQL, and Power BI.

---

## 📊 Project Overview

This project analyzes Ring.com's full digital funnel — from traffic acquisition to purchase — to identify where users drop off, which channels perform best, and what behavioral signals predict conversion.

The analysis spans **January to December 2025** and is built on 8 relational tables covering sessions, pageviews, clicks, scroll depth, cart events, and orders.

---

## 🗂️ Dataset

| Table | Rows | Description |
|---|---|---|
| `session_table` | 146,000 | Traffic source, device, UTM data |
| `pageview_table` | 354,456 | Page paths & navigation flow |
| `click_table` | 204,752 | CTA clicks & element interactions |
| `scroll_table` | 292,106 | Scroll depth per page |
| `add_to_cart_table` | 25,133 | Product add-to-cart events |
| `order_table` | 11,206 | Completed orders & discounts |
| `order_line_item_table` | 22,406 | Product-level order details |
| `user_table` | 102,435 | User purchase history flags |

---

## 🛠️ Tools & Technologies

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=mysql&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)
![PowerPoint](https://img.shields.io/badge/PowerPoint-B7472A?style=flat&logo=microsoft-powerpoint&logoColor=white)

- **Python** — Pandas, NumPy, Matplotlib, Seaborn (EDA & data cleaning)
- **Power BI** — Interactive dashboards, DAX measures, funnel visualization
- **SQL** — Data extraction, joins, aggregations across 8 tables
- **PowerPoint** — Executive summary presentation

---

## 📈 Key Metrics

| Metric | Value |
|---|---|
| Total Sessions | 146,000 |
| Unique Users | 102,435 |
| Total Revenue | $3.33M |
| Total Orders | 11,206 |
| Conversion Rate | 7.68% |
| Avg Order Value | $496 |
| Units Sold | 34,000 |
| Discount Dependency | 67% |

---

## 🔍 Key Findings

### 1. 🚧 Product Page is the #1 Conversion Bottleneck
- **43% of all sessions** end on the product page with no further action
- Users scroll to an average depth of **85%** — they are reading, but not converting
- Only **17.2% of sessions** add to cart after visiting the product page
- Once past the product page, the funnel is remarkably healthy — Cart → Checkout → Purchase maintains **~99% retention**

### 2. 🖱️ 'Buy Now' Click = 2.75x Conversion Lift
- Sessions with a **Buy Now** click convert at **13.47%** vs **4.88%** without
- Scroll depth and device type show **zero differentiation** in conversion
- Buy Now clickers who didn't purchase are the highest-priority retargeting audience

### 3. 📣 Paid Social: High Volume, Low Efficiency
- Paid Social drives **38% of all traffic** (55,930 sessions) — 5x larger than any other channel
- Yet it delivers the **lowest conversion rate** among all channels
- **SMS and Affiliate** convert significantly better with far less spend

### 4. 🎯 Each Product Has a Different Best Channel

| Product | Best Channel | Conv. Rate |
|---|---|---|
| Video Doorbell Pro 2 | SMS | 8.31% |
| Ring Alarm 8-piece | SMS | 8.26% |
| Stick Up Cam Battery | Display | 8.33% |
| Indoor Cam (2nd Gen) | Affiliate / Internal | 8.22% |

> A single channel strategy across all products wastes budget.

### 5. ⚠️ 67% Discount Dependency = Margin Risk
- **Two-thirds of all orders** require a discount to close
- **Video Doorbell & Ring Alarm** account for **76% of total revenue** — over-reliance on two SKUs is a concentration risk

---

## 💡 Recommendations

| Priority | Action | Expected Impact |
|---|---|---|
| 🔴 High | Optimize product page CTA — add reviews, trust badges, urgency signals | 5% improvement ≈ ~3,000 extra orders/year |
| 🔴 High | Retarget Buy Now clickers who didn't purchase | Highest-intent unconverted segment — low cost, high return |
| 🟡 Medium | Shift budget from Paid Social → SMS & Affiliate | Same spend, significantly more conversions |
| 🟡 Medium | Run product-specific channel strategies | Eliminate wasted spend from low-converting combos |
| 🟢 Low | Test bundles & value messaging to reduce discount dependency | Protect margin on $3.33M revenue base |

---

## 📁 Project Structure

```
ring-funnel-analysis/
│
├── Ring.ipynb                          # Python EDA & analysis notebook
├── ring.pbix                           # Power BI dashboard file
├── Ring_Performance_Analysis_2025.pptx # Executive presentation
└── README.md
```

---

## 📊 Dashboard Preview

The Power BI dashboard includes:
- **Funnel visualization** — session drop-off at each stage
- **Channel performance table** — cart rate & conversion rate by UTM medium
- **Revenue breakdown** — by product, channel, and month
- **Discount analysis** — discount given vs not given
- **Traffic trends** — monthly session volume

---

## 🚀 How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/yourusername/ring-funnel-analysis.git
   ```
2. Install dependencies
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
3. Open the notebook
   ```bash
   jupyter notebook Ring.ipynb
   ```
4. Open `ring.pbix` in **Power BI Desktop** to explore the interactive dashboard

---

## 👤 Author

**Vivek Kumar Lunawat**
- 📧 vivekkumarlunawat@gmail.com

---

*This project is part of my data analytics portfolio. Feel free to explore, fork, or reach out with feedback!*
