# Real Estate Data Cleaning Project

## 📌 Project Overview
This project simulates a real‑world task: cleaning a messy property listing database for a boutique real estate firm. The original CSV contained duplicates, inconsistent formatting, missing values, and mixed date/price formats. Using Python (pandas), I performed data cleaning and generated summary statistics and visualizations.

## 🛠️ Skills Demonstrated
- Data cleaning (duplicates, missing values, standardization)
- Python (pandas, matplotlib)
- Data analysis (summary statistics, grouping)
- Data visualization (bar charts, pie charts, histograms)
- Exporting clean data and reporting

## 📂 Files Included
- `messy_properties.csv` – original raw data with issues
- `cleaned_properties.csv` – final clean dataset
- `summary_report.txt` – text summary of cleaning steps and statistics
- `properties_by_city.png` – bar chart of property counts by city
- `status_pie.png` – pie chart of property status breakdown
- `price_distribution.png` – histogram of property prices

## 🔍 Cleaning Steps
1. Removed exact duplicates based on address and MLS.
2. Standardized all dates to YYYY-MM-DD format.
3. Cleaned price column: removed $ and commas, converted "M" suffixes to millions, converted to numeric.
4. Set all states to "CO" (all properties in Colorado).
5. Standardized status to Active/Sold/Pending/Unknown.
6. Identified and counted missing values (address, price, MLS).

## 📊 Key Results
- Total properties after cleaning: (you can fill this in later)
- Duplicates removed: (fill in)
- Price range: (fill in)
- Missing address or price: (fill in)

## 💼 Relevance to Data Entry Analyst Roles
This project demonstrates the ability to:
- Take messy real‑world data and transform it into a clean, usable format.
- Document the cleaning process and report on data quality.
- Create simple visualizations to communicate insights.
- Deliver final outputs (CSV, charts, summary) that meet client needs.
