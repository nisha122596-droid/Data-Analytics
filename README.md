# Patient Healthcare Revenue Cycle Analysis

## Project Overview

This repository contains a **Healthcare Revenue Cycle Analysis project** that focuses on transforming raw healthcare data into meaningful business insights using **Excel and Power BI**.

The project demonstrates how data cleaning, transformation, data modeling, and visualization can be used to analyze healthcare operations and financial performance. The final outcome is an interactive Power BI dashboard designed to support decision-making related to revenue cycle management.

---

## Objective

The main objective of this project is to:

* Clean and preprocess healthcare data using **Excel / Power Query**
* Perform **data modeling and DAX calculations** in Power BI
* Build **interactive dashboards** to analyze operational and financial performance
* Identify **revenue leakage, provider workload distribution, and payer performance**

---

## Dataset

**Source:**
Healthcare dataset generated from practice data resources.

**Domain:**
Patient Healthcare Revenue Cycle

**Time Period:**
January 2024 – January 2025

The dataset includes patient encounters, insurance providers, billing information, and provider specialties.

---

## Key Problem Areas Analyzed

### 1. Revenue Leakage & Claim Performance

* Compare **Amount Billed vs Amount Paid**
* Identify reimbursement gaps across insurance providers

### 2. Patient Encounter Patterns

* Analyze how frequently patients visit
* Identify which **encounter types and specialties receive the most visits**

### 3. Provider Performance

* Evaluate **provider distribution by specialty**
* Identify **overloaded or underutilized specialties**

### 4. Operational vs Financial Performance

* Compare patient encounter volume with financial metrics such as charge amount and payments received.

---

## Tools & Technologies

| Tool        | Purpose                                             |
| ----------- | --------------------------------------------------- |
| Excel       | Data cleaning, transformation, pivot tables         |
| Power Query | Data preprocessing and shaping                      |
| Power BI    | Data modeling, DAX measures, and dashboard creation |
| DAX         | Calculated measures and analytical metrics          |

---

## Data Pre-Processing

Data preparation was performed using **Excel and Power Query**.

Steps included:

* Removing duplicate records
* Handling missing values
* Standardizing data formats
* Creating calculated columns
* Sorting and filtering relevant records
* Using **Pivot Tables** for initial data summarization

---

## Data Modeling (Power BI)

Data relationships were established between tables to support analysis.

Example DAX measures used:

```
Total_Paid = SUM('Insurance Claims'[AmountPaid])

Min_PaidAmount = MIN('Insurance Claims'[AmountPaid])

Max_PaidAmount = MAX('Insurance Claims'[AmountPaid])

Total_Insurance_Providers = COUNTROWS('Insurance Claims')

Avg_ChargeAmount = AVERAGE(Charges[ChargeAmount])
```

These measures support the dashboard's financial and operational insights.

---

## Dashboard Visualizations

The Power BI dashboard includes several visualizations to analyze healthcare revenue cycle performance.

### 1. Amount Billed vs Amount Paid by Insurance Provider

A clustered column chart comparing billed and paid amounts to identify **revenue gaps** across insurers.

### 2. Revenue Contribution by Insurance Provider

A donut chart highlighting which insurance providers contribute the most revenue.

### 3. Providers by Specialty

A pie chart showing **distribution of healthcare providers across specialties**.

### 4. CPT Code Analysis

A line chart analyzing **charge amounts and insurance provider counts by CPT codes**.

### 5. Encounter Volume by Specialty

An area chart showing **patient encounter distribution across specialties**.

---

## Key Insights

### Revenue & Insurance Performance

* Medicare and Aetna generate the largest share of billed revenue.
* A noticeable gap exists between billed and paid amounts.
* Revenue is concentrated among a small number of insurance providers.

### CPT Code Revenue Distribution

* A small number of CPT codes account for a significant portion of total charges.
* High-volume procedures drive most of the revenue.

### Provider Distribution

* General Practice has the highest number of providers.
* Cardiology and Dermatology have relatively fewer providers.

### Encounter Volume

* Neurology records the highest number of patient encounters.
* Cardiology shows comparatively lower encounter volume.

---

## Business Implications

The analysis reveals several important operational and financial patterns:

* Revenue is dependent on a limited number of insurers.
* Payment gaps between billed and received amounts indicate possible reimbursement adjustments.
* Certain specialties handle a significantly higher patient workload.
* Some specialties may be underutilized compared to their provider capacity.

---

## Conclusion

The healthcare revenue cycle analysis highlights key patterns in **insurance reimbursement, provider workload, and service demand**. The findings indicate that revenue performance is influenced by both payer mix and high-volume medical procedures.

By leveraging data analytics through Excel and Power BI, healthcare organizations can better understand operational efficiency, identify revenue leakage, and make informed decisions to improve financial and clinical performance.

---


## Future Improvements

Possible enhancements for future analysis:

* Calculate **collection rate (Paid vs Billed %)**
* Track **revenue per provider**
* Analyze **revenue per encounter**
* Add **time-based trend analysis**
* Include **claim denial analysis**

---

## Author

Healthcare Revenue Cycle Analysis Project
