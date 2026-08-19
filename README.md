# 🤖 AI IN DATA SCIENCE

> A complete learning repository for **Artificial Intelligence and Data Science using Python**, covering Python, NumPy, Pandas, Matplotlib, Machine Learning, and Deep Learning.

---

## 📌 About the Project

**AI in Data Science** combines programming, mathematics, statistics, data analysis, visualization, and artificial intelligence to extract useful insights from data.

This repository provides a structured learning path from **Python basics to Machine Learning and Deep Learning**, along with practical examples, exercises, datasets, and projects.

### 🔄 Learning Path

```text
Python
   ↓
NumPy
   ↓
Pandas
   ↓
Matplotlib / Seaborn
   ↓
Data Analysis & Visualization
   ↓
Machine Learning
   ↓
Deep Learning
   ↓
AI Projects
```

---

## 🎯 Objectives

- Learn Python programming for Data Science.
- Understand numerical computing with NumPy.
- Learn data manipulation and analysis using Pandas.
- Create data visualizations using Matplotlib and Seaborn.
- Perform Exploratory Data Analysis (EDA).
- Understand Machine Learning concepts.
- Implement Machine Learning algorithms.
- Understand the basics of Deep Learning.
- Work with real-world datasets.
- Build practical AI and Data Science projects.

---

## 🛠️ Technologies Used

| Technology | Description |
|---|---|
| 🐍 **Python** | Programming language used for Data Science and AI |
| 🔢 **NumPy** | Numerical computing and array operations |
| 🐼 **Pandas** | Data manipulation, cleaning, and analysis |
| 📊 **Matplotlib** | Data visualization and plotting |
| 🎨 **Seaborn** | Statistical data visualization |
| 🤖 **Scikit-Learn** | Machine Learning algorithms |
| 🧠 **TensorFlow** | Deep Learning and neural networks |
| 📓 **Jupyter Notebook** | Interactive development environment |
| ☁️ **Google Colab** | Cloud-based Python environment |

---

# 📚 Contents

