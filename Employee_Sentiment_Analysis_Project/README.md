# 🏢 Employee Sentiment Analysis Project

**Author:** Doyel Mishra  
**Project Type:** AI/ML / Natural Language Processing  
**Status:** Completed  

---

## 🌟 Project Overview

This project analyzes employee messages to assess **sentiment, engagement, and flight risk**, and builds **predictive models** to forecast trends. It demonstrates skills in **NLP, data preprocessing, exploratory data analysis (EDA), sentiment scoring, ranking, and linear regression modeling**.

> ⚠️ **Note:** The raw dataset (`test(in).csv`) is **not included** due to privacy restrictions.  
> All analyses are performed using **processed data (`processed_data.pkl`)**, and results are available in the included output files.

---

## 📝 Project Workflow

1. **Data Preprocessing & Cleaning**  
   - Clean text data, remove stopwords, punctuation, and irrelevant content.
   - Save **TF-IDF vectorizer** and preprocessed data for reproducibility.

2. **Sentiment Labeling**  
   - Classify employee messages as **Positive**, **Negative**, or **Neutral** using NLP pipelines.

3. **Exploratory Data Analysis (EDA)**  
   - Analyze dataset structure, trends, and anomalies.
   - Output summaries in `eda_summary.csv`.
   - Visualizations stored in the `visualizations` folder.

4. **Monthly Sentiment Scoring**  
   - Assign sentiment scores: Positive (+1), Neutral (0), Negative (-1).  
   - Aggregate scores per employee per month for ranking.

5. **Employee Ranking**  
   - Identify **Top 3 Positive Employees** and **Top 3 Negative Employees** per month.
   - Rankings derived from monthly sentiment scores.

6. **Flight Risk Identification**  
   - Flag employees sending **4 or more negative messages in a rolling 30-day window**.

7. **Predictive Modeling**  
   - Linear regression to predict monthly sentiment scores using features like message frequency, word count, and average message length.

---

## 📁 Repository Structure
```
DoyelMishra_AI-project-submission/
│
├─ Employee_Sentiment_Analysis_Project.ipynb # Main notebook
├─ processed_data.pkl # Preprocessed dataset
├─ tfidf_vectorizer.pkl # TF-IDF vectorizer
├─ sentiment_output.csv # Sentiment-labeled messages
├─ eda_summary.csv # EDA summary
├─ visualizations/ # Charts & graphs
├─ requirements.txt # Dependencies
├─ README.md # This file
└─ .gitignore # Ignore raw data & caches
```

---

## 📊 Key Files

| File | Description |
|------|-------------|
| `Employee_Sentiment_Analysis_Project.ipynb` | Main notebook implementing all tasks |
| `processed_data.pkl` | Preprocessed and vectorized data for reproducibility |
| `tfidf_vectorizer.pkl` | Saved TF-IDF vectorizer for NLP tasks |
| `sentiment_output.csv` | Employee messages labeled with sentiment |
| `eda_summary.csv` | Summary statistics and observations from EDA |
| `visualizations/` | Charts of sentiment trends, top employees, and flight risks |

---

## 🛠️ Technologies & Libraries

- **Programming Language:** Python 3.13  
- **Data Handling:** Pandas, NumPy  
- **NLP & Sentiment Analysis:** HuggingFace Transformers, TextBlob  
- **Machine Learning:** scikit-learn (Linear Regression)  
- **Visualization:** Matplotlib, Seaborn  
- **Serialization:** joblib (for vectorizers & processed data)

---

## 🏃 How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/AI_ML_Projects.git
cd DoyelMishra_AI-project-submission

2. Install dependencies:
```bash
pip install -r requirements.txt

3. Open the Jupyter Notebook:
```bash
jupyter notebook Employee_Sentiment_Analysis_Project.ipynb

4. Run the notebook sequentially. All results are reproducible using the included processed data files.
