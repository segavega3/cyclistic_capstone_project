Cyclistic Capstone Project: Analyzing Member vs. Casual Rider Behavior
Google Data Analytics Professional Certificate Capstone

-Goal: Identify key differences between casual riders and annual members to develop data-driven marketing strategies for converting casual riders into members.
-Tools Used: SQL (BigQuery), Tableau
-Skills Demonstrated: Data cleaning, SQL querying, data visualization, storytelling, business insights


Business Problem
Cyclistic, a bike-share company, aims to increase annual memberships because members provide higher long-term value than casual riders. The marketing team wants to understand how these two user groups behave differently.

Key Business Questions:
1️. How do annual members and casual riders use Cyclistic bikes differently?
2️. What factors influence casual riders to convert to annual memberships?
3️. How can Cyclistic use data-driven strategies to increase memberships?

Business Impact: The insights from this analysis will be used to optimize marketing campaigns, adjust pricing strategies, and improve user experience.

Data Source
The dataset comes from Motivate International Inc. and is publicly available:
🔗 Divvy Trip Data (Cyclistic)--- NEEDS LINK

Data Overview:
Time Range: February 2024 - January 2025

Original Columns:ride_id, rideable_type, started_at, ended_at, start_station_name, start_station_id,
end_station_name, end_station_id, start_lat, start_lng, end_lat, end_lng, member_casual

Columns Used (After Cleaning & Filtering):rideable_type, started_at, ended_at, start_lat, start_lng, end_lat, end_lng, member_casual

Final Processed Dataset: A cleaned dataset was created for analysis & visualization.
Raw Data & Cleaning Steps: SQL Files--- NEEDS LINK

Data Cleaning & Preparation

Key Actions Taken in the Prepare Phase:
- Schema validation across 12 months of data
- Filtered dataset to keep only relevant columns
- Checked for missing values (found 18-23% missing station data)
- Verified duplicates (confirmed unique ride IDs)
- Created a cleaned dataset for visualization
- 
SQL Queries Used: View SQL File


Key Findings & Insights
1️. Ride Frequency & User Behavior
  - Members take 1.81x more trips than casual riders (3.7M vs. 2.1M trips).
  - Casual riders use electric scooters 2.5x more than members (59.04% vs. 40.96%).
  - Electric bikes are the most preferred ride type for both members and casual riders.

2️. Ride Duration & Distance
  - Casual riders take longer trips than members (24.66 min vs. 12.28 min).
  - Members travel slightly longer distances on average (2.18 km vs. 2.11 km for casual riders).

3️. Most Popular Start & End Stations
  - Casual Riders: Streeter Dr & Grand Ave is the most popular start station.
  - Members: Kingsbury St & Kinzie St is the most popular start station.
  - End Station Trends: Casuals often end at tourist-heavy locations, members at commuter hubs.

4️. Ride Route Insights
  - Casual Riders: Most common route → Streeter Dr & Grand Ave ↔ Streeter Dr & Grand Ave (40.1 min avg).
  - Members: Most common route → State St & 33rd St → DuSable Lake Shore Dr & Monroe St (3.58 min avg).
  - Casual riders take leisure rides, while members use bikes for commuting.

5️. Peak Ride Times (Daily, Weekly, Monthly Patterns)
  - Peak ride times for both groups: 4-6 PM (26% of total trips).
  - Casual riders peak on weekends (Saturday 20.7%), while members peak midweek (Wednesday 16.45%).
  - Riding season peaks between July - October.

6️. Ride Type Preferences Over Time
  - Members' most-used ride type: Electric bikes (50.93%).
  - Casuals' most-used ride type: Electric bikes (50.73%).
  - Casual riders are 2.5x more likely to use scooters than members.

7️. Ride Duration by Ride Type

Members:
Electric scooter: 7.75 min
Electric bike: 10.73 min
Classic bike: 14.08 min

Casual Riders:
Electric scooter: 11.44 min
Electric bike: 14.04 min
Classic bike: 37.69 min

SQL Queries Used for These Insights: View SQL File ----NEEDS LINK

Data Visualizations & Insights

Interactive Tableau Dashboards:
View on Tableau Public (Replace with your link)

Static Visuals Available: Visualizations
  - Monthly Ride Comparison
  - Peak Hours Heatmap
  - Ride Duration Distribution
  - Member vs. Casual Geographic Zones

Business Recommendations
1️. Target Casual Riders with Membership Promotions
  Why? Casual riders take longer, more leisure-focused rides but are less consistent.
Strategy: Offer discounts on electric bike memberships, which casual riders prefer.


2️. Optimize Marketing Campaigns Based on Peak Usage
  Why? Casuals peak on weekends, members peak on weekday mornings & evenings.
Strategy:
Weekend Ads: Promote longer ride discounts to casual users.
Weekday Ads: Highlight convenience & cost savings for members.


3️. Adjust Pricing for Electric Scooters
  Why? Casual riders use electric scooters 2.5x more than members.
Strategy: Increase non-member pricing or create a scooter-specific membership option.


4️. Improve Data Collection on Casual Riders
  Why? Both Casual and Member riders do not retain persistent user IDs, making tracking difficult.
Strategy: Offer optional guest profiles or loyalty points to track repeat casual users.

