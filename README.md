# BREAST CANCER RECURRENCE
Breast cancer is the leading cause of cancer mortality among women worldwide. The disease is strongly associated with estrogen-related factors, including early menarche, late menopause, and postmenopausal obesity.
Conversely, early childbirth, multiparity, and breastfeeding confer protective effects.Although genetic mutations significantly increase susceptibility, they account for only a small fraction of cases,
underscoring the multifactorial nature of breast cancer etiology.
## Problem Statement
Breast cancer recurrence remains one of the most critical challenges in oncology, as it significantly impacts patient survival and quality of life. Despite advances in treatment, many patients experience
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
## Univariate Insights
The dataset consists of 286 rows which translates to 286 participants.85 (29.72%) participants had recurrence events as illustrated by the figure below.
 
<img width="669" height="516" alt="output" src="https://github.com/user-attachments/assets/74a2fb8b-b55e-454e-88e8-7560647c1b70" />

The majority of patients were aged 50–59 years (33.6%) and premenopausal (52.4%).
Most participants had:

Tumor sizes of 30–34 mm (20.97%)

0–2 involved lymph nodes (74.48%)

Malignancy grade 2 (45.45%)

Left-sided breast involvement (53.15%), predominantly in the left lower quadrant (38.6%)
Only 23.8% of patients underwent radiation therapy.

<img width="590" height="490" alt="image" src="https://github.com/user-attachments/assets/6835d46f-3648-401c-be95-e826fe427363" /> 

<img width="590" height="490" alt="image" src="https://github.com/user-attachments/assets/3f269a62-0199-4fac-a0ea-7ec9c3bdda24" />

## Bivariate Analysis
### Menopausal status vs Recurrence
<img width="690" height="490" alt="image" src="https://github.com/user-attachments/assets/066b492b-250b-448f-9e62-8fe75496dca8" />

-The premeno (pre-menopausal) and ge40 (age ≥40, likely post-menopausal or perimenopausal) groups represent the vast majority of the patient population.
-The lt40 (age <40) group is a very small minority, with fewer than 10 patients in total.
-The premeno group has the highest number of recurrence events  compared to the other groups, and the highest proportion of recurrence among the three groups.
-The recurrence rate in the ge40 group is lower than the premeno group, suggesting that being in the ge40 status might be associated with a slightly lower relative risk of recurrence compared to premeno.
-While the lt40 group has a substantial recurrence rate, its absolute contribution to the total number of recurrence events is negligible due to the extremely small sample size.
-Further analysis with chi square test revealed no statistical significant relationship between the two variables, χ²= 0.79, p = 0.67. This suggests that menopausal status does not appear to influence recurrence rates in this dataset.

### Tumor size vs recurrence
<img width="989" height="490" alt="image" src="https://github.com/user-attachments/assets/1b909ef3-0610-4130-8f61-6d27a1467c90" />

-The majority of patients, both those with and without recurrence, fall into the intermediate tumor size categories of 20-24 mm, 25-29 mm, and 30-34 mm. These three categories account for the highest absolute number of patients in the dataset.
-The 30-34 mm category has the highest absolute number of recurrence events at 25 patients. The 25-29 mm category follows closely with 18 recurrence events, and the 20-24 mm category has 16. These three groups contribute the most to the overall recurrence burden.
-The smaller (0-4 mm, 5-9 mm, 10-14 mm) and largest (45-49 mm, 50-54 mm) tumor size categories have very low patient counts, both for recurrence and no-recurrence events.
-The recurrence rate generally shows an increasing trend and is highest in the 20-34 mm range, peaking at the 30-34 mm category. This suggests that as the tumor size progresses from 20 mm to 34 mm, the patient's prognosis significantly worsens.
-Further analysis with chi square test revealed no statistical significant relationship between the two variables, χ²= 17.9157, p = 0.0564. This suggests that there is no statistically significant association between tumor size and recurrence. However, the result is near the threshold, indicating a possible weak trend where patients with larger tumors may have a higher recurrence rate. 

### Breast side vs recurrence
<img width="590" height="490" alt="image" src="https://github.com/user-attachments/assets/61a4afb3-6a77-4df3-bc45-8f2668e737ab" />

