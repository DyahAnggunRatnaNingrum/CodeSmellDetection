# Do Machine Learning Models Perform Consistently in Code Smell Detection? Analyzing Code Smell Trends in Python Repositorie
This repository implements a **machine learning–based approach for detecting code smells** in Python software projects. The goal is to improve traditional rule-based and threshold-based detection methods by leveraging software metrics and supervised learning models.


## Overview

Code quality often degrades due to time pressure and changing requirements, leading to **technical debt**. One common indicator of technical debt is **code smell**, which reflects poor design or inefficient implementation.

This project focuses on automatically detecting code smells using machine learning and analyzing their distribution and evolution across large-scale Python repositories.


## Code Smells Studied

The following four types of code smells are analyzed:

- Long Method  
- Large Class  
- Data Class  
- Complex Method  


## Dataset

The dataset is constructed from four popular open-source Python repositories on Github:

- Django  
- Matplotlib  
- NumPy  
- SciPy  

### Extracted Features

Each source code entity is represented using software metrics, including:

- Raw Metrics  
- Cyclomatic Complexity  
- Halstead Metrics
- Object Oriented Matrics


## Machine Learning Models

The following models are implemented and evaluated:

- Logistic Regression  
- Random Forest  
- K-Nearest Neighbor (KNN)  
- Multi-Layer Perceptron (MLP)  
- TabNet  


## Evaluation Method

Model performance is evaluated using:

- Stratified 5-Fold Cross-Validation  
- Accuracy  
- Matthews Correlation Coefficient (MCC)  

To assess statistical significance, the following tests are applied:

- Friedman Test  
- Nemenyi Post-hoc Test  


## Analysis

In addition to model comparison, this project analyzes:

- The distribution of code smells across repositories  
- The evolutionary trends of code smells over time  

This analysis provides insights into how code quality changes during software evolution.


## Research Questions

This study is guided by the following research questions:

- **RQ1:** How does hyperparameter tuning affect the performance of different machine learning models in detecting code smells?

- **RQ2:** How computationally efficient are different machine learning models in terms of training time and prediction time?

- **RQ3:** Which machine learning model is most suitable for detecting each type of code smell based on predictive performance and computational efficiency?

- **RQ4:** How are code smells distributed, and how do their trends evolve across different Python repositories when using the best-performing machine learning model?

## Keywords

code smell, machine learning, software engineering, Python, GitHub
