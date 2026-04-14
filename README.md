# Big Data Analytics for Intelligent Resume Screening and Workforce Classification

This repository contains an end-to-end implementation for classifying resumes using Apache Spark (PySpark) and Machine Learning. The project leverages Big Data technologies to process unstructured text at scale.

## 🚀 Key Improvements & Fixes
- **Robust Data Ingestion**: Added `multiLine=True` to Spark CSV reading to handle complex, multi-line HTML fields common in resume datasets.
- **Data Quality**: Implemented advanced filtering to remove garbage HTML labels, ensuring accurate model training and clean EDA visualizations.
- **Environment Compatibility**: Optimized for Python 3.12+ by including `setuptools` and `packaging` dependencies.
- **Optimized Performance**: Configured Java `ReservedCodeCacheSize` to prevent execution stalls during large-scale processing.

## 📊 Project Overview
Intelligently categorizes over 2,400 resumes into 24 diverse job categories using:
- **Distributed Processing**: Apache Spark for ETL and feature extraction.
- **NLP Pipeline**: Tokenization, StopWords removal, and TF-IDF vectorization.
- **Machine Learning**: Logistic Regression and Naive Bayes classifiers via Spark MLLib.

## 📁 Repository Contents
1. `Resume_Classification_PySpark.ipynb`: Main Jupyter Notebook with EDA, Pipeline, and Model Evaluation.
2. `requirements.txt`: Python dependencies optimized for the latest environments.
3. `dataset/`: The Resume dataset (CSV and partitioned raw files).

## 🛠️ Getting Started

### Prerequisites
- Python 3.8+ (Tested on 3.13)
- Java 8 or 17 (Required for Apache Spark)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/KeyZama10/-Big-Data-Analytics-for-Intelligent-Resume-Screening-and-Workforce-Classification.git
   cd -Big-Data-Analytics-for-Intelligent-Resume-Screening-and-Workforce-Classification
   ```
2. Create and activate a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Notebook
```bash
jupyter notebook Resume_Classification_PySpark.ipynb
```

## 📈 Results
The model achieves a baseline accuracy of ~57% with Logistic Regression, demonstrating the effectiveness of distributed NLP pipelines on messy, unstructured resume data.
