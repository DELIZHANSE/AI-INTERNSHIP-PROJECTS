# 📰 Fake News Prediction

## 📌 Project Overview

Fake News Prediction is a **Machine Learning and Natural Language Processing (NLP)** project that classifies news articles as **FAKE** or **REAL** based on their textual content.

The project demonstrates a complete text-classification workflow, including data preprocessing, text feature extraction, model training, and prediction.

---

## 🎯 Objective

The main objective of this project is to develop a Machine Learning model that can analyze the content of a news article and predict whether it belongs to the **FAKE** or **REAL** category.

---

## 📊 Dataset

The dataset contains **6,335 news articles** with the following main columns:

* `title` — Title of the news article
* `text` — Full text/content of the article
* `label` — Target variable (`FAKE` or `REAL`)

The dataset contains two classification categories:

* **FAKE**
* **REAL**

---

## 🔄 Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Preprocessing
   ↓
Text Cleaning
   ↓
Stopword Removal
   ↓
Stemming
   ↓
TF-IDF Feature Extraction
   ↓
Train-Test Split
   ↓
Logistic Regression
   ↓
Model Evaluation
   ↓
Fake/Real Prediction
```

---

## 🧹 Data Preprocessing

The text data is processed before being passed to the Machine Learning model.

The preprocessing steps include:

* Removing unnecessary characters
* Converting text to lowercase
* Removing English stopwords
* Applying **Porter Stemming**
* Combining relevant text information for classification

NLTK is used for stopword processing and stemming.

---

## 🔤 Feature Extraction

Since Machine Learning models cannot directly process raw text, the textual data is converted into numerical features using:

### TF-IDF — Term Frequency-Inverse Document Frequency

TF-IDF converts the news text into numerical vectors based on the importance of words within the dataset.

This allows the Machine Learning model to identify patterns in the text and distinguish between FAKE and REAL news.

---

## 🤖 Machine Learning Model

### Logistic Regression

**Logistic Regression** is used as the classification algorithm for predicting whether a news article is FAKE or REAL.

The model is trained using the TF-IDF features generated from the processed news text.

---

## 📈 Model Evaluation

The model is evaluated using **accuracy score** on the training and testing datasets.

### Results

| Dataset       |   Accuracy |
| ------------- | ---------: |
| Training Data | **95.15%** |
| Testing Data  | **92.11%** |

The testing accuracy of **92.11%** indicates that the model performed well on the held-out test data.

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **NLTK**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook**

---

## 📚 Libraries Used

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import re

from sklearn.feature_extraction.text import TfidfVectorizer
from nltk.corpus import stopwords
from nltk.stem.porter import PorterStemmer
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score
from sklearn.linear_model import LogisticRegression
```

---

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/DELIZHANSE/AI-INTERNSHIP-PROJECTS.git
```

### 2. Navigate to the project directory

```bash
cd AI-INTERNSHIP-PROJECTS/Fake-News-Prediction
```

### 3. Install the required libraries

```bash
pip install numpy pandas matplotlib seaborn scikit-learn nltk jupyter
```

### 4. Open the Jupyter Notebook

```bash
jupyter notebook FakeNews-Prediction.ipynb
```

### 5. Run the notebook cells

Run the cells sequentially to:

1. Load the dataset
2. Preprocess the text
3. Extract TF-IDF features
4. Train the Logistic Regression model
5. Evaluate the model
6. Make predictions

---

## 💡 Key Learnings

Through this project, I gained practical experience in:

* Natural Language Processing
* Text preprocessing
* Stopword removal
* Stemming
* TF-IDF vectorization
* Binary classification
* Logistic Regression
* Model evaluation
* Building a Machine Learning prediction system

---

## 🔮 Future Improvements

Possible improvements for this project include:

* Comparing multiple classification algorithms
* Hyperparameter tuning
* Cross-validation
* Improving text preprocessing
* Using advanced NLP techniques
* Implementing transformer-based models such as BERT
* Building a web interface for real-time predictions
* Deploying the model as a web application

---

## 📁 Project Structure

```text
Fake-News-Prediction/
│
├── FakeNews-Prediction.ipynb
├── news.csv.zip
└── README.md
```

---

## 👨‍💻 Author

**Deliz Hanse**

B.Tech Computer Science Engineering Student

GitHub:
https://github.com/DELIZHANSE

---

## ⭐ Project

If you found this project useful or interesting, consider giving the repository a ⭐.
