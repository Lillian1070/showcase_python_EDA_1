# Exploratory Data Analysis (EDA) with Python


### Outline

- Project Overview
- Dataset Used
- Key Findings
- Libraries Used
- Further Directions


## Project Overview
This project demonstrates Exploratory Data Analysis (EDA) techniques using Python. The main focus is to uncover patterns, trends, and insights in the dataset. The key elements of the EDA include:

- Data visualization 
- Identifying patterns and trends
- Feature engineering
- Investigating feature importance
- Checking assumptions

  
You can view the full process in the Jupyter Notebook in this repo [here](https://github.com/Lillian1070/showcase_python_EDA_1/blob/main/kaggle_coffeeBean_EDA.ipynb). 


## Dataset Used
The dataset used in this project was sourced from [Kaggle](https://www.kaggle.com/datasets/fatihb/coffee-quality-data-cqi) and has been cleaned using Python in a separate [data cleaning project](https://github.com/Lillian1070/showcase_python_dataCleaning_1). The cleaned dataset includes 206 coffee samples from the Coffee Quality Institute (CQI), and it is characterized by features such as country of origin, company, altitude, harvest year, processing method, sensory attributes, moisture percentage, defects, color, expiration, certification body, and more. You can access the cleaned dataset [here](https://github.com/Lillian1070/showcase_python_dataCleaning_1/blob/main/cleaned_dataset.csv).


## Key Findings
Throughout the exploratory analysis, the following key insights were uncovered:

- **Model Fit**: Explains 18.7% of the variance in `Total Cup Points` (R-squared = 0.187). Significant predictors include `log_Cat_2_Defects`, `Region_New_America`, and `Region_New_Asia`.
- **Insights**:
  - Higher category 2 defects reduce quality by 0.54 points per unit increase in the log scale.
  - Coffees from the Americas and Asia score 1.40 and 1.11 points lower than African coffees.
  - Quadratic effects of altitude and quakers are weakly significant (p=0.054, p=0.066).


These findings provide a clearer picture of the dataset and its relationships, paving the way for more advanced analysis or predictive modeling.


## Libraries Used
- **Pandas**: Load and manipulate the coffee dataset.
- **NumPy**: Perform numerical operations like log transformations.
- **Matplotlib**: Plot diagnostic charts (e.g., residuals, histograms).
- **Seaborn**: Create statistical visualizations (e.g., correlation heatmaps).
- **SciPy** : Conduct statistical tests (e.g., ANOVA, normality).
- **Statsmodels**: Perform autocorrelation (Breusch-Godfrey, Durbin-Watson), homoscedasticity (Breusch-Pagan), and multicollinearity (VIF) tests.
- **Statsmodels**: Build and diagnose regression models.
- **Scikit-learn**: Implement linear regression.


## Further Directions
- **Clustering Analysis**: Grouping coffee samples based on both sensory and non-sensory features could uncover hidden patterns. This may provide insights into quality segmentation.
- **Non-Linear Models**: Since linear regression assumes a straight-line relationship, experimenting with Random Forests, Gradient Boosting, or Polynomial Regression could capture more complex interactions in the data.
- **Further Feature Engineering**: Creating new features (e.g., binning altitude, interaction terms) might help improve predictive power.


💬 _I’d love to hear your thoughts! If you have any suggestions or questions, feel free to connect with me._


