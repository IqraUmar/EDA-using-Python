# EDA-using-Python
A comprehensive exploratory data analysis (EDA) of the Titanic dataset, focusing on data cleaning, feature engineering, and visualization to understand factors influencing survival rates.

## Project Overview
This project performs an in-depth analysis of the Titanic passenger dataset, examining:
- Missing value imputation
- Feature engineering by merging related columns
- Outlier detection
- Statistical analysis
- Visualization of key relationships

## Dataset Information
The dataset contains information about 891 passengers aboard the RMS Titanic, including:
- Demographic information (age, gender)
- Travel details (class, fare)
- Family relationships (siblings/spouses, parents/children)
- Survival outcomes

## Features
After processing, the dataset includes these key features:
- `survival_status`: Merged from 'alive' and 'survived' columns (1 = survived, 0 = deceased)
- `passenger_class`: Merged from 'pclass' and 'class' columns (1 = First, 2 = Second, 3 = Third)
- `age`: Passenger age (missing values filled with mean)
- `sex`: Passenger gender
- `sibsp`: Number of siblings/spouses aboard
- `parch`: Number of parents/children aboard
- `fare`: Passenger fare
- `embark_town`: Port of embarkation
- `who`: Classification of passengers (man, woman, child)

## Data Cleaning
Key data cleaning steps performed:
1. Handled missing values:
   - Age: Filled missing values with mean age (19.8% missing)
   - Removed columns with high missing values: 'embarked', 'deck', 'adult_male'
2. Merged redundant columns:
   - Combined 'alive' and 'survived' into 'survival_status'
   - Combined 'pclass' and 'class' into 'passenger_class'
3. Outlier detection using IQR method for all numerical features

## Exploratory Data Analysis
Key analysis performed:
- Basic statistics for all numerical features
- Unique value counts for categorical features
- Correlation analysis between numerical features
- Distribution analysis of all features

## Visualizations
The project includes several insightful visualizations:

### Categorical Variables
- Passenger gender distribution
- Embarkation town distribution
- Passenger classification (man/woman/child)

### Numerical Variables
- Age distribution (with KDE)
- Sibling/spouse count distribution
- Parent/child count distribution
- Fare distribution
- Survival status distribution
- Passenger class distribution

### Correlation Analysis
- Heatmap showing relationships between numerical features

## Findings
Key insights from the analysis:
1. **Age Distribution**: Most passengers were between 20-40 years old
2. **Survival Rate**: Approximately 38% of passengers survived
3. **Gender Impact**: Significant difference in survival rates between male and female passengers
4. **Class Impact**: Higher survival rates in first class passengers
5. **Fare Correlation**: Positive correlation between fare and survival
