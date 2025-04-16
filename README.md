🧠 Objective
To develop an interpretable predictive model that estimates the probability of diabetes based on various personal and lifestyle health indicators. The goal is to support targeted interventions and improve public health strategies.

📊 Dataset Overview
The dataset includes 20+ health-related attributes for each individual:

Target Variable: Diabetes_012 (0 = no diabetes, 1 = prediabetes, 2 = diabetes)

Predictor Variables: HighBP, HighChol, CholCheck, BMI, Smoker, Stroke, HeartDiseaseorAttack, PhysActivity, Fruits, Veggies, HvyAlcoholConsump, AnyHealthcare, NoDocbcCost, GenHlth, MentHlth, PhysHlth, DiffWalk, Sex, Age, Education, Income

🧪 Methodology
Data Preprocessing: Handling missing values, encoding categorical features, and normalizing continuous variables

Exploratory Data Analysis (EDA): Identified trends, correlations, and outliers using plots and statistical summaries

Modeling:

Logistic Regression: For baseline performance and interpretability

Decision Tree Classifier: For uncovering non-linear relationships and rules

Evaluation Metrics: Accuracy, Confusion Matrix, ROC Curve, and Precision-Recall

📌 Key Findings
Most Predictive Health Indicators:

HighBP (High Blood Pressure)

HighChol (High Cholesterol)

BMI (Body Mass Index)

GenHlth (General Health Rating)

DiffWalk (Difficulty Walking)

Best Performing Model: Logistic Regression achieved 95% accuracy, confirming the effectiveness of simple models in health prediction tasks.

📈 Impact on Decision Making
The results of this analysis can assist healthcare providers and policymakers in:

Identifying high-risk individuals early

Implementing lifestyle intervention and screening programs

Designing targeted health campaigns focused on preventable risk factors

🛠️ Tools & Technologies
Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)

Jupyter Notebook

Git & GitHub

This project demonstrates the power of predictive analytics in healthcare using logistic regression and decision tree models to forecast diabetes risk with high accuracy. The analysis identified key health indicators—such as high blood pressure, cholesterol levels, BMI, and general health status—as the most influential predictors of diabetes.

By transforming raw health data into meaningful insights, this project supports data-driven decision-making for healthcare providers and public health policymakers. The models and dashboards developed can be leveraged to:

Guide early detection and targeted interventions

Optimize resource allocation for diabetes prevention programs

Empower individuals with actionable information about their health risks

Overall, this initiative contributes toward improving population health outcomes by bridging the gap between data and practical healthcare solutions.
