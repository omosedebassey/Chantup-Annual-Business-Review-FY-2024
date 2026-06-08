# 📊 ChantUp 2024 Annual Business Review - Power BI Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)
![Domain](https://img.shields.io/badge/Domain-Business%20Intelligence-blue?style=for-the-badge)

> An end-to-end Business Intelligence project analysing FY 2024 sales performance for **ChantUp**- a social commerce platform serving student entrepreneurs across six Nigerian university campuses.

---

## 📁 Project Structure

```
chantup-annual-review-2024/
│
├── data/
│   ├── Fact_Sales_Simplified.csv       # Core transactional sales data (7,500 records)
│   ├── Dim_Products.csv                # Product catalogue with categories and pricing
│   ├── Dim_Locations.csv               # Campus and regional location data
│   └── Dim_Users.csv                   # User demographics, tier, and gender data
│
├── report/
│   └── ChantUp_Annual_Business_Review_2024.pbix   # Power BI report file (5 pages)
│
├── documentation/
│   └── ChantUp_Annual_Business_Review_2024.docx   # Written analysis report
│
└── README.md
```

---

## 🏢 Business Context

ChantUp is a rapidly growing social commerce platform tailored for student entrepreneurs across Nigerian campuses. As a **Junior Business Intelligence Analyst**, the objective was to deliver an Annual Business Review to the executive board, going beyond stating *what* happened to explaining *why* it happened and recommending *what* the company should do in 2025 to increase profitability.

---

## 🎯 Project Objectives

The analysis addresses four core business challenges plus additional behavioural insights:

| Challenge | Focus Area |
|-----------|------------|
| Challenge 1 | Seasonality: identifying peak sales periods tied to the academic calendar |
| Challenge 2 | Marketing Efficiency: evaluating referral source ROI |
| Challenge 3 | Product Category Performance: identifying margin drivers and hidden gems |
| Challenge 4 | Geographic Expansion: comparing campus performance across Nigeria |
| Bonus | Behavioural Insights: time of day, age group, user tier, and product analysis |

---

## 📊 Dashboard Pages

### Page 1. Title Page
A branded cover page with ChantUp logo, geometric design elements, report title, and analyst credit.

---

### Page 2. Campus Sales Analysis
**Slicers:** Age Group (18-21, 22-25, 26-30, 30+) | Category

**KPI Cards (6):**
| Metric | Value |
|--------|-------|
| Total Revenue | ₦111.72M |
| Profit per Order | ₦9,947 |
| Total Profit | ₦67.45M |
| Profit Margin | 60.23% |
| Complete Orders of 7500 | 6,781 |
| Campuses | 6 |

**Visuals:**
- **Total Revenue and Total Profit by Month** - clustered column chart with profit line overlay, clearly showing the August (₦3.6M) and December (₦4.5M) troughs vs the September-October resumption peak (₦14.2M)
- **Total Revenue, Total Profit and Profit Margin by Campus** - clustered bar chart with profit margin % line overlay; UNILAG leads revenue at ₦19.9M, UNN Nsukka highest margin at 60.89%, University of Ibadan lowest margin at 59.28%
- **Total Complete Orders by Campus** - horizontal bar chart (UNILAG 1,155 → UNN Nsukka 1,086); acts as a cross-filter for all other visuals on the page
- **Total Profit Complete by Gender** - donut chart; Female ₦37.14M (55.1%), Male ₦28.13M (41.7%), Non-Binary ₦2.19M (3.2%)

---

### Page 3. Sales Analysis by Referral Source and Category
**Slicers:** Gender | User Tier | Region

**KPI Cards (6):**
| Metric | Value |
|--------|-------|
| Total Revenue | ₦111.72M |
| Total Orders | 7,500 |
| Failed Transaction | ₦8.01M |
| Refunded Revenue | ₦3.17M |
| Categories | 6 |
| Referral Sources | 5 |

**Transaction Health Cards (3):**
- 🟢 **6,781** - Complete Orders
- 🟠 **204** - Refunded Orders
- 🔴 **515** - Failed Orders

**Visuals:**
- **Total Revenue by Referral Source** - bar chart; Reels dominates at ₦55M, Search lowest at ₦6M
- **Failure Rate % by Referral Source** - horizontal bar chart showing rates not absolute values; Profile Feed highest at 7.28%, Direct Link 7.18%, Search lowest at 6.59%
- **Completed Sales and Profit Margin by Referral Source** - combo chart; Profile Feed achieves the highest margin (61.38%) despite lower volume
- **Total Revenue, Total Profit and Profit Margin by Category** - combo chart with margin line; Digital Skills leads at 87.1%, Subscription second at 85.0%, Electronics lowest at 32.1%

---

### Page 4. Behavioural Insights
**Slicers:** Campus | Category | Gender

**KPI Cards (5):**
| Metric | Value |
|--------|-------|
| Total Revenue | ₦111.719M |
| Total Orders | 7,500 |
| Peak Hour | 8 PM |
| Peak Hour Orders | 2,783 |
| Peak Hour % | 37% |

**Visuals:**
- **Order Count by Hour Label** - column chart running 12AM → 11PM; sharp evening peak at 7PM (934), 8PM (978), 9PM (871); near-zero activity from 12AM–5AM
- **Completed Sales and Profit Margin by Age Group** - combo chart; 18-21 drives highest volume (₦54M) but 26-30 achieves the highest margin (61.43%), an underserved opportunity
- **Order Count by Category** - horizontal bar chart (completed orders only); Fashion leads at 1,953, Food lowest at 938
- **Total Revenue, Total Profit and Profit Margin by Product Name** - combo chart; Power BI Masterclass dominates at ₦41M (87.1% margin), ChantUp Premium Monthly achieves 85% margin at near-zero cost
- **Total Orders by User Tier** - donut chart; Free 4,617 (68%), Premium 1,927 (28%), Influencer 237 (3%)

---

## 🔍 Key Findings

### Challenge 1: Seasonality
- **October** was the single highest revenue month at **₦14.2M**, driven by first-semester resumption
- **September–October combined** generated **₦26.3M** - the year's most critical commercial window
- **August** (₦3.6M) and **December** (₦4.5M) were the lowest months, coinciding with inter-semester holidays
- **June** (₦11.2M) marks a secondary peak driven by exam season purchasing behaviour

### Challenge 2: Marketing Channels
- **Reels** drives the highest volume at ₦55M revenue: ChantUp's dominant acquisition engine
- **Profile Feed** has the highest failure rate at **7.28%**: checkout friction requires a UX review
- **Direct Link** failure rate of 7.18% also exceeds the platform average of 6.9%
- **Search** has the lowest failure rate (6.59%): high-intent buyers, systematically under-invested channel
- **Profile Feed** achieves the highest completed sales margin at **61.38%**: high quality when users do convert

### Challenge 3: Product Categories
- **Digital Skills** - ₦41M revenue, **87.1% margin**: most profitable category by far
- **Subscription** - **85% margin** with a near-zero cost base: the hidden gem
- **Electronics** - ₦32M revenue but only **32.1% margin** due to high procurement costs
- **Fashion** - highest order volume (1,953 completed orders): the platform's gateway product
- **Academic** - solid 75% margin, consistent demand tied to the academic calendar

### Challenge 4: Campus Performance
- **UNILAG** leads in revenue (₦19.9M) and completed orders (1,155)
- **UNN Nsukka** has the highest profit margin (60.89%) despite the lowest order count (1,086)
- Performance gap between campuses is only **18.4%**; strong product-market fit across all regions
- **ABU Zaria** (North West) performs competitively with southern campuses; validates Pan-Nigeria expansion strategy

### Behavioural Insights
- **8 PM** is the peak shopping hour; **7PM–9PM** accounts for **37% of all daily orders**
- Activity is near-zero between 12AM–5AM; no marketing spend warranted in these hours
- **Age 26–30** has the highest profit margin (61.43%) but the smallest order volume; the most underserved segment
- **Free tier** users dominate at 68% of orders; large opportunity to convert to Premium (28%)
- **Influencer tier** represents only 3% of orders but carries disproportionate referral influence

---

## 💡 Strategic Recommendations

| Priority | Area | Recommendation |
|----------|------|----------------|
| 🔴 Critical | Seasonality | Front-load marketing budget into September–October Resumption Rush |
| 🔴 Critical | Digital Skills | Expand course catalogue; introduce certification bundles |
| 🟠 High | Reels | Increase Reels content budget; hire campus video creators |
| 🟠 High | Subscription | Bundle with Digital Skills; promote during onboarding |
| 🟡 Medium | Campus Expansion | Expand to OAU, Covenant University, BUK Kano, FUTA |
| 🟡 Medium | Electronics | Negotiate supplier costs or curate high-margin SKUs only |
| 🟡 Medium | Profile Feed UX | Audit checkout journey to reduce 7.28% failure rate |
| 🔵 Ongoing | Search SEO | Invest in in-app and Google search visibility |
| 🔵 Ongoing | Evening Campaigns | Schedule push notifications and flash sales for 6PM–9PM |
| 🔵 Ongoing | Age 26–30 Segment | Launch career-focused Digital Skills campaign for postgraduates |
| 🔵 Ongoing | Free → Premium | Design upgrade incentives to convert the 68% Free tier users |

---

## 🛠️ Tools & Technologies

| Tool | Usage |
|------|-------|
| **Power BI Desktop** | Dashboard design, data modelling, DAX measures, cross-filtering |
| **Power Query (M Language)** | Data transformation, custom column creation |
| **DAX** | Calculated measures across all dashboard pages |
| **Microsoft Word** | Written business analysis report |
| **CSV** | Raw data sources |

---

## 📐 Data Model

Star schema with one fact table and three dimension tables:

```
Dim_Users ──────────┐
                    │
Dim_Products ───────┼──── Fact_Sales (7,500 rows)
                    │
Dim_Locations ──────┘
```

**Fact_Sales columns:** Order_ID, User_ID, Product_ID, Loc_ID, Order_Date, Quantity, Unit_Price, Unit_Cost, Status, Referral_Source

---

## ⚙️ Power Query Transformations

Custom columns created in Power Query (M Language):

```m
// Extract hour number from Order_Date timestamp
Order_Hour = Time.Hour([Order_Date])

// Convert 24-hour number to readable AM/PM label
Hour_Label =
if [Order_Hour] = 0 then "12 AM"
else if [Order_Hour] < 12 then Text.From([Order_Hour]) & " AM"
else if [Order_Hour] = 12 then "12 PM"
else Text.From([Order_Hour] - 12) & " PM"

// Conditional highlight flag for peak hours (7PM-9PM)
Hour_Highlight =
if [Order_Hour] >= 19 and [Order_Hour] <= 21 then 1 else 0
```

---

## ⚙️ DAX Measures

```dax
// ── Revenue & Profitability ──
Total Revenue = SUMX(Fact_Sales, Fact_Sales[Quantity] * Fact_Sales[Unit_Price])
Total Cost = SUMX(Fact_Sales, Fact_Sales[Quantity] * Fact_Sales[Unit_Cost])
Total Profit = [Total Revenue] - [Total Cost]
Profit Margin % = DIVIDE([Total Profit], [Total Revenue], 0)
Profit per Order = DIVIDE([Total Revenue], [Completed Orders], 0)

// ── Transaction Health ──
Completed Orders = CALCULATE(COUNTROWS(Fact_Sales), Fact_Sales[Status] = "Completed")
Failed Orders = CALCULATE(COUNTROWS(Fact_Sales), Fact_Sales[Status] = "Failed")
Refunded Orders = CALCULATE(COUNTROWS(Fact_Sales), Fact_Sales[Status] = "Refunded")
Failure Rate % = DIVIDE([Failed Orders], COUNTROWS(Fact_Sales), 0)

// ── Behavioural KPIs ──
Peak Hour Orders =
CALCULATE(
    COUNT(Fact_Sales[Order_ID]),
    Fact_Sales[Order_Hour] >= 19,
    Fact_Sales[Order_Hour] <= 21
)

Peak Hour % =
DIVIDE(
    CALCULATE(
        COUNT(Fact_Sales[Order_ID]),
        Fact_Sales[Order_Hour] >= 19,
        Fact_Sales[Order_Hour] <= 21
    ),
    COUNT(Fact_Sales[Order_ID]),
    0
)

Peak Hour =
VAR HourTable =
    ADDCOLUMNS(
        VALUES(Fact_Sales[Order_Hour]),
        "HourCount", CALCULATE(COUNT(Fact_Sales[Order_ID]))
    )
VAR MaxCount = MAXX(HourTable, [HourCount])
VAR PeakHour = MAXX(FILTER(HourTable, [HourCount] = MaxCount), Fact_Sales[Order_Hour])
RETURN
IF(PeakHour = 0, "12 AM",
IF(PeakHour < 12, PeakHour & " AM",
IF(PeakHour = 12, "12 PM",
(PeakHour - 12) & " PM")))

// ── Conditional Formatting ──
Hour Highlight =
VAR SelectedHour = SELECTEDVALUE(Fact_Sales[Order_Hour])
RETURN IF(AND(SelectedHour >= 19, SelectedHour <= 21), 1, 0)
```

---

## 🚀 How to Use

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/chantup-annual-review-2024.git
```

2. **Open the report**
   - Open `report/ChantUp_Annual_Business_Review_2024.pbix` in Power BI Desktop

3. **Refresh data if needed**
   - Go to **Home → Transform Data**
   - Update file paths to match your local `data/` folder location
   - Click **Close & Apply**, then **Home → Refresh**

4. **Navigate the dashboard**
   - Use the **page tabs** at the bottom to move between the 5 pages
   - Use **slicers** on each page to filter by Campus, Gender, Age Group, Category, User Tier, or Region
   - Click any **campus bar** on the Campus Sales Analysis page to cross-filter all visuals on that page
   - **Ctrl + Click** to select multiple slicer values at once

---

## 📈 Results Summary

| Metric | FY 2024 Value |
|--------|---------------|
| Total Revenue | ₦111.72M |
| Total Profit | ₦67.45M |
| Overall Profit Margin | 60.23% |
| Transaction Completion Rate | 90.4% |
| Top Campus by Revenue | UNILAG (₦19.9M) |
| Top Category by Margin | Digital Skills (87.1%) |
| Highest Failure Rate Channel | Profile Feed (7.28%) |
| Peak Shopping Hour | 8 PM |
| Peak Window Share of Orders | 37% (7PM–9PM) |
| Repeat Customer Rate | 99.2% |

---

## 👤 Author

**Omosede Bassey**
Junior Business Intelligence Analyst
📧 *(omosede.bassey@gmail.com)*
🔗 *([https://www.linkedin.com/in/omosede-bassey-978bb1289/])*

---

## 📄 License

This project was completed as part of the **UniF.uk ChantUp Capstone Project**.
Data is fictional and used for educational and portfolio purposes only.
