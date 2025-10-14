# BREAST CANCER RECURRENCE
Breast cancer is the leading cause of cancer mortality among women worldwide.. The disease is strongly associated with estrogen-related factors, including early menarche, late menopause, and postmenopausal obesity.
Conversely, early childbirth, multiparity, and breastfeeding confer protective effects.Although genetic mutations significantly increase susceptibility, they account for only a small fraction of cases,
they account for only a small fraction of cases, underscoring the multifactorial nature of breast cancer etiology.
## Problem Statement
Breast cancer recurrence remains one of the most critical challenges in oncology, as it significantly impacts patient survival.and quality of life. Despite advances in treatment, many patients experience
a return of the disease after initial therapy, often due to complex interactions among clinical, pathological, and treatment-related factors.Understanding which patient characteristics such as tumor size,
menopausal status, lymph node involvement, or radiation therapy are most strongly associated with recurrence can help guide more targeted interventions and improve long-term outcomes. 
## Main Objective
-To identify and quantify the specific clinical and pathological factors that are most strongly associated with the recurrence of breast cancer within the observed patient cohort, thereby describing
the key risk profile for recurrence. 
-The dataset has 7 columns: 

1.age: Patient's age categorized into ranges (e.g., 10-19, 20-29, etc.). 

2.menopause: Menopausal status, characterized as lt40 (less than 40), ge40 (greater equal to 40), or premeno. 

3.tumor-size: Size of the tumor, categorized into specific ranges. 

4.inv-nodes: Number of involved lymph nodes, grouped into ranges. 

5.node-caps: Presence or absence of node caps (yes or no). 

6.deg-malig: Degree of malignancy, graded as 1, 2, or 3. 

7.breast: The affected breast, identified as left or right. 

8.breast-quad: Quadrant of the breast affected (e.g., left-up, right-low). 

9.irradiat: Whether the patient underwent irradiation (yes or no).

## Research Questions
### Univariate Analysis
-What is the baseline percentage of patients in the study who experienced a breast cancer recurrence? 

-How are the patients distributed across different age ranges? 

-Which menopause category has the highest number of patients? 

-Which is the most common tumor size range? 

-Which inv-node category is most frequent? 

-What is the most common malignancy level? 

-Which breast side (left or right) is more commonly affected? 

-Which breast quadrant is most affected? 

-How many patients received radiation therapy?
### Bivariate Analysis
-Is there a relationship between menopausal status and recurrence? 

-Does tumor size category relate to recurrence rate? 

-Is there an association between breast side (left or right) and recurrence? 

-Does receiving radiation therapy relate to recurrence? 

-Which breast quadrant is most affected by recurrence?
### Multivariate Analysis
-Does the recurrence rate differ across tumor size categories and menopausal status? 

-For patients with large tumors (e.g., ≥30mm), how does the recurrence rate compare between those who did and did not receive radiation therapy?
## Introduction
The dataset consists of 286 rows which translates to 286 participants.85 (29.72%) participants had recurrence events,most (33.6%) of the participants were aged between 50-59 years,52.4% of the patients were
premenopausal and only 23.8% of the patients had undergone radiation therapy.



