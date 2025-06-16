# 🌿 Indoor Plant Health: Prediction & Care Clustering

This project aims to predict plant health and identify care-based clusters using a dataset of indoor plants. It combines supervised learning for health score prediction with unsupervised learning for care pattern clustering. The pipeline includes data analysis, preprocessing, feature engineering, model training, and evaluation.

---

## 📌 Project Overview

Understanding how environmental factors and daily care affect plant health is essential for home gardeners and smart garden systems. This project uses a realistic dataset containing care metrics and environmental parameters to:

* Predict plant health scores (1=Dying to 5=Thriving)
* Identify critical features that impact plant health
* Cluster similar plants into groups based on care requirements

---

## 🧠 Features & Techniques

* ✅ Data Loading and Exploration
* ✅ Data Cleaning and Preprocessing (missing values, text parsing, encoding)
* ✅ Feature Engineering (e.g., Watering\_Per\_Day\_ml, Sunlight\_Duration\_hrs, extracting features from Health\_Notes)
* ✅ Exploratory Data Analysis (distributions, heatmaps, boxplots)
* ✅ Supervised Learning (Random Forest Classifier)
* ✅ Hyperparameter Tuning (GridSearchCV)
* ✅ Feature Importance Analysis
* ✅ Unsupervised Learning (K-Means Clustering, Elbow Method, Cluster Profiling)

---

## 📂 Dataset

The **Indoor Plant Health & Growth** dataset includes 1,000 rows and 17 columns:

* `Plant_ID`: Unique plant identifier
* `Height_cm`, `Leaf_Count`, `New_Growth_Count`: Growth metrics
* `Health_Notes`: Qualitative description of plant health
* `Watering_Amount_ml`, `Watering_Frequency_days`: Water care features
* `Sunlight_Exposure`: Text description of light exposure
* `Room_Temperature_C`, `Humidity_%`: Environmental readings
* `Fertilizer_Type`, `Fertilizer_Amount_ml`: Fertilization data
* `Pest_Presence`, `Pest_Severity`: Pest impact
* `Soil_Moisture_%`, `Soil_Type`: Soil condition
* `Health_Score`: Target label (1 to 5)

---

## 🛠️ Tech Stack

* **Language**: Python
* **Libraries**:

  * `pandas`, `numpy`
  * `matplotlib`, `seaborn`
  * `scikit-learn`
  * `re` (for parsing `Health_Notes`)

---

## 📊 Exploratory Data Analysis

* Correlation heatmaps between numeric features and health score
* Boxplots of top features vs. health score
* Count plots for categorical features like pest presence, soil type
* Distribution of plant health scores

---

## 📈 Models Implemented

| Model                    | Description                                           | Accuracy (approx.) |
| ------------------------ | ----------------------------------------------------- | ------------------ |
| Random Forest Classifier | Used for feature importance & prediction              | \~0.25             |
| K-Means Clustering       | Grouped plants into similar care requirement clusters | -                  |

---

## 🧪 Evaluation Metrics

* 📈 Accuracy
* 📉 Confusion Matrix
* 📊 Feature Importance Ranking

---

## ✅ Key Findings

* **Top Influential Features**:

  * `Room_Temperature_C`
  * `Height_cm`
  * `Soil_Moisture_%`
  * `Watering_Per_Day_ml`
  * `Fertilizer_Amount_ml`
  * `Humidity_%`
  * `Leaf_Count`, `New_Growth_Count`

* **Identified Clusters (K=3)**:

  1. **Cool, Dry, Low-Maintenance** – e.g., Snake Plants, Aloe Vera
  2. **Warm, Humid, and Thirsty Tropicals** – e.g., Monsteras, Philodendrons
  3. **Warm & Adaptive, Less Frequent Waterers** – e.g., Spider Plants, Ferns

---

## 🚀 Getting Started

1. **Clone the repository**

   ```bash
   git clone https://github.com/Souvik-Rana/Indoor-Plant-Health-Clustering.git
   cd Indoor-Plant-Health-Clustering
   ```

2. **Install dependencies**

   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```

3. **Run the analysis**
   Open and execute the Jupyter Notebook: `Plant_Health_Analysis.ipynb`

---

## ✅ Future Enhancements

* Apply time-series analysis for tracking plant health over time
* Explore multi-label classification for specific plant ailments
* Use advanced clustering techniques (GMM, DBSCAN)
* Build an interactive UI for personalized care recommendations

---

## 👤 Author

<p align="center">
  <b> SOUVIK RANA </b><br>
  <br><a href="https://github.com/souvikrana17">
    <img src="https://img.shields.io/badge/GitHub-000?style=for-the-badge&logo=github&logoColor=white" style="margin-right: 10px;" />
  </a>
  <a href="https://www.linkedin.com/in/souvikrana17/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" style="margin-right: 10px;" />
  </a>
  <a href="https://www.kaggle.com/souvikrana17">
    <img src="https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white" style="margin-right: 10px;" />
  </a>
  <a href="https://souvikrana17.vercel.app">
    <img src="https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=Firefox&logoColor=white" />
  </a>
</p>


<p align="center">
  <img src="https://raw.githubusercontent.com/souvikrana17/souvikrana17/main/SOUVIK%20RANA%20BANNER.jpg" alt="Banner" width="100%" />
</p>

---

## 🤝 Contributions

Contributions, issues, and feature requests are welcome!
Feel free to fork the repository and submit a pull request.
