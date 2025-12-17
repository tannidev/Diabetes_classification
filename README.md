#Diabetes Prediction Using Health Indicators
This project focuses on predicting whether an individual has diabetes using health and lifestyle indicators. The analysis is based on the **Diabetes Health Indicators Dataset** from Kaggle, derived from the CDC BRFSS 2021 survey. The task is formulated as a **binary classification problem** using multiple machine learning models .



---



## Dataset



The project uses three datasets from Kaggle:



* **diabetes_012_health_indicators.csv**



&nbsp; * Multi-class: No diabetes, Prediabetes, Diabetes

* **diabetes_binary_5050split_health_indicators.csv**



&nbsp; * Binary and balanced dataset

* **diabetes_binary_health_indicators.csv**



&nbsp; * Binary and imbalanced dataset



A **merged dataset** was created by combining all three datasets and converting the multi-class labels into a single binary label (diabetes vs no diabetes), resulting in **539,892 records** .



---



## Features



The datasets include health and demographic indicators such as:



* Blood pressure, cholesterol, BMI

* Smoking and alcohol consumption

* Physical activity, diet (fruits/vegetables)

* General, mental, and physical health

* Age, sex, education, and income



---



## Methodology



* Data preprocessing and validation (no missing values)

* Feature scaling using **StandardScaler**

* Data split:



&nbsp; * 70% Training

&nbsp; * 10% Validation

&nbsp; * 20% Testing

* Performance metrics:



&nbsp; * Accuracy

&nbsp; * Precision

&nbsp; * Recall

&nbsp; * F1 Score 



---



## Models Used



The following machine learning models were implemented and evaluated:



* Logistic Regression

* K-Nearest Neighbors (KNN)

* Bagged Decision Tree

* Random Forest

* XGBoost Classifier



---



## Results (Merged Dataset)



| Model                | Accuracy | Precision | Recall   | F1 Score |
| -------------------- | -------- | --------- | -------- | -------- |
| Logistic Regression  | 0.82     | 0.79      | 0.82     | 0.79     |

| KNN                  | 0.82     | 0.81      | 0.82     | 0.81     |

| Bagged Decision Tree | **0.95** | **0.95**  | **0.95** | **0.95** |

| Random Forest        | **0.95** | **0.95**  | **0.95** | **0.95** |

| XGBoost              | 0.84     | 0.82      | 0.84     | 0.81     |


Bagged Decision Tree and Random Forest achieved the best overall performance on the merged dataset .



---



## Conclusion

This project demonstrates the effectiveness of machine learning for early diabetes detection using health indicators. Ensemble models performed especially well on larger, merged datasets. The results highlight the potential of ML-based decision support systems in healthcare applications .

---

## References
* Diabetes Health Indicators Dataset (Kaggle): https://www.kaggle.com/datasets/julnazz/diabetes-health-indicators-dataset

---


