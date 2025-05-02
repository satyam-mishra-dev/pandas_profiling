
# 📋 Automated EDA with Pandas Profiling

A lightweight project using [Pandas Profiling](https://github.com/pandas-profiling/pandas-profiling) to generate interactive exploratory data analysis reports with minimal code.

---

## 🧠 Overview

Pandas Profiling generates a comprehensive EDA report for a DataFrame in just one line of code — including statistics, distributions, correlations, and missing values visualization.

---

## 🚀 Features

- One-line EDA report generation
- Summary statistics for each column
- Correlation matrix
- Missing value analysis
- Interactive HTML reports

---

## 📁 Project Structure

```

pandas-profiling-eda/
│
├── data/                  # Sample datasets (CSV, JSON)
├── reports/               # Auto-generated HTML reports
├── notebooks/             # Example usage in Jupyter
├── generate\_report.py     # Script to generate a profiling report
├── requirements.txt
└── README.md

````

---

## 🛠️ Installation

```bash
git clone https://github.com/yourusername/pandas-profiling-eda.git
cd pandas-profiling-eda
pip install -r requirements.txt
````

---

## 📈 Usage

**In script:**

```python
import pandas as pd
from pandas_profiling import ProfileReport

df = pd.read_csv("data/your_dataset.csv")
profile = ProfileReport(df, title="EDA Report", explorative=True)
profile.to_file("reports/eda_report.html")
```

**In Jupyter Notebook:**

```python
profile.to_notebook_iframe()
```

---

## 📦 Dependencies

* pandas
* pandas-profiling
* jupyter (optional for notebooks)

---

## 📊 Sample Output

Generated HTML report includes:

* Column-wise summary stats
* Histogram and correlation plots
* Duplicates & missing values visualization

Check `/reports/eda_report.html` for an example.

---

## 📄 License

MIT License – free to use, modify, and share.

---

## 🙌 Acknowledgements

* [Pandas Profiling](https://github.com/pandas-profiling/pandas-profiling)
* [YData](https://github.com/ydataai) for maintaining the tool

