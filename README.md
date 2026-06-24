# 📊 Global Airbnb Performance Dashboard — Power BI Project

> **A 3-page interactive Power BI dashboard analyzing global Airbnb performance across 10 cities — covering listing growth history, market concentration, pricing dynamics, host trust signals, review behavior, and city-level ratings.**
>
> <img width="1376" height="768" alt="airbnb" src="https://github.com/user-attachments/assets/eac32b97-fd88-4f7b-822c-072bbb495233" />


---

## 📌 Project Overview

Airbnb's global dataset is rich — but raw, inconsistent, and spread across multiple dimensions. This project builds a **production-grade Power BI dashboard** that transforms that raw data into a structured, interactive business intelligence product.

The dashboard is designed for three analytical audiences:
- **Business strategists** tracking market concentration and growth lifecycle
- **Marketing teams** understanding seasonal review patterns and city performance
- **Operations teams** analyzing host trust, pricing tiers, and rating gaps

It is not a static report. It's a **navigable BI product** with dynamic views, bookmark-based UI toggling, and conditional formatting — built on a validated star schema data model.

---

## 📐 Dashboard Structure

The project is organized as a **3-page interactive dashboard**, each page solving a distinct analytical problem:

| Page | Title | Focus |
|------|-------|-------|
| Page 1 | New Listings Growth | Historical lifecycle analysis (2008–2021) |
| Page 2 | Market Share & Pricing | City concentration, Superhost vs non-Superhost, avg pricing by property type |
| Page 3 | Ratings & Review Behavior | City-level ratings, review frequency, host trust analysis |

---

## 🔢 Key Metrics at a Glance

| Metric | Value |
|--------|-------|
| Total Listings | **2,79,712** |
| Cities Analyzed | **10** |
| Total Hosts | **1,82,024** |
| Property Types | **144** |
| Total Reviews | **53,73,000+** |

---

## 📈 Page 1 — New Listings Growth Lifecycle

<img width="1073" height="801" alt="Screenshot 2026-06-23 094934" src="https://github.com/user-attachments/assets/404ad778-f5ad-4171-a9a1-b739f994cf2d" />


### Business Question
*How has Airbnb's listing volume evolved over time, and what external forces shaped that growth?*

### Visual
A **multi-line area chart** tracking Total Listings, Entire Place, Hotel Room, Private Room, and Shared Room from **2008 to 2021**, annotated with lifecycle phases.

### Lifecycle Phases Identified

```
Introduction (2008–2010)  →  Slow initial traction
Growth (2010–2013)        →  Take-off point; exponential listing growth
Maturity (2013–2015)      →  Peak new listings reached in 2015
Decline (2016–2017)       →  Regulatory tightening across major cities
Reinvention (2018–2019)   →  New growth phase; hotel rooms increase
COVID-19 (2020–2021)      →  Severe demand and listing collapse
```

### Key Findings
- **2015** saw the highest number of new listings globally — driven primarily by Entire Place category
- **2016–2017** decline was not organic — it was caused by tightening local regulations, not demand loss
- Airbnb became **profitable in H2 2016** and **2017 was its first full profitable year** — despite declining listings
- From **2018**, a new growth wave began, driven by hotel room category expansion
- **COVID-19 (2020)** halted this recovery and collapsed all listing categories simultaneously

---

## 🗺️ Page 2 — Market Share by Cities & Pricing

### Business Question
*Which cities dominate the Airbnb market, and how does pricing vary by property type?*

### Visual 1 — Pareto Bar Chart (Market Share by City)

<img width="1072" height="800" alt="Screenshot 2026-06-23 095003" src="https://github.com/user-attachments/assets/d0d0591c-37df-4e28-a6b5-ef0dae53f60b" />


Stacked bar chart showing Superhost vs Non-Superhost listings per city, with cumulative percentage line.

| City | Cumulative Market Share |
|------|------------------------|
| Paris | 23.1% |
| New York | 36.4% |
| Sydney | 48.4% |
| Rome | 58.3% |
| Rio de Janeiro | 67.8% |
| Istanbul | 76.5% |
| Mexico City | 83.7% |
| Bangkok | 90.6% |
| Cape Town | 97.5% |
| Hong Kong | 100.0% |

**Key Insight:** Paris, New York, and Sydney together account for **48.4% of all listings** and **48% of total reviews** — the top 3 cities drive nearly half the platform's volume.

**Paris leads** with the most listings and reviews. A likely driver: Paris hotel rooms average **$800/night** versus Airbnb Entire Place at **$673** — nearly a 19% price premium for hotels, pushing travelers toward Airbnb.

### Visual 2 — Average Price by Property Type

<img width="1075" height="801" alt="Screenshot 2026-06-23 095016" src="https://github.com/user-attachments/assets/32e81ab4-71c2-47aa-9ccf-edfac7e13c73" />


