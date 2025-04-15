# 🧠 Understanding the Effects on Balance for Elite Platform Divers Using Machine Learning

This project leverages machine learning and deep learning to analyze balance metrics from force plate data collected from elite Division I platform divers. It aims to predict **anterior-posterior (AP) sway**, **medial-lateral (ML) sway**, **trial type**, and **subject identity** based on raw force and moment data.

📄 Presented at: *Understanding the Effects on Balance for Elite Platform Divers Using Machine Learning*  
🧪 Conducted using real-world data from the University of North Carolina Wilmington Diving Team  
🔬 Dataset Size: 4M+ data points from 8 athletes, 36 trials each, 6 trial types  

---

## 🚀 Project Highlights

- 📉 **Regression Models**  
  - Predicted AP and ML sway using multiple regressors  
  - Achieved **R² = 0.9939** for AP sway, **R² = 0.9943** for ML sway using K-Nearest Neighbors

- 🧾 **Classification Models**  
  - Classified `trial_type` and `subject_number` using tree-based models  
  - Achieved **>90% accuracy**, with perfect scores on several classifiers (e.g., Random Forest, XGBoost)

- 🤖 **Deep Learning**  
  - Built fully connected deep neural networks using Keras  
  - Achieved **87% R²** in predicting ML sway over 40 epochs (batch size = 128)

- 📊 **Feature Engineering**  
  - Engineered key features from force plate data (Fx, Fy, Fz, Mx, My, Mz)  
  - Calculated sway using domain-specific physics formulas

---

## 🛠 Tech Stack

- **Languages & Libraries**: Python, NumPy, Pandas, Matplotlib, Seaborn  
- **ML/DL Frameworks**: Scikit-learn, Keras, TensorFlow  
- **Tools Used**: Jupyter Notebooks, MinMaxScaler, Train-Test Split, Correlation Analysis  
- **Models Applied**:
  - Regression: KNN, XGBoost, Ridge, Lasso, ElasticNet  
  - Classification: Random Forest, Extra Trees, Gradient Boosting, CatBoost  
  - Deep Learning: Fully Connected Neural Network (Keras)

---

## 📁 Dataset Overview

Each row in the dataset contains:
- Force readings: `Fx`, `Fy`, `Fz`
- Moment readings: `Mx`, `My`, `Mz`
- Calculated values: `AP_sway`, `ML_sway`, `BodyMass`
- Categorical labels: `TrialType`, `TrialNumber`, `SubjectNumber`

Trial types included:
1. Eyes open – both feet  
2. Eyes closed – both feet  
3. Eyes open – right foot  
4. Eyes open – left foot  
5. Eyes closed – right foot  
6. Eyes closed – left foot

---

## 📈 Visualizations

- **Spaghetti plots** for sway patterns across trials  
- **Box plots** tracking balance deterioration through repeated trials  
- **Correlation matrix** to assess feature redundancy  
- **Predicted vs Actual plots** for regression model validation

---


