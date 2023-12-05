# Abdominal Trauma Detection

## Overview

This repository contains the implementation and findings of the SpringBoard project on "Detecting Abdominal Trauma" by Eric Wolf. The project focuses on leveraging artificial intelligence (AI) and machine learning to enhance the diagnosis of abdominal trauma, with a specific emphasis on severe injuries to internal abdominal organs.

## Introduction

Traumatic injuries pose a significant global health threat, contributing to millions of annual deaths, particularly in the first four decades of life. Timely and accurate diagnosis is crucial for improving patient outcomes, and computed tomography (CT) has become an indispensable tool for evaluating abdominal injuries. This report explores the potential of AI and machine learning to revolutionize the diagnostic process and assist medical professionals in rapidly and precisely detecting injuries and determining their severity.

## RSNA Abdominal Trauma Detection AI Challenge

The project is aligned with the RSNA Abdominal Trauma Detection AI Challenge, organized in collaboration with the American Society of Emergency Radiology (ASER) and the Society for Abdominal Radiology (SAR). The challenge focuses on building models capable of detecting severe injuries to internal abdominal organs, including the liver, kidneys, spleen, and bowel, as well as identifying any active internal bleeding.

## Method

### Data Source

Data for the project was sourced from 23 research institutions across 14 countries. The challenge dataset consists of de-identified abdominal CT studies and related clinical information. The dataset includes target labels for various organs and indicates the severity of injuries.

### Data Wrangling | Exploratory Data Analysis

A comprehensive examination of the raw training data revealed a well-structured dataset with 3,147 entries and 15 attributes. Key insights from exploratory data analysis include the distribution of reported injuries, analysis of CT scan thickness, and the importance of ensuring data integrity.

### Modeling | Results

After meticulous data cleaning and preprocessing, the dataset underwent conversion from DICOM to PNG images. Four distinct models were selected for evaluation: a baseline model, ResNet-50, EfficientNet B7, and Xception. Bayesian Optimization was employed for hyperparameter tuning.

#### Results Summary

- **Base Model:**
  - Best Loss: 3.159
  - Accuracy: 75.5%
  - Recall: 73.9%
  - Precision: 76.2%
- **ResNet-50:**
  - Best Loss: 0.753
  - Accuracy: 100%
  - Recall: 100%
  - Precision: 100%
- **EfficientNet B7:**
  - Best Loss: 1.050
  - Accuracy: 97.8%
  - Recall: 97.7%
  - Precision: 97.9%
- **Xception:**
  - Best Loss: 1.336
  - Accuracy: 94.8%
  - Recall: 94.5%
  - Precision: 95.0%

The report concludes with the recommendation of ResNet-50 as the final model due to its consistent dominance across critical metrics.

## Future Improvements

The project outlines several areas for future improvements, including the iterative refinement of existing models, exploration of ensemble methods, collaboration with the medical community for validation, investigation of advanced architectures, incorporation of interpretability tools, addressing emerging challenges, and continuous refinement of hyperparameter tuning strategies.

Feel free to explore the code and findings in this repository for a detailed understanding of the project. Contributions and feedback are welcome!

---

*Note: This README is a summary and may require additional details based on the actual project structure and content.*