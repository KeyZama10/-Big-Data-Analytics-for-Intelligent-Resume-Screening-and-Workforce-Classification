# Big Data Analytics for Intelligent Resume Screening and Workforce Classification

This repository contains the complete implementation code for the BDA & ML project focusing on Resume Classification using Apache Spark (PySpark).

## Project Overview
Unstructured text data, such as resumes, is generated at an immense volume and velocity globally. This project leverages the **Big Data Analytics (BDA)** ecosystem directly with **Machine Learning (ML)** to intelligently categorize over 2,400 resumes into 24 diverse job categories.

- **Dataset**: `Resume.csv` containing raw unstructured textual resumes and labels.
- **Processing Layer**: Apache Spark (PySpark) handles distributed DataFrame ETL, Tokenization, and TF-IDF extraction.
- **Machine Learning**: Utilized Spark MLLib (Logistic Regression and Naive Bayes) for highly scalable, distributed classifier creation.

## Repository Contents
1. `Resume_Classification_PySpark.ipynb`
   - Complete End-to-End flow:
   - Data Ingestion & Preprocessing (SparkSQL Functions).
   - Exploratory Data Analysis (EDA) visualized through Seaborn.
   - Distributed Machine Learning Pipeline architecture.
2. `requirements.txt`
   - All necessary dependencies to run the notebook locally or on instances.
3. `dataset/`
   - The original dataset partitioned by classification.

## Getting Started
Ensure you have Apache Spark installed alongside Python 3.

```bash
pip install -r requirements.txt
jupyter notebook Resume_Classification_PySpark.ipynb
```

Execute cells sequentially to evaluate Model Accuracy, Precision, Recall, F1 Scores and generate insights on workforce data automation.
