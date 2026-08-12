# 🛒 E-Commerce Conversion Funnel Analysis

## 📌 Project Overview

This project analyzes customer behavior throughout an e-commerce purchasing journey to understand how users move from **browsing to purchasing**, identify where the biggest customer drop-offs occur, and examine how funnel performance varies across different customer and business dimensions.

The analysis was built using **Power BI** to transform raw e-commerce event data into meaningful business insights.

---

## 🎯 Business Problem

An e-commerce business wants to understand:

- How customers move through the purchasing funnel
- Where the highest customer drop-offs occur
- Whether conversion performance differs by channel, device, region, and product category
- Which channels, products, devices, and regions generate the most revenue
- Where the business should focus its attention to improve conversion and revenue

---

## ❓ Business Questions

### Funnel Performance
1. How many sessions reach each stage of the purchasing journey?
2. What is the overall conversion rate?
3. Which stage has the highest drop-off?

### Drop-off Analysis
4. Which marketing channel has the lowest conversion rate?
5. Which device has the lowest conversion rate?
6. Which product category has the lowest conversion rate?
7. Which region has the lowest conversion rate?

### Revenue Analysis
8. Which channel generates the most revenue?
9. Which product category generates the most revenue?
10. Which device generates the most revenue?
11. Which region generates the most revenue?

---

## 📂 Dataset

The dataset contains e-commerce user and session-level event data.

### Columns

| Column | Description |
|---|---|
| `User_ID` | Unique identifier for the customer |
| `Session_ID` | Unique identifier for a browsing session |
| `Event` | Customer action such as Browse, Add to Cart, Checkout, or Purchase |
| `Timestamp` | Date and time of the event |
| `Device` | Device used during the session |
| `Region` | Customer region |
| `Channel` | Marketing/acquisition channel |
| `Product_Category` | Category of product involved |
| `Revenue` | Revenue generated from a purchase |
| `Bounce_Flag` | Indicates whether a session bounced |

---

## 🛠️ Tools & Technologies

- **Power BI** — Data analysis and visualization
- **DAX** — Calculated measures and funnel metrics
- **Power Query** — Data preparation
- **GitHub** — Project documentation and portfolio

---

## 🔄 Analysis Process

### 1. Data Understanding

I examined the dataset structure, available fields, event types, and the customer journey represented by the data.

The main funnel stages were:

**Browse → Add to Cart → Checkout → Purchase**

### 2. Data Preparation

The dataset was prepared for analysis by ensuring that:

- Event values were correctly categorized
- Session IDs could be used to measure unique sessions
- Revenue values were suitable for aggregation
- Timestamp information could be used for date analysis

### 3. Funnel Analysis

Unique sessions were used to measure performance at each funnel stage:

- Browse sessions
- Add-to-cart sessions
- Checkout sessions
- Purchase sessions

Conversion and drop-off rates were calculated between the different stages.

### 4. Drop-off Analysis

Funnel performance was analyzed across:

- Channel
- Device
- Product Category
- Region

### 5. Revenue Analysis

Revenue was analyzed across the same dimensions to identify the strongest revenue-generating channels, devices, regions, and product categories.

---

# 📊 Dashboard

The Power BI report contains **four pages**, each answering a different business question.

## Page 1 — Funnel Overview

**Business question: What is happening in the customer journey?**

The page includes:

- Total Sessions
- Overall Conversion Rate
- Overall Drop-off Rate
- Total Revenue
- E-commerce Conversion Funnel
- Stage Conversion vs Drop-off
- Key Finding

### Key Finding

**Checkout → Purchase has the highest drop-off at 69.35%, making it the biggest funnel bottleneck.**

---

## Page 2 — Drop-off Analysis

**Business question: Where are customers dropping off?**

Conversion and drop-off were analyzed by:

- Channel
- Device
- Product Category
- Region

### Key Finding

**Desktop has the lowest conversion rate at 9.85%, while Tablet leads at 11.52%.**

Interactive filters allow users to explore the analysis by channel, device, and region.

---

## Page 3 — Revenue Analysis

**Business question: Where is the revenue coming from?**

The page includes:

- Total Revenue
- Purchases
- Average Revenue per Purchase
- Revenue by Channel
- Revenue by Product Category
- Revenue by Device
- Revenue by Region

### Key Findings

| Dimension | Top Performer | Revenue |
|---|---|---:|
| Channel | Email | $308.90K |
| Product Category | Electronics | $256.04K |
| Device | Tablet | $415.49K |
| Region | East | $312.15K |

