# 📱 Google Play Store Dataset – EDA & Feature Engineering

This repository contains complete Exploratory Data Analysis (EDA) and Feature Engineering on the Google Play Store dataset.  
The project aims to explore app categories, installation patterns, sizes, ratings, and other important characteristics of mobile apps on Google Play Store.

---

## 📌 Problem Statement
With over **2.56 million** apps available on the Google Play Store, applications have become an essential part of modern digital life.  
The goal of this project is to analyze:

- The most popular categories  
- Apps with the largest number of installs  
- The largest-sized applications  
- Distribution of ratings  
- Trends based on last update date  

---

## 📥 Dataset Information
- **20 Columns**  
- **10,841 Rows**  
- Dataset includes app name, category, rating, size, installs, price, last updated date, and more.

Dataset Source:  
👉 `https://raw.githubusercontent.com/krishnaik06/playstore-Dataset/main/googleplaystore.csv`

---

## 🧹 Steps Performed in This Project
### ✔ 1. Data Cleaning
- Converted non-numeric `Reviews` values into integers  
- Cleaned `Size` column (converted M → 000, removed “Varies with device”)  
- Cleaned `Installs` & `Price` columns (removed + , $ symbols)
- Converted data types appropriately  
- Dropped corrupted rows  
- Handled missing values  

### ✔ 2. Feature Engineering
- Extracted **Day, Month, Year** from `Last Updated` column  
- Converted date to datetime format  
- Removed duplicates based on app name  
- Created a cleaned dataset (`google_cleaned.csv`)  

### ✔ 3. Exploratory Data Analysis (EDA)
- Univariate analysis of numerical & categorical features  
- Top categories by count  
- Most popular categories by installs  
- Top 5 installed apps in each major category  
- Apps with 5-star ratings  
- Visualizations using Seaborn & Matplotlib  

---

## 📊 Key Insights

### 🔹 Most Popular Category (by app count)
- **Family, Games, Tools** dominate the Play Store  
- Least popular categories: Beauty, Comics, Weather

### 🔹 Category with Highest Installations
- **GAME** is the most installed category (~35 Billion installs)

### 🔹 Top Installed Apps (Sample)
- **Game:** Subway Surfers  
- **Communication:** Hangouts  
- **Productivity:** Google Drive  
- **Social:** Instagram  

### 🔹 5-Star Rated Apps
- Total: **271 Apps**  
- Highest-rated example: *CT Brain Interpretation* (Family Category)

---

## 🛠️ Technologies Used
- Python  
- Pandas  
- NumPy  
- Seaborn  
- Matplotlib  
- Jupyter Notebook  

---

## 📂 Project Structure
```
📁 google-playstore-eda-feature-engineering
│── 📄 README.md
│── 📄 playstore_analysis.ipynb
│── 📄 google_cleaned.csv
│── 📁 data/
│── 📁 images/
```

---

## 🚀 How to Run the Project
```
pip install pandas numpy seaborn matplotlib
```

Then open:

```
jupyter notebook playstore_analysis.ipynb
```

---

## ⭐ Support
If you found this project helpful, consider giving the repository a ⭐!

