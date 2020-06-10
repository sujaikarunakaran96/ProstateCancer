# ProstateCancer
SURVIVAL ANALYSIS OF A PATIENT DIAGNOSED WITH PROSTATE CANCER

Univariate Analysis:

1. From the graph of gleason score, we can see that patients with high gleason score do not survive after 7 years of diagnosis.
2. From the tumor diagnosis graph, we can see that the patients who do not survive after 7 years had a bigger tumor compared to people who survived.
3. From the race graph, we can see that most of the patients are under Race 4. Therefore, this level can be used as reference level. 


Treatment of Symptoms:

1. It was found that there were 16 different symptom codes in the column
2. One column for each symptom code was created with type, binary
3. Then chi-square test was run to determine the symptom codes that are significant
4. Given an event has occurred in 1 year but the PSA and Tumor size data is not available for 6 months and 1 year, the time is taken as 180 days
5. Given an event has not occurred in 1 year but the event has occurred in 7 years, then the time is taken as 365 days
6. For an event that has not occurred in 7 years, the time is taken as 2555 days

Survival Analysis: 

1. Survival analysis was run using the cancer related features to understand how treatments contributed to the survivability. For interpretability, I have screenshots of selected output. 
2. A person with stage 4, has a survival probability of 0.933 for the first 1 year whereas, the probability decreases to 0.2 after 1 year of diagnosis.
3. A person with stage 3 has a survival probability of just 0.885 for the first year when multiple therapies are performed whereas this probability reduces to 0.154 after 1 year. This might also be due to the severity of the disease.
3. From the below output, we can see that same tumor size group has different survival probability after 1 year for 7 years due to different combination of therapies in both the cases. 
4. Similarly, survival Analysis was run using the conceptual model
5. Firstly, the demographics features were used to determine the probability of survival after 1 year for 7 years.
6. From the results we can see that a person with age less than 78 and belongs to the race 1 has a probability of 0.422 of survival after 1st year of diagnosis where the same person has the probability of 0.921 of survival for the first 1 year of cancer diagnosis
We can also see that the change in probability of survival is not very dependent on race since the probabilities are approximately the same

Hazard Ratio: 
1. Hazard ratio is like the log odds in the logistic regression. 
2. From the hazard ratio plot, we can get the significant variables which can predict the survival time of a patient. The variable stage, radiation therapy, brachy therapy, surgery, tumor size, age, and few symptoms seem to be significant predictors.
3. From hazard ratio, for example, with reference to the patients with stage I cancer, patients with stage II cancer has 23% more risk of not surviving with 95% confidence interval 1.04 to 1.4. 
4. Similarly, a patient with symptom O10 has 2% less risk of not surviving after 7 years with 95% confidence interval of 0.80 to 1.2







