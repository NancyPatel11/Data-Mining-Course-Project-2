**T03 Smoking and Drinking Dataset with Body Signal Dataset Analysis**
--

**Overview**

This repository documents our analysis of a comprehensive [Somking and Drinking](https://www.kaggle.com/datasets/sooyoungher/smoking-drinking-dataset/) dataset, where we performed exploratory data analysis (EDA), data pre-processing, and classification analysis. Following is an overview of the key outcomes of our dataset.

**Exploratory Data Analysis (EDA) & Preprocessing:**

**T1. Explore the dataset assigned to your team and provide:**

**a. A summary of the dataset (should include information columns present, attribute types, null values, and a summary of each attribute).**


*Summary of the dataset and features:*

"Smoking and Drinking Dataset with Body Signal" is a comprehensive and extensive dataset that was collected from National Health Insurance Service in Korea. This dataset contains columns having body measures of body signals like Systolic blood pressure, Diastolic blood pressure, etc along with some physical features like sex, height, etc. In this dataset each instance refers to a person and each person is classified as smoker/non-smoker and drinker/non-drinker. The summary of each attribute is as given below.

*Summary of the data:*

The various features of the Smoking and Drinking Dataset are discussed below:

1. Sex: 

This feature discribe the sex of the person. It becomes important to know the gender of the person under study when dealing with medical signal as it may vary for different genders. This feature consist of two classes *male* and *female*.

2. Age: 

This feature discribe the age of the person rounded up to 5 years. Again age becomes important when dealing with body signal as it may vary for people with different age. This is a numeric feature.
 
3. Height: 

This feature discribe the height of the person rounded up to 5 cm. Again height becomes important when dealing with body signal as it may be predictive for different body signal. This is also a numeric feature.

4. Weight:

This feature discribe the weight of the person in *kg*. Again weight becomes important when dealing with body signal as it may be predictive for different body signal. This is also a numeric feature.

5. sight_left/sight_right: 

This is again a numeric feature that ranges from 0.1 to 9.9. This feature is almost normally distributed. Eye sight can be directly correlated to different body signal as the body signals like blood pressure can affect the eye sight of a person.

6. hear_left/hear_right: 

This feature is similar to sight_left/sight_right and share similar importance. This consist of two classes 1(normal) and 2(abnormal).

7. SBP: 

SBP, or Systolic Blood Pressure, represents the higher number in a blood pressure reading. It measures the force exerted on artery walls when the heart contracts, indicating the maximum pressure in the circulatory system during a heartbeat. Elevated SBP can be a risk factor for cardiovascular diseases, like hypertension which can result due to smoking and drinking. This is a numeric columns ranging from 67 to 273. It is measured in *mmHg*.
 
8. Waistline: 

This is the measure of the waistline of a person in *cm*.

9. DBP: 

DBP, or Diastolic Blood Pressure, is the lower number in a blood pressure reading. It signifies the pressure in the arteries when the heart is at rest between beats. DBP is crucial for assessing vascular resistance and overall cardiovascular health. High DBP may indicate hypertension and increased risk of heart-related conditions. It is a numeric feature ranging from 32 to 185. It is measured in *mmHg*.

10. BLDS: 

BLDS and FSG (Fasting Blood Glucose) are both related to medical measurements, but BLDS is not a standard medical abbreviation. It's possible that "BLDS" is a specific term used in a particular context, but it's not widely recognized in the medical field. Fasting Blood Glucose (FSG) is a common medical test that measures the level of glucose in the blood after an overnight fast. It's an important indicator for diagnosing and monitoring diabetes and other metabolic conditions. If "BLDS" has a specific meaning in your context, please provide more details for clarification. It is measured in *mg/dL*.
 
11. tot_chole: 

It gives the measure of total cholesterol of a person measured in *md/gL*.

12. HDL_chole: 

High-Density Lipoprotein (HDL) cholesterol is a type of cholesterol considered "good" for cardiovascular health. It transports excess cholesterol from the bloodstream to the liver for removal, reducing the risk of plaque buildup in arteries. Higher levels of HDL are associated with a lower risk of heart disease and stroke. It is a numeric feature measured in *mg/dL*.

13. triglyceride:

Triglycerides are a type of fat found in your blood. They are the most common form of fat in the body and are obtained from the food you eat. Triglycerides are stored in fat cells and released as energy when needed. Elevated levels of triglycerides in the blood can be a risk factor for heart disease and can be influenced by factors such as diet, physical activity, and genetics. Managing triglyceride levels is important for cardiovascular health. It is a numeric feature measured in *mg/dL*.

14. LDL_chole:  

Low-Density Lipoprotein (LDL) cholesterol is often referred to as "bad" cholesterol. It carries cholesterol from the liver to the cells in the body, but if levels are too high, it can lead to the buildup of plaque in arteries, increasing the risk of heart disease and stroke. Reducing LDL cholesterol is a key goal for heart health. It is a numeric feature measured in *mg/dL*.

15. hemoglobin: 

Hemoglobin is a vital protein in red blood cells, responsible for carrying oxygen from the lungs to body tissues and transporting carbon dioxide back to the lungs for exhalation. It is essential for maintaining oxygen levels in the body, and imbalances can lead to conditions like anemia or polycythemia. It is a numeric feature measured in *g/dL*.


16. urine_protein: 

Protein in urine, also known as proteinuria, is the presence of excessive proteins in the urine. It can be a sign of kidney dysfunction, which may be caused by various health conditions, including kidney disease, diabetes, hypertension, or infections. Monitoring and diagnosing proteinuria is essential for assessing kidney health and overall well-being. It has 6 classes categorizsd as 1(-), 2(+/-), 3(+1), 4(+2), 5(+3), 6(+4).
 
17. serum_creatinine	: 

Serum creatinine is a waste product from muscle metabolism that is typically filtered by the kidneys and excreted in the urine. Measuring serum creatinine levels is an important clinical test to assess kidney function. Elevated levels can indicate impaired kidney function, often associated with conditions like kidney disease, dehydration, or certain medications. It's a key parameter in monitoring renal health. It is a numeric feature measured in *mg/dL*.

18. SGOT_AST: 

Serum Glutamic Oxaloacetic Transaminase (SGOT) or Aspartate Aminotransferase (AST) is an enzyme found primarily in the liver and heart cells. Elevated AST levels in the blood can indicate damage to these organs, often due to conditions such as hepatitis, cirrhosis, or a heart attack. It is a key marker in diagnosing and monitoring liver and heart health. It is a numeric feature measured in *IU/L*.

19.SGOT_ALT

Serum Glutamic Oxaloacetic Transaminase (SGOT), also known as Aspartate Aminotransferase (AST), and Serum Glutamic Pyruvic Transaminase (SGPT), or Alanine Aminotransferase (ALT), are enzymes found in the liver and other tissues. They are commonly measured in blood tests to assess liver health. Elevated levels of AST and ALT can indicate liver damage or disease, often caused by factors like alcohol consumption, viral hepatitis, or medication toxicity. Monitoring these enzymes is essential in diagnosing and managing liver conditions. It is a numeric feature measured in *IU/L*.

20. gamma_GTP

Gamma-Glutamyl Transferase (GGT), also known as Gamma-Glutamyl Transpeptidase (GGTP), is an enzyme found in various tissues, with the highest concentration in the liver. A blood test measuring GGT levels is used to assess liver and bile duct function. Elevated GGT levels can be indicative of liver diseases, alcohol abuse, or certain medications, making it a valuable marker for diagnosing and monitoring liver health. It is a numeric feature measured in *IU/L*.

21. SMK_stat_type_cd

This feature classify each instance into one of the three classes that represent the smoking state 1(never), 2(used to smoke but quit), 3(still smoke).

22. DRK_YN

This feature classify each instance into one of the two classes that represent the drinking state.

**Note:** Detailed analysis of each feature is presented in the code.



**b. Data Visualization, summarizing insights about the dataset through EDA.**

All the insights have been mentioned in the .ipynb files in respective branches along with the code.
The reasoning for each of the preprocessing steps has also been provided wherever needed.

**Classification Analysis:**

**T2. Identify and list classification problems on your assigned dataset. Which one does seem the most interesting to you and why?**

We have identified five classification problems on our Smoking and Drinking Dataset:

1.	Predicting if a person is a drinker/non-drinker.
2.	Predicting if a person is a smoker/quiter/non-smoker.
3.	Prediciting the sex of a person.
4.	Predicting the urine protein class of the person.
5.	Predicting the hearing normality of a person.
   
Among these five problems, the best one are 1/2 due to following reasons:

•	**Health Interventions:**  Identifying smokers/drinkers allows for targeted health interventions. Smokers/drinkers can receive counseling, support, and resources to quit, reducing their risk of smoking/drinking-related diseases such as lung cancer, heart/liver disease, and respiratory issues.

•	**Public Health Planning:**  Accurate predictions of smoking/drinking habits can inform public health policies and campaigns. This data can guide the allocation of resources and the development of strategies to reduce smoking prevalence and its associated costs.

•	**Healthcare Management:**  Healthcare providers can use smoking/drinking status to tailor medical care. Smoking/drinking significantly affects treatment decisions, as it can interact with medications and influence disease progression. Predicting smoking/drinking habits can aid in more effective and personalized healthcare.

•	**Insurance and Risk Assessment:** Smoking/drinking status is a key factor in determining life and health insurance premiums. Predicting whether someone is a smoker/drinker helps insurance companies assess risk accurately, leading to fairer pricing and policy customization based on individual habits.


**T3. Build an end-to-end Machine Learning pipeline for your assigned dataset for the aforementioned most interesting classification problems found in T2. Your pipeline should include components for dataset preprocessing, transformation, classification model building, hyperparameter tuning, grid search or optimization, and evaluation. Report results on the classification models with hyperparameter tuning, and report the best hyperparameter values. Report results using at least two relevant evaluation metrics like Accuracy, Precision, Recall, F1 Score. Compare results for different models and give the reasoning for that.**

•	End-to-End Machine Learning Pipeline

We developed an end-to-end machine learning pipeline for the selected classification problem. Our pipeline includes the following components:

Data preprocessing

Feature transformation

Classification model building

Hyperparameter tuning

Model evaluation

**Evaluation Metrics:** 
We assessed the performance of our classification models using, Accuracy, Recall, Precision and F1 Score.

**Model Comparison:** 
We compared the results using appropriate metrics for different classification models like Logisitc Regression, Random Forest Classifier, XGBoost Classifier and Neural Netwoks, and provided the reasoning behind our choices.

**Results:** 

Results have been mentioned in the .ipynb files with accuarte measures.

**CONTRIBUTIONS:**

Each member workes individually on one the five classification problems identified above, which can be accessed in their respective branches, named after the team member.

**Team members :**

1.	Deven Patel	(202101264)
2.	Takshay Makadia	(202101414)
3.	Sakshi Patadiya	(202101469)
4.	Nancy Patel (202101491) (Leader)
5.	Ishita Rathod	(202101516)

