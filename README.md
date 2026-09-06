# <p align="center">Hospital Mortality Analysis  — Python & Power BI</p>

# <p align="center"><img width="900" height="500" alt="image" src="https://github.com/user-attachments/assets/22958ce1-9ea9-438b-81da-616db7544853" />
</p>

#### **Tools Used**: Excel, Python, Power Bi

[Dataset Used](https://www.kaggle.com/datasets/mitishaagarwal/patient)

[Python Analysis (Code)](https://github.com/munigirishbabu2004/Hospital-Mortality-Analysis-Python-Power-BI/blob/main/Project.ipynb)

[Hospital Mortality Dashboard on Power bi](https://github.com/munigirishbabu2004/Hospital-Mortality-Analysis-Python-Power-BI/blob/main/dsahboard.pbix)

- **Business Problem:** Healthcare professionals are trying to identify the main causes of in-hospital mortality for admitted patients. By having a clear understanding of the causes early on, healthcare professionals will be in a better position to develop targeted interventions, and implement evidence-based protocols to address the factors that contribute to in-hospital patient deaths. 

- **My Appraoch To Solving The Problem:** To tackle the business problem of identifying the main causes of in-hospital mortality for admitted patients, I wanted to do a comprehensive analysis leveraging Python and Power Bi. My approach involved obtaining the dataset, importing it into Excel, cleaning the data, then importing it to Jupitar notebook and performed targeted operations to extract valuable information and to derive key insights. Using my Python skills, I delved into the dataset, exploring various patient attributes such as age, ethnicity, gender, weight, BMI, heart rate, and comorbidities. After executing the operations with Python, I uncovered insightful patterns, trends, and correlations within the data. To present my findings in a visually appealing manner, I used Power bi to design an interactive dashboard. The dashboard summarized the key insights derived from my Python analysis, showcasing patterns and trends related to in-hospital mortality. 

- **Insights I Gathered:** Below I will show the results of the Python operation I conducted and provide explanations of the patterns and trends I found throughout the analysis.

1:

![Result1](https://github.com/user-attachments/assets/7f425ff3-5975-49d8-92c8-0752d882d13a)

Out of the 91,713 admitted patients in the hospitals, a total of 7915 patients died, which translates to 8.63%. This meant that understanding the factors contributing to in-hospital mortality was highly important in improving patient care and reducing preventable deaths.

2:

![Result2](https://github.com/user-attachments/assets/1ab91f4f-13cc-42cc-a6c2-47a7eeb67633)

This output showed the amount of patients that died and survived in each age group, categorized by 10-year intervals. There were far more admitted patients between the ages of 50-89 compared to patients who were between 0-49. Observing the results more, each 10-year age group in the 50-89 range had a slight increase in death percentage. Patients aged 70-89 had a combined mortality rate of 11.58%, notably higher than younger age groups.

3:

![Result3](https://github.com/user-attachments/assets/0c4acb3c-7d1f-4147-b126-45e5a9dca7ab)

This output further proves that the death probability of a patient in the hospital rises as they get older.

4:

![Result4](https://github.com/user-attachments/assets/28ee3126-ec8e-4987-9591-68eac1e1eaae)

![Result4.1](https://github.com/user-attachments/assets/e92c02cd-3faf-421a-b8dc-562cb506f9ce)

These two outputs give more insight to the outcomes of patients in each ICU admit source & type. A vast majority of the patients were admitted to the "Accident & Emergency" ICU admit source and it also experienced the highest number of deaths.
In the second output where death results are shown for each ICU type, there is a clear outlier: Med-Surg ICU.

5:

![Result6](https://github.com/user-attachments/assets/37fe24c1-c4fb-46ff-a915-3f4293632758)

Average weight, BMI, and max heart rate among the patients that died.

The average weight of 80.9 kg (~178 lbs) suggests that, on average, patients who passed away were not underweight — weight alone doesn't appear to be a defining risk factor here. The average BMI of 28.31 falls within the "overweight" range, though not dramatically elevated, reinforcing that weight and BMI alone may not be the sole determinants of mortality — individuals across a range of BMI values can face significant health risks and complications leading to hospital death. The average maximum heart rate of 114.68 highlights a potential cardiovascular aspect in these patients' health profiles. Elevated heart rates can be indicative of underlying conditions (([source](https://www.mayoclinic.org/diseases-conditions/tachycardia/symptoms-causes/syc-20355127)),), such as cardiac distress or organ failure, which may have contributed to the hospital mortality outcomes observed.

6:

![Result6](https://github.com/user-attachments/assets/c67076a0-64ec-4ef0-9fc7-1ea290a3bb9a)
![Result6.1](https://github.com/user-attachments/assets/86458a8d-60aa-498c-8118-934b8d572759)

Comorbidities among admitted patients and their associated mortality.

Diabetes mellitus is by far the most prevalent comorbidity in the dataset, affecting 20,492 patients — more than 7 times the next most common condition (immunosuppression, 2,381 patients). It also accounts for the largest single share of deaths among comorbid patients (1,595), simply due to its sheer prevalence.
However, prevalence and risk are not the same thing. 

7:

![Result7](https://github.com/user-attachments/assets/fc91cd1e-a191-48aa-bd69-83203f002958)

Patients aged 60 and above: survived vs. died.

Among patients aged 60 and older, 51,583 survived while 6,200 died — a mortality rate of roughly 10.7% within this age group. This is noticeably higher than the overall dataset mortality rate of 8.63%, reinforcing that older age is one of the strongest individual risk factors for in-hospital death, consistent with the age-group breakdown seen earlier (60-69: 9.56%, 70-79: 10.31%, 80-89: 13.34%).

8:

![Result8](https://github.com/user-attachments/assets/66446230-3111-49ed-b542-bc7542060b70)

Generally speaking, and as shown by this output, prolonged stays in the ICU are associated with higher mortality rates ([source](https://pubmed.ncbi.nlm.nih.gov/26571190/#:~:text=One%2Dyear%20mortality%20was%2026.6,the%20need%20for%20mechanical%20ventilation.)). An increased length of stay in the ICU can be due to a number of reasons, such as cardiovascular system diseases, nervous system diseases, infections, underlying illnesses, and increased exposure to potential complications ([source](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5884409/#:~:text=Our%20study%20showed%20a%20significantly,the%20length%20of%20stay%20increases.)). According to this output, a patient who stayed in the ICU for longer than a day had a higher chance of death compared to someone who spent less than a day in the ICU. 

- **Conclusion:** Age was the first big predictor of in-hospital mortality from this dataset. Consistently, advanced age has been associated with higher rates of medical conditions, complications, and death. According to the dataset, nearly 13% of the patients who were 80 years old or older experienced in-hospital mortality. This finding highlights the significant impact of age on mortality risk among older individuals. Another strong predictor of in-hospital mortality is comorbidities. Diabetes emerged as the most common comorbidity, though solid tumor with metastasis and immunosuppression had higher mortality rates among patients diagnosed with those conditions, at 18.48% and 16.13% respectively, compared to 7.78% for diabetes. Heart rate can also be very telling to predict mortality as it reflects the cardiovascular status and overall physiological stability of patients. Abnormalities in heart rate, such as tachycardia (elevated heart rate) or bradycardia (low heart rate), often indicate underlying cardiovascular dysfunction or compromised perfusion
([source](https://www.mayoclinic.org/diseases-conditions/tachycardia/symptoms-causes/syc-20355127)). Research has consistently shown a strong association between abnormal heart rates and increased mortality risk. In this dataset, the average max heart rate for patients that died was 114.68. Generally, a resting heart rate is high if it is over 100 bpm ([source](https://www.healthline.com/health/dangerous-heart-rate)). The length of stay at an ICU was also an important indicator of mortality, showing that patients who stayed for a shorter duration at the ICU had a much better chance for survival.
