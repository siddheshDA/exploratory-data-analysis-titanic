# Task 5 — Exploratory Data Analysis (EDA) on Titanic Dataset

**Internship Project:** Data Analyst Internship — Task 5  
**Tools Used:** Python, Pandas, Matplotlib, Seaborn  
**Dataset:** Titanic (train.csv from Kaggle)  

---

## 📌 Objective
To perform an in-depth Exploratory Data Analysis (EDA) on the Titanic dataset, uncovering insights, patterns, and relationships using visual and statistical exploration.

---

## 🗂 Project Structure

---

## 🔍 Steps Performed

1. **Data Loading & Inspection**
   - Loaded dataset with Pandas
   - Checked shape, column data types, and previewed first rows

2. **Data Cleaning**
   - Checked missing values and duplicate rows
   - Created new features: `FamilySize`, `IsAlone`, `Title`
   - Flagged missing ages and performed median imputation

3. **Univariate Analysis**
   - Histograms for numeric variables (`Age`, `Fare`)
   - Countplots for categorical variables (`Survived`, `Pclass`, `Sex`, `Embarked`, `Title`)

4. **Bivariate Analysis**
   - Survival rates by `Sex`, `Pclass`, and `Title`
   - Boxplots: `Age` vs `Pclass`, `Fare` vs `Pclass`
   - Scatterplot: `Age` vs `Fare` (colored by `Survived`)

5. **Multivariate Analysis**
   - Correlation heatmap for numeric features
   - Pairplot for selected variables

6. **Observations & Recommendations**
   - Higher survival rate for females (~74%) than males (~19%)
   - First-class passengers had the highest survival rates
   - Cabin data mostly missing — careful engineering required
   - Age imputation necessary for modeling
   - Fare is right-skewed — log transform recommended for models

---

## 📊 Key Insights
- **Overall survival rate:** ~38%
- **Female survival rate:** ~74% vs **Male:** ~19%
- **By Class:** Pclass 1 (~63%) > Pclass 2 (~47%) > Pclass 3 (~24%)
- Large proportion of missing values in `Cabin` and `Age`
- `Title` extracted from passenger names correlates with survival chances

---

## 💡 Recommendations
- Impute missing `Age` based on `Title` and `Pclass`
- Engineer `FamilySize` and `IsAlone` for better prediction
- Drop or engineer `Cabin` into deck features
- Log-transform `Fare` to reduce skew
- Encode categorical variables (`Sex`, `Embarked`, `Title`) for ML models

---


