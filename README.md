📊 Facebook Ad Campaign Performance Dashboard


This project analyzes Facebook ad campaign data using Power BI to evaluate the performance and efficiency of marketing efforts.
The dashboard provides actionable insights into conversion rates, audience engagement, ad spending, and ROI.

🎯 Objectives

This dashboard aims to answer the following key business questions:

-How well did the ad campaign perform overall?

-Which posts or ads had the highest engagement and conversions?

-What was the Click-Through Rate (CTR) and Return on Investment (ROI)?

-What insights can help improve the next campaign?

📂 Dataset Overview

File name: KAG_conversion_data_raw.csv
Source: Kaggle Facebook Ad Campaign Data

Column Name	Description
ad_id	Unique ID of the advertisement
campaign_id	Unique campaign identifier
fb_campaign_id	Facebook’s campaign reference ID
age	Age group targeted by the ad
gender	Gender targeted by the ad
interest1, interest2, interest3	Audience interest categories
impressions	Number of times the ad was displayed
clicks	Number of clicks the ad received
spent	Amount spent on the ad campaign
total_conversion	Total number of conversions (leads/purchases)
approved_conversion	Number of approved conversions
reporting_start	Start date of the campaign
reporting_end	End date of the campaign


⚙️ Data Cleaning & Preparation

Performed in Power Query Editor (Power BI):

-Removed null, blank, and error rows in campaign_id and fb_campaign_id (23% error resolved).

Changed data types:

impressions, clicks, spent, total_conversion, approved_conversion → Whole/Decimal Number

reporting_start, reporting_end → Date

Created new calculated columns & measures for better insights:

CTR = clicks / impressions

CPC (Cost per Click) = spent / clicks

CPM (Cost per 1000 impressions) = (spent / impressions) * 1000

CPA (Cost per Action) = spent / total_conversion

ROI = (approved_conversion * CPC) / spent

Engagement Rate = (clicks + conversions) / impressions



📊 Dashboard Visuals

Main KPIs (Cards):

Conversion Rate

CTR (Click Through Rate)

CPC (Cost per Click)

CPM (Cost per Mille)

CPA (Cost per Action)

ROI

Charts & Visuals Used:

Bar Chart: Gender-wise Age Group Performance

Column Chart: Age-Gender Wise Sales

Stacked Column Chart: Gender & Age-wise Ad Spend

Gauge Chart: Total Sales

Donut Chart: Clicks vs Impressions

Table: Top Target Categories by Conversion Rate

Table: Top Performing Ads by Conversion and Spend

Pie Chart: Impressions by Age & Gender



💡 Key Insights

Conversion Rate: 33.53% overall, with Males 40–44 years performing best.

CTR: 0.020%, showing moderate engagement.

CPC: $1.495 indicates efficient ad performance.

Females (30–34) had higher spend but slightly lower conversion efficiency.

Top 5 interest categories delivered over 50% conversion rates.



🧠 Tools & Technologies Used

Power BI Desktop – Dashboard creation and analysis

DAX – For calculated KPIs and measures

Power Query Editor – Data cleaning and transformation

CSV Dataset – Raw ad campaign data



🚀 How to Use

Clone or download this repository.

Open Facebook_Ad_Analysis.pbix in Power BI Desktop.

Load the dataset: KAG_conversion_data_raw.csv.

Refresh the data to update visualizations.

Explore insights interactively through filters (age, gender, interests, campaign ID)."# FUTURE_DS_02" 
