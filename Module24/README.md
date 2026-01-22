Network Intrusion Detection Using Machine Learning
Project Overview

Modern computer networks generate massive volumes of traffic, making it difficult to detect malicious activity using traditional rule-based security systems alone. Cyberattacks such as denial-of-service (DoS), port scanning, brute-force attacks, and infiltration attempts can disrupt services, compromise sensitive data, and lead to financial and operational losses.

This capstone project develops a machine-learning-based Network Intrusion Detection System (NIDS) that automatically classifies network traffic as benign or malicious using structured network flow data. The project applies classical supervised machine-learning techniques to a real-world cybersecurity dataset and evaluates their effectiveness through a complete end-to-end data science workflow.

The goal of this project is not only to build accurate models, but also to compare multiple approaches, interpret results clearly, and communicate findings in a way that is understandable to both technical and non-technical audiences.

Dataset

This project uses the CICIDS-2017 dataset, a well-known benchmark dataset created by the Canadian Institute for Cybersecurity. The dataset contains real-world network traffic captured over multiple days and includes both normal traffic and a wide variety of attack types such as:

DoS and DDoS attacks

Port scanning

Brute-force attacks

Infiltration and web-based attacks

The raw dataset consists of multiple CSV files and millions of records. To make modeling computationally feasible and statistically meaningful, the data is cleaned, filtered, and sampled during preprocessing.

Project Structure
├── data/
│   └── (raw and/or processed dataset files)
├── notebooks/
│   └── FinalCapstone.ipynb
├── models/
│   └── saved model files (if applicable)
├── README.md


FinalCapstone.ipynb contains the complete analysis, modeling, visualizations, and results.

All code, outputs, and explanations are organized and clearly labeled for readability and reproducibility.

Methodology

This project follows a structured data science workflow:

1. Data Loading and Cleaning

Combined multiple dataset files into a single dataframe

Removed irrelevant or non-generalizable features (e.g., identifiers and timestamps)

Handled missing, infinite, and invalid values

Verified data quality and consistency

2. Exploratory Data Analysis (EDA)

Examined class distributions and imbalance

Explored key numerical and categorical features

Used visualizations to understand traffic patterns and anomalies

3. Feature Engineering

Selected relevant features for modeling

Encoded categorical variables where necessary

Scaled numerical features for models that require normalization

4. Modeling

Three supervised machine-learning models were trained and evaluated:

Logistic Regression
Used as a baseline linear classifier to establish a performance reference.

Decision Tree Classifier
Provides interpretable, rule-based decisions and insight into feature importance.

Random Forest Classifier
An ensemble approach that improves robustness and generalization by combining multiple decision trees.

Hyperparameter tuning and cross-validation were used where appropriate to improve model performance and reduce overfitting.

5. Model Evaluation

Models were evaluated using clearly defined metrics such as:

Accuracy

Confusion matrices

Classification performance comparisons

Visualizations were used to support interpretation and highlight differences between models.

Results and Findings

All three models successfully learned patterns in network traffic data.

Random Forest achieved the strongest overall performance, demonstrating high accuracy and stability.

Decision Tree offered strong performance with the advantage of interpretability.

Logistic Regression served as a useful baseline but was less effective for complex, non-linear patterns.

The results show that ensemble-based models are particularly well-suited for intrusion detection tasks involving high-dimensional and non-linear data.

Key Takeaways

Machine learning is highly effective for detecting malicious network traffic.

Feature engineering and proper preprocessing significantly impact model performance.

Ensemble methods such as Random Forest provide strong accuracy and robustness.

Clear evaluation metrics and visualizations are essential for interpreting and communicating results.

How to Run the Project

Clone the repository:

git clone <your-github-repo-url>


Install required libraries:

pip install -r requirements.txt


Open the Jupyter Notebook:

jupyter notebook


Run FinalCapstone.ipynb from top to bottom.

Conclusion and Next Steps

This capstone demonstrates a complete, end-to-end application of machine learning to a real-world cybersecurity problem. By comparing multiple classification models and interpreting their results, the project provides practical insights into building effective intrusion detection systems.

Future improvements could include:

Testing additional models (e.g., gradient boosting)

Handling class imbalance with advanced sampling techniques

Evaluating performance on additional intrusion detection datasets

Exploring real-time or streaming-based intrusion detection

Author

Rishitha Chintamreddy
