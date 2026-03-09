# Data dictionary — Meta Ads weekly export

## Dataset overview
- **Source:** Meta Ads Manager export
- **Granularity:** 1 row = **Week × Ad set**
- **Period:** 2024-03-01 to 2025-03-01
- **Currency:** EUR (for spend and cost metrics)
- **Privacy/confidentiality:** Campaign/ad set names are excluded; **platform IDs** are used for identification.

## Identifier / descriptive columns
- **Campaign ID**: Unique campaign identifier from Meta
- **Week**: Week interval shown as start–end date
- **Objective**: Campaign objective (e.g., Traffic, Engagement)
- **Ad set ID**: Unique ad set identifier from Meta
- **Delivery status**: Delivery state (e.g., completed)
- **Delivery level**: Reporting level (campaign/ad set)

## Reach & exposure
- **Reach**: Unique accounts reached
- **Impressions**: Total impressions
- **Frequency**: Impressions per reached account

## Results & attribution
- **Attribution setting**: Attribution window used in reporting
- **Result type**: The metric counted as a “result” for the objective
- **Results**: Number of results for the selected result type
- **Result rate**: Results divided by the relevant base metric (platform-defined)

## Spend & efficiency
- **Amount spent (EUR)**: Total spend in EUR
- **Cost per result**: Spend divided by results
- **CPC (cost per link click)**: Spend per link click
- **CPM (cost per 1,000 impressions)**: Spend per 1,000 impressions
- **Cost per unique link click**: Spend per unique link click

## Clicks & landing page
- **Link clicks**: Number of link clicks
- **Landing page views**: Number of landing page views
- **Clicks (all)**: Total clicks (all types)

## Time fields
- **Starts / Ends**: Campaign/ad set start and end dates (as exported)
- **Reporting starts / Reporting ends**: Reporting interval boundaries

## Budget fields (context)
- **Ad Set Budget**: Budget value set at ad set level (if used)
- **Ad Set Budget Type**: Daily or lifetime (platform-defined)
- **Campaign Budget**: Budget value set at campaign level (if used)
- **Campaign Budget Type**: Daily or lifetime (platform-defined)

## Notes
- Because Excel locale settings may interpret `.` and `,` differently, the **Amount spent (EUR)** column is parsed as numeric using the **en-US** decimal format.
- Campaign/Ad set IDs are stored as **text** to prevent scientific notation and possible rounding/precision loss in Excel.
