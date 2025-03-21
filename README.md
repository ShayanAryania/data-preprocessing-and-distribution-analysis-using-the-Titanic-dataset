# data-preprocessing-and-distribution-analysis-using-the-Titanic-dataset
# 📌 Interpretation of the Code  

This script demonstrates **data preprocessing and distribution analysis** using the **Titanic dataset** from Kaggle. The main focus is on **handling missing values, normality tests, and transformations of the Age column** to improve its statistical properties. Below is a breakdown of the steps involved:  

---

## 1️⃣ Dataset Loading  

- The script starts by installing and setting up Kaggle in Google Colab.  
- It downloads the **Titanic dataset** from **Kaggle** and loads it into a **Pandas DataFrame**.  
- The first few rows of the dataset are displayed to understand its structure.  

---

## 2️⃣ Exploratory Data Analysis (EDA)  

### 🔹 Histogram of the Dataset  
- A **histogram** is generated to visualize the distribution of numerical features.  
- This helps in understanding the spread and skewness of different variables.  

---

## 3️⃣ Normality Tests on Age Column  

### 📊 Shapiro-Wilk & Kolmogorov-Smirnov Tests  
- The script performs **Shapiro-Wilk** and **Kolmogorov-Smirnov** tests on the **Age** column to check if the data follows a normal distribution.  
- If the **p-value is small (< 0.05)**, it indicates that the data is **not normally distributed**.  

---

## 4️⃣ Skewness and Visualization of Age Distribution  

### 📌 Skewness Calculation  
- **Skewness** measures the asymmetry of data distribution.  
- The script calculates **skewness for the Age column** and visualizes it using a **histogram with a KDE plot**.  

---

## 5️⃣ Data Transformation to Reduce Skewness  

### 🔹 Log Transformation  
- **Logarithmic transformation** (`np.log1p()`) is applied to **Age** to **reduce skewness**.  
- The transformed distribution is visualized using a histogram.  

### 🔹 Box-Cox Transformation  
- The **Box-Cox transformation** is applied as an alternative method for **normalizing the data**.  
- The new skewness value is calculated and visualized.  

---

## 6️⃣ Standardization & Normalization of Age  

- The final step involves **scaling and normalizing** the Age column.  
- The script **compares the standard and normalized distributions** using histograms to observe how the transformations affect data distribution.  

---

## ✅ Key Takeaways  

✔ The **Age column** in the Titanic dataset is **not normally distributed** (as indicated by normality tests).  
✔ Several **transformations** (log and Box-Cox) help in **reducing skewness** and making the data more **symmetric**.  
✔ **Standardization and normalization** further improve the data structure for **machine learning applications**.  

This preprocessing is **crucial for improving model performance** in predictive analytics, as many ML algorithms assume **normally distributed input features**. 🚀
