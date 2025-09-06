# vpd_crime_analysis
Vancouver Crime Trends & Hotspots Dashboard
Overview

This project analyzes publicly available crime data from the Vancouver Police Department to uncover patterns, hotspots, and trends that can support resource allocation and public safety initiatives. The goal is to transform raw open data into actionable insights through data cleaning, analysis, and visualization.

Data Source

Vancouver Police Department Open Data Portal (Crime data, 2020-2025).

Dataset is anonymized and spatially adjusted to protect privacy.

Methodology

Data Cleaning: Removed duplicates, standardized formats, and derived fields (year, month, weekday, hour).

SQL Analysis: Wrote queries to calculate monthly crime counts, top neighbourhoods, crime types by year, and peak days/hours.

NoSQL Analysis (Optional): Used MongoDB pipelines for grouping by neighbourhood and crime type.

Python Visualization: Created line charts for monthly trends, bar charts for neighbourhood rankings, and heatmaps for time patterns.

Power BI Dashboard: Built an interactive dashboard with three pages – Overview, Geography, and Time Patterns.

Key Insights

Downtown, West End, and Mount Pleasant consistently rank as top neighbourhoods by crime volume.

Theft-related incidents (e.g., theft from vehicle) make up a significant share, with peaks during weekends.

Crimes peak in summer months, suggesting seasonal patterns.

Time analysis reveals late evenings and weekends as critical hours for certain crime types.

Deliverables

Cleaned dataset (crime_clean.csv).

SQL queries (analysis.sql) and MongoDB pipelines.

Python notebook (trend_analysis.ipynb).

Power BI dashboard (vpd_crime_dashboard.pbix).

Tools

SQL, MongoDB, Python (pandas, matplotlib, seaborn).

Power BI for interactive visualization.

Next Steps

Future improvements could include integrating weather or 911 call data, predictive modeling, and real-time dashboard updates.
