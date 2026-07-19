# ✈️ Flight Delay Analysis and Prediction

A comprehensive data analytics and machine learning project that analyzes and predicts flight delays using the 2022 U.S. Flight Dataset. The project leverages **PySpark** for big data processing, **Spark MLlib** for machine learning, and **PyTorch** for deep learning to identify factors affecting flight delays and build accurate prediction models.

---

## 📌 Project Overview

This project performs an end-to-end analysis of flight delays, including:

- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Feature engineering
- Data visualization
- Machine Learning model training
- Deep Learning model development
- Clustering analysis using K-Means
- Model evaluation and comparison

The objective is to predict whether a flight will be delayed and discover the most influential factors contributing to delays.

---

## 📊 Dataset

- **Source:** Flight Delay Dataset (2022)
- **Original Size:** 4,078,318 records
- **After Cleaning:** 3,944,916 records
- **Features:** 61 columns

The dataset includes:

- Flight information
- Airlines
- Airports
- Departure & arrival delays
- Air time
- Flight distance
- Cancellation and diversion status
- Schedule information

---

## 🛠 Technologies Used

- Python
- PySpark
- Spark MLlib
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- PyTorch
- Jupyter Notebook

---

## 📂 Project Structure

```
Flight-Delay-Prediction/
│
├── flight_delay_2022_full_enhanced.ipynb
├── flight_delay_final.pptx
├── README.md
└── images/
```

---

## 🔍 Data Preprocessing

The preprocessing pipeline includes:

- Removing cancelled flights
- Removing diverted flights
- Handling missing values
- Removing duplicates
- Data type conversion
- Feature scaling
- Encoding categorical variables

---

## ⚙️ Feature Engineering

Several new features were created, including:

- **IsDelayed** → Target variable (Arrival Delay > 15 minutes)
- **DepHour** → Scheduled departure hour
- **isWeekend** → Weekend indicator

Additional preprocessing:

- StringIndexer
- OneHotEncoder
- VectorAssembler
- StandardScaler

---

## 📈 Exploratory Data Analysis

EDA was performed to analyze:

- Delay distribution
- Monthly delay trends
- Weekly delay trends
- Airline performance
- Flight distance
- Air time
- Delay outliers
- Summary statistics

---

## 🤖 Machine Learning Models

The following models were trained and evaluated:

### Logistic Regression

- Accuracy ≈ 84%
- AUC ≈ 0.88

---

### Random Forest

- 100 Trees
- Max Depth = 8
- Accuracy ≈ 89%
- AUC ≈ 0.95

---

### Gradient Boosted Trees (GBT)

- Max Iterations = 50
- Max Depth = 6

---

### Neural Network (PyTorch)

- 20 Training Epochs
- Accuracy ≈ 93.6%
- AUC ≈ 95.6%
- F1 Score ≈ 93.3%

---

## 📊 Clustering Analysis

K-Means clustering was used to discover natural delay groups.

Features:

- Departure Delay
- Arrival Delay
- Air Time
- Distance
- Departure Hour

Results:

- Best K = 3
- Silhouette Score = 0.4712

PCA was used for cluster visualization.

---

## 📉 Model Comparison

| Model | Accuracy | AUC |
|---------|----------|------|
| Logistic Regression | ~84% | ~0.88 |
| Random Forest | ~89% | ~0.95 |
| Gradient Boosted Trees | High | ~0.94 |
| Neural Network | **93.6%** | **95.6%** |

---

## 📷 Results

Key findings:

- Summer months showed the highest delays.
- Fridays experienced the highest average delays.
- Random Forest achieved the best performance among Spark ML models.
- The PyTorch Neural Network achieved the highest overall prediction accuracy.
- Feature engineering significantly improved model performance.

---

## 🚀 How to Run

1. Clone the repository

```bash
git clone https://github.com/yourusername/Flight-Delay-Prediction.git
```

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Open the notebook

```bash
jupyter notebook
```

4. Run all notebook cells.

---

## 📌 Future Improvements

- Deploy the model using Streamlit or Flask
- Real-time flight delay prediction
- Hyperparameter optimization
- Incorporate weather data
- Add explainable AI (SHAP/LIME)

---

## 👥 Team Members

- Shahd Ahmed
- Sohila Ayman
- Sarah Muhammed

---

## 📄 License

This project is developed for educational and research purposes.
