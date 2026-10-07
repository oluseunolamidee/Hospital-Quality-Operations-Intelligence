# Hospital Intelligence System

## Healthcare Data Analytics, Quality & Patient Safety Intelligence

A synthetic Hospital Intelligence System (HIS) designed to demonstrate how healthcare data can be transformed into reliable analytical insights for clinical quality, patient safety, laboratory operations, pharmacy operations, financial performance, quality management, and clinical research.

The project follows a relational healthcare data workflow from raw data ingestion and quality auditing through PostgreSQL transformation and analytical reporting in Power BI.

---

## Project Overview

Healthcare organizations generate large volumes of data across clinical, laboratory, pharmacy, financial, quality, and operational systems.

However, raw healthcare data is not immediately suitable for decision-making. Data must first be checked for completeness, consistency, accuracy, and logical validity before it can be used for reporting and analysis.

This project simulates that process by building a synthetic hospital data environment and developing an analytical layer for hospital intelligence.

The workflow is:

**Raw Data → PostgreSQL Staging → Data Quality Audit → Data Cleaning & Transformation → Analytical Views → Power BI Dashboards → Healthcare Insights**

The project was designed around principles relevant to:

- Healthcare data analytics
- Clinical quality management
- Patient safety
- Laboratory quality
- Pharmacy operations
- Healthcare financial analysis
- Quality improvement
- Clinical research analytics

---

# Objectives

The main objectives of this project were to:

1. Build a relational hospital database using synthetic healthcare data.
2. Load raw datasets into a PostgreSQL staging environment.
3. Audit the datasets for data quality issues.
4. Identify temporal, referential, completeness, and consistency errors.
5. Clean and transform the data into an analytical healthcare data layer.
6. Develop SQL views for hospital-level KPIs.
7. Create Power BI dashboards for management and operational decision-making.
8. Demonstrate how healthcare data can support quality improvement and patient-safety monitoring.

---

# Technology Stack

| Technology | Purpose |
|---|---|
| **PostgreSQL** | Database management, data cleaning and transformation |
| **SQL** | Data validation, analysis, KPI development and analytical views |
| **Power BI** | Interactive dashboards and data visualization |
| **Excel / CSV** | Initial synthetic datasets and data ingestion |
| **GitHub** | Version control and project documentation |

---

## Hospital Domains
The system models several healthcare domains:
- Clinical
- Patients
- Admissions
- Diagnoses
- Procedures
- Vital signs
- Allergies
  
Laboratory
- Laboratory orders
- Laboratory results
- Result timing
- Post-discharge results
- Laboratory quality indicators
  
Pharmacy
- Prescriptions
- Dispensing
- Medication administration
- Prescription-to-dispensing turnaround time
  
Patient Safety
- Clinical incidents
- Corrective and Preventive Actions (CAPA)
- Incident-to-CAPA relationships
- CAPA timing
  
Quality Management
- Audits
- Quality standards
- Quality improvement projects
- Patient feedback
  
Clinical Research
- Clinical trials
- Trial enrolments
- Trial timing and eligibility checks
  
Hospital Operations
- Departments
- Staff
- Rooms
- Beds
- Bed assignments
  
Financial
- Bills
- Payments
- Insurance claims
- Payment status
- Financial reconciliation

## Data Quality & Validation
A major focus of this project was not simply analysing the data, but determining whether the data could be trusted before analysis.
The data-quality audit examined areas such as:
- Missing values
- Duplicate records
- Referential integrity
- Invalid dates
- Chronological inconsistencies
- Impossible event sequences
- Records occurring after discharge
- Invalid CAPA timing
- Invalid clinical-trial enrolment timing
- Payments occurring before billing
- Bed assignment chronology
  
## Data Quality Philosophy
An important principle of this project is:
A dashboard is only as reliable as the data behind it.

Instead of immediately building visualizations, the project prioritizes:
1. Data ingestion
2. Data profiling
3. Data-quality auditing
4. Error identification
5. Cleaning and transformation
6. Analytical validation
7. KPI development
8. Visualization
This approach mirrors the importance of data governance in healthcare environments where inaccurate data can lead to misleading operational or clinical conclusions.

## Project Workflow
1. Synthetic data generation
            
2. CSV / Excel data preparation
             
3. PostgreSQL staging
             
4. Data inventory and profiling
             
5. Data-quality audit
             
6. Cleaning and transformation
             
7. HIS analytical schema
             
8. SQL analytical views
             
9. KPI validation
             
10. Power BI dashboards
             
11. Healthcare insights

