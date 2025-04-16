Diabetes Health Indicators Analytics

Project Overview:
The aim of this project is to develop an interpretable predictive model that estimates the probability of diabetes based on various personal and lifestyle health indicators. The overarching goal is to support targeted healthcare interventions and enhance public health strategies. By identifying high-risk individuals, the model can assist healthcare providers in crafting personalized prevention and management plans, ultimately improving population health outcomes.

Dataset Overview:
The dataset used in this project includes a wide array of health-related attributes that capture key lifestyle and personal factors:

Target Variable:  
  `Diabetes_012`  
  The target variable indicates the presence or likelihood of diabetes. It takes three values:
  - `0` = No diabetes
  - `1` = Prediabetes
  - `2` = Diabetes

  Predictor Variables:  
  These are the health and lifestyle factors that potentially influence the likelihood of diabetes. Some key predictors include:
  HighBP: High Blood Pressure
  HighChol: High Cholesterol
  BMI: Body Mass Index
  GenHlth: General Health Rating (a subjective self-assessment of general health)
  DiffWalk: Difficulty Walking (a measure of physical limitation)
  Smoker: Whether the individual smokes
  Stroke, HeartDiseaseorAttack: History of stroke or heart disease
  Age, Income, Education: Demographic information

These variables represent various factors that have been linked to the development of diabetes, including metabolic conditions, physical activity levels, socio-economic status, and medical history.

Methodology:

Data Preprocessing:
Before applying predictive models, data preprocessing was necessary to ensure the quality and integrity of the dataset:
Handling Missing Values: Missing data were managed using imputation techniques or removing instances depending on the nature and amount of missing data.
Encoding Categorical Variables: Some variables in the dataset, such as `Sex,` `Smoker,` and `HeartDiseaseorAttack,` are categorical in nature. These were converted to numerical values using one-hot encoding or label encoding.
Normalizing Continuous Variables: Variables like `BMI`, `Age`, and `Income` were normalized to bring them to a similar scale, ensuring that no single variable would disproportionately influence the model due to differing magnitudes.

Exploratory Data Analysis (EDA):
Exploratory Data Analysis was performed to:
Understand the distribution of each variable and identify potential outliers.
Visualize correlations between health indicators and diabetes status to uncover any underlying patterns.
Identify trends in variables such as `BMI,` `Age,` and `GenHlth` that might correlate with higher diabetes prevalence.

Modeling Approach:
Given the objective of predicting diabetes incidence based on various health factors, two modeling approaches were chosen:

1. Logistic Regression:
   - Logistic regression is a widely used statistical model for binary classification problems. In this case, it was applied to predict the likelihood of diabetes occurrence (`0` = no diabetes, `1` = diabetes, or `2` = prediabetes) based on the input variables.
   - The simplicity of logistic regression makes it a strong baseline model. It also provides coefficients that quantify the influence of each predictor on the target variable, which makes the model easy to interpret.

2. Decision Tree Classifier:
   - A decision tree classifier was employed to capture non-linear relationships in the data and to understand complex decision boundaries.
   - This model works by splitting the dataset at each node based on feature values, making it capable of capturing intricate interactions between predictors.
   - Decision trees also provide a clear, visual representation of the decision-making process, which helps in understanding which health indicators contribute most to diabetes risk.

Evaluation Metrics:
To evaluate the model performance, the following metrics were used:
- Accuracy: Proportion of correct predictions made by the model.
- Confusion Matrix: Provides insights into true positives, false positives, true negatives, and false negatives, offering a detailed view of model performance.
- ROC Curve and AUC: These metrics helped evaluate how well the model distinguishes between diabetes classes.
- Precision-Recall Curve: Focuses on evaluating model performance when the dataset is imbalanced (i.e., not all classes are equally represented).

Key Findings:

Most Predictive Health Indicators:
Through the analysis, the following health indicators emerged as the strongest predictors of diabetes:
- High BP (High Blood Pressure): High blood pressure was found to have a strong association with diabetes, likely due to its impact on vascular health and metabolic processes.
- HighChol (High Cholesterol): Cholesterol levels contribute to arterial plaque buildup, which may exacerbate other risk factors for diabetes.
- BMI (Body Mass Index): Obesity and overweight are well-documented risk factors for developing type 2 diabetes.
- GenHlth (General Health Rating): Individuals rating their general health poorly were more likely to develop diabetes, potentially due to undiagnosed or poorly managed health conditions.
- DiffWalk (Difficulty Walking): Physical mobility challenges often correlate with sedentary lifestyles, which are known to increase the risk of diabetes.

Model Performance:
- Logistic Regression achieved 95% accuracy, demonstrating that simple models can perform effectively in predicting diabetes when the right features are used.
- The Decision Tree Classifier performed slightly lower but was still effective in highlighting non-linear patterns and interactions between features.

Impact on Decision Making:
The findings from this analysis have important implications for healthcare providers and policymakers:
- Early Identification of High-Risk Individuals: Predictive models can help identify individuals at high risk of developing diabetes, allowing for earlier interventions.
- Targeted Lifestyle Interventions: By focusing on risk factors such as high blood pressure, cholesterol, and BMI, personalized lifestyle programs can be implemented to reduce diabetes incidence.
- Public Health Campaigns: Policymakers can use these insights to design campaigns that address key risk factors, such as promoting physical activity, healthy diets, and regular health checkups.

Tools & Technologies:
The following tools and libraries were utilized in the analysis:
- Python: Programming language used for data manipulation, analysis, and model building.
  - Libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- Jupyter Notebook: Environment for interactive data exploration and visualization.
- Git & GitHub: This is for version control and project collaboration.

Conclusion:
This project demonstrates the potential of predictive analytics in healthcare, utilizing logistic regression and decision tree models to effectively forecast diabetes risk. The key findings identify specific health indicators—such as high blood pressure, high cholesterol, BMI, and general health rating as the most significant predictors of diabetes.

By leveraging data-driven insights, this project provides healthcare professionals and policymakers with the tools to:
- Identify high-risk individuals early
- Implement targeted interventions for diabetes prevention
- Optimize healthcare resources for diabetes management and education

Overall, the project contributes to improving public health by transforming health data into actionable, personalized, and timely interventions.

