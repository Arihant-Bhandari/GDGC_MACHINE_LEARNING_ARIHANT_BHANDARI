# GDGC_MACHINE_LEARNING_ARIHANT_BHANDARI

* DATASET LINK: https://www.kaggle.com/datasets/lainguyn123/student-performance-factors

* Features:

| Attribute | Description |
|-----------|-------------|
| Hours_Studied | Number of hours spent studying per week. |
| Attendance | Percentage of classes attended. |
| Parental_Involvement | Level of parental involvement in the student's education (Low, Medium, High). |
| Access_to_Resources | Availability of educational resources (Low, Medium, High). |
| Extracurricular_Activities | Participation in extracurricular activities (Yes, No). |
| Sleep_Hours | Average number of hours of sleep per night. |
| Previous_Scores | Scores from previous exams. |
| Motivation_Level | Student's level of motivation (Low, Medium, High). |
| Internet_Access | Availability of internet access (Yes, No). |
| Tutoring_Sessions | Number of tutoring sessions attended per month. |
| Family_Income | Family income level (Low, Medium, High). |
| Teacher_Quality | Quality of the teachers (Low, Medium, High). |
| School_Type | Type of school attended (Public, Private). |
| Peer_Influence | Influence of peers on academic performance (Positive, Neutral, Negative). |
| Physical_Activity | Average number of hours of physical activity per week. |
| Learning_Disabilities | Presence of learning disabilities (Yes, No). |
| Parental_Education_Level | Highest education level of parents (High School, College, Postgraduate). |
| Distance_from_Home | Distance from home to school (Near, Moderate, Far). |
| Gender | Gender of the student (Male, Female). |
| Exam_Score | Final exam score. |

* Objective: Creating ML models based on given data.

* Task type: **Regression** / **Classification**

---

* Current Models: 

1. **CNN (1D CONV)** (Best trained model)

Mean Absolute Error: 0.7680674906699888

Root Mean Square Error: 2.057193799923042

2. **Linear Regression**

Mean Absolute Error: 1.031871259932816

Root Mean Square Error: 2.1871791291732707

---

* Task type: **Classification** (if Exam_Score is binned into Grade)

* Current Models: 

1. **CNN (1D CONV)** (Best trained model)

Accuracy: 95.36%

Precision (weighted): 95.38%

Recall (weighted): 95.36%

F1 Score (weighted): 95.35%

2. **Logistic Regression**

Accuracy: 85.58%

Precision (weighted): 84.92%

Recall (weighted): 85.58%

F1 Score (weighted): 85.11%

3. **K-Nearest Neighbors**

Accuracy: 94.35%

Precision (weighted): 94.28%

Recall (weighted): 94.35%

F1 Score (weighted): 94.24%

---

* Pipeline:

1. Data Exploration: Loading the data, printing top and bottom 5 values, printing shape of the data

2. Exploratory Data Analysis (EDA): printing various graphs like histplots for numerical and countplots for categorical features, feature information, numerical features' statistics, presence of null or duplicate values

3. Data Imputation and Encoding: Scikit-Learn Pipeline

4. Model Creation and Model Evaluation

a. Regression (target = Exam_Score)

splitting data into training : validation : testing = 70:15:15 

Applying on conv1d + dense layer based CNN model and a linear regression model.

b. Classification (target = Grade or binned Exam_Score)

Binning Exam_Score into Grade to obtain categories to apply metrics like Accuracy, Precision, Recall and F1-score.

splitting data into training : validation : testing = 70:15:15 

Applying on conv1d + dense layer based CNN model, k-nearest neighbors model and a logistic regression model.

---

*NOTE: Appropriate comments and analysis have been provided for both data and model.*

*NOTE: Run both task separately for no data leakage.*