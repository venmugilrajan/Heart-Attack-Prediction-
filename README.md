# Heart-Attack-Prediction
❤️ Heart Attack Risk Analysis

This project analyzes a dataset of 8,763 patients with demographic, lifestyle, and medical features to explore risk factors for heart attack. The dataset includes clinical attributes (blood pressure, cholesterol, BMI, diabetes, etc.) along with lifestyle indicators (smoking, exercise, stress, sleep).

📂 Dataset Overview

Rows: 8,763

Columns: 29 (after preprocessing)

Key Features:

Demographics: Age, Sex, Country, Continent

Clinical: Cholesterol, Blood Pressure (Systolic/Diastolic), Heart Rate, Diabetes, BMI, Triglycerides

Lifestyle: Smoking, Obesity, Alcohol Consumption, Exercise Hours, Stress Level, Sleep Hours

Target: Heart Attack Risk (0 = No Risk, 1 = Risk)

⚙️ Preprocessing

Data Cleaning

No missing values found.

No duplicate patient IDs.

Feature Engineering

Split Blood Pressure into Systolic & Diastolic.

Encoded Sex → Male = 1, Female = 0.

Created new metrics:

Pulse Pressure = Systolic – Diastolic

Cholesterol_BMI_Ratio = Cholesterol / (BMI + 1)

Filled NaN values in numeric columns with median values.

📊 Exploratory Data Analysis (EDA)

Demographics

Males: 6111 (70%) | Females: 2652 (30%)

Top countries: Germany, Argentina, Brazil, UK, Australia

Clinical Insights

Avg Age: 53.7 years

Avg Cholesterol: 259.8 mg/dL

Avg BMI: 28.9

Risk Distribution

No Risk (0): ~64%

Risk (1): ~36%

📈 Visualizations

Histograms: Age, Cholesterol, BMI distributions

Bar Plots: Gender distribution, Heart Attack risk count

Line Plots: Avg Cholesterol by Age, Avg BMI across age groups

Heatmap: Correlation between numeric features

🚀 Tools Used

Pandas & NumPy → Data cleaning & preprocessing

Matplotlib & Seaborn → Visualizations

Feature Engineering → Derived new medical metrics

🔑 Key Insights

Heart attack risk increases with age, high cholesterol, and BMI.

Men are more represented in the dataset and show higher risk counts.

Pulse Pressure and Cholesterol_BMI_Ratio provide useful new indicators.

Some non-lifestyle factors (genetics, diabetes, previous heart problems) strongly correlate with risk.
