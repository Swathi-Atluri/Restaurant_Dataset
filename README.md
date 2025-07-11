# Restaurant_Dataset# 🍽️ Restaurant Data Analysis & Machine Learning Suite

A comprehensive suite of four projects focused on understanding, modeling, and leveraging restaurant data to solve real-world problems — from predicting ratings to offering personalized restaurant recommendations.

---

## 📂 Project Overview

| Task No. | Task Name                     | Problem Type                |
|----------|-------------------------------|-----------------------------|
| 1        | Cuisine Classification        | Multi-class Classification  |
| 2        | Location & Cuisine Clustering | Unsupervised Learning       |
| 3        | Rating Prediction             | Regression                  |
| 4        | Restaurant Recommendation     | Rule-based Filtering        |

---

## 🧠 1. Cuisine Classification

### 🎯 Objective
Classify the **primary cuisine** of a restaurant based on features like city, cost, rating, and service availability.

### ⚙️ Approach
- Only the first listed cuisine is considered the **target label**.
- Rare cuisines are removed to improve model generalization.
- Categorical features (e.g., City, Cuisine) are label-encoded.
- Numeric features are scaled.

### 🤖 Model Used
- **Logistic Regression**

### 📌 Key Features Used
- City  
- Average Cost for Two  
- Aggregate Rating  
- Votes  
- Table Booking  
- Online Delivery  

### 📈 Results
- Established a **baseline accuracy** for cuisine prediction.
- Highlighted challenges such as **class imbalance** and overlapping feature influence.

---

## 🗺️ 2. Location & Cuisine-Based Clustering

### 🎯 Objective
Uncover spatial and cuisine trends by clustering restaurants using unsupervised techniques.

### ⚙️ Approach
- Geographic clustering based on **City** and **Locality** (not just coordinates).
- Cuisine clustering based on the **first-listed cuisine**.
- Aggregated and visualized average ratings by area.

### 🤖 Model Used
- No ML model; **grouping logic + visualization**

### 📌 Key Features Used
- City  
- Locality  
- Latitude & Longitude  
- Cuisine  
- Aggregate Rating  

### 📈 Results
- High-rated localities: *SM Megamall*, *Century City Mall*
- Common cuisines: *Japanese*, *Filipino*
- Hotspot cities: *Makati City*, *Pasay City*

---

## 📊 3. Rating Prediction

### 🎯 Objective
Predict a restaurant’s **aggregate rating** using regression algorithms.

### ⚙️ Approach
- Cleaned and preprocessed numeric/categorical columns.
- Trained and compared two regression models.
- Evaluated with metrics like MSE and R² Score.

### 🤖 Models Used
- **Linear Regression**
- **Decision Tree Regressor**

### 📌 Key Features Used
- Average Cost for Two  
- Votes  
- Table Booking  
- Online Delivery  
- City  

### 📈 Results

| Model             | MSE   | R² Score |
|-------------------|-------|----------|
| Linear Regression | 1.34  | 0.44     |
| Decision Tree     | 0.06  | 0.97     |

- **Decision Tree** captured non-linear patterns well and outperformed Linear Regression.

---

## 🌟 4. Restaurant Recommendation System

### 🎯 Objective
Recommend restaurants to users based on preferences like **cuisine**, **city**, **locality**, and **budget**.

### ⚙️ Approach
- Filtered data based on user-input criteria.
- Case-insensitive matching and `'Any'` as wildcard supported.
- Output displayed in a clear tabular format.

### 🤖 Model Used
- No ML model; **rule-based filtering**

### 📌 Key Features Used
- City  
- Locality  
- Cuisine  
- Price Range  
- Aggregate Rating  

### 📈 Results
- Efficient and **user-friendly recommendation system**.
- Supports flexible queries while maintaining clean output display.

#### 🧪 Sample Output

| Restaurant Name  | Locality         | City         | Cuisines  | Price for 2  | Aggregate rating |
|------------------|------------------|--------------|-----------|--------------|------------------|
| Izakaya Kikufuji | Legaspi Village  | Makati City  | Japanese  | PHP 1200     | 4.5              |

---

## 📊 Visualizations Used

- Cuisine frequency bar plots
- Area-wise average rating bar charts
- Geographic scatter plots
- Cuisine distribution count plots

---

## 🧰 Requirements

- Python 3.x
- Libraries:
  - `pandas`, `numpy`
  - `matplotlib`, `seaborn`
  - `scikit-learn` (for classification & regression)

---


