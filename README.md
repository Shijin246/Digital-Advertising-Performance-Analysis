Digital Advertising Performance Analysis

An interactive Power BI dashboard designed to analyze digital advertising campaign performance, audience behavior, engagement, conversions, and timing patterns.


Project Overview

This project uses Microsoft Power BI to transform digital advertising data into an interactive business intelligence dashboard.

The dashboard provides a consolidated view of campaign performance, audience characteristics, advertising engagement, purchase activity, conversion behavior, and time-based patterns.

The project focuses on turning raw advertising event data into meaningful visual insights that can support campaign monitoring and performance analysis.

Project Objectives

The main objectives of this project are:

- Monitor overall digital advertising performance
- Analyze campaign-level performance
- Measure Click-Through Rate (CTR)
- Analyze advertising engagement
- Track impressions, clicks, and purchases
- Understand audience behavior by age and gender
- Analyze audience targeting patterns
- Identify purchase patterns across audience segments
- Analyze advertising activity by country
- Identify time-based advertising patterns
- Analyze the advertising event funnel
- Compare current performance with previous periods
- Provide an interactive dashboard for business analysis

Tools & Technologies

- Microsoft Power BI
- Power Query
- DAX
- Data Modeling
- Data Visualization
- Interactive Dashboard Design

---
Key KPIs

The dashboard tracks several important advertising performance indicators:

| KPI | Description |
|---|---|
| Total Budget | Total advertising budget |
| Total Impressions | Number of times advertisements were displayed |
| Total Clicks | Number of advertisement clicks |
| CTR | Click-Through Rate measuring click activity relative to impressions |
| Total Purchases | Number of purchase events |
| Conversion Rate | Measures conversion performance |
| Engagement Rate | Measures audience engagement with advertisements |

Dashboard Pages
1. Overview

The Overview page provides a high-level summary of the overall advertising performance.

Main components:

- Total Budget
- Total Impressions
- Total Clicks
- CTR
- Total Purchases
- Conversion Rate
- Engagement Rate
- Performance Trend Over Time
- Advertising Event Funnel
- Date filter
- Campaign filter
- Platform filter
- Performance Metric selector
- Previous-period performance comparison

Dashboard Preview
Overview Dashboard(Screenshots/01_Overview.png)

2. Campaign Performance

The Campaign Performance page focuses on comparing individual advertising campaigns.

Main components:

- Campaign performance KPI cards
- Campaign performance table
- Budget vs Purchases analysis
- CTR by Ad Type
- Top 10 Campaigns by Purchases
- Engagement Rate by Platform

The Budget vs Purchases visualization helps examine the relationship between advertising budget and purchase activity across campaigns.

Dashboard Preview

Campaign Performance(Screenshots/02_Campaign_Performance.png)

3. Audience Insights

The Audience Insights page analyzes the characteristics and behavior of the advertising audience.

Main components:

- Total Users
- Average User Age
- Male Users
- Female Users
- Audience Countries
- Purchase by Age Group
- Targeting Accuracy by Age Group
- Targeting Accuracy by Gender
- Events by Country
- Engagement Rate by Gender
- Purchase by Gender

The targeting analysis compares the intended targeting segments with the observed audience distribution.

Dashboard Preview

Audience Insights(Screenshots/03_Audience_Insights.png)

4. Timing Patterns

The Timing Patterns page analyzes when advertising activity occurs.

Main components:

- Best Day
- Best Time Slot
- Events by Time of Day
- Purchases by Day of Week
- Events by Hour
- Weekday vs Weekend analysis
- Day and Time heatmap

These visualizations help identify patterns in advertising activity across different days and time periods.

Dashboard Preview

Timing Patterns(Screenshots/04_Timing_Patterns.png)

5. Campaign Details

The Campaign Details page provides a more detailed campaign-level analysis through a drill-through experience.

This allows users to move from an overall campaign analysis into a more focused view of a selected campaign.

Dashboard Preview

Campaign Details(Screenshots/05_Campaign_Details.png)


DAX & Calculations

DAX measures were created to calculate important advertising performance metrics and period-over-period comparisons.

Example: Previous Month CTR

```DAX
CTR Previous Month =
CALCULATE(
    [CTR],
    DATEADD(
        DimDate[Date],
        -1,
    )
)
        MONTH
    )
)
