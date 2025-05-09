# 🌐 Economics' Influence on Emissions

A machine learning analysis exploring how historical economic indicators can be used to predict greenhouse gas emissions — and what deviations between actual vs predicted outputs reveal about national environmental policy effectiveness.

---

## 📊 Project Summary

- Developed for: **MIS 776 – Business Analytics & Machine Learning**
- Technologies: `Python`, `Pandas`, `Scikit-learn`, `Keras`, `RandomForestRegressor`, `Neural Networks`, `PCA`

---

## 📈 Research Objectives

1. **Predict CO₂, Methane, and Nitrous Oxide Emissions**  
   → Can future emissions be predicted from historical economic data?  
   → *Business value:* Helps stakeholders forecast environmental impacts tied to industrial or developmental policy.

2. **Infer Policy Impact via Model Deviations**  
   → Where do actual emissions diverge from model predictions?  
   → *Insight:* Negative deviation suggests strong environmental performance, possibly due to policy.

---

## 🗂️ Data Sources

- **[World Bank Development Indicators (WDI)](https://databank.worldbank.org/source/world-development-indicators)**  
  Global economic and social indicators from the 1960s onward.

- **[Our World in Data – Emissions Data](https://github.com/owid/co2-data)**  
  National CO₂, methane, and nitrous oxide emissions data from OWID.

- 🔗 **[Google Drive – Data Files & Model Outputs](https://drive.google.com/drive/folders/1kFK9Vu5M1jHPjHA3hrTxJG3SwX5lsYZ5?usp=sharing)**

---

## 🧠 Modeling Approaches

- **PCA (Principal Component Analysis)**  
  Reduced dimensionality from over 1,400 indicators to ~200 most predictive variables.

- **Random Forest Regression**  
  Achieved **R² = 0.8849**, explaining ~88.5% of variance in emissions using historical economic indicators.

- **Neural Network Model (Keras)**  
  Achieved **R² = 0.9581**, capturing non-linear relationships with high accuracy. Slight tendency to overpredict emissions.

---

## 🌍 Example: Country-Level Divergence

We used model prediction errors to assess how actual emissions deviate from expected levels, given a country's economic profile. This offers a way to infer *real-world policy impact* — highlighting nations that may be over- or under-performing in environmental regulation.

| Country | Trend vs Model               | Interpretation                    |
|---------|------------------------------|------------------------------------|
| 🇳🇴 Norway | Actual emissions **below** predicted | Suggests strong climate policy effectiveness |
| 🇨🇦 Canada | Actual emissions **above** predicted | Indicates room for stronger mitigation efforts |

These deviations serve as a proxy to assess national environmental performance — especially between countries at a similar level of development.

---

### 📊 Visual Analysis


![image](https://github.com/user-attachments/assets/8beb55f6-c513-4b34-938c-7270f4fc172e)
**What the visuals show:**
- **Top Row (Scatter Plots):**  
  Predicted vs actual emissions for CO₂, Methane, and Nitrous Oxide across all countries. Points above the red diagonal line represent countries emitting more than expected.

![image](https://github.com/user-attachments/assets/72907ba7-1b1f-45ff-a73b-e8bb5406cfe5)
- **Middle (Choropleth Map):**  
  A global map highlighting model residuals — blue indicates lower-than-predicted emissions; red indicates higher-than-predicted emissions.
  
![image](https://github.com/user-attachments/assets/ef72c019-7083-488f-94f1-990cc4cc6f07)

- **Bottom Row (Line Graphs):**  
  Yearly comparisons for **Canada** and **Norway** (2015–2019):  
  - **Canada:** Emissions trend higher than expected — policy may be lagging.  
  - **Norway:** Emissions trend lower than predicted — suggesting effective mitigation.

> These visuals help connect statistical predictions with real-world environmental outcomes, revealing how countries diverge based on their policy choices and economic structures.

## 📎 Files Included

| Notebook | Description |
|----------|-------------|
| `Economic_Data_Preprocess.ipynb` | Filters and prepares WDI + OWID datasets |
| `Data_Transformer.ipynb` | PCA reduction, alignment, and normalization |
| `RDMForest.ipynb` | Random Forest + Neural Network model training and evaluation |
| `MIS 776 Presentation.pptx` | Final presentation deck with visualizations |

---

## 🔍 Future Work

- Compare top diverging countries’ environmental policies  
- Introduce time-series models to account for momentum and structural breaks  
- Expand scope to include trade-based emissions or consumption-side metrics  

---

## 🧾 Citation

If using the dataset or methodology, cite as:  
> Allen, Z., Stoddard, J., & Janasz, T. (2025). *Economics' Influence on Emissions*. MIS 776, University of Nevada, Las Vegas.

