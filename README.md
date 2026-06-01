# ElevateLabs-Task2
# 📊 Exploratory Data Analysis (EDA) on Titanic Dataset

## 📌 Project Overview

Exploratory Data Analysis (EDA) is a crucial step in the Machine Learning workflow that helps understand the structure, characteristics, and quality of a dataset before building predictive models.

In this project, EDA was performed on the **Titanic Dataset** to uncover patterns, identify trends, detect anomalies, and gain insights through statistical analysis and visualizations.

---

## 🎯 Objectives

* Generate summary statistics for numerical features
* Analyze feature distributions using histograms
* Detect outliers using boxplots
* Explore relationships between variables
* Visualize correlations among features
* Identify patterns, trends, and anomalies
* Draw meaningful insights from the data

---

## 🛠️ Tech Stack

| Tool       | Purpose                   |
| ---------- | ------------------------- |
| Python     | Programming Language      |
| Pandas     | Data Analysis             |
| NumPy      | Numerical Computing       |
| Matplotlib | Data Visualization        |
| Seaborn    | Statistical Visualization |

---

## 📂 Dataset

### Titanic Dataset

The dataset contains information about Titanic passengers, including:

* Passenger Class (Pclass)
* Age
* Gender
* Fare
* Embarkation Port
* Number of Siblings/Spouses
* Number of Parents/Children
* Survival Status

The dataset contains both numerical and categorical variables, making it suitable for EDA and Machine Learning practice.

---

## 🔍 Exploratory Data Analysis Workflow

### 1️⃣ Dataset Inspection

Initial exploration was performed to understand:

* Dataset dimensions
* Feature names
* Data types
* Missing values

Methods used:

```python
df.head()
df.info()
df.shape
df.isnull().sum()
```

---

### 2️⃣ Summary Statistics

Descriptive statistics were generated to understand the central tendency and spread of numerical features.

Metrics analyzed:

* Mean
* Median
* Standard Deviation
* Minimum
* Maximum
* Quartiles

```python
df.describe()
```

Additional statistics:

```python
df.median(numeric_only=True)
df.var(numeric_only=True)
df.mode()
```

---

### 3️⃣ Univariate Analysis

#### 📈 Histograms

Histograms were used to visualize feature distributions.

```python
df.hist(figsize=(12,8))
```

Key observations:

* Age distribution is concentrated around young and middle-aged passengers.
* Fare distribution is highly right-skewed.
* Most passengers belonged to lower fare categories.

---

#### 📦 Boxplots

Boxplots were used to identify outliers and understand feature spread.

```python
sns.boxplot()
```

Key observations:

* Significant outliers were observed in the Fare feature.
* Some features showed large variability among passengers.

---

### 4️⃣ Bivariate Analysis

#### 🔗 Pairplots

Pairplots were created to visualize relationships between multiple numerical features.

```python
sns.pairplot()
```

Insights:

* Certain passenger groups exhibited clustering patterns.
* Survival trends appeared related to passenger class and fare.

---

### 5️⃣ Correlation Analysis

A correlation matrix and heatmap were generated to identify relationships between numerical variables.

```python
corr = df.corr(numeric_only=True)
```

Visualization:

```python
sns.heatmap(corr, annot=True)
```

Interpretation:

* Positive values indicate direct relationships.
* Negative values indicate inverse relationships.
* Values near zero indicate weak or no linear relationship.

---

## 📊 Key Findings

### Age

* Most passengers were between 20 and 40 years old.
* Age distribution was moderately skewed.
* Missing values were present.

### Fare

* Fare distribution was highly right-skewed.
* Several extreme outliers were observed.
* Most passengers paid relatively low fares.

### Passenger Class

* Majority of passengers traveled in 3rd class.
* Passenger class appeared related to fare and survival.

### Survival

* Higher-class passengers generally showed better survival outcomes.
* Fare appeared to have some relationship with survival probability.

### Correlation Analysis

* Fare and Passenger Class showed a noticeable relationship.
* Most numerical features exhibited weak to moderate correlations.

---

## 📈 Visualizations Included

* Histograms
* Boxplots
* Pairplots
* Correlation Heatmap

These visualizations helped uncover trends, distributions, and relationships within the dataset.

---

## 📁 Project Structure

```text
Titanic-EDA/
│
├── data/
│   └── Titanic.csv
│
├── notebooks/
│   └── EDA.ipynb
│
├── images/
│   ├── histograms.png
│   ├── boxplots.png
│   ├── pairplot.png
│   └── correlation_heatmap.png
│
├── README.md
│
└── requirements.txt
```

---

## 🚀 Getting Started

### Clone the Repository

```bash
git clone https://github.com/PushkarAgrawal17/ElevateLabs-Task2.git
```

### Navigate to Project Directory

```bash
cd ElevateLabs-Task2
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
EDA.ipynb
```

---

## 🎓 Learning Outcomes

Through this project, I learned:

* Descriptive statistical analysis
* Data visualization techniques
* Feature distribution analysis
* Outlier detection
* Correlation analysis
* Data interpretation and storytelling
* Extracting insights from real-world datasets

---

## 🔮 Future Improvements

* Perform advanced statistical analysis
* Add interactive visualizations using Plotly
* Conduct feature engineering
  Build predictive Machine Learning models using the analyzed dataset

---

## 👨‍💻 Author

**Pushkar Agrawal**

B.Tech CSE Student | Machine Learning Enthusiast | AI Learner
