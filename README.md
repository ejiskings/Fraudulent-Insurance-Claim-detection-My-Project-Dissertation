🕵‍♂ Detecting Fraudulent Insurance Claims

📌 Overview
This project is part of my dissertation focused on identifying fraudulent insurance claims using machine learning techniques. 
The goal is to build robust predictive models that can distinguish between legitimate and fraudulent claims based on structured data. 
The repository includes exploratory data analysis, feature engineering,model development,and advanced techniques such as SMOTE for handling class imbalance and advanced feature engineering.

📂 Repository Structure
Code
├── data/
│   ├── raw/                # Original datasets(insurance/employee/vendor)
│   ├── merged/             # Combined datasets
│   ├── processed/          # Cleaned and transformed datasets (train/test)
├── notebooks/
│   ├── EDA.ipynb           # Exploratory Data Analysis
│   ├── Feature_Engineering.ipynb
│   ├── Model_Building.ipynb
│   ├── SMOTE_Model.ipynb
│   ├── Advanced_Features.ipynb
├── models/
│   ├── saved_models/       # Serialized model files
├── README.md

🔍 Methodology
1. 🧪 Exploratory Data Analysis (EDA)
Visualized distributions, correlations, and outliers

Identified key patterns and anomalies in claim behavior

2. 🛠 Feature Engineering
Created domain-specific features (e.g., claim frequency, claim-to-premium ratio)

Encoded categorical variables and handled missing values

3. 🤖 Model Building
Trained baseline models including Logistic Regression, Random Forest, XGBoost and lightGBM

Evaluated performance using metrics like accuracy, precision, recall, F1-score and AUC-ROC

4. ⚖ SMOTE for Class Imbalance
Applied Synthetic Minority Over-sampling Technique (SMOTE)

Improved model sensitivity to fraudulent cases

5. 🚀 Advanced Feature Engineering
Features were engineered for a fraud detection model using time-based, behavioral, and missing data signals.
This process gives the model more meaningful information, improving its accuracy in detecting fraudulent insurance claims.

⚠ Gaps addressed by this Research

Existing insurance fraud models lack generalizability across different insurance types and regions. 
They often sacrifice interpretability, making it hard for stakeholders to trust them.
Many studies also fail to benchmark different algorithms, and they overlook real-world challenges like data drift and scalability, making them difficult to deploy.

📊 Results
Best-performing model: AUC-ROC

F1-Score: 0.229

ROC-AUC: 0.913

🧠 Key Learnings
Feature engineering significantly boosts model performance

SMOTE helps mitigate bias toward majority class

Fraud detection requires balancing precision and recall to avoid false positives

🛑Models Limmitations

Model limitations include using default settings for XGBoost and LightGBM
training on a publicly available dataset.

🚀 Future Work

Interpretability can be improved using SHAP and adjusting model settings.
Future work can improve the models by using hyperparameter tuning to find optimal settings 
training on real-world data to improve generalizability.
Deploy model as an API for real-time claim scoring
Explore deep learning approaches for unstructured data (e.g., claim descriptions)

Integrate external data sources for richer feature sets

🙌 Acknowledgements
Thanks to my academic advisors, peers, and the open-source community for their support and inspiration throughout this project.
