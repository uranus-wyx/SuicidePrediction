# Suicide Prediction: A Socioeconomic Analysis

This **Suicide Prediction System** leverages data science to analyze various environmental and socioeconomic factors, including GDP, weather conditions, happiness index, suicide rates, and temperature of different countries. By examining these factors, the system aims to identify trends and patterns in suicide rates and develop predictive models to assess suicide risks. The project utilizes machine learning techniques to provide insights that can help organizations and mental health professionals take proactive measures to prevent suicides and improve public health outcomes.

## Section 1 - Suicide Prediction Website

Check out our live website for the Suicide Prediction System [here](https://atharva1000ak.wixsite.com/suicide-prediction).

## Section 2 - Data Collection, Preparation, Cleaning & Visualizations

### Data Collection
This project uses data from multiple sources, including:
- **GDP**: Economic data of various countries.
- **Weather**: Climate data such as temperature and weather conditions.
- **Happiness Index**: Global happiness scores.
- **Suicide Rates**: Historical data on suicide rates.
- **Population**: Population statistics for each country.

### Data Preparation
- Data was collected using web scraping and APIs to ensure authenticity and reliability.
- The collected data was cleaned by:
  - **Handling Missing Values**: Imputed or removed missing data points as appropriate.
  - **Removing Outliers**: Identified and removed anomalies to ensure data integrity.
  - **Ensuring Consistency**: Standardized formats across different datasets.
- Multiple CSV files were merged to create a comprehensive dataset for analysis.

### Data Visualizations
- Various data visualizations, including bar charts, scatter plots, and line graphs, are used to represent relationships between factors and suicide rates.
- Each visualization provides insights into trends and correlations that influence suicide rates, helping to visualize complex data in an understandable manner.

### Data Sample
- Below is a snippet of what the dataset looks like before and after cleaning:
  
  **Before Cleaning:**
  
- GDP Data
  | Country  | 1999     | 2000 | 2001 | 2002 |
  |----------|---------|----------------|--------------|-------------|
  | Country A| 162.64  | 160.88           | 161.32          | 164.12          |

- Weather Data
    | Country  | 1999     | 2000 | 2001 | 2002 |
  |----------|---------|----------------|--------------|-------------|
  | Country A| 13  | 15          | 14          | 14.5          |
- Happiness Index Data
    | Country  |  Overall Rank  | Life Evaluation  |
  |----------|---------|----------------|
  | Country A| 4  | 1.7666| 
- Suicide Rates Data
    | Country  | male_suicide_rate  | female_suicide_rate | both_suicide_rate|
  |----------|---------|----------------|--------------|
  | Country A| 4.4  | 2.4    | 3.2       |
  
- Population Data

    | Country  | 1988 | 1989 | 1990|
  |----------|------------|------------|--------------|
  | Country A| 720859132  |720907282   | 720889272    |
  
  **After Cleaning:**
  | Country  | GDP     | Happiness Index | male suicide Rate |female suicide Rate |both suicide Rate |population | Temperature | Year|
  |----------|---------|----------------|--------------|-------------|-------------|-------------|-------------|-------------|
  | Country A| 165  | 1.766 | 4.4  | 2.4 |3.2  | 720859132 | 15 | 1988
  | Country A| 163  | 1.643 |4.5   | 2.6 |3.05 | 720907282 | 14.7 | 1989

---

### Insights from Visualizations
- **Bar Charts**: Show the suicide rate across the countries.
- **Scatter Plots**: Illustrate correlations between population and suicide rates.
- **Heatmap**: Display the correlation between these factors.

## Section 3 - Model Implementation  

### Models Implemented
* XGBOOST
* RANDOM FOREST MODEL
* KNN
* LIGHT GBM
* SUPPORT VECTOR MACHINE (SVM)
  
### Conclusion
This project explores the application of machine learning techniques to predict suicide risk levels (low, medium, and high) using socioeconomic and demographic data. By leveraging models such as Random Forest, K-Nearest Neighbors (KNN), LightGBM, Support Vector Machines (SVM), and XGBoost, we successfully demonstrated how advanced algorithms can classify risk levels with high accuracy. KNN and Random Forest emerged as the top-performing models, achieving 97% and 93.9% accuracy, respectively, with strong precision and recall metrics.

Key socioeconomic factors, including GDP, Population Size, and Happiness Index, were identified as critical predictors of suicide risk. These findings underscore the potential of integrating data science into public health initiatives to provide actionable insights for suicide prevention. While the models performed well overall, medium-risk classifications presented challenges, highlighting opportunities for further optimization through feature engineering and advanced ensemble techniques.

This project not only showcases the predictive power of machine learning but also emphasizes the importance of ethical considerations and interpretability in sensitive applications like suicide prevention. Future work will focus on refining model performance, incorporating additional data sources, and exploring real-time prediction capabilities to enhance the practical utility of this research.
