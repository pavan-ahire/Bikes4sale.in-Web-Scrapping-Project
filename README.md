# 🚀 Used Bike Market Analysis – Bikes4Sale.in  
This project is a complete end-to-end Data Analytics workflow, starting from **Web Scraping real marketplace data**, transforming it into a clean structured dataset, and performing deep **Exploratory Data Analysis (EDA)** to uncover insights about India’s used bike market.

This project reflects real-world industry practices used in Data Analytics, Business Intelligence, and Data Science roles.

---

## 📌 1. Project Introduction

The Indian used two-wheeler market is booming, with thousands of listings posted daily on platforms like Bikes4Sale.in. Yet, **no public dataset** exists that captures bike pricing, popularity, model behavior, or city-wise demand.

To fill this gap, I created a dataset **from scratch** through web scraping and used it to answer key market questions.

### Why This Project Is Important
- The automotive resale market is **data-driven**, yet publicly available insights are limited.  
- Buyers often need guidance on **price fairness**, **brand reliability**, and **value retention**.  
- Sellers and dealerships require data to understand **market demand**, **competition**, and **regional behavior**.  
- This project showcases the **entire analytics pipeline**, proving real-world skill, not just theoretical knowledge.

This README explains every step with clarity to demonstrate strong analytical, technical, and business storytelling skills.

---

## 🔄 2. Project Workflow (Detailed Explanation)


### What Each Step Means

#### **1. Web Scraping**
The platform does not offer APIs. Therefore, BeautifulSoup was used to extract structured data directly from HTML pages.

#### **2. Data Cleaning**
Raw scraped data is usually messy. Missing values, inconsistencies, merged fields, and text noise are removed.

#### **3. Feature Engineering**
New attributes such as **Brand Origin**, **Model Type**, and **City-State split** were created to enrich the dataset.

#### **4. EDA**
Using plots and statistics to understand the dataset from:
- Single-variable perspective (Univariate)  
- Two-variable relationships (Bivariate)  
- Multi-factor interactions (Multivariate)

#### **5. Insight Generation**
Insights are written from a business perspective, not just technical.

#### **6. Conclusion**
Final learnings and actionable takeaways are listed.

This pipeline resembles how real analytics teams work in finance, marketing, operations, and product analysis.

---

## 🛠 3. Tech Stack (Detailed)

### 🧩 Languages & Libraries

#### **Python**
Chosen for its simplicity and data ecosystem strength.

#### **BeautifulSoup**
Used for HTML parsing, extracting bike details like model name, price, and city from raw web pages.

#### **Requests**
Handles HTTP page fetching.

#### **Pandas**
The backbone of cleaning, transformation, and table manipulation.

#### **NumPy**
Used for numeric manipulation, type conversion, and scaling.

#### **Matplotlib & Seaborn**
Generated visualization to detect patterns, compare distributions, and analyze relationships.

### 🧰 Tools

#### **Google Colab / Jupyter**
Notebook environment for experimenting and visualizing the data.

#### **Git & GitHub**
Version control, project tracking, and portfolio presentation.

#### **CSV**
Lightweight format used to store raw and cleaned data.

Every tool contributes to a real-world workflow used in analytics teams.

---

## 🌐 4. Web Scraping (In-Depth Explanation)

The scraping process involved navigating 40 pages of live bike listings.

### Steps Followed:
1. **Sending HTTP requests** to each page link  
2. **Parsing HTML tags** for bike name, model year, price, location, and finance status  
3. **Extracting raw text** inside div and span tags  
4. **Converting them into structured rows**  
5. **Storing results into Pandas DataFrame**

### Scraped Fields (Raw)
- Bike Model (contains brand + name)  
- Model Year  
- Raw Price (mixed commas, currency symbols)  
- Location (City + State merged)  
- Finance Availability (Yes/No)

### Example Raw Entry
- Bike Name : Royal Enfield Classic 500
- Year : 2016
- Location : Gurgaon, Haryana
- Price : 70,000
- Finance Available : Yes

  
### 🧮 Before Cleaning (Raw Dataset)
**1628 rows × 5 columns**

