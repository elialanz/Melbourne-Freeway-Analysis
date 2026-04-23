# Phase 2 Data Strategy

## Purpose
This document defines the Phase 2 data strategy for the Melbourne Freeway Traffic Analysis project.

The focus of this phase is to establish a reliable SQL-based data foundation for later reporting and dashboard development. This includes ingesting selected raw TIRTL traffic count files, validating their structure, and preparing a cleaned reporting-ready dataset for Power BI.

## Phase 2 Scope
Phase 2 is limited to raw ingestion, data structure validation, staging, cleaning, and preparation of a reporting-ready traffic dataset.

This phase does not include dashboard development, advanced analysis, forecasting, or external data enrichment beyond the supplied site reference file.

## Reporting Window
Selected reporting window:

**2026-03-16 to 2026-03-29**

This period represents two full weeks (Monday to Sunday coverage) and was selected to keep the project manageable while still supporting realistic traffic pattern analysis.

## Included Source Files
The following source files are included in Phase 2:

- TIRTL daily traffic count CSV files for 2026-03-16 to 2026-03-29
- TIRTL sites CSV file

## Excluded for This Phase
The following data sources or additions are intentionally excluded at this stage:

- incident data
- weather data
- live traffic feeds
- full-month ingestion
- external road or location enrichment beyond the provided site file

## Why SQL Staging Comes Before Power BI
SQL staging is completed before Power BI development to ensure:

- raw files are ingested and preserved consistently
- data types and structures are validated before reporting
- cleaning and transformation logic is documented and reusable
- Power BI connects to a controlled reporting layer rather than inconsistent raw files
- data quality issues are identified earlier in the workflow

This approach better reflects a professional analytics pipeline and supports maintainability.

## Expected Phase 2 Outputs
The expected outputs of this phase are:

- raw staging tables
- cleaned staging table or view
- reporting-ready table or view for Power BI

## Key Phase 2 Deliverable Goal
At the end of Phase 2, the project should have a validated and documented SQL data layer that supports Phase 3 reporting and dashboard design.
