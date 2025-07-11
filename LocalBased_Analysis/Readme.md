# Location-Based Restaurant Analysis

## Objective
The goal of this project is to perform a comprehensive **geographical analysis** and **cuisine-based clustering** of restaurants using an unsupervised learning approach. The analysis leverages clustering algorithms and data visualization techniques to uncover patterns in restaurant locations, cuisines, and their average ratings.

---

## Dataset
The dataset contains detailed information about restaurants, including:
- Restaurant name
- City, Locality, and Address
- Geographic coordinates (Latitude and Longitude)
- Cuisines offered
- Average cost for two
- Aggregate ratings and votes
- Delivery and booking availability

---

## Steps and Analysis

### 1. Geographic Clustering
- **Objective:** Group restaurants based on their geographical locations.
- **Method:** Restaurants are grouped using their provided **city** and **locality** information. This is more meaningful than clustering based solely on coordinates, as city and locality names offer real-world context.
- **Visualization:** 
  - A scatter plot of restaurant locations colored by **city** was created using Matplotlib.
  - An additional bar chart shows the **average restaurant rating by area (Locality)**, allowing identification of top-rated areas.

### 2. Cuisine-Based Clustering
- **Objective:** Cluster restaurants based on the type of cuisines they serve.
- **Method:** 
  - The primary cuisine (first listed) was extracted from the multiple cuisines column.
  - Restaurants were grouped based on this dominant cuisine type.
- **Visualization:**
  - A count plot shows the distribution of restaurants across different cuisines.
  - This helps to understand which cuisines are most prevalent in the dataset.

### 3. Area-Wise Rating Analysis
- **Objective:** Identify which areas (localities) have higher average-rated restaurants.
- **Method:**
  - The dataset was grouped by **Locality**, and the average of the aggregate ratings was computed.
- **Visualization:**
  - A bar plot displays the **average restaurant rating per locality**.
  - This allows identification of high-performing areas in terms of customer ratings.

---

## Algorithms and Techniques Used
- **Clustering:**
  - For geographic clustering, grouping was done based on **City** and **Locality** columns for more meaningful analysis.
  - For cuisine clustering, dominant cuisine extraction was used to cluster restaurants.
  
- **Visualization Tools:**
  - All visualizations were created using **Matplotlib** and **Seaborn** to maintain simplicity and compatibility within the Kaggle environment.

---

## Key Findings
- Certain localities such as *SM Megamall* and *Century City Mall* have higher average restaurant ratings.
- **Japanese** and **Filipino** cuisines are among the most frequently served cuisines in the dataset.
- Cities like *Makati City* and *Pasay City* have a significant concentration of top-rated restaurants.

---

## Requirements
- Python 3
- Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn (for optional clustering)

---


