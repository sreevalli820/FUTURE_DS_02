# Social Media Campaign Performance Tracker

### Overview
This repository contains the solution for **Future Interns Data Science & Analytics Task 2**, which involved designing and analyzing a **Social Media Campaign Performance Tracker** dashboard. The dashboard visualizes and interprets key metrics using a Facebook Ads dataset, providing actionable recommendations for future marketing campaigns.

### Task Description
The project aims to:
- Analyze social media campaign performance by evaluating spend, conversions, CTR (Click-Through Rate), CPC (Cost Per Click), ROI (Return on Investment), ad engagement, and demographic breakdowns.
- Create a dashboard summarizing campaign effectiveness and offering data-driven recommendations for optimization.

### Dataset

This project uses the "Facebook Ad Campaign" dataset from Kaggle. Each record corresponds to a particular ad shown to a certain demographic, with information about engagement and outcomes.

#### Column Descriptions & Significance

| Column               | Description                                                                       | Significance                                              |
|----------------------|-----------------------------------------------------------------------------------|-----------------------------------------------------------|
| ad_id                | Unique identifier for each ad                                                     | Distinguishes individual ads                              |
| reporting_start      | Reporting period start date                                                       | Identifies campaign timeline                              |
| reporting_end        | Reporting period end date                                                         | Identifies campaign timeline                              |
| campaign_id          | Company’s internal campaign ID                                                    | Groups ads under a single campaign                        |
| fb_campaign_id       | Facebook’s campaign tracking ID                                                   | Groups ads from Facebook’s perspective                    |
| age                  | Age group targeted by the ad (e.g., 30-34, 35-39)                                | Enables demographic analysis                              |
| gender               | Gender of the target audience (M/F)                                               | Enables gender-based analysis                             |
| interest1, interest2, interest3 | Codes for audience interest categories as described in Facebook profiles | Used to segment audience types and measure ad performance |
| impressions          | Total number of times the ad was shown                                            | Measures reach of the ad                                  |
| clicks               | Number of clicks received by the ad                                               | Indicates engagement level                                |
| spent                | Amount spent ($) on running the ad                                                | Used to compute ROI and CPC                               |
| total_conversion     | Total number of inquiries/leads after seeing the ad                               | Measures effectiveness of ad in generating interest       |
| approved_conversion  | Number of leads that converted to sales or target action                          | Key indicator of campaign success                         |

### Data Cleaning & Preprocessing

To ensure data quality and reliable analysis, several cleaning and transformation steps were performed during data preparation:

1. **Filtering Out Invalid Campaign IDs:**
   - Removed rows where `fb_campaign_id` had non-numeric values such as "F" or "M" to ensure only valid campaign data is analyzed.
  
2. **Column Type Adjustments:**
   - Changed the columns to their relevant data type.  

**Purpose:**  
These steps help guarantee that the analysis runs on clean, consistent, and accurate data, minimizing errors and improving the reliability of dashboard insights.

### Dashboard Features

- **Summary KPIs:** Total spent, approved conversions, CTR, ROI, CPC, and conversions.
- **Demographic Analysis:** Conversion trends by age, gender, and interests.
- **Temporal Analysis:** Trends of ad spend vs. conversions over time.
- **Campaign Table:** Key performance metrics broken down by campaign/ad.
- **Donut Chart:** Approved conversions by gender.
- **Recommendations:** Strategic insights and next-step suggestions.

### Insights & Recommendations

- Higher **ROI** achieved by focusing on groups with strong engagement.
- **Younger age groups** and certain interests show higher conversions—targeting them improves performance.
- **Female segment** contributed most to approved conversions.
- Test ad creatives and time-of-day placements to further improve CTR and ROI.


### Acknowledgements

- Dataset source: Kaggle, "Facebook Ad Campaign" by madislemsalu
- Task and problem framing by Future Interns.

