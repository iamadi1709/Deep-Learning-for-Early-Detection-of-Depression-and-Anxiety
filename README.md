**🧠 Deep Learning for Early Detection of Depression & Anxiety**

**Description:** **Depression is a severe mental disorder characterized by symptoms like persistent sadness, emptiness, anxiety, and sleep disturbances, often leading to a loss of interest in daily activities. Additional symptoms can include feelings of guilt, worthlessness, fatigue, difficulty concentrating, and in severe cases, suicidal thoughts or psychotic episodes. The severity of depression depends on the number, intensity, and duration of symptoms, as well as its impact on social and work life. Depression is also a common feature of Bipolar Disorder, a psychiatric condition distinguished by alternating periods of depression and mania. While both are genetic in nature, environmental factors like disrupted biological rhythms (due to lifestyle changes, seasonal variations, or social stressors) can trigger mood episodes. Factors like physical health, substance abuse, and significant life events also play a role. Globally, around 15% of the population will experience depression in their lifetime, with many more facing less severe depressive episodes. Actigraphy, the measurement of motor activity, is emerging as an objective method for studying depression, though more research is needed in this area.**

![image](https://github.com/user-attachments/assets/607e48f3-be5d-4ff0-8c7f-199e206e95ef)

This project aims to leverage machine learning to predict depression using healthcare data 🏥. By making the process accessible and replicable, we hope this work contributes to improving mental health diagnosis 💡.

🗂 Repository Structure

README.md: You're looking at it! 📜 An overview of the project for reviewers.

Anxiety_Prediction.ipynb: 📓 Initial exploration and data cleaning steps.

Model.ipynb: 📊 Continuation into data exploration and modeling.

Predicting_Early_Depression and_Anxiety.pdf: 🎤 PDF version of our project presentation.

project_functions/: 🛠 Custom functions used across notebooks.

Dashboard/: 📊 Companion dashboard files.

✨ Abstract
Mental health issues affect millions worldwide, with depression being one of the leading causes of disability and death by suicide 😔. Despite this, many primary care physicians lack the necessary training to address mental health problems. Through this project, we explore how machine learning can help doctors better identify patients at risk of depression early on. Using data from the CDC National Health and Nutrition Examination Survey (NHANES), this project predicts depression based on patient information often available in medical files. These insights could be used to alert healthcare providers or even trigger automated mental health referrals, thereby making treatment more accessible.

💡 Key Result: Our model accurately identified 71% of depressed individuals and 80% of non-depressed individuals, demonstrating the feasibility of this approach. There’s room for improvement, but this project provides a solid proof of concept!

![image](https://github.com/user-attachments/assets/933cf6ca-29ba-458c-92a1-4d34a7dda59e)

📚 Introduction
Depression affects over 264 million people worldwide 🌍, and suicide is among the leading causes of death, especially for young adults. In 2017, 7.1% of U.S. adults experienced a major depressive episode, with young adults being the most vulnerable. Despite this, only a small fraction of patients receive proper mental health care. In fact, about 70% of individuals with depression go undiagnosed. This project aims to develop a low-cost, automated solution using machine learning to detect depression, bridging the gap between primary care and specialized mental health services.

🎯 Goal
We want to predict depression using data that can typically be found in a patient’s medical record 📋. This prediction could:

Help refer patients to mental health professionals faster 💬.
Flag patients’ files for follow-up during doctor visits 🚩.
Provide an easy way for doctors to initiate conversations about mental health.
📊 Data
Our dataset comes from the CDC National Health and Nutrition Examination Survey (NHANES). We used data from 2005 to 2018, which contains health data for 36,259 U.S. adults.

To predict depression, we used answers from the PHQ-9 depression screening tool 📑. People were labeled as "depressed" if they scored 10 or above on this test.

🔍 Approach
We used various machine learning models to identify which ones performed best in predicting depression. Here’s a breakdown of the methodology:

Data Preprocessing: Feature engineering, handling missing values, and scaling.
Model Selection: Tried multiple models, including logistic regression, linear SVM, SGD classifier, and tree-based models 🌲.
Evaluation: We used the F-beta score, confusion matrices, and ROC-AUC plots to assess model performance 📊.
⚙️ Methods
Our Stochastic Gradient Descent (SGD) classifier emerged as the top-performing model 🎯.

Depressed class accuracy: 71%
Non-depressed class accuracy: 80%
Other models, like XGBoost and Extra Trees, showed promise but required further tuning for better results. Linear models, in general, were the most effective in predicting depression.
![image](https://github.com/user-attachments/assets/6fef4e68-39d4-4e3d-b481-f6d6579c4aa4)

💡 Recommendations
Healthcare professionals should be aware of certain patterns observed in our model:

Patients with memory issues 🧠.
Those with low income, low education, or unable to work 💼.
Patients experiencing sleep problems 🛏️ (too much or too little).
Doctors should be prepared to address these indicators and take the necessary steps for mental health referrals. Tree-based models didn’t perform well for this task, while linear models showed the best results.

![image](https://github.com/user-attachments/assets/18942a8b-467f-4985-ac1c-39b3f7653eb1)


🚀 Future Directions
Try more models: Neural networks could provide better results, though at the cost of interpretability 🧬.
Optimize the dataset: Adding more patient entries rather than features may help reveal patterns while keeping model complexity low.
Experiment with new techniques: Testing different parameter combinations and techniques, like custom F-statistics, could further improve model accuracy ⚙️.
📝 Conclusion
Mental health is a critical, yet often neglected, part of healthcare. Machine learning can bridge this gap by offering a low-cost, scalable solution to predict depression before it worsens. Our project shows promising results, but there is still much to explore!

🔗 References

World Health Organization Depression Overview: https://www.who.int/news-room/fact-sheets/detail/depression

National Institute of Mental Health on Major Depression: https://www.nimh.nih.gov/health/statistics/major-depression.shtml

APA on Psychology in Health Care: https://www.apa.org/health/briefs/primary-care.pdf

JAMA Study on Team-Based Care: https://jamanetwork.com/journals/jama/fullarticle/2545685

PHQ-9 Depression Screener Validation: https://pubmed.ncbi.nlm.nih.gov/11556941/

Feel free to check out the project, and don’t hesitate to contribute! 💻
