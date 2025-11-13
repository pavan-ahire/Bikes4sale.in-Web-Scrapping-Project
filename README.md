# 🚀 Used Bike Market Analysis – Bikes4Sale.in  
A complete end-to-end **Data Analytics Project** involving **Web Scraping**, **Data Cleaning**, **Feature Engineering**, and **Exploratory Data Analysis (EDA)** on the Indian used two-wheeler market.

---

## 📌 1. Project Introduction
This project analyzes real-world data scraped from **Bikes4Sale.in**, one of India’s leading used bike marketplaces.

The objective is to understand:

- 📈 Market demand patterns  
- 💰 Pricing trends  
- 🏍 Brand competitiveness  
- 🏙 City-wise market behavior  
- 📅 Influence of model year, brand & model type on price  

This project demonstrates strong skills in **Python, Web Scraping, EDA, Visualization**, and deriving **business insights** from real data.

---

## 🔄 2. Project Workflow

  Web Scraping → Data Cleaning → Feature Engineering → EDA (Univariate • Bivariate • Multivariate) → Insights & Conclusion

Each step follows a clean, industry-standard approach.

---

## 🛠 3. Tech Stack

### 🧩 Languages & Libraries
- Python  
- BeautifulSoup (Web Scraping)  
- Requests  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  

### 🧰 Tools
- Google Colab / Jupyter Notebook  
- Git & GitHub  
- CSV for dataset storage  

---

## 🌐 4. Web Scraping

Data was scraped from **40 pages** of used bike listings on Bikes4Sale.in.

### 📥 Extracted Fields
- Brand  
- Bike Model  
- Model Year  
- Price  
- City  
- State  
- Finance Availability  
- Model Type (Engineered later)  

### 📦 Example Scraped Record

- Bike Name : Royal Enfield Classic 500
- Year : 2016
- Location : Gurgaon, Haryana
- Price : 70,000
- Finance Available: Yes

  
---

## 📊 5. Dataset Overview

### 🧮 Before Cleaning (Raw Dataset – 1628 rows × 5 columns)
Upload your image and rename the path:

<img width="720" alt="before_cleaning" src="https://github.com/user-attachments/assets/before.png" />
**Issues Identified**
- Missing values  
- Duplicate rows  
- Unstructured text  
- Location column merged  
- Brand embedded inside Model  
- No model-type classification  
- Inconsistent formatting  

---

### 🧼 After Cleaning (Final Dataset – 1501 rows × 9 columns)

Upload your image and rename the path:

<img width="720" alt="before_cleaning" src="https://github.com/user-attachments/assets/after.png" />


**Transformations Applied**
- Removed duplicates  
- Fixed missing values  
- Corrected data types  
- Split *Location → City, State*  
- Extracted *Brand* from Model  
- Added **Brand Origin**  
- Added **Model Type**  
- Standardized formatting  

---

## 🔍 6. Exploratory Data Analysis (EDA)

### 📘 6.1 Univariate Analysis
Fields analyzed:
- Brand  
- Model Year  
- City  
- State  
- Model Type  
- Finance Availability  
- Price  

**Key Highlights**
- Bajaj, Royal Enfield, Honda dominate listings  
- Most bikes listed belong to **2022–2023**  
- Price distribution is **right-skewed**  
- EV & premium bike segments are rising  

---

### 📗 6.2 Bivariate Analysis
Relationships evaluated:
- State vs Average Price  
- Brand Origin vs Price  
- Model Type vs Price  
- Brand vs Price  
- City vs Price  

**Key Findings**
- Pondicherry has the **highest average bike prices**  
- USA-origin bikes are the most expensive  
- Adventure bikes show the widest price range  

---

### 📙 6.3 Multivariate Analysis
Analyzed combined effects of:
- State + Model Type + Price  
- Brand Origin + Model Type + Price  

**Insights**
- Karnataka & Haryana show **premium pricing**  
- Japanese & Italian brands dominate sports/adventure segments  
- Indian brands dominate commuter & EV categories  

---

## ⭐ 7. Key Insights Summary

- **Royal Enfield Classic 350** is the most frequently listed bike  
- **Bajaj, Royal Enfield, Honda** dominate Indian market supply  
- Newer models (2020–2025) show **stronger resale value**  
- **Bangalore, Pune, Hyderabad, Delhi** are major hubs  
- Price variation depends on:  
  - Brand value  
  - Model year  
  - City economics  
  - Bike segment (Commuter, Sports, EV, Adventure)  

---

## 📞 10. Contact

**👤 Author:** Pavan Ahire  
**🔗 LinkedIn:** https://www.linkedin.com/in/pavan-ahire-260940364  
**💻 GitHub:** https://github.com/pavan-ahire  

---
<h3>📊 Before Cleaning</h3>

<img width="720" alt="before_cleaning" src="images/before.png" />

<h3>🧼 After Cleaning</h3>

<img width="720" alt="after_cleaning" src="images/after.png" />

  