## Key Skills Demonstrated
Technical Skills
- SQL
- PostgreSQL
- Data cleaning
- Data validation
- Relational database design
- Data modelling
- KPI development
- Analytical views
- Power BI
- Dashboard development
- Data visualization
  
Healthcare Analytics Skills
- Clinical data analysis
- Patient safety analytics
- Laboratory quality analytics
- Pharmacy analytics
- Healthcare financial analytics
- Quality management
- Clinical research analytics
- Healthcare data-quality management
  
Analytical Skills
- Problem identification
- Data-quality investigation
- Root-cause thinking
- KPI design
- Data reconciliation
- Operational insight generation
- Decision-support reporting

## Raw Data
[Arian_Hospital_Final_Relational_HIS_Dataset_v2.xlsx](https://github.com/user-attachments/files/33157573/Arian_Hospital_Final_Relational_HIS_Dataset_v2.xlsx)


## Analyzed Data
[analytics.v_pharmacy_operations.csv](https://github.com/user-attachments/files/33157415/analytics.v_pharmacy_operations.csv)
[analytics.v_patient_experience.csv](https://github.com/user-attachments/files/33157410/analytics.v_patient_experience.csv)
[analytics.v_patient_admissions.csv](https://github.com/user-attachments/files/33157404/analytics.v_patient_admissions.csv)
[analytics.v_medication_administration.csv](https://github.com/user-attachments/files/33157402/analytics.v_medication_administration.csv)
[analytics.v_lab_orders_results.csv](https://github.com/user-attachments/files/33157398/analytics.v_lab_orders_results.csv)
[analytics.v_financial_transactions.csv](https://github.com/user-attachments/files/33157393/analytics.v_financial_transactions.csv)
[analytics.v_clinical_trials.csv](https://github.com/user-attachments/files/33157389/analytics.v_clinical_trials.csv)
[analytics.pbi_kpis.csv](https://github.com/user-attachments/files/33157385/analytics.pbi_kpis.csv)
[SQL Analysis.sql](https://github.com/user-attachments/files/33157600/SQL.Analysis.sql)

## Dashboard
<img width="958" height="538" alt="Quality Management" src="https://github.com/user-attachments/assets/143e9753-774b-41f9-88b9-d974c244358c" />
<img width="959" height="543" alt="Pharmacy Operations" src="https://github.com/user-attachments/assets/0bffc49e-e7fc-4c5f-952a-d4974c4af965" />
<img width="957" height="542" alt="Laboratory Quality dashboard" src="https://github.com/user-attachments/assets/13b98102-625f-411d-9d6c-fce2d81545ee" />
<img width="964" height="541" alt="Executive dashboard" src="https://github.com/user-attachments/assets/a61c89bf-c04b-447e-a6ec-35a5e79250c8" />
<img width="958" height="541" alt="Clinical Trials" src="https://github.com/user-attachments/assets/01ee90e8-8ba4-4f9e-90cd-afbaab152007" />
<img width="959" height="542" alt="Clinical Safety" src="https://github.com/user-attachments/assets/d6b1be84-992b-4a35-bf4b-4fc58a37c992" />
[Power BI.pdf](https://github.com/user-attachments/files/33157981/Power.BI.pdf)


  
# Data Architecture

The project uses a layered approach to separate raw data from validated analytical data.

```text
                 RAW DATA
                    │
                    ▼
          ┌───────────────────┐
          │ PostgreSQL        │
          │ STAGING           │
          └─────────┬─────────┘
                    │
                    ▼
          DATA QUALITY AUDIT
                    │
                    ▼
          CLEANING & TRANSFORMATION
                    │
                    ▼
          ┌───────────────────┐
          │ PostgreSQL        │
          │ HIS SCHEMA        │
          └─────────┬─────────┘
                    │
                    ▼
          ANALYTICAL SQL VIEWS
                    │
                    ▼
          ┌───────────────────┐
          │     POWER BI      │
          │    DASHBOARDS     │
          └───────────────────┘
                    │
                    ▼
          HOSPITAL INSIGHTS

Important Disclaimer
This project uses synthetic data created for educational and portfolio purposes.
It does not contain real patient information, protected health information (PHI), or confidential hospital records.
The hospital name and records are fictional and are intended only to demonstrate healthcare analytics, database management, data-quality practices, and business intelligence techniques.

Author
Olamide Oluseun
BSc Microbiology | Healthcare Data Analytics | SQL | PostgreSQL | Power BI
This project represents my transition from a life-science background into healthcare data analytics, with a focus on transforming complex healthcare data into reliable information for decision-making.
