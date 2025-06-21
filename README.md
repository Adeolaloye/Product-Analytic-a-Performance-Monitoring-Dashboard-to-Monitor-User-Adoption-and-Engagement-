## Product Analytics: Implementing a Performance Monitoring Dashboard to Monitor User Adoption and Engagement on VendBridge App
This repository contains the analytical work, Tableau dashboards, and insights derived from tracking the market performance and user engagement of the VendBridge App within the first 3 months of its launch.
### Table of Content
- [Project Overview](#project-overview)
- [Key Dashboards](#key-dashboards)
- [Business Problem](#business-problem)
- [Project Objectives](#project-objectives)
- [Tech Stack](#tech-stack)
- [Data Description](#data-description)
- [Process](#process)
- [Key Insights](#key-insights)
- [Recommendations](#recommendations)
### Project Overview
VendBridge, a brainchild of NexaLink- a renowned tech giant, is a digital platform that effortlessly connects buyers and sellers in today's dynamic marketplace.Recognizing the growing need for a platform that not only facilitates transactions but also fosters trust and loyalty, NexaLink launched Vend Bridge as a strategic move to capitalize on the increasing trend of digital commerce. VendBridge was born out of the aspiration to simplify and enhance the way people engage in online commerce. It aims to provide a seamless and transparent platform where buyers can effortlessly discover products they desire and connect with sellers who offer them. Through VendBridge, NexaLink aspires to set new benchmarks in e-commerce, fostering trust and ensuring both parties involved in a transaction are satisfied and well-served.
### Key Dashboards
- **User Acquisition Dashboard**: App installs, sign-ups, uninstalls.
- **User Engagement Dashboard**: Daily active users, transactions, average time spent.
- **Regional Leaderboard**: Regional performance scorecards and tier classification.
- **Forecasting Dashboard**: Predicted KPIs with month-on-month analysis.

 ![Capture overview](https://github.com/user-attachments/assets/a9567043-ad1b-4569-8abd-7f073b39ccb6)

![Capture engage](https://github.com/user-attachments/assets/e820dffe-eae9-4a5e-a598-6055e42878c0)

![Capture leader](https://github.com/user-attachments/assets/94fd33c6-ea51-4634-a1d1-97af316769bc)

![Capture forcast](https://github.com/user-attachments/assets/d9eda444-766c-4f0a-ac6a-19a9a691744e)

### Business Problem
NexaLink introduced VendBridge to the market just three months ago, following an extensive series of pre-launch and post-launch marketing campaigns. With a significant investment in promotional efforts, the product team wants to monitor the performance of VendBridge since its inception. The team is keen on understanding the extent to which VendBridge has been embraced by the market and also constantly monitor the app performance. Key performance metrics (KPIs) such as daily active users (DAUs), installation rates, user sign-up figures, transaction counts, and other product analytics metrics will be used to assess VendBridge's reception and impact. By meticulously assessing these metrics, the product team can gain a precise understanding of VendBridge's reception and impact in the market as well as its performance. This will help the product team can gain valuable insights into the performance of VendBridge and identify areas where it can be improved to better meet the needs of its users.

### Project Objectives
1. **Track and Visualize Key Performance Indicators (KPIs)**  
   Monitor critical metrics such as daily active users, app installs, user sign-ups, uninstalls, app crashes, and transactions via Tableau dashboards.
2. **Evaluate Market Adoption and User Engagement**  
   Understand how users interact with the app and assess market penetration post-launch.
3. **Compare Regional Performance**  
   Analyze KPIs by region using a composite performance score and segment regions into strategic tiers (e.g., Platinum, Gold, Silver, Bronze, Basic).
4. **Forecast Future Performance**  
   Use Tableau’s forecasting features to predict future performance trends based on historical data.
5. **Identify Growth Drivers and Risk Indicators**  
   Pinpoint the KPIs positively and negatively influencing product success to support improvement strategies

### Tech Stack
- **Google Sheet**
- **Data Visualization**: Tableau  
- **Data Source**: VendBridge performance dataset (CSV)  
- **Forecasting**: Tableau in-built time series forecasting  
- **Performance Metrics**: Aggregated KPIs, calculated fields, parameters, and filters
  
### Data Description
 download dataset here[VendBridge.xlsx](https://github.com/user-attachments/files/20846401/VendBridge.xlsx)
- Date : The specific day on which the recorded data points were observed.
- Total App Installs: The total number of times the app was downloaded and installed on a device.
-  User Sign-Ups: The total number of users who have registered or created an account on the app up to the specified date.
-  Daily Active Users: The number of unique users who interacted with the app on the specified date.
-  Num_Transactions: The total number of trade transactions executed by users within the VendBridge app on the specified date.
-  Uninstalls: The number of times the VendBridge app was removed from devices on the specified date.
-  Number of App Crashes: The total instances where the VendBridge app unexpectedly stopped working and closed on the specified date.
-  Avg Time Spent per User (min): The average duration, in minutes, that each user spent interacting with the VendBridge app on the specified date . 
-  Region: The region in which the data was collected
-  Device: The device on which the data was collected
 
### Process
#### 1. **Data Understanding**
- Reviewed raw dataset and cleaned the data where necessary.
- Upload the cleaned data into Tableau  
- Created calculated fields (Performance Score, MoM%, tiering logic)  
- Designed interactive dashboards with filters and KPIs  
- Applied Tableau forecasting tools to predict future KPI trends  
- Summarized and presented findings with actionable insights
  
#### 2. **KPI Identification**
- **Growth Drivers:** App Installs, Sign-Ups, DAUs, Transactions, Avg Time Spent  
- **Risk Indicators:** App Crashes, Uninstalls, Declining Engagement

#### 3. **Dashboard Development**
- **User Acquisition Dashboard:** Market penetration and adoption trends
- **User Engagement Dashboard:** Usage patterns and retention signals
- **Regional Leaderboard:** Tiered region performance using a weighted performance score
- **Forecasting Dashboard:** Predicted KPIs for the next month using historical trends

#### 4. **Performance Score Model**
- Created a custom metric combining:
  - DAUs, Transactions, Installs, and Sign-Ups (positive influence)
  - Deducted weights for Uninstalls, Crashes, and drop in Avg Time Spent

#### 5. **Tiering and Segmentation**
- Grouped regions into 5 tiers: **Platinum**, **Gold**, **Silver**, **Bronze**, **Basic**
- Tiering logic based on performance scores and ranking

#### 6. **Forecasting**
- Used Tableau's exponential smoothing (ETS) to forecast KPIs for September
- Compared forecasted KPIs with August to calculate MoM% growth/decline

### Key Insights
#### 1. Strong Market Penetration Post-Launch
The app recorded steady month-over-month (MoM) growth in installations and user sign-ups across most regions, indicating effective pre-launch and post-launch marketing campaigns.
#### 2. High Engagement in Top Regions
The U.S. and EMEA regions showed the highest performance scores, driven by consistently high Daily Active Users (DAUs), total transactions, and average time spent on the app.
#### 3 LATAM Underperformance
LATAM region consistently underperformed across all KPIs, ranking lowest in installs, engagement, and transaction activity, with a higher uninstall and crash rate.
#### 4. Positive KPI Growth Plateauing
Forecasting shows a flattening or decline in most growth KPIs (e.g., DAUs, transactions) by September, except a marginal increase in sign-ups and installs.
#### 5. User Churn Risk Identified
A noticeable rise in uninstall rates and decreased average time spent in some regions indicate a risk of churn and low user retention, especially after initial install.
#### 6. Tier-Based Performance Clarity
The regional leaderboard helped segment the 5 regions into meaningful tiers (Platinum to Basic), providing a clearer framework for strategy, resource allocation, and communication.

### Recommendations
#### 1. Focus on Retention Strategies in LATAM & Canada
Launch localized campaigns, improve onboarding, and enhance support to reduce uninstall rates and increase user time on the app in underperforming regions.
#### 2 Strengthen Engagement Features in Low-Spend Regions
Introduce interactive features, loyalty programs, or gamification elements to increase user stickiness and DAU numbers.
#### 3 Optimize App Performance to Reduce Crashes
Prioritize bug fixes and performance optimization in regions showing higher crash rates to improve user experience and retention.
#### 4 Use Tiering to Guide Strategic Resource Allocation
Assign more marketing and development resources to top-tier (Platinum & Gold) regions to scale growth, while applying targeted fixes in lower-tier areas.
#### 5 Monitor Leading Indicators Weekly
Build automated alerts or mini-dashboards for early signs of decline in key KPIs like time spent, DAUs, or uninstall spikes.
#### 6 Prepare for Plateauing Growth
Since forecasts indicate slowing growth, consider launching new features, cross-promotions, or partnership campaigns to reignite user interest and drive continued adoption.
