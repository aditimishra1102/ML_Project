# A Comparative Study for Time-to-Event Analysis and Survival Prediction for Heart Failure Condition using Machine Learning Techniques
## ABSTRACT

Heart Failure, an ailment in which the heart isn’t functioning as effectively as it should, causing in an insufficient cardiac output. The effectual functioning of the human body is dependent on how well the heart is able to pump oxygenated, and nutrient rich blood to the tissues and cells. Heart failure falls into the category of cardiovascular diseases - the disorders of the heart and blood vessels. One of the leading causes of global deaths resulting in an estimated 17.9 million deaths globally every year. The condition of heart failure results out of structural changes to the cardiac muscles majorly in the left ventricle. The weakened muscles cause the ventricle to lose its ability to contract completely. Since the left ventricle generates the required pressure for blood circulation, any kind of a failure condition results in the reduction of cardiac power output. This study aims to conduct a thorough survival analysis and survival prediction on the data of 299 patients classified into the class III/IV of heart failure and diagnosed with left ventricular systolic dysfunction. Survival analysis involves the study of the effect of a mediation assessed by measuring the number of subjects survived after that mediation over a period of time. The time starting from a distinct point to the occurrence of a certain event, for example death is known as survival time and the corresponding analysis is known as survival analysis. The analysis was performed using the methods of Kaplan-Meier (KM) estimates and Cox Potential Hazard regression. KM plots showed the survival estimates as a function of each clinical feature and how each feature at various levels affect survival over the period of time. Cox regression modelled the hazard of death event around the clinical features used for the study. As a result of the analysis, ejection fraction, serum creatinine, time and age were identified as highly significant and major risk factors in the advanced stages of heart failure. Age and rise in level of serum creatinine have a deleterious effect on the survival chances. Ejection Fraction has a beneficial effect on survival and with a unit increase in the in the EF level the probability of death event decreases by ~5.2%. Higher rate of mortality is observed during the initial days post diagnosis and the hazard gradually decreases if patients have lived for a certain number of days. Hypertension and anemic condition also seem to be high risk factors. Machine learning classification models for survival prediction were built using the most significant variables found from survival analysis. SVM, decision tree, random forest, XGBoost, and LightGBM algorithm were implemented, and all the models seem to perform well enough. However, the availability of more data will make the models more stable and robust. Smart solutions, like this can reduce the risk of heart failure condition by providing accurate prognosis, survival projections, and risk predictions. Technology and data can combine together to address any disparities in treatment, design better care plan, and improve patient health outcomes. Smart health AI solutions would enhance healthcare policies, enable physicians to look beyond the conventional practices, and increase the patient satisfaction levels not only in case of heart failure conditions but healthcare in general.

 ## DATASET
 
 The dataset contains cardiovascular medical records taken from 299 patients. The patient cohort comprised of 105 women and 194 men between 40 and 95 years in age. All patients in the cohort were diagnosed with the systolic dysfunction of the left ventricle and had previous history of heart failures. As a result of their previous history every patient was classified into either class III or class IV of New York Heart Association (NYHA) classification for various stages of heart failure.
 
 #### FEATURE DESCRIPTION
 
 Feature | Explanation | Measurement	| Range
------------- | ------------- |------------- | -------------
Age	|Age of the patient	|Years |	[40,..., 95]
Anaemia	|Decrease of red <br> blood cells or hemoglobin |	Boolean|	0, 1
High blood pressure |	If a patient has hypertension |	Boolean	 |0, 1
Creatinine phosphokinase<br>(CPK) |	Level of the CPK enzyme <br>in the blood |	mcg/L|	[23,..., 7861]
Diabetes|	If the patient has diabetes |	Boolean	| 0, 1
Ejection fraction|	Percentage of blood leaving<br>the heart at each contraction|Percentage	|	[14,..., 80]
Sex	| Woman or man |	Binary|	0, 1
Platelets|	Platelets in the blood|	kiloplatelets/mL|	[25.01,..., 850.00]
Serum creatinine|	Level of creatinine in the blood|	mg/dL|	[0.50,..., 9.40]
Serum sodium|	Level of sodium in the blood|	mEq/L|	[114,..., 148]
Smoking|	If the patient smokes|	Boolean	|0, 1
Time|	Follow-up period|	Days|	[4,...,285]
DEATH EVENT<br>(TARGET)|	If the patient died during the follow-up period|	Boolean|	0, 1
