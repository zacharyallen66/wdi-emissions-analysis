🌐 Economics' Influence on Emissions
A machine learning analysis exploring how historical economic indicators can be used to predict greenhouse gas emissions — and what deviations between actual vs predicted outputs reveal about national environmental policy effectiveness.

📊 Project Summary
Developed for: MIS 776 – Business Analytics & Machine Learning

Collaborators: Zachary Allen, Joshua Stoddard, Tommy Janasz

Technologies: Python, Pandas, Scikit-learn, Keras, RandomForestRegressor, Neural Networks, PCA

📈 Research Objectives
Predict CO₂, Methane, and Nitrous Oxide Emissions
→ Can future emissions be predicted from historical economic data?
→ Business value: Helps stakeholders forecast environmental impacts tied to industrial or developmental policy.

Infer Policy Impact via Model Deviations
→ Where do actual emissions diverge from model predictions?
→ Insight: Negative deviation suggests strong environmental performance, possibly due to policy.

🗂️ Data Sources
World Bank Development Indicators (WDI)
Global economic and social indicators from the 1960s onward.

Our World in Data – Emissions Data
National CO₂, methane, and nitrous oxide emissions data from OWID.

🔗 Also available here: Google Drive - Data Files & Model Outputs

🧠 Modeling Approaches
PCA (Principal Component Analysis)
Reduced dimensionality from over 1,400 indicators to ~200 most predictive variables.

Random Forest Regression
Achieved R² = 0.8849, explaining ~88.5% of variance in emissions using historical economic indicators.

Neural Network Model (Keras)
Achieved R² = 0.9581, capturing non-linear relationships with high accuracy. Slight tendency to overpredict emissions.

📊 Example: Country-Level Divergence
Country	Trend vs Model	Interpretation
🇳🇴 Norway	Actual emissions below predicted	Suggests strong policy impact
🇨🇦 Canada	Actual emissions above predicted	Suggests weaker mitigation efforts

These deviations hint at the effectiveness (or lack) of national policies — especially in countries at a similar development tier.

📎 Files Included
Notebook	Description
Economic_Data_Preprocess.ipynb	Filters and prepares WDI + OWID datasets
Data_Transformer.ipynb	PCA reduction, alignment, and normalization
RDMForest.ipynb	Random Forest + Neural Network model training and evaluation
MIS 776 Presentation.pptx	Final presentation deck with visualizations

🔍 Future Work
Compare top diverging countries’ environmental policies

Introduce time-series models to account for momentum and structural breaks

Expand scope to include trade-based emissions or consumption-side metrics

🧾 Citation
If using the dataset or methodology, cite as:

Allen, Z., Stoddard, J., & Janasz, T. (2025). Economics' Influence on Emissions. MIS 776, University of Nevada, Las Vegas.