#### Problems Found
- Price had rupee signs, commas, and blank fields  
- City and State were merged inside a single string  
- Brand was inside Model Name  
- Duplicate rows across multiple pages  
- Model year had inconsistent formats  
- No structured categorization (bike type, origin, etc.)  
- Some bikes had missing or irrelevant values  

This stage required heavy preprocessing before any analysis.

---

## 🧼 After Cleaning (Final Dataset)
**1501 rows × 9 columns**

### ✔ All Fixes & Transformations
- Removed 120+ duplicate entries  
- Standardized price to integer format  
- Separated Location → **City** and **State**  
- Extracted **Brand** from model name  
- Recategorized bikes into **Model Type**:
  - Commuter  
  - Sports  
  - Cruiser  
  - Adventure  
  - Scooter  
  - Electric  
- Added **Brand Origin** (India, Japan, Austria, China, UK, USA, etc.)  
- Fixed inconsistent capitalization  
- Removed noisy symbols and formatting errors  

This created an analytics-ready dataset.

---

## 🔍 6. Exploratory Data Analysis (EDA)

### 📘 6.1 Univariate Analysis (Detailed)

Here, each column is studied individually.

#### 1. **Brand Distribution**
Identifies which brands dominate the used market.

#### 2. **Model Year Distribution**
Shows whether buyers prefer new or old models.

#### 3. **Price Distribution**
Right-skew helps identify:
- Budget bikes  
- Median pricing  
- Premium outliers (Harley, BMW, Ducati)

#### 4. **Location Analysis (City/State)**
Helps determine which regions have the most active markets.

#### Key Insights
- Bajaj, Royal Enfield, Honda appear most frequently  
- 2022–2023 models dominate  
- Majority prices lie between 50,000–1,50,000  
- Bangalore, Pune, Hyderabad lead in listings  

---

### 📗 6.2 Bivariate Analysis (Detailed)

Studies relationships between two variables.

#### Examples:
- Does price vary across states?  
- Do foreign brands cost more than Indian ones?  
- Which bike types show wide price variation?  
- Which city has the highest average resale price?

#### Major Findings:
- Pondicherry shows premium listing prices  
- USA-origin bikes (Harley-Davidson) lead pricing  
- Adventure bikes have the largest price spread  
- Commuter and scooter segments stay affordable  

---

### 📙 6.3 Multivariate Analysis (Detailed)

Here, multiple factors are compared together to reveal deeper insights.

#### Example Combinations:
- Model Type + State + Price  
- Brand Origin + Model Type + Price  

#### Discoveries:
- Karnataka & Haryana show higher premium pricing  
- Italian/Japanese brands dominate high-end sports bikes  
- Indian brands dominate commuter & EV segments  

---

## ⭐ 7. Key Insights Summary (Expanded)

- **Royal Enfield Classic 350** is the most popular and most listed model  
- **Bajaj, Honda, and Royal Enfield** form the backbone of the market  
- Newer bikes (2020+) have significantly better resale value  
- Metro cities create higher demand and faster sales  
- Foreign brands retain value better but have limited presence  
- Price depends on:
  - Brand reputation  
  - Bike type  
  - City economics  
  - Age of the vehicle  

These insights are actionable for buyers, sellers, and dealerships.

---

## 📈 8. Business Impact of This Project

This project provides:
- A **market overview** for buyers  
- Competitive positioning insights for sellers  
- A structured dataset for future **price prediction models**  
- City-level pricing intelligence  
- Brand-level performance indicators  
- Insights into emerging segments (EVs, premium bikes)

Companies in automotive resale, marketing, finance, or analytics can use this dataset for strategy building.

---

## 📞 9. Contact

**Author:** Pavan Ahire  
**LinkedIn:** https://www.linkedin.com/in/pavan-ahire-260940364  
**GitHub:** https://github.com/pavan-ahire  

