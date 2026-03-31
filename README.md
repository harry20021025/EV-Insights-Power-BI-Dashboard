⚡ EV Adoption in India – Power BI Dashboard
📌 Overview

This project, developed by Hariom Dixit, provides an in-depth analysis of Electric Vehicle (EV) adoption in India using Power BI.
It focuses on understanding state-wise EV growth, vehicle category trends, and charging infrastructure readiness.

The dashboard helps identify how India is transitioning towards sustainable transportation and highlights gaps in infrastructure.

🎯 Objective
Analyze EV adoption trends across India
Identify top-performing states in EV growth
Understand category-wise EV demand (2W, 3W, 4W, etc.)
Evaluate the availability of charging infrastructure
Provide data-driven insights for future EV expansion
📂 Dataset Details
1️⃣ EV Sales Dataset

Contains detailed EV sales data:

Year
Month_Name
Date
State
Vehicle_Class
Vehicle_Category
Vehicle_Type
EV_Sales_Quantity
2️⃣ Charging Stations Dataset

Provides infrastructure data:

State/UT
Charging Stations Installed
📊 Key DAX Measures
Total EV Sales = 
SUM(EV_Sales[EV_Sales_Quantity])

YoY Growth = 
DIVIDE(
    [Total EV Sales] - 
    CALCULATE([Total EV Sales], DATEADD(EV_Sales[Date], -1, YEAR)),
    CALCULATE([Total EV Sales], DATEADD(EV_Sales[Date], -1, YEAR))
)
📈 Dashboard Features
📍 State-wise EV Sales Analysis
📅 Year-over-Year Growth Trends
🛵 Vehicle Category Distribution
🔌 Charging Infrastructure Mapping
📊 KPI Cards (Total Sales, Growth %, etc.)
📉 Interactive Filters (State, Year, Category)
🔍 Key Insights
🚀 EV adoption in India is growing rapidly year by year
🏆 Top States: Uttar Pradesh, Tamil Nadu, West Bengal
🛵 Two-Wheelers dominate (~50% of total EV sales)
🔌 Around 26,000 charging stations available nationwide
⚠️ Approximately 133 EVs per charging station → infrastructure gap
🌍 EV adoption has spread across 34 States & UTs
🧠 Business Insights
High EV demand in populous states indicates strong market potential
Two-wheelers are the primary drivers of EV adoption due to affordability
Charging infrastructure expansion is critical for sustained growth
Government policies are significantly influencing EV adoption
📌 Conclusion

India’s EV ecosystem is expanding rapidly, supported by government initiatives and increasing consumer awareness.
However, charging infrastructure must scale alongside EV adoption to ensure long-term sustainability.

This project demonstrates how Power BI can transform raw data into actionable insights for real-world problems.

🛠️ Tools & Technologies
📊 Power BI
🧮 DAX (Data Analysis Expressions)
📁 Data Cleaning & Modeling
📈 Data Visualization
🚀 How to Use
Download the .pbix file
Open in Power BI Desktop
Explore interactive dashboards
Apply filters for deeper insights
📸 Dashboard Preview

(Add your dashboard screenshot here)

👨‍💻 Author

Hariom Dixit
📍 Mumbai, India
🔗 LinkedIn: https://www.linkedin.com/in/hariom-dixit-2b522a27a/

💻 GitHub: (Add your GitHub link here)

⭐ If you like this project

Give it a ⭐ on GitHub and share your feedback!