| Property Type | Average Price |
|---------------|--------------|
| Hotel Room | **$800** |
| Entire Place | **$673** |
| Shared Room | **$580** |
| Private Room | **$462** |

**Key Insight:** Shared rooms are disproportionately priced relative to private rooms — only a $118 gap despite a significant difference in privacy. This suggests pricing inefficiency or supply scarcity in the shared room category.

---

## ⭐ Page 3 — Ratings & Review Behavior

<img width="1070" height="807" alt="Screenshot 2026-06-23 095032" src="https://github.com/user-attachments/assets/b5323379-456e-4ec9-864c-aafd9b2f48fa" />


### Business Question
*Which cities perform best on quality metrics, and how reliable is review data as a proxy for satisfaction?*

### Visual 1 — Overall Ratings by City (Bar Chart)

| City | Average Rating |
|------|---------------|
| Mexico City | 94.8 |
| Rio de Janeiro | 94.6 |
| Cape Town | 94.4 |
| New York | 93.8 |
| Rome | 93.5 |
| Sydney | 93.2 |
| Paris | 93.1 |
| Bangkok | 93.0 |
| Istanbul | 91.1 |
| Hong Kong | 89.7 |

**Key Insight:** Mexico City and Rio de Janeiro are the **best-rated cities**. Hong Kong and Istanbul are the **worst-rated**. Globally, **Cleanliness** and **Value for Money** are the two dimensions that score lowest across cities — representing the most actionable improvement areas for hosts.

### Visual 2 — Detailed Ratings Heatmap (City × Dimension)

Interactive toggle between **Overall Ratings** and **Detailed Ratings** views using Power BI bookmarks.

| City | Accuracy | Cleanliness | Communication | Location | Value |
|------|----------|-------------|---------------|----------|-------|
| Mexico City | 9.7 | 9.6 | 9.8 | 9.8 | 9.6 |
| Cape Town | 9.6 | 9.5 | 9.7 | 9.7 | 9.5 |
| Rio de Janeiro | 9.6 | 9.4 | 9.8 | 9.8 | 9.3 |
| New York | 9.6 | 9.3 | 9.7 | 9.6 | 9.4 |
| Paris | 9.6 | 9.2 | 9.7 | 9.7 | 9.3 |
| Hong Kong | 9.2 | 9.0 | 9.4 | 9.6 | 9.0 |
| Istanbul | 9.3 | 9.1 | 9.5 | 9.4 | 9.2 |

Conditional **gradient color formatting** applied — red = low, green = high — to identify rating gaps at a glance.

### Visual 3 — Review Frequency Distribution

| Reviews Written | % of Reviewers | Cumulative % |
|----------------|----------------|--------------|
| 1 | 86.3% | 86.3% |
| 2 | — | 96.4% |
| 3 | — | 98.6% |
| 4–5 | — | 99.3–99.6% |
| 6+ | — | ~99.8% |
| Max (283 reviews) | 1 user | 99.8% |

**Key Insight:** **86.3% of reviewers wrote only once**. This means review count is a highly skewed metric — a listing with 50 reviews has near-unique demand signals. The outlier with 283 reviews (two Bangkok listings, Oct 2020) is flagged as a likely data anomaly.

Filtering threshold applied: **reviews > 85** to remove low-frequency noise from visual calculations.

### Visual 4 — Seasonal Review Patterns (Monthly % by City)

Cities tracked: Paris, Rome, New York, Sydney, Mexico City

- **Paris and Rome dominate** review share from **April to August** — reflecting European summer travel peaks
- **New York surges** in **November–December** during the holiday season
- Sydney shows consistent year-round activity with mild winter dips

### Visual 5 — Host Trust Signal Matrix

| | No Profile Pic | Profile Pic |
|---|---|---|
| **Identity Not Verified** | 0.1% | 26.5% |
| **Identity Verified** | 0.1% | **73.2%** |

**Key Insight:** **73.2% of hosts are fully verified** (verified identity + profile photo). Only **0.1% of hosts are completely anonymous** (no photo, no verification). This indicates strong platform-level trust enforcement — Airbnb's trust infrastructure is working.

---

## 🛠️ Technical Implementation

### Data Modeling — Star Schema

```
         ┌─────────────────┐
         │  dim_listings   │
         │  (Property info)│
         └────────┬────────┘
                  │
┌──────────┐      │      ┌──────────────┐
│dim_hosts │◄─────┼─────►│  fact_reviews│
│(Host data)│     │      │(Review events)│
└──────────┘      │      └──────────────┘
                  │
         ┌────────┴────────┐
         │   dim_cities    │
         │ (Location data) │
         └─────────────────┘
```

Relationships validated for referential integrity. Star schema ensures fast DAX query performance and clean slicing across all visuals.

---

### Power Query — Data Cleaning Steps

