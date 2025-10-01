# H-1B Visa Application Classification
This project focuses on H-1B Visa Application Classification using deep learning techniques. The dataset used is the U.S. Department of Labor’s H-1B Labor Condition Application (LCA) Disclosure Data for FY2020–FY2024, which contains details of employer filings, job roles, salaries, and final outcomes of visa petitions.

The aim of the project is to build a predictive model that can classify visa cases based on application features. Such a system can help in understanding key factors influencing visa approvals, assist policymakers, and provide insights to employers and applicants.

👥 Team Members

Kundan Sharma

Anmol Narayan

Priyanshu

📊 Dataset

Source: U.S. Department of Labor LCA Disclosure Data (2020–2024)

File used: Combined_LCA_Disclosure_Data_FY2020_to_FY2024.csv from Kaggle

Features include:

JOB_TITLE (title of the position)

EMPLOYER_NAME (organization applying)

EMPLOYER_STATE and WORKSITE_STATE

WAGE_RATE_OF_PAY and related salary info

CASE_STATUS (target label: Approved/Denied/Certified-Withdrawn, etc.)

Various metadata about the visa filing process

🧹 Data Preprocessing & Cleaning

The raw dataset contains millions of records with missing and duplicate values. The preprocessing steps included:

Handling missing numeric features by median imputation.

Dropping rows with critical missing fields (JOB_TITLE, EMPLOYER_NAME, EMPLOYER_STATE, WORKSITE_STATE).

Removing duplicate entries.

Encoding categorical features (employer, job title, work location).

Normalizing numerical attributes (wages, SOC codes, etc.).

🤖 Model Architecture

Several machine learning and deep learning models were explored for classification. The final pipeline involved:

Exploratory Data Analysis (EDA): Understanding feature distributions and relationships.

Feature Engineering: Converting categorical fields to embeddings or one-hot vectors.

Modeling Approaches:

Logistic Regression, Random Forest (baseline)

Artificial Neural Networks (ANN) with multiple hidden layers

Training & Evaluation: Models were trained with stratified splits and evaluated using accuracy, precision, recall, F1-score, and confusion matrix.

📈 Results & Insights

Deep learning models significantly outperformed traditional baselines.

Features such as job title, wage level, and worksite state were strong predictors of visa approval.

The model demonstrated the potential for automation in analyzing large-scale immigration datasets and attained accuracy of 94.05% .
