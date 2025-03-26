# Airbnb
# Predicting and Profiling Superhosts: A Data-Driven Strategy for Airbnb

This repository presents a comprehensive data science project that aims to help Airbnb hosts achieve and maintain Superhost status through predictive modeling and clustering techniques. The project was developed as part of the **AI for Business Decisions** course at **Purdue University**.

## 📌 Project Overview

Superhost status on Airbnb is a prestigious badge awarded to top-performing hosts based on criteria such as reviews, responsiveness, and cancellations. However, many hosts are unaware of the key drivers behind this status or how to improve their performance to achieve it.

This project addresses this gap by:
- Predicting which hosts are likely to become Superhosts.
- Identifying at-risk Superhosts and high-potential non-Superhosts through clustering.
- Highlighting key performance indicators that drive Superhost status.

## 🎯 Objectives

1. **Classification Modeling**  
   Build a predictive model to classify whether a host will be a Superhost in the upcoming evaluation period.

2. **Clustering Analysis**  
   Segment Superhosts and non-Superhosts separately to identify:
   - Superhosts at risk of losing their status.
   - Non-Superhosts who are close to achieving Superhost level.

3. **Insight Generation**  
   Identify top drivers influencing Superhost status using data and visual analytics.

## 🗃️ Data Sources

The dataset comprises Airbnb listings in **Chicago**, spanning **8 Superhost evaluation periods**, and includes:

- **Host behavior metrics:** response rates, cancellations, reviews.
- **Listing attributes:** price, bedrooms, bathrooms, instant booking, etc.
- **Superhost history:** past status across periods.
- **Neighborhood demographics:** population density, market competition.

## 🛠️ Methodology

### 1. **Data Cleaning & Preprocessing**
- Missing values handled through:
  - Mode imputation for categorical data.
  - Prior period/neighborhood averages for continuous values.
- Selected and engineered features:
  - Historical Superhost trends.
  - Revenue per room.
  - Instant booking status.
  - Photo count, review counts, response rate, and cancellation rate.

### 2. **Exploratory Data Analysis (EDA)**
- Only about 33% of listings were Superhosts, indicating class imbalance.
- Superhosts showed:
  - Consistently higher average ratings (> 4.8).
  - Higher 5-star review percentages.
  - More listing photos and better responsiveness.
- **Key Insight**: Revenue is not a primary driver — it's supportive but not sufficient alone.

### 3. **Predictive Modeling**
- Models tested: Logistic Regression, Random Forest, XGBoost.
- Evaluation Metrics: Accuracy, Precision, Recall, F1-Score, ROC-AUC.
- Class imbalance handled using SMOTE and stratified sampling.
- **Best performing model**: Random Forest.

### 4. **Clustering & Personas**
Separate KMeans clustering was performed for:
- **Superhosts**:
  - **Power Superhosts** – High performance, high volume. Strategy: retain, reward, expand.
  - **High Quality, Low Volume** – Deliver quality over quantity. Strategy: encourage growth.
  - **At-Risk Superhosts** – May lose status due to recent drops. Strategy: proactive support.

- **Non-Superhosts**:
  - **Emerging Superhosts** 🟢 – Almost there! Strategy: promotion, nudges.
  - **Risky but Strong Hosts** 🟡 – Strong performance with risks (e.g., cancellations). Strategy: operational help.
  - **Quality Concern Power Users** 🔴 – High volume, low guest satisfaction. Strategy: quality improvement programs.

## 📊 Key Takeaways

- Most influential factors:
  - Average rating and 5-star review rate.
  - Host responsiveness and cancellations.
  - Listing quality (photos, amenities, booking flexibility).
- Revenue alone is not predictive—consistency and guest experience matter more.
- Airbnb could implement targeted messaging based on cluster personas to optimize host retention and satisfaction.

## 💡 Business Implications

- **For Airbnb:**  
  Enable internal dashboards to flag at-risk hosts and promote emerging Superhosts with actionable insights.

- **For Hosts:**  
  A clearer path to Superhost status through focus areas like rating quality, responsiveness, and guest experience.

- **For Strategy & Ops Teams:**  
  Persona-based interventions improve host outcomes and reduce churn in the Superhost program.

## 🛠 Tech Stack

- **Languages:** Python
- **Libraries:** pandas, NumPy, scikit-learn, XGBoost, matplotlib, seaborn, Plotly
- **Tools:** Jupyter Notebook, Git, Medium (for blog publication)

## 📖 Blog Article

Read the full write-up here: [Medium Article](https://medium.com/p/2e0331681afa)
