# Hospital-Administration-System

## Overview

This project examines hospital administrative data to uncover trends and key factors linked to elevated readmission rates. In my role as a data analyst focused on enhancing patient care quality, the study tackles the pressing issue of minimizing avoidable hospital readmissions—thereby supporting more efficient use of healthcare resources and ensuring adherence to regulatory standards.

---

## Dataset

This project utilizes a comprehensive hospital administration dataset designed to explore the drivers of patient readmission. The data, available for download from [Kaggle: Hospital Admission Data](https://www.kaggle.com/datasets/shivavashishtha/hospital-admission-data), captures detailed information on patient encounters and clinical workflows. Each record is uniquely identified by `patient_id` and `encounter_id`, ensuring traceability across visits. Demographic variables such as `race`, `gender`, `age`, and `weight` (the latter noted for substantial missingness) provide patient context. Clinical and administrative details include length of stay (`time_in_hospital`), admitting `medical_specialty`, and treatment intensity metrics like `num_lab_procedures`, `num_procedures`, and `num_medications`. The dataset also tracks prior healthcare utilization through counts of outpatient, emergency, and inpatient visits over the past year. Diagnostic information is represented via up to five diagnosis codes (`diag_1` to `diag_5`) and a total `number_diagnoses`. Additionally, 25 anonymized columns (`X1`–`X25`) indicate prescribed medications, supplemented by flags for diabetic medication changes (`change`) and whether diabetes-related drugs were administered (`diabetesMed`). The primary outcome variable, `readmitted`, denotes whether a patient was readmitted within 30 days of discharge. Together, these features enable a multidimensional analysis of clinical, operational, and demographic predictors of hospital readmissions.

---

## Analysis Outcome

- This study was designed to uncover the primary drivers and recurring patterns behind 30-day patient readmissions, examining influences across demographic, clinical, and operational dimensions.

- **Demographic Insights:** Assessed how variables such as **age, gender, and race** correlate with readmission likelihood, helping identify potential inequities in health outcomes or care delivery.

- **Clinical & Treatment Indicators:** Investigated whether factors like **hospital stay duration**, **admitting specialty**, **volume of lab tests performed**, and **number of prescribed medications** significantly influence readmission risk.

- **Diabetes-Specific Analysis:** Focused on diabetic patients to evaluate how **adjustments in medication regimens** and the use of specific diabetes-related drugs (represented by anonymized fields `X1–X25`) impact readmission rates.

- **Utilization History & Complexity:** Examined whether prior healthcare engagement—such as **outpatient, emergency, or inpatient visits**—and the presence of **multiple concurrent diagnoses** increase the probability of return admissions.

- **Operational & Temporal Patterns:** Analyzed trends in readmission frequency over **time periods (monthly or seasonal)** and evaluated variations linked to **discharge status categories**, where data permitted.

- **Data Integrity & Deep Dives:** Tackled challenges like the prevalence of **missing weight records** and conducted advanced explorations—including **medication prescribing trends by specialty** and interactions between **weight groups and primary diagnoses**.

These findings offer actionable intelligence for designing precision interventions, optimizing staffing and resource deployment, and refining clinical pathways—all aimed at minimizing preventable readmissions and enhancing overall patient care quality.


---


## Dashobard

**⚠️ IMPORTANT: To use this dashboard, open the file `Solution.xlsx` and navigate to the “Dashboard” sheet. All interactive elements function only within this tab.**

- This dashboard delivers a comprehensive view of 30-day hospital readmission trends across key clinical, demographic, and operational dimensions.
- Highlights include a **total patient count of 48,911**, an overall **readmission rate of 46.22%**, and an **average readmission age of 65**, with patients staying **4.4 days** on average.
- Visuals break down readmissions by **medical specialty**, revealing higher rates in Internal Medicine and Surgery-General, while specialties like Cardiology and Nephrology show moderate risk.
- A line chart illustrates how **readmission likelihood increases with the number of medications prescribed**, indicating polypharmacy as a potential risk factor.
- Demographic insights compare **readmission by gender** (slightly higher among females) and **by race**, showing African American patients account for 76% of readmissions, followed by Caucasian (19%) and others.
- The **number of diagnoses** chart reveals that patients with 10+ comorbidities face significantly elevated readmission risk.
- Designed for hospital administrators and clinical leaders to identify high-risk cohorts, allocate resources strategically, and develop targeted care improvement initiatives.


![HA](Hospital.PNG)

## Author & Contact
- Name: `Kshitij Saini`
- / [LinkedIn]([https://www.linkedin.com/in/pratyushpuri](https://www.linkedin.com/in/kshitij-saini-b950b7299?utm_source=share_via&utm_content=profile&utm_medium=member_android))
