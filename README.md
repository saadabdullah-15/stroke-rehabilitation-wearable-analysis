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

stroke-rehabilitation-wearable-analysis/  
│  
├── 📄 stroke_rehabilitation_wearable_data_analysis.ipynb   # Main analysis notebook  
├── 📄 README.md                                            # Project documentation  
└── 📄 requirements.txt                                    # Project dependencies  

---

## 📥 Dataset Citation and Description

This project uses the **Stroke Rehabilitation Wearable Sensor Dataset**, available on **Zenodo**.

### 📌 Citation:
> Please cite the dataset using the following DOI, which refers to **all versions**:
>
> **DOI:** [10.5281/zenodo.10534054](https://doi.org/10.5281/zenodo.10534054)

### 📌 Dataset Description:
The dataset consists of data from **ten stroke patients** who completed both rehabilitation visits. The dataset includes:

- **Raw Data (`raw/`)**:
  - Tri-axial acceleration and angular velocity data from IMU sensors.
  - Participant information such as demographics (height, weight), FAC scores at both visits, and gait improvement evaluations (in `participant_info.csv`).
---

### 📌 Link to the dataset:
- [Zenodo Stroke Rehabilitation Dataset (DOI: 10.5281/zenodo.10534054)](https://doi.org/10.5281/zenodo.10534054)

---

## 📊 Workflow Summary:
1. **Data Preprocessing:**
   - Cleaning participant information and IMU datasets.
   - Handling missing values.
   - Feature extraction (mean, std, range, energy, etc.) from sensor signals.

2. **Exploratory Data Analysis (EDA):**
   - Visualizations of participant demographics (age, gender).
   - Comparison of Visit 1 vs. Visit 2 features.
   - Analysis of FAC improvement across participants.

3. **Statistical Analysis:**
   - Paired t-tests on Visit 1 vs. Visit 2 features.
   - Comparison of feature distributions across improvement groups.

4. **Machine Learning:**
   - Logistic Regression (best performer).
   - Random Forest, Support Vector Machine, HistGradientBoosting.
   - Cross-validation to evaluate model performance.
   - Confusion matrix visualizations.

5. **Results:**
   - Logistic Regression achieved the best performance (75% cross-validated accuracy).
   - High variance in F1-score due to the small dataset.
   - Inconsistent model performance across folds.

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
- Small dataset (limited participants and visits).
- High variability across cross-validation folds.
- Models are sensitive to small data splits.
- Results should be interpreted with caution.

---

## 🚀 Future Improvements:
- Expand the dataset with more participants.
- Apply balancing techniques (e.g., SMOTE).
- Perform hyperparameter tuning for model optimization.
- Explore feature importance to identify key biomechanical markers.
- Try ensemble methods or stacked models.

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

