# AIML-Exploratory-DataAnalysis
Quick stats, clear visuals, and smart groupings reveal who survived the Titanic and why. See how class, gender, and age shaped fate—simple, sharp, and insightful.
# Exploratory Data Analysis (EDA) on Titanic Dataset

This project performs a detailed exploratory data analysis on the Titanic dataset to understand patterns, relationships, and insights that can help in further modeling or reporting.

---

## 1. Generate Summary Statistics

- Used `df.describe()` to get **mean, median, standard deviation, min, max, and quartiles** for numeric features.
- Used `df.describe(include='object')` to summarize categorical/text features.
- Checked data types and missing values with `df.info()` and `df.isnull().sum()`.

**Purpose:**  
Understand the central tendency, spread, data completeness, and types of the dataset features.

---

## 2. Create Histograms and Boxplots for Numeric Features

- Created **histograms** for features like Age, Fare, SibSp, and Parch to visualize their distributions.
- Created **boxplots** to identify outliers and understand data spread for the same numeric features.

**Purpose:**  
Visualize data distributions and detect anomalies or outliers.

---

## 3. Use Pairplot and Correlation Matrix for Feature Relationships

- Created a **correlation heatmap** to see relationships between numeric features and the target variable (`Survived`).
- Created **pairplots** (scatterplot matrices) to observe pairwise relationships and how features cluster based on survival.

**Purpose:**  
Understand inter-feature relationships and detect possible predictors for survival.

---

## 4. Identify Patterns, Trends, or Anomalies in the Data

- Analyzed survival counts overall and grouped by important features like `Pclass`, `Sex`, and `AgeGroup`.
- Observed survival rates vary significantly with passenger class, gender, and age.
- Checked for data imbalances and missing values in features like `Cabin` and `Embarked`.

**Purpose:**  
Detect meaningful patterns and anomalies that influence survival rates.

---

## 5. Make Basic Feature-Level Inferences from Visuals

- Found that **1st class passengers had higher survival rates** than 2nd or 3rd class.
- **Females had a much higher survival rate** compared to males.
- **Younger passengers (children) had better survival odds** than older passengers.
- Fare and family size (`SibSp`, `Parch`) also showed trends correlated with survival.

**Purpose:**  
Extract actionable insights and hypotheses to guide modeling or further analysis.

---

## Additional Notes

- Used `groupby` with `.mean()` to calculate survival percentages for categorical features.
- Converted survival rates to **percentage format** with `%` signs for better readability.
- Visualizations were created using **Seaborn** and **Matplotlib** libraries.

---

Feel free to explore the notebook and visualizations for a deeper understanding of the Titanic survival patterns!


Additional Notes
Used groupby with .mean() to calculate survival percentages for categorical features.

Converted survival rates to percentage format with % signs for better readability.

Visualizations were created using Seaborn and Matplotlib libraries.
