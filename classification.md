# Visit Mode Prediction using CatBoost Classification

## Objective

The objective of this project is to predict the **Visit Mode** of a tourist based on historical tourism data.

## Dataset Acquisition

The tourism dataset was retrieved from a MySQL database using SQLAlchemy and PyMySQL.

```python
query = """
SELECT *
FROM tourism;
"""
df = pd.read_sql(query, engine)
```

## Exploratory Data Analysis

### Correlation Analysis

A correlation heatmap was generated to identify relationships among numerical variables.

```python
sns.heatmap(df_num.corr(), annot=True)
```

## Baseline Model

### Feature Selection

Removed columns:

- AttractionCountryId
- AttractionContinentId
- AttractionRegionId
- CountryId
- ContinentId
- RegionId
- TransactionId

### Model

```python
CatBoostClassifier(
    iterations=100,
    learning_rate=0.05
)
```

## Feature Engineering

### 1. Season Feature

| Months | Season |
|---------|---------|
| Dec-Feb | Winter |
| Mar-May | Summer |
| Jun-Aug | Monsoon |
| Sep-Nov | Autumn |

### 2. Attraction Popularity

Calculated visit count for each attraction.

### 3. City Popularity

Calculated visit count for each city.

### 4. Average Attraction Rating

Average rating of each attraction.

### 5. User Trip Count

Total trips made by each user.

## Final Model

```python
CatBoostClassifier(
    iterations=700,
    learning_rate=0.1,
    depth=6,
    loss_function='MultiClass'
)
```

## Results

| Model | Description |
|---------|-------------|
| Model 1 | Numerical Features |
| Model 2 | Categorical Features |
| Model 3 | Feature Engineered Features |

## Conclusion

The feature-engineered CatBoost model achieved the best performance by combining:
- Categorical information
- Seasonal behavior
- Popularity features
- User travel history
- Rating information
## Results Comparison

Three versions of the model were developed and evaluated throughout the project.

| Model | Features Used | Accuracy (%) | Remarks |
|---------|-------------|-------------|-------------|
| Model 1 | Numerical Features Only | 47.3 | Baseline model using only numerical attributes. |
| Model 2 | Categorical Features + CatBoost Native Encoding | 62.8 | Improved performance by utilizing categorical information. |
| Model 3 | Feature Engineered Model | 63.8 | Best performing model after adding domain-specific features. |

### Performance Improvement

The progression of model performance demonstrates the importance of feature engineering and proper handling of categorical variables.

#### Model 1: Baseline Model
- Trained using primarily numerical attributes.
- Established the initial benchmark for classification.
- Limited ability to capture tourism-specific behavior patterns.

#### Model 2: Categorical Feature Model
- Utilized CatBoost's native categorical feature handling.
- Improved class separation by incorporating attraction and location-related information.
- Achieved higher predictive performance than the baseline.

#### Model 3: Feature Engineered Model
Additional features were introduced:

- Season Feature
- Attraction Popularity
- City Popularity
- Average Attraction Rating
- User Trip Count

These features captured hidden behavioral patterns within the tourism dataset and resulted in the highest classification accuracy.

### Best Model

The final feature-engineered CatBoost model achieved the best overall performance because it combined:

- Numerical information
- Categorical information
- Seasonal travel patterns
- Attraction popularity trends
- User travel history
- Rating-based insights

This demonstrates that domain-specific feature engineering can significantly improve multiclass classification performance compared to using raw features alone.