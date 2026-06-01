# Tourism Experience Analytics: Classification, Prediction & Recommendation System

## 📌 Project Overview

### Project Title

**Tourism Experience Analytics: Classification, Prediction and Recommendation System**

### Domain

Tourism Analytics

### Skills Demonstrated

* Data Cleaning & Preprocessing
* Exploratory Data Analysis (EDA)
* Data Visualization
* SQL
* Machine Learning

  * Regression
  * Classification
  * Recommendation Systems
* Streamlit Deployment

---

# 🎯 Problem Statement

Tourism agencies and travel platforms aim to improve customer experience by leveraging user behavior, travel patterns, attraction characteristics, and demographic data.

This project focuses on:

1. Predicting attraction ratings.
2. Predicting user visit modes.
3. Recommending attractions based on user preferences.
4. Generating tourism insights for businesses.

---

# 🚀 Business Use Cases

## Personalized Recommendations

Recommend attractions based on:

* Historical visits
* User preferences
* Similar travelers

## Tourism Analytics

Analyze:

* Popular destinations
* Travel trends
* Regional tourism patterns

## Customer Segmentation

Classify tourists based on:

* Travel habits
* Demographics
* Visit behavior

## Customer Retention

Improve engagement through personalized recommendations.

---

# 🎯 Project Objectives

## 1️⃣ Regression: Attraction Rating Prediction

### Goal

Predict the rating a tourist may assign to an attraction.

### Input Features

* Continent
* Region
* Country
* City
* Visit Year
* Visit Month
* Visit Mode
* Attraction Type
* Attraction Location

### Target Variable

Rating (1–5)

### Evaluation Metrics

* MAE
* MSE
* RMSE
* R² Score

---

## 2️⃣ Classification: Visit Mode Prediction

### Goal

Predict visitor type:

* Business
* Family
* Couples
* Friends
* Solo

### Input Features

* User demographics
* Attraction characteristics
* Historical visits
* Temporal information

### Target Variable

Visit Mode

### Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1 Score

---

## 3️⃣ Recommendation System

### Goal

Recommend attractions likely to interest users.

### Recommendation Approaches

#### Collaborative Filtering

Recommendations based on similar users.

#### Content-Based Filtering

Recommendations based on attraction features.

#### Hybrid Recommendation

Combination of collaborative and content-based approaches.

### Evaluation Metrics

* MAP
* Precision@K
* Recall@K
* RMSE

---

# 📂 Dataset Description

## Transaction Data

| Column        | Description            |
| ------------- | ---------------------- |
| TransactionId | Transaction Identifier |
| UserId        | User Identifier        |
| VisitYear     | Visit Year             |
| VisitMonth    | Visit Month            |
| VisitMode     | Travel Mode            |
| AttractionId  | Attraction Identifier  |
| Rating        | User Rating            |

---

## User Data

| Column      | Description     |
| ----------- | --------------- |
| UserId      | User Identifier |
| ContinentId | User Continent  |
| RegionId    | User Region     |
| CountryId   | User Country    |
| CityId      | User City       |

---

## Attraction Data

| Column            | Description           |
| ----------------- | --------------------- |
| AttractionId      | Attraction Identifier |
| Attraction        | Attraction Name       |
| AttractionTypeId  | Attraction Category   |
| AttractionCityId  | Attraction City       |
| AttractionAddress | Attraction Address    |

---

# 🛠 Project Workflow

## Phase 1: Data Preparation

### Tasks

* Handle missing values
* Remove duplicates
* Standardize categories
* Handle outliers
* Merge datasets

### Deliverables

* Cleaned Dataset
* Data Cleaning Report

---

## Phase 2: Feature Engineering

### Tasks

* Label Encoding
* One-Hot Encoding
* User Profile Creation
* Attraction Popularity Metrics
* Aggregated Features

### Deliverables

* Model Ready Dataset

---

## Phase 3: Exploratory Data Analysis

### Analysis Areas

#### User Analysis

* Users by continent
* Users by country
* Users by region

#### Attraction Analysis

* Most visited attractions
* Highest rated attractions
* Popular attraction types

#### Visit Mode Analysis

* Seasonal travel patterns
* Family vs Business travelers

#### Rating Analysis

* Rating distributions
* Regional rating trends

### Deliverables

* EDA Report
* Business Insights

---

# 🤖 Machine Learning Models

## Regression Models

* Linear Regression
* Random Forest Regressor
* XGBoost Regressor

### Best Model Selection

Based on:

* RMSE
* MAE
* R² Score

---

## Classification Models

* Logistic Regression
* Random Forest Classifier
* XGBoost Classifier
* LightGBM Classifier

### Best Model Selection

Based on:

* Accuracy
* Precision
* Recall
* F1 Score

---

## Recommendation Models

### Collaborative Filtering

User-item interaction matrix.

### Content-Based Filtering

Attraction similarity based on:

* Location
* Type
* Popularity

### Hybrid Recommendation

Combined recommendation strategy.

---

# 📊 SQL Analysis

## Queries to Develop

* Top Attractions
* Top Countries
* Most Popular Visit Modes
* Tourism Trends by Month
* Tourism Trends by Region
* User Segmentation Analysis

---

# 📈 Visualizations

## User Insights

* Users by Continent
* Users by Country
* Users by Region

## Attraction Insights

* Top Rated Attractions
* Most Visited Attractions
* Attraction Type Distribution

## Tourism Trends

* Monthly Trends
* Seasonal Trends
* Travel Mode Analysis

---

# 🌐 Streamlit Application

## Dashboard Module

Features:

* KPIs
* Charts
* Filters
* Tourism Insights

---

## Visit Mode Prediction

### Input

* Country
* Region
* Attraction Type

### Output

Predicted Visit Mode

---

## Rating Prediction

### Input

* User Details
* Attraction Details

### Output

Predicted Rating

---

## Recommendation Engine

### Input

* User Preferences
* Attraction Type

### Output

Top Recommended Attractions

---

# 📁 Repository Structure

```bash
Tourism-Analytics/
│
├── data/
├── notebooks/
├── sql/
├── models/
├── src/
│   ├── preprocessing/
│   ├── eda/
│   ├── regression/
│   ├── classification/
│   └── recommendation/
│
├── streamlit_app/
├── reports/
├── screenshots/
│
├── requirements.txt
├── README.md
└── developer_guide.md
```

# 📅 Project Timeline

## Week 1

* Dataset Understanding
* Data Cleaning

## Week 2

* Feature Engineering
* SQL Analysis

## Week 3

* Exploratory Data Analysis

## Week 4

* Regression Model Development

## Week 5

* Classification Model Development

## Week 6

* Recommendation System Development

## Week 7

* Streamlit Application

## Week 8

* Deployment & Documentation

---

# ✅ Expected Outcomes

* Tourism Trend Analysis
* Attraction Rating Prediction
* Visit Mode Prediction
* Personalized Attraction Recommendations
* Interactive Streamlit Dashboard
* Actionable Business Insights

---

# 👨‍💻 Author

**Nitya Zijoo**

B.Tech CSIT Student | Data Analytics & Machine Learning Enthusiast
