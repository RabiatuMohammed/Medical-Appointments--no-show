## Predictive Analysis for No-Show-Medical-Appointments

## Project Overview:
This project examines a dataset of medical appointments to anticipate no-shows and identify variables that contribute to this problem. The insights collected are intended to aid medical institutions in boosting patient appointment attendance.

## Data loading
The dataset was put into a Pandas DataFrame for processing. Initial data investigation identified critical columns such as'specialty', 'appointment_time', and 'no_show', as well as multiple occurrences of NaN values that required a complete data cleaning procedure.

## Data cleaning and preprocessing
Detailed procedures were made to sanitise the data.
- Categorical data with missing values, such as'specialty' and 'city', were marked as 'Unknown'.
- 'no_show_reason' columns with missing values were marked as 'Not Applicable'.
- Date columns with erroneous entries were fixed, and rows with missing critical dates were eliminated.
- Duplicates, detected by 'icd' codes, were removed to ensure data uniqueness.
- The 'rain_intensity' column was converted to a numerical type and classified as 'Low', 'Medium', and 'High' based on quantiles.

## Exploratory Data Analysis (EDA).
Through EDA, we discovered patterns and correlations:
- Bar graphs and histograms depicted the distribution of no-show rates across appointment shifts and other categorical factors.
- Correlation heatmaps measured the strength of relationships between numerical variables.
- Scatter plots investigated the association between patient age and no-show probability.

  ## Statistical Analysis.
To establish if age was a significant influence, a T-test was performed on no-show rates for younger and older patients. Correlation coefficients measured the association between age and no-show rates.

## Key insights
Visualisations and statistical testing revealed that appointment time and external factors such as weather might impact no-show rates.

## Conclusion:
The EDA revealed useful insights, indicating that a predictive model may be constructed to forecast no-shows, thereby assisting medical facilities in improving patient attendance policies.
