# Washington-state-EV-market-trend-analysis
Interactive Excel dashboard analyzing EV market trends in Washington State, including YoY growth, BEV vs PHEV adoption, brand dominance, average EV range, and CAFV eligibility patterns through exploratory data analytics (EDA) using WA DOL public dataset.

# 1. Background & Project Overview
Understanding EV adoption patterns is increasingly important for transportation planning, infrastructure forecasting, incentive allocation, and market insight. This project organizes Washington State’s EV population data (2000–2026) into a stakeholder-ready interactive dashboard designed to support:

* EV market performance reporting
* BEV vs PHEV adoption trend analysis
* Clean Alternative Fuel Vehicle (CAFV) eligibility evaluation
* Manufacturer market share insights
* Electric range improvement monitoring

The dashboard consolidates KPIs, trend visualizations, and slicer-driven interactivity to provide both high-level summaries and deep-dive analytics.

# 2. Data Import and Tranformation
The project uses the Washington State Department of Licensing (DOL) EV Population Dataset, containing ~257,635 vehicle records.
The full dataset was cleaned, shaped, and transformed using Power Query before analytical modeling and dashboard creation.

- Power Query Processing Summary:

    * Loaded 257K+ rows into Excel via Power Query
    * Standardized column names and data types
    * Created analytical flags (BEV/PHEV, CAFV eligibility)
    * Removed inconsistent values and handled missing fields
    * Formatted the dataset into an analysis-ready structured table

![Power Query Screenshot](https://raw.githubusercontent.com/sriramsandilya/Washington-state-EV-market-trend-analysis/main/PowerQuery.png)

# 3. Data Structure Overview
The dataset contains statewide EV registration records, where each row represents a single vehicle. Key fields include:
* Make, Model, Model Year
* Electric Range (miles)
* EV Type: Battery Electric (BEV) or Plug-In Hybrid (PHEV)
* CAFV Eligibility Status
* Base MSRP
* City, County, State

While the dataset is structured as a single flat file, it follows a typical fact table with several descriptive attributes.

# 4. Executive Summary
Washington State’s EV market has expanded rapidly over the past decade, with accelerated growth beginning around 2020. BEVs account for the majority of the market, driven by improvements in range and an expanding charging network. Tesla remains the dominant manufacturer statewide, significantly influencing overall trends. Range performance continues to improve YOY, while CAFV eligibility has increased modestly.

Below is a snapshot of the dashboard used to explore these trends:

<img width="558" height="350" alt="image" src="https://github.com/user-attachments/assets/5f5f47e9-c3d8-4f27-a46e-ace45a018ffc" />

# 5. Insights Deep Dive
* EV Adoption Over Time
EV registrations surged beginning in 2020, reflecting market expansion and better vehicle availability but saw a steep decrease post 2023.
YoY EV Growth (2024 → 2025): –48%
(Note: 2026 data is incomplete, which influences comparisons.)

* BEV vs PHEV Market Share
BEVs account for the majority of the EV population and continue to grow faster than PHEVs.
BEV Share of Total EVs: ~79%

* Brand Market Distribution
Tesla maintains a significantly higher adoption rate than any other manufacturer, shaping most statewide trends.
Tesla Total Vehicles: 107,535 (Top Brand)

* Electric Range Trends
Battery ranges continue to improve due to advancements in EV technology.
Avg. EV Range YoY Improvement: +10.11%

* CAFV Eligibility Patterns
Eligibility improved modestly, suggesting more new EVs meet incentive requirements.
CAFV Eligible Vehicles YoY Change: +3.74%

# 6. Recommendation Summary

Based on analyzed statewide trends:

* Reevaluate CAFV Incentive Thresholds: 
Many EVs exceed current eligibility criteria; adjusting caps could broaden program effectiveness.
* Prioritize BEV-Focused Infrastructure: 
With BEVs dominating market growth, investment should emphasize fast-charging networks.
* Encourage Manufacturer Diversity: 
Tesla's outsized share introduces market concentration risks. Incentives may help diversify adoption.
* Monitor Cost-to-Range Efficiency: 
Tracking range-per-dollar over time helps assess improvements in consumer value and market competitiveness.
* Segment EV Adoption by Region: 
Geographic insights can guide targeted infrastructure and outreach strategies.

# Technical Notes
Technical details (KPI calculations, pivot tables, data cleaning steps, and formula breakdowns) are included in the project files for transparency and reproducibility.

# Caveats & Assumptions

* 2026 data is incomplete and can influence YoY results.
* Duplicate VINs exist due to registration updates; this project preserves the original dataset.
* MSRP values vary by trim and region; averages reflect raw dataset values.
* Eligibility rules change over time and may not match current consumer-facing criteria.

# Data Source
Washington State Department of Licensing — Electric Vehicle Population Data
https://catalog.data.gov/dataset/electric-vehicle-population-data

# Attribution
Dashboard Design & Analysis © 2025 Sriram Kambhampati
Licensed under the MIT License.
