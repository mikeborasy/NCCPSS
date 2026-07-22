# NCCPSS Database Design

## Overview

This project designs a centralized analytics platform for the North Carolina Certified Peer Support Specialist (NCCPSS) program by integrating fragmented data sources into a scalable Microsoft Fabric architecture.

The solution enables reliable reporting, longitudinal tracking of individuals, and improved decision-making through standardized data engineering pipelines and Power BI dashboards.

---

## Problem Statement

NCCPSS program data was distributed across multiple systems, including Microsoft Access and Drupal.

This created several challenges:

- Data silos
- Duplicate records
- Inconsistent schemas
- Limited longitudinal tracking
- Difficult reporting
- Poor data quality

These limitations prevented stakeholders from efficiently monitoring certification activity and program outcomes.

---

## Technology Stack

- Microsoft Fabric
- PySpark
- Power BI
- SQL

---

## Data Sources

The project integrates multiple operational systems, including:

- NCCPSS Registry (Microsoft Access)
- Drupal Application Data
- Drupal Recertification Data

---

## Solution Architecture

The project implements a Medallion Architecture consisting of:

### Bronze Layer

- Raw source ingestion
- Data preservation
- Schema capture

### Silver Layer

- Data cleaning
- Standardization
- Schema normalization
- Quality validation

### Identity Layer

Designed a tiered identity resolution framework to reconcile individuals across multiple source systems despite inconsistent identifiers.

This enabled accurate longitudinal tracking throughout each participant's certification lifecycle.

### Gold Layer

Built analytics-ready tables optimized for reporting and dashboard development.

---

## Data Engineering Work

Major engineering tasks included:

- Standardizing inconsistent schemas across systems
- Resolving time-varying field overwrites
- Normalizing person-level and event-level records
- Designing scalable transformation pipelines
- Improving overall data quality
- Creating reusable reporting datasets

---

## Reporting & Analytics

Built Power BI dashboards to provide stakeholders with:

- Certification tracking
- Program participation metrics
- Individual lifecycle reporting
- Operational insights

---

## Project Outcome

The completed solution provided:

- Centralized database architecture
- Improved data quality
- Reliable identity resolution
- Scalable ETL pipelines
- Analytics-ready reporting tables
- Improved decision support through Power BI

---

## Repository Structure

```
NCCPSS/
│
├── notebooks/
├── pipelines/
├── data/
├── dashboards/
├── README.md
```

---

## Key Takeaways

This project demonstrates experience with:

- Data engineering
- ETL pipeline development
- Microsoft Fabric
- PySpark
- Identity resolution
- Data modeling
- Medallion architecture
- Power BI
- Data integration
