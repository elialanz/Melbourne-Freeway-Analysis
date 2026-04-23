# Victorian Traffic Volume, Speed & Vehicle Mix Monitoring Dashboard

## Project Overview

This project is an end-to-end Power BI case study built to analyse and monitor road traffic activity across Victorian TIRTL monitoring sites using transport operations data from the Victorian open data ecosystem.

The project focuses on transforming raw traffic count and site reference data into a structured reporting dataset suitable for operational monitoring, trend analysis, and stakeholder-facing dashboarding. The final output is designed as a professional reporting product that supports analysis of traffic volume, speed distribution, vehicle mix, site-level variation, and directional traffic patterns.

Rather than approaching the data as a simple visualisation exercise, this project is framed as a transport reporting and performance-monitoring use case, with emphasis on data preparation, validation, reporting logic, KPI design, and clear communication of findings.

---

## Business Scenario

A transport operations or network performance team needs a reporting solution to monitor traffic behaviour across selected Victorian road monitoring sites over a recent two-week period.

The team requires a dashboard that can help identify:
- the busiest monitoring locations
- peak traffic periods
- directional traffic differences
- vehicle class composition
- speed band patterns
- traffic behaviour differences between weekdays and weekends

The purpose of the dashboard is to support operational review, site comparison, and evidence-based discussion around traffic movement patterns across the monitored network.

---

## Business Problem

Raw TIRTL traffic count files are highly granular and split across multiple daily extracts. On their own, they are not immediately suitable for management reporting or business analysis.

To make the data useful, the project needs to:
- combine multiple daily files into a consistent reporting dataset
- validate data structure and key fields
- enrich the traffic data with site reference information
- create analysis-ready tables for reporting
- define business-friendly KPIs and reporting logic
- present the results in a clean, stakeholder-oriented Power BI dashboard

---

## Project Objectives

The objectives of this project are to:

1. Build a clean and trusted traffic monitoring dataset from raw TIRTL data files  
2. Stage and prepare the data using SQL Server before modelling in Power BI  
3. Analyse recent traffic behaviour across Victorian monitoring sites over a controlled two-week reporting window  
4. Create a professional dashboard for traffic volume, speed, and vehicle mix reporting  
5. Generate practical insights and recommendations in a format suitable for portfolio presentation and stakeholder-style communication  

---

## Dataset Summary

This project uses:

- **TIRTL Traffic Counts and Classification** daily CSV files
- **TIRTL Sites** reference file

### Traffic count fields used
- `date`
- `time_bin`
- `site`
- `heading`
- `vehicle_class`
- `speed_bin`
- `volume`

### Site reference fields used
- `site`
- `site_description`
- `latitude`
- `longitude`

### Reporting period
This project uses a controlled reporting window covering:

**16 March 2026 to 29 March 2026**

This two-week Monday-to-Sunday scope was selected to provide enough data for:
- weekday vs weekend comparison
- intraday traffic pattern analysis
- site-level comparison
- directional analysis
- vehicle mix analysis
- speed distribution analysis

while keeping the dataset manageable for staging, validation, and reporting.

---

## Tools Used

- **SQL Server / SSMS** — raw staging, cleaning, validation, and reporting table preparation  
- **Power BI** — data modelling, DAX measures, dashboard development, and final reporting  
- **Excel / Markdown documentation** — data dictionary, checks, notes, and project documentation  
- **GitHub** — project versioning and portfolio presentation  

---

## Project Structure

```text
[01] Project Brief & Planning
[02] Data
[03] SQL Scripts
[04] Analysis & Visualizations
[05] Final Deliverables
