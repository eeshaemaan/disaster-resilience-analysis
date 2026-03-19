# Resilience Under Pressure: Global Disaster Risk & Recovery Analytics

## Project Overview

This project develops a comprehensive data-driven analytical framework to measure and visualize global disaster resilience. By integrating multi-source datasets across disaster events, socio-economic indicators, and climate risk factors, the system quantifies how nations **prepare for, absorb, and recover from disasters**.

The project was conducted as part of the Data Analysis & Visualization course at FAST-NUCES and implements custom computational indices alongside an interactive Tableau dashboard to support policy-driven insights.

---

## Team Members

* **Eesha Emaan**
* **Ayesha Amer**

 Detailed contributions are listed in `authors.txt`

---

## Problem Statement

Disaster resilience is a **multi-dimensional concept that cannot be directly measured**. Existing global tools fail to integrate disaster exposure, socio-economic vulnerability, and recovery capacity into a unified analytical system.

This project addresses:

* Fragmented global datasets
* Lack of standardized resilience metrics
* Limited tools for cross-country comparison and recovery analysis

---

## Objectives

* Integrate multi-domain datasets (disaster, economic, climate, development)
* Engineer meaningful indicators for exposure, vulnerability, and capacity
* Develop computational indices:

  * Disaster Impact Index (DII)
  * Resilience Recovery Score (RRS)
  * Composite Resilience Index (CRI)
* Build an interactive Tableau dashboard for global comparative analysis

---

## Data Sources

This project integrates four major global datasets:

* **EM-DAT** – Disaster occurrence and impact data
* **World Bank** – Economic and governance indicators
* **UNDP (HDI)** – Human development metrics
* **CPRI (Climate Risk Data)** – Environmental and climate exposure indicators

---

## Methodology

### Data Preprocessing

* Missing value handling using median imputation, interpolation, and forward/backward filling
* Country name standardization for dataset merging
* Outlier detection using IQR capping
* Data normalization and scaling (MinMax, log transformations)

### Feature Engineering

Derived key attributes including:

* Mortality Rate
* Affected Population Percentage
* Annualized Disaster Frequency
* Exposure (frequency × severity)
* Climate Exposure Index
* Infrastructure Exposure
* Loss Normalized by GDP per capita

---

##  Computational Models

###  Disaster Impact Index (DII)

Measures disaster severity relative to economic capacity and population:

* Combines fatalities, affected population, GDP per capita, and severity

###  Resilience Recovery Score (RRS)

Captures recovery capability using:

* GDP growth changes
* Human Development Index (HDI)
* Governance Effectiveness

###  Composite Resilience Index (CRI)

Final resilience metric:

* CRI = Adaptive Capacity / (Exposure × Vulnerability)

Higher CRI indicates stronger resilience.

---

##  Tableau Dashboard

The interactive dashboard enables:

*  **Geographical Analysis** → Choropleth maps of CRI, RRS, DII
*  **Comparative Analysis** → Scatter plots (GDP vs CRI, Governance vs CRI)
*  **Temporal Trends** → Time-series by HDI groups
*  **Risk Classification** → Exposure vs Vulnerability quadrants
*  **Filters** → Year, Region, Disaster Type, HDI category

---

##  Project Structure

* `/dashboard` → Tableau dashboard (.twbx)
* `/data_and_report` → final merged dataset and IEEE formatted report
* `/images` → dashboard previews
* `authors.txt` → contribution details

---

##  Key Insights

* **Governance is a stronger predictor of resilience than economic wealth**
* Some countries maintain **low vulnerability despite high exposure**
* **Low-HDI nations face a widening resilience gap** due to rising climate risks
* Effective policy must be evaluated against **actual disaster impact (DII)**

---

##  Limitations

* Data inconsistencies across countries (reporting bias)
* Subjectivity in index weighting
* Correlation-based analysis (limited causal inference)
* Country-level aggregation limits localized insights

---

##  Future Work

* Integration of climate projections and predictive modeling
* Machine learning-based resilience forecasting
* Real-time disaster response analytics (satellite + social data)
* Sector-specific recovery modeling

---

##  How to Use

1. Download the Tableau `.twbx` file
2. Open in Tableau Desktop / Tableau Public
3. Use filters to explore resilience across time, regions, and disaster types

---

##  References

* EM-DAT Disaster Database
* World Bank Open Data
* UNDP Human Development Reports
* Climate Physical Risk Index (CPRI)

---

Data Analysis & Visualization
Demonstrates data fusion, feature engineering, and analytical storytelling
