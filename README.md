# 🎬 Netflix Data Cleaning & Preprocessing Project

## 📓 View Notebook

- 🔗 [Open in Google Colab](https://colab.research.google.com/drive/1fFgKRmPJxNo1EeNoml7RzPJ5ThgQZzd6?usp=sharing)
> ⚠️ If the notebook does not render properly on GitHub, please use the links above.

---

## 📌 Overview
This project focuses on cleaning and preprocessing the Netflix Movies and TV Shows dataset.  
Real-world datasets often contain missing values, duplicates, and inconsistent formats. This project demonstrates how to handle such issues using Python and Pandas.

---

## 🎯 Objective
- Handle missing values
- Remove duplicate records
- Standardize inconsistent formats
- Convert data types
- Prepare clean dataset for analysis

---

## 📊 Dataset Information
- **Total Records:** 8807  
- **Total Columns:** 12  

---

## ⚠️ Data Issues Identified
- Missing values in:
  - `director` (2634)
  - `cast` (825)
  - `country` (831)
  - `date_added` (10)
  - `rating` (4)
  - `duration` (3)
- Inconsistent date formats (leading spaces)
- Duplicate records
- Unclean column names

---

## 🧹 Data Cleaning Steps

### 1. Handling Missing Values
- Filled `director` and `cast` with **"Unknown"**
- Filled `country` with **"Not Specified"**
- Removed rows with missing `date_added`
- Filled `rating` and `duration`

### 2. Removing Duplicates
- Used Pandas to remove duplicate rows

### 3. Standardizing Data
- Converted column names to lowercase
- Replaced spaces with underscores
- Trimmed extra spaces in text fields

### 4. Fixing Date Format
- Removed leading spaces using `.str.strip()`
- Converted to datetime using `pd.to_datetime()`
- Used `errors='coerce'` to handle invalid values

---

## 🛠️ Tools & Technologies
- Python
- Pandas
- Google Colab

---

## 📁 Project Structure

```
netflix-data-cleaning/
│
├── netflix_titles.csv
├── cleaned_netflix_data.csv
├── data_cleaning.ipynb
└── README.md
```

## ✅ Final Output
- Clean dataset with:
  - No missing values
  - Consistent formats
  - Correct data types
- Ready for analysis or visualization

---

## 📈 Key Learnings
- Handling real-world messy data
- Data preprocessing techniques
- Debugging data conversion issues
- Importance of clean data before analysis

---

## 🚀 Future Improvements
- Perform Exploratory Data Analysis (EDA)
- Create visualizations
- Build recommendation system

---

## 👩‍💻 Author
Yasodha Krishna Sajja
---

⭐ If you found this project useful, consider giving it a star!
