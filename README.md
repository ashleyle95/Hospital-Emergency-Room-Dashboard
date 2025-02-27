![Hospital-Overview_header2-2-scaled](https://github.com/user-attachments/assets/51aa4938-4f7a-4e90-9109-98afe00abc67)
# Hospital Emergency Room Dashboard
[Power BI-Hospital Dashboard](https://app.fabric.microsoft.com/view?r=eyJrIjoiNGQ2ZjFhOWQtOWE0My00MzQ3LWIwMGUtYzg4MmI3MzI0YTA1IiwidCI6IjA2N2UxZTE5LWExMWEtNDhlNS04Yjc5LTBiOWVlNzQ1YTdhMiJ9)

## Project Overview
A hospital, A, is collecting data for enhanced patient care and operational efficiency in ER management. This dataset encapsulates comprehensive patient information collected from a hospital emergency room (ER) dashboard. It serves as a valuable resource for healthcare analytics, focused on understanding patient demographics, treatment outcomes, and operational efficiency within emergency departments.

## Objective
This dashboard can uncover the trend of ER performance to improve efficiency, reduce wait times, and enhance patient care.

Key questions:

How many patients visited the ER during a specific period? What are the demographics of ER patients (age, gender, race)?

What is the average wait time for ER patients? Does waiting time affect the satisfaction score of patients?

What is the patient satisfaction score? How is the satisfaction score in term of race, referral department and age group?

What are the busiest days and hours for ER visits? Which departments refer the most patients to the ER?

## Stakeholders:
Hospital Administrators & Management: monitor the efficiency of ER and staffing

Doctors & Nurses: to reduce waiting time and enhance patient care by satisfaction score

Emergency Room Coordinators: to manage patient flow to collaborate with other departments

Healthcare Policy Makers: improve the regulations to review the process by KPI and analyze the trend 

## Data Process:

During the data profiling process in Power BI, we identified that the patient_sat_score column contains a significant number of null values. This column represents patient satisfaction scores, which are optional ratings provided by patients regarding their experience with the hospital's emergency services.

After careful consideration, we have decided to retain these null values rather than imputing or removing them. The primary reason for this decision is that patient satisfaction ratings are often voluntary, and missing values do not necessarily indicate an error but rather a lack of response. Excluding these records could introduce bias into the analysis by disproportionately focusing on patients who chose to leave a rating.

## Reporting dashboard 
[Embedded Demo in Power BI service](https://github.com/user-attachments/assets/51aa4938-4f7a-4e90-9109-98afe00abc67)

Page 1: `Visit Overew`: Provides an overview of the hospital's emergency room visits
![image](https://github.com/user-attachments/assets/7d62a267-7f53-40b6-997a-9c27a8e71409)

Page 2: `Detail`: Provides detailed insights into operational performance.
![image](https://github.com/user-attachments/assets/df7933ae-1928-4807-8614-67c7d2f5bde8)
