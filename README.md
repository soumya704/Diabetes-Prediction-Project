# Diabetes-Prediction-Project
Diabetes Prediction Project in Human Being


📝 Project Summary: Diabetes Prediction System

This project focuses on building a Diabetes Prediction System using the Pima Indians Diabetes Dataset. The aim was to analyze patient health parameters and develop machine learning models that can accurately predict whether an individual is diabetic (Outcome=1) or not (Outcome=0).

🔍 Exploratory Data Analysis (EDA)

Performed data inspection using .head(), .info(), and .describe() to understand the structure.

Identified missing or invalid values (0 entries in medical columns such as Glucose, BloodPressure, Insulin, SkinThickness, and BMI).

Replaced these invalid entries with mean/median imputation to clean the dataset.

Visualized relationships and distributions using:

Correlation Heatmap → revealed strong correlation of Glucose and BMI with diabetes outcome.

KDE plots & Violin plots → showed how features like Urea, Glucose, and BMI varied across diabetic vs. non-diabetic patients.

Boxplots → detected skewness and outliers.

⚙️ Preprocessing

Separated features (X) and target (y).

Split dataset into training (67%) and testing (33%) sets using train_test_split.

Normalized & handled imbalanced values for stable training.

🤖 Model Training

Implemented multiple models for prediction:

K-Nearest Neighbors (KNN)

Tested neighbors from 1–10.

Observed training vs. testing accuracy trends to avoid overfitting.

Decision Tree Classifier

Trained with different max_depth values.

Generated accuracy vs. depth graph.

Controlled complexity to balance bias-variance trade-off.

(Optional in your notebook but recommended) Models like Logistic Regression, Random Forest, and SVM can also be added for better benchmarking.

📊 Model Evaluation

Accuracy scores compared between models and parameter settings.

For Decision Tree:

Lower depth → underfitting but more generalization.

Higher depth → risk of overfitting (training accuracy ↑, test accuracy ↓).

Confusion Matrix and Classification Report (Precision, Recall, F1-score) highlighted model performance beyond raw accuracy.

🎯 Final Prediction

Built a prediction function where a new patient’s medical values (Glucose, BP, BMI, Insulin, etc.) can be entered to predict the likelihood of diabetes.

✅ Conclusion

Glucose, BMI, Insulin, and SkinThickness are critical indicators in predicting diabetes.

Decision Tree with tuned depth achieved a good balance between accuracy and interpretability.

The system demonstrates how machine learning can aid healthcare by providing an early-warning tool for diabetes detection.
