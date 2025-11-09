# 🎙️ Voice-Based Health Classification

## 📖 Project Overview
This project explores how **acoustic features extracted from human voice recordings** can be used to predict vocal health.  
By combining Exploratory Data Analysis (EDA), data visualization in **Power BI**, and supervised **machine learning models**, the project identifies measurable differences between **healthy** and **unhealthy** voices.

---

## 🎯 Objectives
- Analyze the acoustic feature dataset (`VowelA_High_latest.csv`) to uncover key patterns.
- Build and evaluate machine learning models to classify vocal health.
- Visualize results and insights through an interactive **Power BI dashboard**.
- Document findings and workflow in a professional report.

---

## 🧠 Key Insights
- Healthy voices exhibit **lower energy irregularity (RMSE)** and **less noisiness (ZCR)**.
- Unhealthy voices show **higher spectral variability** and **entropy**, indicating instability.
- Ensemble models like **Random Forest** and **XGBoost** achieved the highest performance:
  - **XGBoost**: 92% accuracy, 0.96 AUC
  - **Random Forest**: 91% accuracy, 0.95 AUC
- Energy and spectral features were the most predictive across models.

---

## 🧩 Project Structure
📦 Voice-Based Health Classification
├── 📁 data
│ ├── VowelA_High_latest.csv # Original dataset
│ ├── Cleaned_VowelA_High_latest.csv # Processed dataset
│ ├── model_metrics.csv # Model KPI summary
│ ├── confusion_matrix.csv # Classification results
│ ├── roc_curve.csv # ROC data points
│ └── feature_importance.csv # Model feature importances
│
├── 📁 notebooks
│ ├── Voice-Based Health EDA.ipynb # Data exploration & visualization
│ └── Predictive_Model.ipynb # Model building & evaluation
│
├── 📁 dashboard
│ └── Voice-Based Health.pbix # Power BI interactive dashboard
│
├── 📁 report
│ └── Voice-Based Health Classification.docx / .pdf
│
└── README.md # Project overview (this file)

---

## ⚙️ Methodology

### **1. Data Preparation**
- Cleaned missing values, normalized numeric features.
- Encoded categorical data (Gender, Label).
- Split dataset 80/20 for training/testing.

### **2. Exploratory Data Analysis**
- Identified correlations between MFCCs, RMSE, and spectral features.
- Visualized feature distributions by health status.
- Observed clear separation between healthy and unhealthy voice clusters.

### **3. Modeling**
Trained and evaluated multiple classifiers:
- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost

**Evaluation Metrics:** Accuracy, Precision, Recall, F1-Score, AUC.

### **4. Visualization**
Developed an interactive **Power BI dashboard** with:
- Dataset Overview
- Acoustic Feature Comparison
- Voice Health Summary
- Model Performance (dynamic model selector, KPI cards, ROC, and Confusion Matrix)

---

## 📊 Model Performance Summary
| Model | Accuracy | Precision | Recall | F1 | AUC |
|--------|-----------|------------|--------|-----|------|
| Logistic Regression | 0.87 | 0.85 | 0.88 | 0.86 | 0.91 |
| Decision Tree | 0.89 | 0.88 | 0.90 | 0.89 | 0.92 |
| Random Forest | 0.91 | 0.89 | 0.93 | 0.91 | 0.95 |
| **XGBoost** | **0.92** | **0.90** | **0.94** | **0.92** | **0.96** |

---

## 💻 Tools & Technologies
| Category | Tools Used |
|-----------|-------------|
| **Languages** | Python, DAX |
| **Libraries** | Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, XGBoost |
| **Visualization** | Power BI |
| **Environment** | Google Colab, Power BI Desktop |
| **Documentation** | Word / PDF Report, Markdown (GitHub) |

---

## 🧾 Deliverables
- ✅ Cleaned dataset  
- ✅ EDA & Model notebooks  
- ✅ Power BI Dashboard (`.pbix`)  
- ✅ Final Report (`.docx` / `.pdf`)  
- ✅ GitHub Repository with documentation

---

## 🚀 Results & Conclusions
- Voice acoustics are strong indicators of vocal health.  
- Machine learning achieved high accuracy (>90%) using spectral and energy features.  
- The Power BI dashboard provides a clear, interactive way to explore both data and model results.

**Next Steps:**
- Extend dataset with more recordings and additional vowels.
- Explore deep learning (e.g., CNNs on spectrograms).
- Integrate SHAP or LIME for explainable AI insights.

---

## 👤 Author
**Christopher Mauro**  
📅 *November 2025*  
🔗 *GitHub Repository:* [Add your GitHub repo link here]

---

## 📜 License
This project is released under the MIT License.  
Feel free to use, modify, or share with attribution.

---

*“Turning voice into insight — one frequency at a time.”* 🎧
