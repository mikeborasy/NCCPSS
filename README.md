# NCCPSS Database Design

## Project Overview
This project focuses on designing a centralized database system for the North Carolina Certified Peer Support Specialist (NCCPSS) program. The goal is to unify fragmented data sources and enable better reporting, tracking, and decision-making.

---

## Problem Statement
NCCPSS data is currently stored across multiple systems such as Access and Drupal. This creates data silos, making it difficult to track individuals over time, ensure data quality, and generate reliable reports.

---

## Solution / Approach
Our team built a structured data pipeline using a medallion architecture:

- **Silver Layer:** Cleaned and standardized data  
- **Identity Layer:** Matched individuals across systems using tiered logic  
- **Gold Layer:** Structured tables for reporting and analysis  
- **Dashboards:** Built in Power BI for stakeholder insights  

---

## Data Sources
- NCCPSS Registry (Access Database)  
- Drupal Application & Recertification Data  

---

## Technology Stack
- Microsoft Fabric  
- PySpark  
- Power BI  

---

## Team Members
- Taylor Baldwin  
- Claudia Dare  
- Michael Borasy  
- Usman Siddiqui  

---

## Project Outcome
- Centralized and structured database  
- Data pipeline for cleaning and integration  
- Identity layer for tracking individuals  
- Dashboards for reporting and insights  