1. [Python](#-1-python)
2. [NumPy](#-2-numpy)
3. [Pandas](#-3-pandas)
4. [Matplotlib](#-4-matplotlib)
5. [Seaborn](#-5-seaborn)
6. [Data Analysis](#-6-data-analysis)
7. [Machine Learning](#-7-machine-learning)
8. [Deep Learning](#-8-deep-learning)
9. [Datasets](#-9-datasets)
10. [Projects](#-10-projects)
11. [Installation](#-installation)
12. [Learning Roadmap](#-learning-roadmap)
13. [How to Use](#-how-to-use)
14. [Contributing](#-contributing)
15. [Author](#-author)

---

# 🐍 1. Python

Python is the foundation of this repository.

## Topics Covered

### Basics

- Variables
- Keywords
- Identifiers
- Comments
- Data Types
- Type Checking
- Type Casting
- Input and Output

### Operators

- Arithmetic Operators
- Relational Operators
- Logical Operators
- Assignment Operators
- Bitwise Operators
- Membership Operators
- Identity Operators

### Control Flow

- `if`
- `if-else`
- `if-elif-else`
- Nested Conditions

### Loops

- `for` loop
- `while` loop
- Nested loops
- `break`
- `continue`
- `pass`

### Data Structures

- List
- Tuple
- Set
- Dictionary
- String

### Functions

- Function Definition
- Parameters
- Arguments
- Return Statement
- Default Arguments
- Keyword Arguments
- `*args`
- `**kwargs`
- Lambda Functions

### Advanced Python

- List Comprehension
- Dictionary Comprehension
- Set Comprehension
- Packing and Unpacking
- Slicing
- Exception Handling
- File Handling
- Object-Oriented Programming
- Inheritance
- Polymorphism
- Encapsulation
- Abstraction

---

# 🔢 2. NumPy

**NumPy (Numerical Python)** is used for numerical computing and working with arrays.

## Topics Covered

- NumPy Introduction
- NumPy Installation
- NumPy Arrays
- Array Creation
- Array Attributes
- Indexing
- Slicing
- Reshaping
- Iteration
- Mathematical Operations
- Statistical Operations
- Broadcasting
- Aggregation Functions

## Example

```python
import numpy as np

arr = np.array([10, 20, 30, 40, 50])

print(arr)
print("Mean:", arr.mean())
print("Maximum:", arr.max())
print("Minimum:", arr.min())
```

---

# 🐼 3. Pandas

**Pandas** is mainly used for data manipulation, data cleaning, and data analysis.

## Topics Covered

### Series

- Creating Series
- Indexing
- Slicing
- Custom Index
- Series Operations

### DataFrame

- Creating DataFrame
- Reading Data
- Selecting Columns
- Selecting Rows
- Indexing
- Filtering
- Sorting

### Data Cleaning

- Missing Values
- `isnull()`
- `notnull()`
- `dropna()`
- `fillna()`
- Duplicate Values
- Data Type Conversion

### Data Analysis

- `head()`
- `tail()`
- `info()`
- `describe()`
- `shape`
- `columns`
- `dtypes`
- `value_counts()`

### Combining DataFrames

- `merge()`
- `join()`
- `concat()`

### Grouping

- `groupby()`
- Aggregation
- Multiple Aggregations

## Example

```python
import pandas as pd

data = {
    "Name": ["A", "B", "C"],
    "Marks": [80, 90, 75]
}

df = pd.DataFrame(data)

print(df)

print("Average Marks:", df["Marks"].mean())
```

---

# 📊 4. Matplotlib

**Matplotlib** is a Python library used for creating graphs and visualizations.

## Visualizations Covered

- Line Plot
- Bar Chart
- Horizontal Bar Chart
- Scatter Plot
- Histogram
- Pie Chart
- Box Plot

## Customization

- Title
- X-axis Label
- Y-axis Label
- Legend
- Grid
- Figure Size
- Markers
- Line Style
- Line Width

## Example

```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [10, 20, 15, 25, 30]

plt.plot(x, y, marker="o")

plt.xlabel("X Values")
plt.ylabel("Y Values")
plt.title("Line Plot")

plt.grid()
plt.show()
```

---

# 🎨 5. Seaborn

**Seaborn** is a Python visualization library built on top of Matplotlib.

## Topics Covered

- Line Plot
- Bar Plot
- Scatter Plot
- Histogram
- Box Plot
- Violin Plot
- Count Plot
- Heatmap
- Pair Plot

## Example

```python
import seaborn as sns
import matplotlib.pyplot as plt

sns.scatterplot(
    x="bill_length_mm",
    y="bill_depth_mm",
    data=df,
    hue="sex"
)

plt.show()
```

---

# 📈 6. Data Analysis

Data Analysis is the process of inspecting, cleaning, transforming, and interpreting data.

## Data Analysis Process

```text
Collect Data
     ↓
Understand Data
     ↓
Clean Data
     ↓
Transform Data
     ↓
Analyze Data
     ↓
Visualize Data
     ↓
Find Patterns
     ↓
Generate Insights
```

---

# 🔍 Exploratory Data Analysis (EDA)

EDA helps us understand the structure and patterns present in a dataset.

## EDA Includes

- Understanding Dataset
- Checking Shape
- Checking Data Types
- Missing Value Analysis
- Duplicate Analysis
- Statistical Analysis
- Univariate Analysis
- Bivariate Analysis
- Multivariate Analysis
- Data Visualization
- Finding Correlations

---

# 🤖 7. Machine Learning

Machine Learning enables computers to learn patterns from data and make predictions or decisions.

## Types of Machine Learning

### Supervised Learning

The model learns from **labeled data**.

Examples:

- Regression
- Classification

### Unsupervised Learning

The model finds patterns in **unlabeled data**.

Examples:

- Clustering
- Dimensionality Reduction

---

## 📌 Regression

Regression is used when the output is generally a continuous numerical value.

Examples:

- House Price Prediction
- Sales Prediction
- Salary Prediction

### Algorithms

- Linear Regression
- Multiple Linear Regression
- Polynomial Regression
- Decision Tree Regression
- Random Forest Regression

---

## 📌 Classification

Classification is used to predict categories or classes.

Examples:

- Spam / Not Spam
- Pass / Fail
- Disease / No Disease
- Customer Churn

### Algorithms

- Logistic Regression
- K-Nearest Neighbors
- Decision Tree
- Random Forest
- Support Vector Machine
- Naive Bayes

---

## 📌 Clustering

Clustering groups similar data points together.

### Algorithms

- K-Means
- Hierarchical Clustering
- DBSCAN

---

# 🧠 8. Deep Learning

Deep Learning is a subset of Machine Learning that uses artificial neural networks with multiple layers.

## Topics Covered

- Artificial Neural Networks
- Neurons
- Input Layer
- Hidden Layer
- Output Layer
- Activation Functions
- Forward Propagation
- Backpropagation
- Loss Functions
- Optimizers
- Epochs
- Batch Size
- Model Training
- Model Evaluation

---

## 🧠 Neural Network Structure

```text
Input Layer
     ↓
Hidden Layer 1
     ↓
Hidden Layer 2
     ↓
Hidden Layer 3
     ↓
Output Layer
```

---

## Deep Learning Applications

- Image Classification
- Face Recognition
- Object Detection
- Speech Recognition
- Natural Language Processing
- Chatbots
- Recommendation Systems
- Computer Vision

---

# 📂 9. Datasets

Datasets are used for practicing Data Science, Machine Learning, and Deep Learning concepts.

## Example Datasets

- Iris Dataset
- Titanic Dataset
- Penguins Dataset
- Student Performance Dataset
- Sales Dataset
- Customer Dataset
- Housing Dataset

Datasets can be stored inside:

```text
Datasets/
```

---

# 🚀 10. Projects

This repository can contain practical projects such as:

### 📊 Data Analysis Projects

- Student Performance Analysis
- Sales Data Analysis
- Customer Data Analysis
- Employee Data Analysis

### 🤖 Machine Learning Projects

- House Price Prediction
- Student Score Prediction
- Customer Churn Prediction
- Spam Detection
- Iris Classification

### 🧠 Deep Learning Projects

- Image Classification
- Handwritten Digit Recognition
- Object Detection
- Sentiment Analysis

---

# 📁 Repository Structure

```text
AI-IN-DATASCIENCE/
│
├── README.md
│
├── Python/
│   ├── Basics/
│   ├── Data_Types/
│   ├── Operators/
│   ├── Conditions/
│   ├── Loops/
│   ├── Functions/
│   ├── Data_Structures/
│   ├── File_Handling/
│   └── OOP/
│
├── NumPy/
│   ├── Arrays/
│   ├── Indexing/
│   ├── Slicing/
│   └── Operations/
│
├── Pandas/
│   ├── Series/
│   ├── DataFrame/
│   ├── Data_Cleaning/
│   ├── GroupBy/
│   ├── Merge/
│   ├── Join/
│   └── Concat/
│
├── Matplotlib/
│   ├── Line_Plot/
│   ├── Bar_Plot/
│   ├── Scatter_Plot/
│   ├── Histogram/
│   └── Pie_Chart/
│
├── Seaborn/
│   ├── Line_Plot/
│   ├── Scatter_Plot/
│   ├── Box_Plot/
│   ├── Count_Plot/
│   └── Heatmap/
│
├── Machine_Learning/
│   ├── Regression/
│   ├── Classification/
│   ├── Clustering/
│   └── Projects/
│
├── Deep_Learning/
│   ├── Neural_Networks/
│   ├── CNN/
│   ├── RNN/
│   └── Projects/
│
├── Datasets/
│
└── Projects/
```

---

# 💻 Installation

## Step 1: Install Python

Install Python on your system.

## Step 2: Install Required Libraries

```bash
pip install numpy
pip install pandas
pip install matplotlib
pip install seaborn
pip install scikit-learn
pip install tensorflow
```

Or install everything together:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow
```

---

# 📓 Google Colab

This repository can also be used with **Google Colab**.

Example:

```python
!pip install numpy pandas matplotlib seaborn scikit-learn
```

To upload files:

```python
from google.colab import files

uploaded = files.upload()
```

---

# 🧪 Basic Data Science Example

```python
import pandas as pd
import matplotlib.pyplot as plt

data = {
    "Student": ["A", "B", "C", "D"],
    "Marks": [80, 90, 70, 85]
}

df = pd.DataFrame(data)

print(df)

plt.bar(df["Student"], df["Marks"])

plt.xlabel("Students")
plt.ylabel("Marks")
plt.title("Student Marks")

plt.show()
```

---

# 🔄 Complete AI & Data Science Workflow

```text
                    DATA
                      │
                      ↓
              Data Collection
                      │
                      ↓
               Data Cleaning
                      │
                      ↓
               Data Processing
                      │
                      ↓
                 EDA / Analysis
                      │
                      ↓
                Visualization
                      │
                      ↓
             Feature Engineering
                      │
                      ↓
              Machine Learning
                      │
                      ↓
                Model Training
                      │
                      ↓
               Model Evaluation
                      │
                      ↓
                  Prediction
                      │
                      ↓
               Deep Learning
                      │
                      ↓
                  AI Project
```

---

# 🗺️ Learning Roadmap

## Level 1 — Python

```text
Python Basics
     ↓
Data Types
     ↓
Control Flow
     ↓
Functions
     ↓
Data Structures
     ↓
OOP
```

## Level 2 — Data Science Libraries

```text
NumPy
  ↓
Pandas
  ↓
Matplotlib
  ↓
Seaborn
```

## Level 3 — Data Analysis

```text
Data Cleaning
     ↓
EDA
     ↓
Statistics
     ↓
Visualization
```

## Level 4 — Machine Learning

```text
ML Basics
   ↓
Regression
   ↓
Classification
   ↓
Clustering
   ↓
Model Evaluation
```

## Level 5 — Deep Learning

```text
Neural Networks
      ↓
Deep Neural Networks
      ↓
CNN
      ↓
RNN
      ↓
AI Applications
```

---

# 📊 Machine Learning Workflow

```text
Dataset
   ↓
Data Cleaning
   ↓
Feature Selection
   ↓
Train-Test Split
   ↓
Model Selection
   ↓
Model Training
   ↓
Prediction
   ↓
Evaluation
   ↓
Model Improvement
```

---

# 📌 Important Python Libraries

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import accuracy_score
```

---

# 🌍 Applications of AI & Data Science

AI and Data Science are widely used in:

- 🏦 Banking and Finance
- 🏥 Healthcare
- 🛒 E-Commerce
- 📱 Mobile Applications
- 🚗 Autonomous Vehicles
- 🎬 Recommendation Systems
- 🔍 Fraud Detection
- 📈 Business Analytics
- 🖼️ Computer Vision
- 💬 Natural Language Processing
- 🎤 Speech Recognition
- 🤖 Robotics

---

# 🎓 Learning Outcomes

After completing this repository, learners will be able to:

- Write Python programs.
- Work with NumPy arrays.
- Manipulate datasets using Pandas.
- Clean real-world datasets.
- Perform Exploratory Data Analysis.
- Create meaningful visualizations.
- Understand Machine Learning.
- Train basic ML models.
- Evaluate ML models.
- Understand Neural Networks.
- Understand the fundamentals of Deep Learning.
- Build basic AI projects.

---

# ⭐ Why This Repository?

This repository is designed as a **step-by-step learning resource**.

It focuses on:

```text
📖 Theory
   +
💻 Code
   +
🧪 Practice
   +
📊 Data Analysis
   +
🤖 Machine Learning
   +
🧠 Deep Learning
   =
🚀 AI & Data Science Skills
```

---

# 🤝 Contributing

Contributions are welcome!

If you want to contribute:

1. Fork this repository.
2. Create a new branch.
3. Add your changes.
4. Commit your changes.
5. Push the branch.
6. Create a Pull Request.

Example:

```bash
git clone <repository-url>

cd AI-IN-DATASCIENCE

git checkout -b feature/new-topic

git add .

git commit -m "Add new Data Science topic"

git push origin feature/new-topic
```

---

# 📜 License

This repository is created for **educational and learning purposes**.

You are free to use the examples and learning materials for educational purposes.

---

# 👨‍💻 Author

## Chetan

**AI | Data Science | Python | Machine Learning | Deep Learning**

---

# ⭐ Support

If you find this repository useful:

- ⭐ Star the repository
- 🍴 Fork the repository
- 📢 Share it with other learners
- 🤝 Contribute to the project

---

# 🚀 Keep Learning

```text
Learn → Practice → Analyze → Build → Improve
```

> **"Data is the foundation. AI is the intelligence. Python connects them both."** 🤖📊
