EV Adaptation in India - Power BI Project

Introduction:
This Power BI project, created by Hariom Dixit, analyses the adoption of Electric Vehicles (EVs) across India. The goal is to understand how different states are adapting to EVs and how charging infrastructure supports this growth.
Datasets Used:
1. EV_Sales: Contains columns like Year, Month_Name, Date, State, Vehicle_Class,Vehicle_Category, Vehicle_Type, and EV_Sales_Quantity.
2. ChargingStations: Contains columns like State/UT and the number of Electric Vehicle Charging Stations Installed.

Key DAX Measures:
• Total EV Sales = SUM(EV_Sales[EV_Sales_Quantity])
• YoY Growth = DIVIDE([Total EV Sales] - CALCULATE([Total EV Sales], DATEADD(EV_Sales[Date], -1, YEAR)), CALCULATE([Total EV Sales], DATEADD(EV_Sales[Date], -1, YEAR)))

Key Insights:
1. India’s EV sales have grown rapidly every year, showing strong adoption of electric vehicles across the country.
2. Uttar Pradesh, Tamil Nadu, and West Bengal are the leading states in total EV sales, making them the biggest contributors to India’s EV growth.
3. Two-wheelers (2W personal) make up almost 50% of all EV sales, proving they are the most preferred electric vehicle category in India.
4. India has around 26,000 charging stations, but there are about 133 EVs per charging station, showing that charging points need to increase as EV usage grows.
5. 34 States and Union Territories have started adopting EVs, showing that electric mobility is spreading across almost all parts of India.

Conclusion:
India’s EV market is growing fast, driven by government initiatives and rising consumer interest. While EV sales are increasing each year, there is still a need to expand charging infrastructure to match demand. This project highlights the potential of Power BI in visualizing real-world sustainability trends.
