![Hospital-Overview_header2-2-scaled](https://github.com/user-attachments/assets/51aa4938-4f7a-4e90-9109-98afe00abc67)
# Hospital Emergency Room Dashboard
## Project Links
[Power BI-Hospital Dashboard](https://app.fabric.microsoft.com/view?r=eyJrIjoiNGQ2ZjFhOWQtOWE0My00MzQ3LWIwMGUtYzg4MmI3MzI0YTA1IiwidCI6IjA2N2UxZTE5LWExMWEtNDhlNS04Yjc5LTBiOWVlNzQ1YTdhMiJ9)
## Table of contents
[1. Project Overview](#1-project-overview)

[2. Data Process](#2-data-process) 

[3. Reporting Dashboard](#3-reporting-dashboard)

[4. Findings/Recommendations](#4-findingsrecommendations)

[5. Limitations](#5-limitations)
## 1. Project Overview
A hospital, A, is collecting data for enhanced patient care and operational efficiency in ER management. This dataset encapsulates comprehensive patient information collected from a hospital emergency room (ER) dashboard. It serves as a valuable resource for healthcare analytics, focused on understanding patient demographics, treatment outcomes, and operational efficiency within emergency departments.

### Objective
This dashboard can uncover the trend of ER performance to improve efficiency, reduce wait times, and enhance patient care.

**Key questions:**

+ How many patients visited the ER during a specific period? What are the demographics of ER patients (age, gender, race)?

+ What is the average wait time for ER patients? Does waiting time affect the satisfaction score of patients?

+ What is the patient satisfaction score? How is the satisfaction score in term of race, referral department and age group?

+ What are the busiest days and hours for ER visits? Which departments refer the most patients to the ER?

### Stakeholders:
+ Hospital Administrators & Management: monitor the efficiency of ER and staffing

+ Doctors & Nurses: to reduce waiting time and enhance patient care by satisfaction score

+ Emergency Room Coordinators: to manage patient flow to collaborate with other departments

+ Healthcare Policy Makers: improve the regulations to review the process by KPI and analyze the trend 

## 2. Data Process:

During the data profiling process in Power BI, we identified that the `patient_sat_score` column contains a significant number of null values. This column represents patient satisfaction scores, which are optional ratings provided by patients regarding their experience with the hospital's emergency services.

After careful consideration, we have decided to retain these null values rather than imputing or removing them. The primary reason for this decision is that patient satisfaction ratings are often voluntary, and missing values do not necessarily indicate an error but rather a lack of response. Excluding these records could introduce bias into the analysis by disproportionately focusing on patients who chose to leave a rating.

## 3. Reporting dashboard 
[Embedded Demo in Power BI service](https://app.fabric.microsoft.com/view?r=eyJrIjoiNGQ2ZjFhOWQtOWE0My00MzQ3LWIwMGUtYzg4MmI3MzI0YTA1IiwidCI6IjA2N2UxZTE5LWExMWEtNDhlNS04Yjc5LTBiOWVlNzQ1YTdhMiJ9)

**1. Page 1: `Visit Overew`**: Provides an overview of the hospital's emergency room visits
![image](https://github.com/user-attachments/assets/90b95930-9348-4188-8323-bca3fb5f51f2)

+ 9,216 patients visited the ER during the reported period, reflecting a 44.1% increase in total patient visits compared to the same period last year. This indicates a positive trend in patient visits.

Another key performance indicator (KPI) is the average satisfaction score, which has remained stable. However, efforts should be made to increase this score to meet the target of 7 out of 10.

+ The average waiting time has increased slightly by 1.2%, with patients now waiting around 35 minutes for a visit.
![image](https://github.com/user-attachments/assets/b81f25f0-ba76-4a03-a292-0b31349e26c0)


+ The demographic of patients visiting the ER during this period shows that 51% of the patients are male, while 48.69% are female. Monday and Saturday is the busiest day in the week. The period of collected data is from 01 April 2019 to October 30, 2020 so during that period, the patient visits in 2020 is higher compared to previous year
![image](https://github.com/user-attachments/assets/7ce3de18-ca23-45f5-8554-1c6536034272)

By drilling down into the graph, the trend by quarter can be revealed. Patient visits remained consistent throughout the quarters of 2020, except for the last quarter (Q4), which experienced a sharp decline with only 471 visits due to data being collected only until October 2020. The graph allows for easy drilling down to uncover trends over time by date, month, quarter, or year for further analysis if needed.

![image](https://github.com/user-attachments/assets/88678f1e-736c-4618-a616-7ca97d9473e5)


+ Department Referral:
41.4% of all patients are referred from other departments, with General Practice having the highest referral rate. It also has the second-lowest average waiting time.

There is no significant difference in the average waiting time for department referrals, which ranges from 34 to 36 minutes.

Renal is the department with the shortest waiting time; however, it has the lowest satisfaction score compared to other departments. This should be addressed with a focus on improvement.

General Practice, despite receiving the most department referrals, has the second-lowest satisfaction score

![image](https://github.com/user-attachments/assets/67c2b68e-f086-45cd-87b4-0503a76df6f7)

+ Race

White and African American patients have the highest patient visits, both with a satisfaction score of 5.4 out of 10. In contrast, Native American/Alaska Native patients have the lowest number of visits and experience the highest average waiting time.

Pacific Islander patients have the lowest waiting time but also the second-lowest patient visits. This may contribute to their highest satisfaction score.

There is no significant gap in satisfaction scores between the other racial groups, except for Pacific Islander.
![image](https://github.com/user-attachments/assets/893c5980-f0a8-4b91-a687-4f8881c6c85f)


**2. Page 2: `Detail`**: Provides detailed insights into operational performance.
![image](https://github.com/user-attachments/assets/2b721678-fba1-4430-9da7-522f9fd68d45)



+ Total Patients:
On Mondays, the ER is generally quite busy except  from 3 PM to 8 PM. The busiest period is at 11:00 PM, requiring effective staff management to handle the surge in emergency cases.

![image](https://github.com/user-attachments/assets/560a6687-8463-4b23-b805-ad66adce1e79)

+ Average Satisfaction Score:
Before 7 AM and after 10 PM, the average satisfaction score tends to be lower than during other hours. This suggests that service improvement efforts are needed, possibly due to staff shortages during these times.

![image](https://github.com/user-attachments/assets/14ec95f4-89a6-4c7e-93e0-abf2764a788f)


+ Average Waiting Time:
The highest waiting times are observed at 11:00 PM and between 8 AM and 1 PM. This indicates a need for resource optimization during these periods to reduce waiting times.

![image](https://github.com/user-attachments/assets/e182ba37-b498-4d00-a074-76a79888cfc8)

Infancy has the lowest waiting time, which correlates with the highest satisfaction score, highlighting the priority for maintaining efficient service for this age group.

Early childhood, teenagers, and seniors are the age groups that require improvement in their satisfaction ratings.
![image](https://github.com/user-attachments/assets/cd911b80-a937-46bb-936e-76e00b37b23f)

## 4. Findings/Recommendations

+ Staff Management During Peak Hours:

Given that 11:00 PM is the busiest period, ensure that there is adequate staffing to handle emergency cases, particularly during late-night hours.
Consider implementing staggered shifts or on-call staff during the busiest hours, such as late evenings and weekends, to prevent delays.
Improving Satisfaction Scores 
During Off-Hours, the lower satisfaction scores before 7 AM and after 10 PM could be linked to reduced staffing. It’s recommended to review staff coverage during these hours and ensure that service levels are maintained.

+ Reducing Waiting Times:
  
Consider enhancing communication, such as providing timely updates to patients about waiting times, during these periods to manage expectations.
Since waiting times are highest at 11:00 PM and between 8 AM and 1 PM, consider reviewing processes during these hours to streamline patient flow.

+ Addressing Age Group-Specific Needs:

Infancy patients have the highest satisfaction scores, so maintaining fast service for this group should remain a priority.
For early childhood, teenagers, and seniors, review the factors contributing to lower satisfaction scores and target service improvements in these areas, such as quicker service or personalized care. A review of communication and staff training could also be beneficial for these groups.

+ Department-Specific Focus:

Since Renal has the lowest satisfaction despite the shortest waiting times, it would be useful to identify any other issues impacting the patient experience in this department, such as communication or care quality.
For departments with high referral rates, such as General Practice, further investigate factors contributing to the lower satisfaction scores despite increased patient volume, and consider adjusting resources or care protocols.

+ Improving Racial Group-Specific Satisfaction:

Since Pacific Islanders report the highest satisfaction despite low patient volume, consider studying the service models that work well for this group and apply these practices across other racial groups.
Explore why Native American/Alaska Native patients experience the highest waiting times and lowest satisfaction scores, and focus on strategies to reduce waiting time and improve their overall experience.

## 5. Limitations
+ The data collection period spans from April 1, 2019, to October 30, 2020, which may limit my ability to uncover trends. For more comprehensive analysis, collecting data for over two years could provide deeper and more insightful findings.

+ The current dashboard does not capture the underlying reasons for patient wait times, such as staff shortages or high-acuity cases. Additionally, real-time patient feedback is not included in the satisfaction scores, limiting the depth of analysis. More than 70% of patients do not provide a satisfaction score, which makes the analysis less comprehensive. For more accurate insights, we recommend integrating real-time patient tracking to dynamically predict wait times. Additionally, implementing a user-friendly interface to encourage patients to leave comments and ratings can provide more valuable feedback for further analysis and service improvement.

| [Table of Contents](#table-of-contents) | [Project Links](#project-links) |

![1_wIQXN2jlsadoLTW-imrR8g](https://github.com/user-attachments/assets/530d1d76-5f51-4f3d-a836-a56215a0a83f)
