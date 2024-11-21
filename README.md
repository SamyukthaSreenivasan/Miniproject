# FIBROVISION: OPENCV POWERED INSIGHTS FOR IPF PROGRESSION
## Problem Statement
Idiopathic Pulmonary Fibrosis (IPF) is a life-threatening lung disease characterized by progressive scarring of lung tissue, leading to difficulty in breathing. Despite advances, predicting disease progression is complex due to its diverse impact on patients. Timely early diagnosis and personalized treatment plans are critical for improving patient outcomes.

## Aim
To develop an AI-powered predictive system using clinical and imaging data (CT scans) to predict the progression of IPF. This system will help clinicians make data-driven decisions regarding disease management, improving patient outcomes.

## Objectives
Data Preprocessing: Efficiently prepare clinical and imaging data for machine learning models.
Predictive Modeling: Use advanced algorithms like Gradient Boosting to predict Forced Vital Capacity (FVC) and disease progression.
CT Scan Image Analysis: Integrate medical imaging with clinical data for more accurate predictions.
Hyperparameter Optimization: Fine-tune the model for optimal performance using RandomizedSearchCV.
Evaluation: Assess the model's effectiveness using Mean Absolute Error (MAE).

## Methodology
![image](https://github.com/user-attachments/assets/a283a099-a635-41a8-b552-82c787a8ef00)

### Data Preprocessing
Clinical Data: Handle missing values, encode categorical features, and scale numerical data.
Image Preprocessing: Use OpenCV for segmentation and calculate disease spread from CT scans.

### Model Development
Gradient Boosting Regressor (GBR):
Used for prediction, GBR enhances model accuracy through iterative corrections, making it a powerful method for regression tasks.
Hyperparameter tuning with RandomizedSearchCV helps optimize the model’s performance.

### CT Scan Image Analysis
Image Segmentation using OpenCV helps identify regions of interest (ROIs) in CT scans.
Disease Spread Score: A measure of the extent of lung fibrosis is calculated and integrated into the model.

### Model Evaluation
Mean Absolute Error (MAE): Measures prediction accuracy, with the goal to minimize MAE for the most accurate predictions.

## Streamlit Integration
Streamlit is used to create an interactive web application for IPF progression prediction. It allows clinicians and researchers to upload clinical data and CT scans, and receive real-time predictions of disease progression.


## Output
![image](https://github.com/user-attachments/assets/4e43587d-b88a-4b1b-b549-023fb63910b8)

![image](https://github.com/user-attachments/assets/2eeb8269-d899-4098-910a-a719b8856f20)

![image](https://github.com/user-attachments/assets/038a1380-e2af-4f93-be22-841f6400ab66)

![image](https://github.com/user-attachments/assets/5d84a662-dd3c-4504-b98b-42410493d168)

![image](https://github.com/user-attachments/assets/a7620446-2f98-4aaa-ba98-251b9df941df)

## Results
Predictive Performance: The Gradient Boosting model achieved a low MAE, ensuring high accuracy in predicting disease progression.
Disease Spread Visuals: The CT scan analysis showed clear visualizations of lung fibrosis severity, helping to track the extent of disease.
Clinical Data Integration: Using clinical data such as age, sex, and FVC significantly improved the model’s prediction accuracy.

## Conclusion
This AI-powered system integrates clinical data and medical imaging to predict the progression of Idiopathic Pulmonary Fibrosis (IPF). By incorporating machine learning models like Gradient Boosting and CT scan analysis, the system can predict disease progression with high accuracy, improving patient management.

Streamlit provides a user-friendly interface, allowing clinicians to easily interact with the model, making real-time predictions for personalized treatment.

## Key Highlights

### Terminologies:
Forced Vital Capacity (FVC): A critical measure of lung function.
CT Scan Segmentation: Key technique for assessing the spread of fibrosis.
Gradient Boosting: A powerful regression technique that iteratively improves predictions.
Mean Absolute Error (MAE): A metric used to assess the model's accuracy.
### Techniques Used:
Gradient Boosting Regressor for prediction.
RandomizedSearchCV for hyperparameter tuning.
OpenCV for image segmentation.
Streamlit for creating an interactive web app.

## Future Work
Refinement of the model with more advanced image processing techniques like Convolutional Neural Networks (CNNs).
Incorporating longitudinal data to improve the prediction of disease progression over time.
Deployment in clinical settings for real-time use.
Together, these techniques offer a powerful solution to predict the progression of IPF, improving clinical decision-making and enhancing patient outcomes.