```
1. Missing value handling        → Null imputation for price, rating, and host fields
2. Categorical normalization     → Standardized property_type and room_type labels
3. Date parsing                  → Converted string date columns to proper Date type
4. Review count filtering        → Applied >85 threshold to remove noise listings
5. Outlier flagging              → Identified 283-review anomaly for manual review
6. Trust signal encoding         → Derived binary flags for identity_verified + has_photo
```

---

### DAX Measures Engineered

```dax
-- Cumulative Listings over time
Cumulative Listings =
CALCULATE(
    COUNT(listings[listing_id]),
    FILTER(
        ALL(dim_date[year]),
        dim_date[year] <= MAX(dim_date[year])
    )
)

-- % of Monthly Reviews by City
% Monthly Reviews =
DIVIDE(
    COUNTROWS(fact_reviews),
    CALCULATE(COUNTROWS(fact_reviews), ALL(dim_cities[city]))
)

-- Average Daily Price by Property Type
Avg Daily Price =
AVERAGEX(
    listings,
    listings[price_usd]
)

-- Host Trust Score (Verified + Photo)
Fully Verified Hosts % =
DIVIDE(
    COUNTROWS(FILTER(dim_hosts, dim_hosts[identity_verified] = TRUE
                             && dim_hosts[has_photo] = TRUE)),
    COUNTROWS(dim_hosts)
)
```

---

### Dynamic UI — Bookmarks & Navigation

The dashboard uses **Power BI Bookmarks + Button Actions** to create a seamless toggle between two rating views on the same page:

```
[Overall Ratings View]  ←──────────────→  [Detailed Ratings View]
     Bar Chart                              Heatmap Table
  (City avg scores)                   (City × Dimension matrix)
```

Users switch between views via on-page buttons — no page navigation required. This eliminates the need for a separate page and keeps the dashboard compact.

---

### Conditional Formatting Logic

Applied **gradient-based conditional formatting** across the detailed ratings heatmap:

```
Score < 9.1   →  Red    (Poor — action required)
Score 9.1–9.4 →  Amber  (Average — monitor)
Score > 9.4   →  Green  (Strong — benchmark)
```

Applied to: Accuracy, Cleanliness, Communication, Location, Value columns.

---

## 📁 Project Structure

```
airbnb-performance-dashboard/
│
├── Airbnb_Dashboard.pbix              # Main Power BI file
├── datasets/
│   ├── listings_raw.csv               # Raw listings data
│   ├── reviews_raw.csv                # Raw reviews data
│   └── hosts_raw.csv                  # Raw host data
├── screenshots/
│   ├── page1_listings_growth.png
│   ├── page2_market_share.png
│   ├── page2_pricing.png
│   ├── page3_ratings_overall.png
│   ├── page3_ratings_detailed.png
│   └── page3_review_frequency.png
├── dax/
│   └── measures.dax                   # All custom DAX measures
└── README.md
```

---

## 💡 Key Business Insights Summary

| Insight | Implication |
|---------|-------------|
| Top 3 cities = 48.4% of all listings | Airbnb's supply is heavily concentrated — market risk if regulations change in Paris, NYC, or Sydney |
| 2015 peak + 2016 regulatory decline | Platform growth is policy-sensitive, not just demand-driven |
| Hotel rooms avg $800 vs Airbnb $673 | Price advantage is Airbnb's core Paris demand driver |
| 86.3% of reviewers write only once | Review count ≠ customer loyalty; not a reliable frequency metric |
| Cleanliness & Value score lowest | Two highest-impact areas for host quality improvement programs |
| 73.2% of hosts fully verified | Trust infrastructure is strong — low anonymous host risk |
| Paris + Rome peak April–August | Seasonal supply planning window for European markets |

---

## 🛠️ Tools & Environment

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Power Query](https://img.shields.io/badge/Power_Query-217346?style=for-the-badge&logo=microsoft&logoColor=white)

- **BI Tool:** Microsoft Power BI Desktop
- **Data Modeling:** Star Schema (Fact + Dimension tables)
- **Data Transformation:** Power Query (M language)
- **Analytics Layer:** DAX (custom measures + calculated columns)
- **UI Features:** Bookmarks, Button Navigation, Conditional Formatting
- **Dataset:** Global Airbnb listings and reviews data

---

## 🔮 Future Enhancements

- **Price Prediction Model** — Python regression integrated via Power BI Python visual
- **Occupancy Rate Analysis** — Estimated occupancy from review frequency patterns
- **ROI Calculator** — Host-facing expected earnings by city and property type
- **Real-time Data Refresh** — Scheduled dataset refresh via Power BI Service
- **Superhost Conversion Analysis** — What separates Superhost from regular hosts by metric

---

## 👤 Author

**Sandip** — EDP Analyst | Aspiring Data Analyst
📍 Nagpur, Maharashtra, India
🔗 [LinkedIn](https://linkedin.com/in/yourprofile) | [GitHub](https://github.com/yourusername)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

*If this project helped you, consider giving it a ⭐ on GitHub.*
