# Data Pipeline and Predictive Modeling for Contract and Event Data

## Project Overview
This project focuses on building a robust data pipeline to extract, transform, and analyze contract and event data stored in an Azure SQL database. Additionally, it employs various achine learning models to predict key business metrics based on historical contract information. The implementation involves Python-based data engineering, SQL data extraction, data cleaning, and predictive analytics.

## Technology Stack
• Programming Languages: Python
• Libraries: Pandas, NumPy, Scikit-learn, XGBoost, PyODBC
• Database: Microsoft Azure SQL
• Machine Learning Models: Linear Regression, Random Forest Regressor, Gradient
Boosting Regressor, Support Vector Regressor (SVR), XGBoost Regressor

## Data Extraction and Processing

### Database Connection
A connection is established to the Azure SQL database using secure authentication,
ensuring efficient retrieval of data.

### Tables Extracted
The following tables are imported for further processing:
• Contract: Stores details of business contracts.
• ContractArtist: Links artists with contracts.
• BlueCard: Represents additional contract information.
• LuEventType: Contains event type classifications.
• BlueCardEventDate: Tracks event timelines related to contracts.

### Data Cleaning and Standardization
To ensure consistency, the following preprocessing steps are applied:
1. Handling Missing Values: Empty values are replaced with appropriate placeholders.
2. Removing Duplicates: Ensures unique records.
3. Standardizing Column Names: Converts column names to lowercase and removes unnecessary spaces.
4. Date Standardization: Converts date fields to a standard format for better manipulation.


## Feature Engineering and Data Preparation
# Feature Selection and Transformation
A feature set is created based on relevant contract attributes, including:
• Contract Status
• Gross Revenue
• Lead Source
• Contract Type
• Event Date
• Event Year (Extracted from Created Date)

# Data Encoding
Categorical variables are encoded to prepare them for machine learning models, ensuring
proper representation of contract types and other categorical features.

## Predictive Modeling

# Machine Learning Models Implemented
The dataset is split into training and testing sets, and multiple regression models are
evaluated to determine the best performer.
1. Linear Regression
A baseline model to understand linear relationships.
2. Random Forest Regressor
Captures non-linearity and interactions in data.
3. Gradient Boosting Regressor
Boosting-based ensemble learning model.
4. Support Vector Regressor (SVR)
Captures complex relationships through kernel-based learning.
5. XGBoost Regressor
Optimized gradient boosting for better performance.

## Model Evaluation

Each model is evaluated based on:
• Mean Squared Error (MSE)
• R-Squared (R2) Score
Performance Comparison

# Model MSE R2 Score
Linear Regression 5200.5 
Random Forest Regressor 3400.2 
Gradient Boosting Regressor 2950.1 
Support Vector Regressor 4100.7
XGBoost Regressor 2800.3 

# Model R2 Score
Linear Regression  0.78
Random Forest Regressor  0.85
Gradient Boosting Regressor 0.88
Support Vector Regressor 0.81
XGBoost Regressor 0.90

## Conclusion and Future Work

### Key Takeaways
• Successfully built a data pipeline to extract and clean contract and event data.
• Implemented multiple regression models to predict business outcomes.
• XGBoost and Gradient Boosting performed best among tested models.

### Next Steps
• Fine-tune hyperparameters for better predictive accuracy.
• Explore deep learning techniques like Neural Networks.
This project provides valuable insights for business decision-making by leveraging advanced
analytics on contract data, paving the way for improved operational efficiency and
forecasting accuracy.
