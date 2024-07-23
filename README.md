# Student Performance Prediction

## Overview

This project focuses on analyzing student performance to predict outcomes for new students based on historical data. Using a machine learning model trained on existing data, we predict various performance metrics for new students. The model and its application are hosted on AWS to leverage cloud computing benefits such as scalability, reliability, and accessibility.

## Dataset

The dataset used (`stud.csv`) contains various features related to student's academic and personal backgrounds. Key attributes include study hours, previous scores, and demographic information which are crucial for predicting their academic success.

### Columns in the Dataset

- `Student_ID`: Unique identifier for each student.
- `Study_Hours`: Number of hours spent studying per week.
- `Previous_Scores`: Scores from previous tests.
- `Age`: Age of the student.
- `Gender`: Gender of the student.
- `Attendance`: Attendance percentage.

## Model

The predictive model is built using Python's scikit-learn library. We've employed a RandomForestClassifier, chosen for its robustness and ability to handle non-linear data efficiently.

### Training the Model

The model is trained on 80% of the data, with 20% reserved for testing to validate the model's accuracy.

### Model Accuracy

The model achieved an accuracy of approximately 85%, indicating a strong ability to generalize on unseen data.

## Deployment

The application is deployed on AWS, utilizing several services:

- **Amazon EC2**: Hosts the web application allowing users to interact with the model in real-time.
- **Amazon S3**: Stores the dataset and the trained model securely.
- **AWS Lambda**: Manages the model's prediction requests, ensuring efficient scaling and cost management.
- **Amazon RDS**: Manages structured student data in a relational database to enhance query performance and data integrity.
