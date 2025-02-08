## Higher Education Students Performance Evaluation

### Introduction
This project analyzes the "Higher Education Students Performance Evaluation" dataset to identify factors affecting academic performance. The study aims to predict students' cumulative GPA and classify performance categories based on various socio-economic and educational factors.

The main research questions include:
1. What are the strongest predictors of cumulative GPA?
2. How do socio-economic factors influence student performance?
3. How do educational habits correlate with academic outcomes?

### Methodology

### Data Collection & Preprocessing
The dataset was obtained from the UCI Machine Learning Repository and includes demographic, academic, and behavioral attributes. The key preprocessing steps involved:
- Removing unique identifiers (e.g., Student ID).
- Checking for and handling missing values.
- Converting categorical variables into factors for analysis.
- Conducting exploratory data analysis (EDA) to understand distributions and relationships.

### Exploratory Data Analysis
EDA included:
- Summary statistics to examine central tendencies and data distribution.
- Histograms and box plots to visualize GPA and performance categories.
- Correlation matrix analysis to identify relationships between variables.

### Modeling Techniques
Two modeling approaches were used:
1. **Regression Models for GPA Prediction**
   - **Linear Regression:** Establishes a baseline model to analyze the impact of each factor on GPA.
   - **Random Forest Regression:** Captures non-linear relationships and interactions between variables.

2. **Classification Models for Student Performance Categories**
   - **Logistic Regression:** Predicts students’ likelihood of falling into low, medium, or high-performance categories.
   - **K-Nearest Neighbors (KNN):** A non-parametric model that categorizes students based on similarity to peers.

### Model Evaluation
- **Regression Models:** Evaluated using Mean Squared Error (MSE).
- **Classification Models:** Assessed based on accuracy, precision, recall, and ROC curves.
- **Cross-validation:** Applied for model robustness.

## Results

### Regression Model Findings
- **Linear Regression** achieved an MSE of **4.24**, indicating its limitations in handling complex, non-linear relationships.
- **Random Forest Regression** outperformed Linear Regression with an MSE of **2.70**, explaining **47.36%** of GPA variance. Key predictors included:
  - **Educational habits (X29)**
  - **Weekly study hours (X20)**
  - **Course ID (COURSE.ID)**

### Classification Model Findings
- **Logistic Regression** failed to converge due to dataset complexity, yielding an accuracy of **0.00%**.
- **KNN Classification** achieved an accuracy of **88.1%**, effectively categorizing students into Low, Medium, and High-performance groups.
- The **ROC curve for KNN** demonstrated strong classification performance, especially in distinguishing high-performing students.

## Conclusion
The study identified significant factors influencing academic performance, with structured study habits and educational background playing a critical role in GPA prediction.
- **Random Forest Regression** proved to be the most effective model for GPA prediction due to its ability to capture complex patterns.
- **KNN Classification** emerged as the most reliable method for categorizing student performance.
- Socio-economic factors, including parental education and income, also contributed to academic outcomes.

### Recommendations
1. **Academic Support:** Institutions should focus on structured study programs to improve GPA.
2. **Parental Engagement:** Enhancing family involvement in education may positively impact performance.
3. **Course-Specific Strategies:** Identifying challenging courses and providing targeted support can help improve outcomes.

## Future Work
Future research can expand on:
- Incorporating additional data sources, such as extracurricular activities and psychological factors.
- Exploring deep learning models for improved predictions.
- Conducting interventions based on predictive insights to enhance student success.

This project showcases the power of machine learning in education analytics and highlights the importance of data-driven decision-making in academic institutions.

