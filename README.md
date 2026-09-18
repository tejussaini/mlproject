# Student Performance Indicator

## 📌 Project Overview

The **Student Performance Indicator** is a Machine Learning project that analyzes how different student-related factors affect their performance in examinations.

The project studies the relationship between students' test scores and variables such as **gender, race/ethnicity, parental level of education, lunch type, and test preparation course**.

The project follows the complete Machine Learning project lifecycle, starting from understanding the problem and collecting data to exploratory data analysis, preprocessing, model training, and selecting the best-performing model.

---

## 🎯 Problem Statement

The objective of this project is to understand how a student's performance in examinations is affected by different demographic, educational, and preparation-related factors.

The target performance measures in the dataset are:

* Math Score
* Reading Score
* Writing Score

The project explores how these scores vary according to the available categorical features.

---

## 📊 Dataset

The dataset contains **1,000 student records and 8 columns**.

### Dataset Source

The dataset is obtained from Kaggle:

`https://www.kaggle.com/datasets/spscientist/students-performance-in-exams`

### Dataset Features

| Feature                       | Description                                       |
| ----------------------------- | ------------------------------------------------- |
| `gender`                      | Gender of the student                             |
| `race_ethnicity`              | Ethnicity group of the student                    |
| `parental_level_of_education` | Parent's final education level                    |
| `lunch`                       | Lunch type: standard or free/reduced              |
| `test_preparation_course`     | Whether the test preparation course was completed |
| `math_score`                  | Mathematics examination score                     |
| `reading_score`               | Reading examination score                         |
| `writing_score`               | Writing examination score                         |

---

## 🔄 Machine Learning Project Lifecycle

The project follows these major stages:

1. Understanding the Problem Statement
2. Data Collection
3. Data Checks
4. Exploratory Data Analysis
5. Data Pre-Processing
6. Model Training
7. Model Selection

---

## 🛠️ Technologies and Libraries Used

The project uses Python and the following libraries:

* **Python**
* **NumPy** – Numerical operations
* **Pandas** – Data manipulation and analysis
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Scikit-learn** – Machine Learning

---

## 🔍 Data Exploration and Analysis

The dataset is explored using Pandas, Matplotlib, and Seaborn.

The analysis includes:

* Viewing the first few records
* Checking the shape of the dataset
* Checking data types
* Checking missing values
* Checking duplicate records
* Finding unique values
* Examining statistical characteristics
* Exploring categorical variables
* Separating numerical and categorical features

The dataset contains:

* **3 numerical features**

  * `math_score`
  * `reading_score`
  * `writing_score`

* **5 categorical features**

  * `gender`
  * `race_ethnicity`
  * `parental_level_of_education`
  * `lunch`
  * `test_preparation_course`

---

## 🧹 Data Quality Checks

Several checks are performed before proceeding with the analysis.

### Missing Values

The dataset was checked for missing values. No missing values were found in the available columns.

### Duplicate Values

The dataset was checked for duplicate records. No duplicate records were found.

### Data Types

The dataset contains:

* 5 categorical/object columns
* 3 numerical/integer columns

---

## 📈 Feature Engineering

Two additional features are created from the examination scores:

### Total Score

The total score is calculated by adding the math, reading, and writing scores.

```python
df['total score'] = (
    df['math_score'] +
    df['reading_score'] +
    df['writing_score']
)
```

### Average Score

The average score is calculated from the total score.

```python
df['average'] = df['total score'] / 3
```

These features provide an overall representation of a student's examination performance.

---

## 📊 Statistical Analysis

The numerical features are analyzed using descriptive statistics such as:

* Count
* Mean
* Standard deviation
* Minimum
* 25th percentile
* Median
* 75th percentile
* Maximum

The observed mean scores in the dataset are approximately:

| Subject | Mean Score |
| ------- | ---------: |
| Math    |      66.09 |
| Reading |      69.17 |
| Writing |      68.05 |

---

## 📁 Project Structure

```text
Student-Performance-Indicator/
│
├── data/
│   └── stud.csv
│
├── notebook/
│   └── EDA.ipynb
│
├── src/
│   ├── components/
│   ├── pipeline/
│   ├── exception.py
│   ├── logger.py
│   └── utils.py
│
├── artifacts/
│
├── requirements.txt
│
├── setup.py
│
└── README.md
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone <your-repository-url>
cd Student-Performance-Indicator
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate the virtual environment on Windows:

```bash
venv\Scripts\activate
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

---

## 🚀 Running the Project

After installing the dependencies, run the project components according to the project structure.

For exploratory analysis, open the Jupyter Notebook:

```bash
jupyter notebook
```

Then open the project notebook and execute the cells sequentially.

---

## 📌 Key Observations

The exploratory analysis provides an overview of:

* Student demographic information
* Parental education levels
* Lunch categories
* Test preparation status
* Mathematics performance
* Reading performance
* Writing performance
* Overall student performance through total and average scores

---

## 🔮 Future Improvements

Possible future improvements include:

* Implementing multiple Machine Learning regression models
* Comparing model performance using appropriate evaluation metrics
* Hyperparameter tuning
* Creating a complete prediction pipeline
* Building a web interface for predictions
* Deploying the application using cloud services
* Adding automated model training and evaluation

---

## 👨‍💻 Author

**Tejus Saini**

B.Tech — Artificial Intelligence / Data Science / IIoT

---

## 📄 License

This project is intended for educational and learning purposes.
