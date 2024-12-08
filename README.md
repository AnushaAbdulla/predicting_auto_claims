# Allstate Predicting Claim Data

**Project Overview**  
This project was developed as part of the AI Studio Final Presentation for the eCornell Break Through Tech AI program in December 2024. The goal was to predict the total cost of an auto claim to Allstate, leveraging multiple machine learning models to identify the best predictive approach and provide actionable insights for financial planning and claims management.

## Objectives and Goals
1. Predict the total cost of auto claims, including repair, injury, and other expenses.
2. Experiment with various predictive model types to identify the most effective one.
3. Recommend a model with the lowest prediction error and closest match to actual claim costs.

## Methodology
1. **Exploratory Data Analysis**:  
   - Visualized the loss distribution to identify skewness and outliers.  
   - Conducted correlation analyses among continuous features.  
   - Applied Cramér’s V and Chi-Square tests for categorical variables to assess dependencies.  

2. **Data Preparation**:  
   - Addressed multicollinearity by aggregating highly correlated continuous features.  
   - Encoded categorical variables using target encoding and one-hot encoding.  
   - Split data into training (60%), validation (20%), and test (20%) sets.  

3. **Model Development**:  
   - Developed and evaluated models, including LightGBM, XGBoost, Random Forest, and a baseline Mean Model.  
   - Tuned hyperparameters using RandomizedSearchCV and GridSearchCV.  
   - Compared model performances based on metrics like RMSE, R², precision, recall, and F1 score.

4. **Evaluation**:  
   - Selected LightGBM as the best-performing regression model with an RMSE of 1840.78 and R² of 0.585.  
   - Noted challenges in predicting high-loss claims due to class imbalance.

## Results and Key Findings
- **Best Model**: LightGBM, offering a balance between speed, accuracy, and robustness.  
- **Feature Engineering Impact**: Preprocessing steps significantly improved model performance.  
- **Challenges**: High-loss claims (above $40k) were underrepresented, leading to underpredictions in extreme cases.  

## Visualizations
- Loss distribution and outliers.  
- Feature importance rankings.  
- Model comparison metrics, including RMSE and R².  

## Potential Next Steps
1. Gather additional data for higher loss brackets (e.g., claims exceeding $10k).  
2. Explore ensemble methods combining Random Forest and XGBoost.  
3. Investigate methods to address data imbalance, such as oversampling or SMOTE.  

## Individual Contributions
- **Anusha Shakir Abdulla**: Data preprocessing, Random Forest implementation, model evaluation.  
- **Lorena Milian**: EDA, XGBoost Implementation, feature engineering.  
- **Jesse Incoom**: LightGBM implementation, hyperparameter tuning.  
- **Maria Santos Perez**: Insights presentation and business impact analysis.  
- **Livia John**: Data visualization, documentation, and reporting.

## Installation Instructions
1. **Clone the Repository**:  
   ```bash
   git clone https://github.com/your-username/allstate-claims.git
   cd allstate-claims
   ```
2. **Install Dependencies**:  
   Ensure Python 3.x is installed and run:  
   ```bash
   pip install -r requirements.txt
   ```
3. **Prepare the Data**:  
   You must find your own data. The data provided by Allstate is classified and not allowed to be shared.

4. **Train Models**:  
   Run the model scripts for LightGBM, XGBoost, or Random Forest:  
   ```bash
   python train_lightgbm.py  
   python train_xgboost.py  
   python train_rf.py  
   ```

5. **Evaluate Models**:  
   Use evaluation scripts to generate performance metrics:  
   ```bash
   python evaluate.py  
   ```

## Contact
For questions or collaboration, reach out to the team:  

Anusha:
 - [**GitHub**](https://github.com/AnushaAbdulla)
 - [**LinkedIn**](https://www.linkedin.com/in/AnushaAbdulla)

Jesse:
 - [**GitHub**](https://github.com/Jesse-TD)
 - [**LinkedIn**](https://www.linkedin.com/in/jesseincoom/)

Livia:
 - [**GitHub**](https://github.com/liviajohn)
 - [**LinkedIn**](https://www.linkedin.com/in/livia-mary-john/)

Lorena:
 - [**GitHub**](https://github.com/)
 - [**LinkedIn**](https://www.linkedin.com/in/)

Maria:
 - [**GitHub**](https://github.com/)
 - [**LinkedIn**](https://www.linkedin.com/in/)
