# ⚡ EV Adoption in India — Power BI Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Data Analysis](https://img.shields.io/badge/Data%20Analysis-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

> An in-depth Power BI analysis of Electric Vehicle adoption across India — covering state-wise growth, vehicle category trends, and charging infrastructure readiness.

---

## 📸 Dashboard Preview

![EV Dashboard](assets/dashboard_overview.png)

---

## 📌 Project Overview

This project provides a comprehensive analysis of **Electric Vehicle (EV) adoption in India** using Power BI. It focuses on understanding state-wise EV growth, vehicle category trends, and charging infrastructure readiness — helping identify how India is transitioning towards sustainable transportation and where the critical gaps remain.

**Highlights:**
- 🗺️ State-wise EV sales analysis across 34 States & UTs
- 📅 Year-over-Year growth trend tracking
- 🛵 Vehicle category breakdown (2W, 3W, 4W and more)
- 🔌 Charging infrastructure gap analysis
- 📊 KPI cards, interactive filters, and dynamic visuals

---

## 🎯 Objectives

- Analyze EV adoption trends across India
- Identify top-performing states in EV growth
- Understand category-wise EV demand
- Evaluate the availability of charging infrastructure
- Provide data-driven insights for future EV expansion

---

## 📂 Dataset Details

### 1️⃣ EV Sales Dataset

| Column | Description |
|---|---|
| `Year` | Year of sale |
| `Month_Name` | Month of sale |
| `Date` | Full date |
| `State` | Indian state |
| `Vehicle_Class` | Class of vehicle |
| `Vehicle_Category` | Category (2W, 3W, 4W, etc.) |
| `Vehicle_Type` | Specific vehicle type |
| `EV_Sales_Quantity` | Number of EVs sold |

### 2️⃣ Charging Stations Dataset

| Column | Description |
|---|---|
| `State/UT` | State or Union Territory |
| `Charging Stations Installed` | Number of stations installed |

---

## 🧮 DAX Measures
```dax
-- Total EV Sales
Total EV Sales =
SUM(EV_Sales[EV_Sales_Quantity])

-- Year-over-Year Growth
YoY Growth =
DIVIDE(
    [Total EV Sales] -
    CALCULATE([Total EV Sales], DATEADD(EV_Sales[Date], -1, YEAR)),
    CALCULATE([Total EV Sales], DATEADD(EV_Sales[Date], -1, YEAR))
)

-- Total Charging Stations
Total Charging Stations =
SUM(Charging_Stations[Charging Stations Installed])

-- EVs per Charging Station
EVs per Charging Station =
DIVIDE([Total EV Sales], [Total Charging Stations], 0)

-- Top State by Sales
Top State =
TOPN(1, VALUES(EV_Sales[State]), [Total EV Sales], DESC)
```

---

## 📊 Dashboard Features

| Feature | Description |
|---|---|
| 📍 State-wise Analysis | EV sales breakdown across all Indian states |
| 📅 YoY Growth Trends | Year-over-year adoption growth chart |
| 🛵 Category Distribution | Sales split by vehicle category (2W, 3W, 4W) |
| 🔌 Infrastructure Mapping | Charging station availability by state |
| 📊 KPI Cards | Total Sales, Growth %, Stations, EVs per Station |
| 🎛️ Interactive Filters | Slice by State, Year, and Vehicle Category |

---

## 💡 Key Insights

### 🚀 Rapid Growth
EV adoption in India is accelerating year by year, with sales volumes increasing consistently across nearly all states and categories.

### 🏆 Top Performing States
**Uttar Pradesh, Tamil Nadu, and West Bengal** lead the country in EV sales, driven by large populations, state-level incentives, and growing urban demand.

### 🛵 Two-Wheelers Dominate
Two-wheelers account for approximately **50% of total EV sales** — the most affordable entry point into the EV market and the primary driver of mass adoption.

### 🔌 Infrastructure Gap
With around **26,000 charging stations** nationwide and roughly **133 EVs per charging station**, the infrastructure is significantly lagging behind vehicle adoption rates.

### 🌍 Nationwide Reach
EV adoption has now spread across **34 States and Union Territories**, showing this is no longer limited to metro cities — it's a national movement.

### 📅 Seasonal Trends
Sales data reveals clear seasonal patterns, with demand peaking in certain months aligned with government subsidy cycles and festive buying seasons.

---

## 🧠 Business Insights

- **High EV demand in populous states** signals strong untapped market potential for manufacturers and dealers
- **Two-wheelers are the affordability gateway** — focusing on this segment accelerates mass adoption faster than any other category
- **Charging infrastructure is the bottleneck** — every 133 EVs sharing one station is unsustainable and will slow adoption if not addressed urgently
- **Government policy is a key driver** — states with active FAME II scheme implementation and local EV policies show noticeably stronger growth
- **Rural expansion is the next frontier** — current adoption is urban-heavy; rural infrastructure investment could unlock the next wave of growth

---

## 📝 Conclusion

India's EV ecosystem is expanding rapidly, backed by strong government initiatives, rising fuel costs, and growing consumer awareness. The data tells a clear story: **demand is outpacing infrastructure**, and the two-wheeler segment is leading the charge.

This project demonstrates how Power BI can turn complex, multi-source government and sales data into a clean, actionable dashboard. From state-level rankings to infrastructure gap analysis, every visual is designed to answer a real business question about India's transition to sustainable transport.

The road ahead is electric — and the data shows India is already on it.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Power BI Desktop | Dashboard building & data modeling |
| DAX | Custom measures & calculated columns |
| Power Query | Data cleaning & transformation |
| Excel / CSV | Raw data sources |

---

## 🚀 Getting Started

1. Clone or download this repository
2. Open `EV_Dashboard.pbix` in Power BI Desktop
3. Explore the interactive dashboard
4. Use filters (State, Year, Category) for deeper insights

---

## 📁 Repository Structure
```
ev-adoption-india-powerbi/
├── EV_Dashboard.pbix
├── README.md
├── dataset/
│   ├── ev_sales.csv
│   └── charging_stations.csv
├── dax/
│   └── measures.dax
└── assets/
    └── dashboard_overview.png
```

---

## 📺 Project Demo

👉 [Watch on YouTube](#) *(add your link)*

---

## 👨‍💻 Author

**Hariom Dixit**
📍 Mumbai, India

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/hariom-dixit-2b522a27a/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/YOUR_GITHUB)

---

*If this project helped you or gave you ideas, please give it a ⭐ on GitHub — it means a lot!*
