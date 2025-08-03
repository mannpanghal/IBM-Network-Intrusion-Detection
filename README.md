# Network Intrusion Detection using Machine Learning on IBM Cloud

This repository contains the code and documentation for a capstone project focused on building a **Network Intrusion Detection System (NIDS)**. The project was developed as part of the IBM SkillsBuild program.

---

## Table of Contents
- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Technology Stack](#technology-stack)
- [Methodology](#methodology)
- [Results](#results)
- [How to Run](#how-to-run)

---

## Project Overview
This project demonstrates the development of a robust NIDS using a **data-driven approach**.  
A machine learning model was trained on a labeled dataset to learn the patterns of normal network traffic versus various types of cyber-attacks.  
The entire workflow, from data preparation to model evaluation, was conducted on the **IBM Cloud** platform using **Watson Studio**.

---

## Problem Statement
The challenge is to create a system capable of analyzing network traffic data to automatically identify and classify malicious activities (like **Denial of Service**, **Probes**, etc.) and distinguish them from normal, legitimate traffic, thereby enhancing network security.

---

## Technology Stack
- **Cloud Platform:** IBM Cloud (Lite Plan)
- **Primary Service:** IBM Watson Studio
- **Development Tool:** Jupyter Notebook
- **Programming Language:** Python 3.11
- **Key Libraries:**
  - `pandas`: For data loading and manipulation.
  - `scikit-learn`: For building, training, and evaluating the machine learning model.

---

## Methodology
1. **Data Preparation:**  
   - The raw dataset from Kaggle was loaded into IBM Cloud Object Storage.  
   - Text-based features (like protocol type, service, flag) were converted into a numerical format using Label Encoding.

2. **Model Selection:**  
   - A **Decision Tree Classifier** was chosen for its effectiveness and interpretability.

3. **Training:**  
   - The model was trained on 80% of the dataset within a Jupyter Notebook running on IBM Watson Studio.

4. **Evaluation:**  
   - The trained model's performance was evaluated on the remaining 20% of the data (the test set) to measure its accuracy on unseen data.

---

## Results
The trained **Decision Tree** model demonstrated **excellent performance** in identifying network intrusions.

- **Final Model Accuracy:** `99.58%`

This high accuracy proves that the machine learning approach is a highly effective and viable solution for building a modern Network Intrusion Detection System.

---

## How to Run
1. Download the dataset from the Kaggle link.  
2. Create a project in **IBM Watson Studio**.  
3. Upload the `Train_data.csv` and `Test_data.csv` files as data assets.  
4. Create a new **Jupyter Notebook** (`.ipynb`).  
5. Follow the steps outlined in the `NIDS-Model.ipynb` file to load the data, train the model, and evaluate its performance.
