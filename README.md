[![Python](https://img.shields.io/badge/Python-3.9-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Google%20Colab-orange.svg)](https://colab.research.google.com/github/saadabdullah-15/stroke-rehabilitation-wearable-analysis/blob/main/stroke_rehabilitation_wearable_data_analysis.ipynb)
[![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)]()
[![Libraries](https://img.shields.io/badge/Libraries-pandas%2C%20numpy%2C%20matplotlib%2C%20seaborn%2C%20scikit--learn-grey.svg)]()

---

# 🧠 Stroke Rehabilitation Analysis Using Wearable Device Data

This project analyzes wearable sensor data collected during stroke rehabilitation to assess patient recovery progress. The focus is on extracting features from IMU (Inertial Measurement Unit) signals and predicting improvements in the Functional Ambulation Category (FAC) using machine learning models.

---

## 📌 Objectives:
- Perform exploratory data analysis (EDA) on participant demographics and sensor data.
- Preprocess raw IMU signals and extract statistical features.
- Compare rehabilitation progress between Visit 1 and Visit 2.
- Analyze the relationship between sensor features and FAC improvement.
- Build machine learning models to predict FAC improvement.
- Evaluate model performance with cross-validation and confusion matrices.

---

## 📂 Repository Structure

```
stroke-rehabilitation-wearable-analysis/  
│  
├── 📄 stroke_rehabilitation_wearable_data_analysis.ipynb   # Main analysis notebook  
├── 📄 README.md                                            # Project documentation  
└── 📄 requirements.txt                                     # Project dependencies  
```

---

## 📥 Dataset Citation and Description

This project uses the **Stroke Rehabilitation Wearable Sensor Dataset**, available on **Zenodo**.

### 📌 Citation:
> Please cite the dataset using the following DOI (covers **all versions**):
>
> **DOI:** [10.5281/zenodo.10534054](https://doi.org/10.5281/zenodo.10534054)

### 📌 Dataset Description:
The dataset consists of data from **ten stroke patients** who completed both rehabilitation visits. The dataset includes:

- **Raw Data (`raw/`)**:
  - Tri-axial acceleration and angular velocity data from IMU sensors.
  - Participant information such as demographics (height, weight), FAC scores at both visits, and gait improvement evaluations (in `participant_info.csv`).

🔗 **Dataset Link:** [Zenodo Stroke Rehabilitation Dataset (DOI: 10.5281/zenodo.10534054)](https://doi.org/10.5281/zenodo.10534054)

---

## 🚀 How to Run the Project

Follow these steps to set up and execute the project:

---

### ✅ 1. Clone the Repository
```bash
git clone https://github.com/saadabdullah-15/stroke-rehabilitation-wearable-analysis.git
cd stroke-rehabilitation-wearable-analysis
```

---

### ✅ 2. Install Project Dependencies
```bash
pip install -r requirements.txt
```

---

### ✅ 3. Download the Dataset
Download the dataset from Zenodo:
🔗 [https://doi.org/10.5281/zenodo.10534054](https://doi.org/10.5281/zenodo.10534054)

Extract and place `raw/`, `interim/`, and `processed/` in the working directory.

---

### ✅ 4. Run the Analysis Notebook
- **Google Colab:**  
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/saadabdullah-15/stroke-rehabilitation-wearable-analysis/blob/main/stroke_rehabilitation_wearable_data_analysis.ipynb)

- **Locally:**  
```bash
jupyter notebook stroke_rehabilitation_wearable_data_analysis.ipynb
```

---

### ✅ 5. Optional: Push Changes to GitHub
```bash
git add .
git commit -m "Updated analysis and results"
git push origin main
```

---

## 📊 Workflow Summary:
1. **Data Preprocessing:** Cleaning, missing values, feature extraction.
2. **EDA:** Visualize demographics, compare visits, analyze FAC improvement.
3. **Statistical Analysis:** Paired t-tests, feature comparisons.
4. **Machine Learning:** Logistic Regression, Random Forest, SVM, HistGradientBoosting.
5. **Results:** Logistic Regression best (75% accuracy), high F1-score variance.

---

## 🧪 Models Performance Summary:
| Model                   | Accuracy | F1-Score (Improvement) |
|-------------------------|----------|------------------------|
| Logistic Regression     | 0.75     | 0.47                  |
| Random Forest           | 0.50     | 0.50                  |
| Support Vector Machine  | 0.50     | 0.00                  |
| HistGradientBoosting    | 0.50     | 0.00                  |

---

## ⚠️ Limitations:
- Small dataset.
- High cross-validation variability.
- Sensitive to small data splits.

---

## 🚀 Future Improvements:
- More participants.
- Balancing techniques (SMOTE).
- Hyperparameter tuning.
- Feature importance exploration.
- Advanced ensemble methods.

---

## 🛠️ Tech Stack:
- **Python**
- **Google Colab**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**
- **Scikit-learn**

---

## 🏷️ Topics:
`stroke-rehabilitation`, `machine-learning`, `wearable-sensors`, `biomechanics`, `IMU-data`, `time-series-analysis`, `python`, `scikit-learn`, `data-science`

---

## ✨ Author:
[Saad Abdullah](https://github.com/saadabdullah-15)
