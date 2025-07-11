# Cuisine Classification from Restaurant Dataset

## Objective

This project focuses on developing a machine learning model to classify restaurants based on their primary cuisine type. The classification task uses restaurant attributes such as location, cost, ratings, and availability features to predict the main cuisine served by the restaurant.

## Dataset Description

The dataset includes several attributes:
- Restaurant details: Name, City, Address, Longitude & Latitude.
- Services: Table booking, Online delivery availability.
- Ratings and popularity: Aggregate rating, votes.
- Financials: Average cost for two, currency.
- Cuisine information: Multiple cuisines listed per restaurant.

## Code Overview

The code follows a structured pipeline, starting from data preprocessing to model evaluation and visualization.

### 1. Data Preprocessing
- **Handling Missing Values:** The dataset is cleaned by dropping or imputing missing entries to ensure model reliability.
- **Primary Cuisine Extraction:** For classification purposes, only the first listed cuisine is considered as the primary target label. This simplifies the task from multi-label to single-label classification.
- **Encoding Categorical Variables:** Categorical features such as `City` and `Primary Cuisine` are encoded into numeric form using label encoding, enabling them to be used in machine learning models.
- **Filtering Rare Classes:** Cuisines with only one sample are removed to ensure sufficient representation in both training and testing splits.

### 2. Feature Selection
Features selected for model input include:
- City
- Average Cost for Two
- Aggregate Rating
- Votes
- Availability flags (Table booking, Online delivery)

Numeric features are scaled to improve model performance.

### 3. Model Building
- A **Logistic Regression** model is used as the classifier, providing an interpretable baseline for this multiclass classification task.
- The dataset is split into training and testing sets using stratified sampling to maintain cuisine distribution across splits.
- Model training is performed on the processed feature set.

### 4. Model Evaluation
- The model is evaluated using classification metrics such as **accuracy**, **precision**, **recall**, and **F1-score**.
- A classification report provides a breakdown of the model's performance across different cuisine categories.
- Challenges such as class imbalance and overlapping features are acknowledged in the evaluation.

### 5. Data Visualization
- A **bar chart** visualizes the distribution of the number of cuisines listed per restaurant, providing insight into how many restaurants serve single vs. multiple cuisines.
- Additional visualizations are used to inspect the frequency of top cuisines, aiding in understanding dataset balance before model training.

## Results

The Logistic Regression model demonstrates baseline performance on the cuisine classification task. Results highlight the challenges associated with class imbalance and the simplicity of available features. Filtering rare classes and focusing on frequent cuisines helps improve stability but leaves room for further optimization.
