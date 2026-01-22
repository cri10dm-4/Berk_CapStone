# Network Intrusion Detection Using Machine Learning

## Project Overview

Modern computer networks generate massive volumes of traffic, making it difficult to detect malicious activity using traditional rule-based security systems. Cyberattacks such as denial-of-service (DoS), port scanning, brute-force attacks, and infiltration attempts can disrupt services, compromise sensitive data, and result in significant financial and operational losses.

This capstone project develops a **machine-learning-based Network Intrusion Detection System (NIDS)** that automatically classifies network traffic as **benign** or **malicious** using structured network flow data. The project applies classical supervised machine-learning techniques and evaluates their effectiveness through a complete end-to-end data science workflow.

This repository contains the **full capstone project**, including data preparation, feature engineering, model training, validation, evaluation, and final findings.

---

## Dataset

The project uses the **CICIDS-2017** dataset, a widely recognized real-world benchmark dataset created by the Canadian Institute for Cybersecurity. The dataset contains network traffic representing both normal behavior and multiple categories of cyberattacks, including:

- DoS and DDoS attacks  
- Port scanning  
- Brute-force attacks  
- Infiltration and web-based attacks  

The raw dataset consists of multiple CSV files and millions of records. During preprocessing, the data is cleaned, filtered, and sampled to ensure quality, balance, and computational feasibility.

---

## Project Structure

├── FinalCapstone.ipynb
└── README.md

- **FinalCapstone.ipynb** contains the complete analysis, modeling, visualizations, and results.
- All files and directories are named and organized for clarity and reproducibility.

---

## Methodology

This project follows a structured data science workflow:

### Data Cleaning and Preprocessing
- Combined multiple dataset files into a single dataframe
- Removed non-generalizable features such as identifiers and timestamps
- Handled missing, infinite, and invalid values
- Ensured data consistency and quality

### Exploratory Data Analysis (EDA)
- Analyzed class distributions and potential imbalance
- Explored key numerical and categorical features
- Used visualizations to understand traffic patterns and anomalies

### Feature Engineering
- Selected relevant features for modeling
- Encoded categorical variables where necessary
- Scaled numerical features for models requiring normalization

### Modeling
Three supervised machine-learning models were implemented and compared:

- **Logistic Regression** – baseline linear classification model  
- **Decision Tree** – interpretable, rule-based classifier  
- **Random Forest** – ensemble model for improved accuracy and generalization  

Hyperparameter tuning and cross-validation were applied to improve performance and reduce overfitting.

### Model Evaluation
Models were evaluated using clearly defined metrics, including:
- Accuracy
- Confusion matrices
- Comparative performance analysis across models

Visualizations were used to support interpretation and highlight differences in model behavior.

---

## Results and Findings

- All three models successfully learned meaningful patterns in network traffic data.
- **Random Forest** achieved the strongest overall performance, demonstrating high accuracy and stability.
- **Decision Tree** performed well while offering interpretability of decision rules.
- **Logistic Regression** served as a strong baseline but was less effective for complex, non-linear patterns.

The results indicate that ensemble-based models are particularly well-suited for intrusion detection tasks involving high-dimensional network data.

---

## Key Takeaways

- Machine learning is highly effective for detecting malicious network traffic.
- Data cleaning and feature engineering significantly impact model performance.
- Random Forest provides the best balance of accuracy and robustness.
- Clear evaluation metrics and visualizations improve interpretability and communication of results.

---

## How to Run the Project

1. Clone the repository:
   git clone <your-github-repository-url>
2. Install required dependencies:
   pip install -r requirements.txt
3. Launch Jupyter Notebook:
   jupyter notebook
4. Open and run:
   FinalCapstone.ipynb

## Conclusion and Next Steps

This capstone demonstrates a complete, end-to-end application of machine learning to a real-world cybersecurity problem. By comparing multiple classification models and interpreting their results, the project provides practical insights into building effective intrusion detection systems.

Potential future improvements include:

- Testing additional machine-learning models  
- Addressing class imbalance using advanced sampling techniques  
- Evaluating performance on additional intrusion detection datasets  
- Exploring real-time intrusion detection systems  


