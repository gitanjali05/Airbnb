# Airbnb Superhost Prediction & Clustering

This project predicts Airbnb Superhost status and segments hosts using machine learning. Built as part of Purdue’s *AI for Business Decisions* course.

## 🔍 Project Goals
- Predict if a host will become a Superhost using historical listing data.
- Cluster hosts to identify top performers, at-risk Superhosts, and high-potential non-Superhosts.
- Provide actionable insights to Airbnb and hosts.

## 📊 Dataset
- 8 Superhost evaluation periods from Airbnb listings in Chicago.
- Features include: review scores, responsiveness, cancellations, revenue, photos, listing type, etc.

## ⚙️ Methods
- **Models**: Logistic Regression, Random Forest
- **Clustering**: KMeans (separately for Superhosts and non-Superhosts)
- **Key Metrics**: Accuracy, F1-score, ROC-AUC

## 💡 Insights
- Revenue is not a strong standalone predictor.
- Key drivers: 5-star review rate, responsiveness, cancellations, photo count.
- Defined personas:
  - **Power Superhosts** – reward & retain
  - **At-Risk Superhosts** – intervene early
  - **Emerging Superhosts** – promote
  - **Quality Concern Users** – improve

## 🛠 Tech Stack
Python, pandas, scikit-learn, matplotlib, seaborn

## 📖 Medium Article
[Read full story](https://medium.com/p/2e0331681afa)
