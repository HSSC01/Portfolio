# VLCC Fleet Utilisation Analysis — Q1–Q2 2025

## Project Overview

**Business Objective**  
This simulation project analyses the utilisation performance of a VLCC (Very Large Crude Carrier) fleet over the first half of 2025 (January–June).  
The goal was to understand how efficiently vessels were deployed, identify any underperforming vessels or trade routes, and highlight areas for operational improvement.  
This insight helps the commercial and operations teams make informed decisions about voyage planning, routing, and future asset deployment.

## Analytical Objectives

**1. Data Preparation & Validation**  
- Loaded and validated 300 monthly vessel records for 50 VLCCs.
- Confirmed no null values or duplicate rows.
- Checked that Idle_Days, Loaded_Days, and Ballast_Days sum correctly to the number of days in each month.
- Created calculated fields:
  - Total_Days = sum of activity days.
  - Utilisation (%) = Loaded Days as a percentage of Total Days.
  - Extracted Origin and Destination from Route.

**2. Descriptive Trends**  
- Generated descriptive statistics for numeric and categorical fields.
- Analysed fleet-level monthly utilisation trends (Jan–Jun 2025).
- Plotted Loaded, Idle, and Ballast days over time to check for seasonal variation.
- Explored utilisation by Region, Route, Origin, and Destination to spot consistent underperformance.

**3. Vessel-Level Outlier Detection**  
- Calculated fleet average utilisation (~75%).
- Defined underperformance threshold at 12.5% below the fleet mean (~65%).
- Identified 6 vessels consistently underperforming.
- Visualised vessel-level performance with reference lines for fleet average and threshold.
- Checked for consistent patterns by vessel and flagged for further investigation.

**4. Recommendations & Limitations**  
- Highlighted that the fleet is generally well-utilised with minimal seasonal fluctuation.
- Flagged North Sea, Caribbean, and West Africa routes as slightly below average — recommended further operational review.
- Proposed closer monitoring of the 6 low-performing vessels with daily tracking.
- Noted that root cause analysis requires additional data such as port logs, routing details, or maintenance records — not covered in this dataset.

## Deliverables

- **Cleaned Dataset:** Prepared CSV file with all calculated fields.
- **Python Analysis Notebook:** Includes data loading, QA checks, descriptive stats, grouped trends, visualisation, and outlier plots.
- **Visuals & Presentation:**  
  - Fleet-wide utilisation trend (line chart).  
  - Loaded/Idle/Ballast days by month (line chart).  
  - Region, Origin, and Destination comparisons (bar charts).  
  - Vessel-level scatter plot with underperformance thresholds.
- **Presentation Slides:** Final slides summarising:
  - Project objective and scope
  - Key trends and observations
  - Outlier vessels and route-level findings
  - Actionable recommendations and next steps


## Key Insights

- Fleet-wide utilisation remained stable at ~73–76% with no major seasonality detected.
- The North Sea region and US destinations averaged 1–3% lower utilisation than the fleet mean — worth investigating for possible routing or port-related delays.
- Six VLCCs consistently performed below the underperformance threshold (~65%) — recommended for operational review.
- Additional operational data such as port calls, bunkering delays, or maintenance logs would help confirm root causes and refine recommendations.