-There is a slight predominance of left-sided cases in this dataset.
-The left side contributes a larger absolute percentage to the total number of recurrence events compared to the right side.
-Further analysis with chi square test showed no statistically significant association between the two variables. Although recurrence appeared slightly higher in the left breast (49 cases) compared to the right (36 cases), the difference was not significant. This suggests that breast side does not have a meaningful influence on recurrence rates in this dataset. 

### Radiation therapy vs Recurrence
<img width="590" height="490" alt="image" src="https://github.com/user-attachments/assets/a01ba92f-8361-478c-a17b-83e358d1b825" />

-A large majority of the patients in this study were not treated with radiation therapy.
-The absolute burden of recurrence is much higher in the group that did not receive radiation compared to the group that did receive radiation.
*Clinical Selection Bias: Radiation therapy is typically not given indiscriminately. It is usually reserved for patients with higher risk features e.g., larger tumors
The "Yes Radiation" group likely consists of patients who were already at a much higher risk of recurrence at baseline. Despite receiving the treatment, their underlying poor prognosis drove the high recurrence rate.
-Recurrence events were somewhat more frequent in those who had not undergone radiation therapy.
The chi square test revealed a significant (χ²= 9.7806, p = 0.0018) association between the two variables indicating that radiation therapy has a significant impact on recurrence in this dataset. 

### Breast quadrant vs Recurrence
<img width="790" height="490" alt="image" src="https://github.com/user-attachments/assets/3abb365c-c117-4a0f-95dd-df9fec3d61c3" />

-The left breast is overwhelmingly the most common site for the primary tumor in this dataset, particularly the left lower and left upper quadrants.
-The majority of the recurrence burden is driven by tumors originating in the left breast quadrants.
-The Chi-Square test showed no statistically significant association between breast-quad and recurrence status (χ² = 5.871, p = 0.319).
-This means that differences in recurrence across categories of breast quadrant could be due to chance rather than a real underlying relationship.

## Multivariate analysis
### Menopausal Status and Age vs Recurrence
<img width="1687" height="495" alt="image" src="https://github.com/user-attachments/assets/3b39cc05-c465-40df-a23e-abccbb7edb96" /> 

-The multivariate bar plots display recurrence percentages across age groups separately for each menopausal status. 
-The plots suggest higher recurrence proportions in middle-age bins (30–49) for both premenopausal and postmenopausal groups (e.g., 42.9% recurrence in premenopausal 30–39, ~44.4% in postmenopausal 40–49). 
-However, many age×menopause combinations contain few observations, especially in the lt40 strata, so percentages are unstable. 

### Effect of Tumor size and menopausal status on Recurrence
<img width="1626" height="421" alt="image" src="https://github.com/user-attachments/assets/1d28a7fa-963a-48d8-a348-1b369bf87c61" /> 

-The ge40 group generally maintains lower recurrence rates across most tumor sizes compared to the 'premeno' group. The highest recurrence rate in this group is 50.0% (at 45-49mm).
-The premeno group experiences the highest recurrence rates across several common tumor size ranges. The highest recurrence rate in this group is 50.0% (50-54mm).
-The data for the le40 group is too sparse (very small sample size, as seen by the high percentage of 100% or 0% across most categories) to draw reliable conclusions about recurrence risk.
-Menopausal status acts as an effect modifier. Being pre-menopausal significantly amplifies the risk of recurrence, particularly for small and medium-sized tumors (10-19mm), where the difference in risk between the two menopausal groups is most pronounced.

## Conclusion
This study underscores that breast cancer recurrence is a multifactorial outcome influenced by both biological and treatment-related factors.
While tumor size and menopausal status shape recurrence patterns, radiation therapy emerges as a strong protective factor.

-Key conclusions:

Larger tumors are associated with higher recurrence rates.

Radiation therapy significantly reduces recurrence risk, particularly in patients with large tumors.

Breast side and quadrant location have no significant impact on recurrence outcomes.

-Overall implication:
Early detection of small tumors and judicious use of adjuvant radiation remain pivotal strategies to reduce recurrence and improve survival outcomes in breast cancer patients.












