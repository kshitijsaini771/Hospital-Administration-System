# Hospital Readmission Risk Analytics

## Problem Statement
Unplanned 30-day readmissions strain hospital resources, increase costs, and signal gaps in care quality. This project analyzes hospital administration data to **identify key drivers of elevated readmission rates** and surface **actionable insights** that help clinical and administrative teams minimize avoidable readmissions while maintaining regulatory compliance.

---

## Analysis Done
- Explored a rich **hospital admission dataset** containing demographics, diagnoses, procedures, medications, utilization history, and readmission outcomes (`readmitted` within 30 days).
- Profiled patients using:
  - Demographics: **age, gender, race, weight** (with careful handling of missingness).
  - Clinical intensity: **time_in_hospital, num_lab_procedures, num_procedures, num_medications, number_diagnoses**.
  - Utilization history: counts of prior **outpatient, emergency, and inpatient visits**.
- Investigated:
  - How **age, gender, and race** correlate with readmission risk.
  - The impact of **length of stay, medical_specialty, and treatment intensity** on likelihood of return.
  - The relationship between **polypharmacy** (high number of medications) and readmission.
- Conducted **diabetes-focused analysis**:
  - Evaluated changes in diabetic medication (`change`) and use of diabetes drugs (`diabetesMed`, `X1–X25`) and their link to readmissions.
- Addressed data-quality issues:
  - Managed **missing weight** and other incomplete fields.
  - Performed deep dives into **medication patterns by specialty** and interactions between **weight bands, diagnoses, and readmission**.
- Synthesized patterns across demographic, clinical, and operational dimensions to support **targeted interventions** and **risk stratification**.

---

## Dashboard Overview
> To use the dashboard, open `Solution.xlsx` and go to the **“Dashboard”** sheet. All interactivity is available on this tab.

The Excel dashboard summarizes 30-day readmission performance and key risk factors:

- **Headline metrics:**
  - Total patients: **48,911**
  - Overall readmission rate: **46.22%**
  - Average readmission age: **65 years**
  - Average length of stay: **4.4 days**
- **Specialty-level insights:**
  - Readmissions broken down by **medical_specialty**, with higher risk in **Internal Medicine** and **Surgery-General**, and moderate rates in **Cardiology** and **Nephrology**.
- **Treatment intensity:**
  - A line chart shows **readmission probability increasing with number of medications**, highlighting polypharmacy as a potential focus area.
- **Demographic patterns:**
  - Readmission split by **gender** (slightly higher among females).
  - Readmission by **race**, with African American patients forming the largest share, followed by Caucasian and other groups.
- **Clinical complexity:**
  - A chart on **number of diagnoses** shows significantly higher readmission risk for patients with **10+ comorbidities**.
- Built for **hospital administrators, quality teams, and clinical leaders** to spot high-risk cohorts, prioritize resources, and design targeted care pathways.

![Hospital Readmission Dashboard](Hospital.PNG)

---

## Recommendations
- **Deploy targeted care plans for high-risk groups:** Focus on older patients, those with **10+ diagnoses**, and specialties with elevated readmission rates (e.g., Internal Medicine, Surgery-General).
- **Manage polypharmacy proactively:** Implement medication reconciliation, pharmacist reviews, and deprescribing strategies for patients on a high number of medications.
- **Strengthen discharge planning:** Provide clear discharge instructions, follow-up appointments, and post-discharge support for patients with complex conditions or frequent prior visits.
- **Address equity gaps:** Monitor outcomes by **race and gender**, and develop interventions where specific groups show disproportionately higher readmissions.
- **Build readmission risk monitoring into operations:** Use this dashboard as a recurring review tool in quality meetings to track trends, evaluate interventions, and continuously refine care pathways.

---

**Author:** `Kshitij Saini`  
**LinkedIn:** [Kshitij Saini](https://www.linkedin.com/in/kshitij-saini-b950b7299?utm_source=share_via&utm_content=profile&utm_medium=member_android)
