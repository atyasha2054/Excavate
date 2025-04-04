# 💡 CHEMSPARK: Machine Learning Model for Material Classification and Band Gap Prediction

![banner](https://img.shields.io/badge/ML-Materials%20Science-blue) ![python](https://img.shields.io/badge/Python-ML-green) ![status](https://img.shields.io/badge/Status-Completed-brightgreen)

### 📌 Team BizGenius (1st Runner Up at Excavate event of COMPOSIT'25)

---

## 🌟 Overview

**CHEMSPARK** is an AI-driven project designed to accelerate **materials discovery** by predicting the electronic behavior of **perovskite oxides**—materials widely used in **solar cells, semiconductors, batteries, and optoelectronics**. We developed two robust machine learning models to:
- 🔍 **Classify** perovskites as **insulators** or **non-insulators**.
- 🎯 **Predict** the **exact band gap** of insulating materials.

---

## 🧪 Motivation

Perovskite oxides have tunable properties making them excellent candidates for electronic applications. One of their defining traits is the **band gap (Eg)**, which determines whether a material is a **conductor**, **semiconductor**, or **insulator**. Traditional experimentation is costly and time-consuming—our solution? **Machine learning!**

---

## 📊 Dataset & Preprocessing

- 📦 **5152 perovskite compositions**
- 🔍 Features: Atomic, structural, and electronic properties
- ✅ Preprocessing:
  - Data cleaning
  - Feature selection via correlation analysis
  - Label encoding & normalization
  - Train-test split (80:20)

---

## 🧠 Models

### 1️⃣ Binary Classification Model (Model 1)

- 🔧 **Algorithm**: `RandomForestClassifier (n=100)`
- 🎯 **Target**: `is_insulator` (1 = Insulator, 0 = Non-Insulator)
- 📈 **Accuracy**: 93%
- 📌 Key Insight: Feature importance revealed predictors like HOMO levels and atomic radii.

### 2️⃣ Regression Model for Band Gap Prediction (Model 2)

- 🔧 **Algorithm**: `XGBoost Regressor` (with GridSearchCV tuning)
- 🎯 **Target**: Exact `PBE Band Gap (Eg in eV)` for insulating materials
- 📊 Features: Both encoded categorical and correlated numerical features
- ✅ **Evaluation**: R² score, residual analysis, actual vs predicted plots
- 💾 Model saved using `pickle` for future use.

---

## 📈 Analysis & Insights

- 🔍 **Feature Importance**: A-site oxidation state (A_OS), B_OS, atomic radii, and electron affinity are highly influential.
- 📉 **Residual Analysis**: Distribution centered around zero, minimal bias.
- 📐 **Prediction Quality**: High correlation between actual and predicted values.

---

## 📊 Visual Dashboard

- 🧩 Created an interactive **Power BI dashboard** for in-depth exploratory analysis and visualization of trends in band gap behavior.

---

## 🔬 Real-World Applications

| Domain                      | Application |
|----------------------------|-------------|
| ☀️ Solar Cell Design       | Select perovskites with optimal band gaps for energy efficiency |
| 💾 Semiconductor Industry  | Engineer materials for transistors and circuits |
| 🔋 Battery Tech            | Discover materials for next-gen energy storage |
| 📺 Display Technology      | Improve performance of LEDs and OLEDs |

---

## 📚 References

- **Chen et al.**: *"Correlation between Band Gap Energy and Chemical Bonding of Oxide Perovskites"*
- **Sun et al.**: *"Machine Learning for Perovskite Materials Design and Discovery"*
- **Zhang et al.**: *"Data-Driven Band Gap Prediction Using Machine Learning"*

---

## ✅ Conclusion

Our work demonstrates the power of ML in revolutionizing **materials science**, cutting down experimental overhead and uncovering actionable insights. Both models—**classification and regression**—achieved high performance, providing a scalable solution for future research and industrial applications.

---

## 🚀 Future Work

- 🧠 Integrate **deep learning** architectures
- 🧬 Enrich the dataset with more diverse chemical descriptors
- 🧪 Combine with **real-time experimental validation**
- 🌍 Build a complete **AI-powered materials discovery platform**

---

## 🧑‍💻 Contributors

- **Sandeep Sarkar**  
- **Atyasha Bhattacharyya**  
- **Subhanjan Saha**