---

## Page 4 — Executive Summary & Recommendations

**Business question: What should the business pay attention to?**

### Key Findings

- **69.35%** of customers drop off between Checkout and Purchase.
- **Desktop** has the lowest conversion rate at **9.85%**.
- **Email** generates the highest channel revenue at **$308.90K**.
- **Tablet** generates the highest device revenue at **$415.49K**.
- **Electronics** generates the highest product-category revenue at **$256.04K**.
- **East** generates the highest regional revenue at **$312.15K**.

### Recommendations

**1. Investigate checkout friction**

Examine the Checkout → Purchase journey to understand the factors contributing to the high abandonment rate.

**2. Review the desktop experience**

Investigate the desktop purchasing journey, particularly the checkout stage, since desktop has the lowest conversion rate.

**3. Learn from high-performing channels**

Examine what is working well with Email and identify practices that could potentially be applied to other channels.

**4. Investigate high-revenue segments**

Further analyze Tablet users and Electronics products to understand the factors contributing to their strong revenue performance.

> **Note:** The dataset identifies where customers drop off, but it does not provide enough information to determine the exact causes of abandonment. Additional data such as payment errors, shipping information, website analytics, or customer feedback would be required to determine the specific causes.

---

# 📈 Key Metrics

| Metric | Result |
|---|---:|
| Total Sessions | 10,000 |
| Add to Cart Sessions | 7,059 |
| Checkout Sessions | 3,524 |
| Purchase Sessions | 1,080 |
| Overall Conversion Rate | 10.80% |
| Overall Drop-off Rate | 89.20% |
| Checkout → Purchase Drop-off | 69.35% |
| Total Revenue | $1.18M |
| Highest Revenue Channel | Email — $308.90K |
| Highest Revenue Device | Tablet — $415.49K |
| Highest Revenue Product Category | Electronics — $256.04K |
| Highest Revenue Region | East — $312.15K |

---

# 💡 Key Takeaways

The analysis shows that the largest challenge in the customer journey occurs between **Checkout and Purchase**, where 69.35% of sessions are lost.

Channel, device, product category, and regional analysis also reveal differences in conversion and revenue performance.

The findings provide a starting point for investigating checkout friction, improving the desktop experience, optimizing high-performing channels, and understanding the factors behind high-revenue segments.

---

## 📁 Project Structure

```text
E-Commerce-Conversion-Funnel-Analysis/
│
├── README.md
│
├── Dataset/
│   └── ecommerce_funnel_dataset.csv
│
├── PowerBI/
│   └── ecommerce_conversion_funnel.pbix
│
└── Screenshots/
    ├── page-1-funnel-overview.png
    ├── page-2-drop-off-analysis.png
    ├── page-3-revenue-analysis.png
    └── page-4-executive-summary.png
```

## 📚 What I Learned

Through this project, I strengthened my ability to:

- Translate a business problem into clear analytical questions
- Understand and analyze an e-commerce customer journey
- Build and interpret a conversion funnel
- Calculate and analyze conversion and drop-off rates using DAX
- Analyze customer behavior across channels, devices, regions, and product categories
- Distinguish between conversion performance and revenue performance
- Design a multi-page Power BI dashboard with a clear business story
- Turn data-driven findings into practical business recommendations
- Communicate insights in a way that supports business decision-making
- Avoid making assumptions beyond what the available data can actually explain

---

## 👩🏽‍💻 About Me

I am an aspiring **Data Analyst** passionate about using data to solve business problems and turn raw information into meaningful insights.

I am building my skills in **Excel, SQL, Power BI, DAX, and Python**, while working on real-world projects to strengthen my analytical and problem-solving abilities.

Through hands-on projects like this one, I am learning not only how to build dashboards, but also how to think like an analyst — starting with the business problem, asking the right questions, finding meaningful patterns in the data, and communicating insights clearly.

---

### 🛠️ Skills & Tools

- **Data Analysis:** Excel, SQL, Python
- **Data Visualization:** Power BI, Excel
- **Business Intelligence:** Power BI, DAX
- **Data Preparation:** Power Query, Pandas
- **Other:** Data Cleaning, Exploratory Data Analysis, KPI Analysis, Dashboard Development

---

## 📫 Connect With Me

- **LinkedIn:** https://www.linkedin.com/in/victoria-okafor-4720a02b8
- **GitHub:** https://github.com/vicokafor
