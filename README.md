# Customer Churn Analysis Dashboard

A comprehensive Tableau dashboard for analyzing customer churn patterns and identifying key factors that influence customer retention in the banking sector.

## Overview

This project presents an interactive visualization dashboard built in Tableau that analyzes customer churn behavior across multiple dimensions including demographics, account characteristics, and engagement metrics. The dashboard helps identify at-risk customer segments and provides actionable insights for retention strategies.

## Dataset

**Source:** Customer Churn Prediction Dataset
**Size:** 10,000 customer records
**Features:**
- Customer demographics (Age, Gender, Geography)
- Account information (Credit Score, Balance, Tenure)
- Product usage (Number of Products, Has Credit Card, Active Member status)
- Financial data (Estimated Salary)
- Churn indicator (Exited: 0 = Retained, 1 = Churned)

## Key Metrics

- **Total Customers:** 10,000
- **Churned Customers:** 2,037
- **Overall Churn Rate:** 20.37%

## Dashboard Components

### 1. Geographic Analysis
- **Churn by Geography:** Identifies regional churn patterns
- Highest churn: Germany (32.44%)
- Medium churn: Spain (16.67%)
- Lowest churn: France (16.15%)

### 2. Demographic Analysis
- **Churn by Gender:**
  - Female customers: 25.07% churn rate
  - Male customers: 16.46% churn rate
- **Churn by Age Group:**
  - Highest risk: 46-55 and 56-65 age groups (>50% churn rate)
  - Lowest risk: 18-25 age group (7.53% churn rate)

### 3. Product & Engagement Analysis
- **Churn by Number of Products:**
  - 3-4 products: 100% and 82.71% churn rates (high risk)
  - 2 products: 27.71% churn rate
  - 1 product: 7.58% churn rate
- **Active vs Inactive Members:**
  - Inactive members: 26.85% churn rate
  - Active members: 14.27% churn rate

### 4. Financial Analysis
- **Credit Score Distribution:** Shows churn patterns across credit score ranges (350-850)
- **Balance Analysis:** Examines churn rates across different balance groups
  - Low balance (1-50k): 34.67% churn rate
  - High balance (100-150k): 25.77% churn rate
  - No balance: 13.82% churn rate
- **Tenure Analysis:** Line chart showing churn rate fluctuations over customer tenure (0-10 years)

### 5. KPI Cards
- Total Customers
- Churned Customers
- Overall Churn Rate

## Key Insights

1. **Geographic Risk:** German customers are twice as likely to churn compared to other regions
2. **Gender Disparity:** Female customers show significantly higher churn rates than males
3. **Age Factor:** Middle-aged customers (46-65) are at highest risk of churning
4. **Product Paradox:** Customers with 3-4 products have extremely high churn rates
5. **Engagement Matters:** Inactive members have nearly 2x higher churn rate than active members
6. **Balance Impact:** Customers with low balances (1-50k) show highest churn tendency

## Calculated Fields

- **Churn Rate:** `SUM([Exited])/COUNT([CustomerId])`
- **Age Group:** Bins customers into segments (18-25, 26-35, 36-45, 46-55, 56-65, 66+)
- **Churn Status:** Categorical field ("Churned" or "Retained")
- **Balance Group:** Categorizes account balances (No Balance, Low, Medium, High, Very High)
- **Active Status:** Binary field ("Active" or "Inactive")

## Files

- `Churn Analysis.twbx` - Tableau packaged workbook containing all visualizations and data

## How to Use

1. **Download** the `Churn Analysis.twbx` file
2. **Open** with Tableau Desktop (2025.2 or later recommended)
3. **Explore** the interactive dashboard with filters for Geography and Age Group
4. **Click** on any visualization element to cross-filter other charts
5. **Export** insights or create custom views as needed

## Technical Details

- **Tool:** Tableau Desktop Public Edition 2025.2
- **Data Connection:** CSV file (Customer Churn Prediction Dataset.csv)
- **Extract:** Hyper extract for optimized performance
- **Visualizations:** 11 worksheets, 1 interactive dashboard

## Recommendations

Based on the analysis, the following strategies are recommended:

1. **Target German Market:** Investigate why German customers churn at higher rates and implement region-specific retention programs
2. **Female Customer Focus:** Develop retention initiatives specifically addressing female customer needs
3. **Age-Appropriate Strategies:** Create targeted campaigns for 46-65 age group with personalized offers
4. **Product Portfolio Review:** Investigate why multi-product customers churn more frequently
5. **Engagement Programs:** Implement re-engagement campaigns for inactive members
6. **Balance Monitoring:** Identify customers with declining balances for proactive outreach

## Future Enhancements

- Predictive modeling integration for churn probability scoring
- Time-series analysis for trend identification
- Cohort analysis for customer lifecycle understanding
- Cost-benefit analysis of retention strategies
- Real-time dashboard updates with live data connection

## Author

Created by Kristina Angelina

## License

This project is available for educational and analytical purposes.

---

**Note:** This dashboard is part of a data analytics portfolio demonstrating skills in business intelligence, data visualization, and customer analytics.
