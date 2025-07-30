# Cholera Outbreak Predictor 🦠📊

This AI-enabled project was created during my 3MTT learning journey. It attempts to predict potential cholera outbreaks in Nigeria by leveraging machine learning with historical weekly data.

## Why This Project?

Cholera remains endemic in Nigeria. During my learning journey, I created this project to understand the role of AI in bolstering public health initiatives. I developed a classifier based on data pulled from the Nigerian Centre for Disease Control (NCDC) Weekly Epidemiological Reports (2021–2025) that marks weeks as **“Outbreak”** or **“No Outbreak”**.

## Project Structure

- `Cholera_outbreak_predictor.ipynb`: Main notebook containing the complete workflow for data analysis, including data cleaning, exploratory analysis, model creation, and evaluation.
- `Cholera_Report_Cleaned_new.csv`: Preprocessed dataset used for model building and analysis, compiled from NCDC Weekly Epidemiological Reports.
- `README.md`: Project overview, objectives, methodologies, and workflow.
- `.pkl` files: Trained logistic regression model(s) for prediction.

## What the Project Covers

- **Data Collection**: Weekly cholera reports from NCDC including suspected and confirmed cases, deaths, and case fatality rates.
- **Data Cleaning & Exploration**: Checked for duplicates and missing values; explored patterns using data visualization.
- **Feature Engineering**: Created new features from existing relevant data to improve model performance.
- **Model Training**: Tested multiple classification models; chose Logistic Regression for its reasonable accuracy.
- **Model Evaluation**:
  - *No Outbreak (Class 0)*: Recall = 1.00, Precision = 0.92
  - *Outbreak (Class 1)*: Precision = 1.00, Recall = 0.50
  - Threshold adjusted to improve outbreak detection.

## Insights

The model performs well in detecting weeks with no outbreaks. With threshold tuning, its ability to detect potential outbreaks improves significantly.

## Tools & Technologies

- **Platform**: Google Colab  
- **Languages**: Python  
- **Libraries**: Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn  

## Data Source

[NCDC Weekly Epidemiological Reports](https://ncdc.gov.ng/reports) were used as the primary data source for this project.
