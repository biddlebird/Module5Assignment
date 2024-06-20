# Module5Assignment
UCB Data Analytics Bootcamp Module 5 Assignment - Mouse Study with different Regimens to minimize tumors
Certainly! Below is the README.md file summarizing the Mouse Coding Project:

---

# Mouse Coding Project

This project involves analyzing a dataset of mouse data obtained from a study on various drug regimens aimed at reducing tumor volume. The dataset is comprised of two main files: `Mouse_metadata.csv` and `Study_results.csv`.

## Dependencies and Setup
The project uses the following Python libraries:
- Matplotlib (`matplotlib.pyplot`)
- Pandas (`pandas`)
- Scipy (`scipy.stats`)
- NumPy (`numpy`)

Ensure these libraries are installed in your Python environment to run the code successfully.

## Dataset
- **Mouse_metadata.csv**: Contains metadata about each mouse including its ID, drug regimen, sex, and weight.
- **Study_results.csv**: Provides the results of the study, including timepoints and tumor volume for each mouse.

## Code Overview

### Data Integration
- The two CSV files (`Mouse_metadata.csv` and `Study_results.csv`) are merged into a single DataFrame (`merged_data`) using the `pd.merge()` function.

### Data Cleaning
- Duplicate entries based on `Mouse ID` and `Timepoint` are identified and removed to ensure data integrity.
- The cleaned DataFrame (`cleaned_data`) is created by dropping duplicate mouse entries.

### Summary Statistics
- Summary statistics are calculated for each drug regimen, including mean, median, variance, standard deviation, and SEM of the tumor volume using Pandas' `groupby()` and aggregation functions.

### Data Visualization
- **Bar Plots**: Display the total number of observations (Mouse ID/Timepoints) for each drug regimen using both Pandas and Matplotlib.
- **Pie Charts**: Show the distribution of female versus male mice using Pandas and Matplotlib.
- **Box Plot**: Illustrates the distribution of tumor volume for each treatment regimen, highlighting potential outliers.
- **Line Plot**: Depicts the tumor volume progression over time for a single mouse treated with Capomulin.
- **Scatter Plot**: Represents the relationship between mouse weight and the average observed tumor volume for the Capomulin regimen, along with a linear regression analysis.

### Statistical Analysis
- **Outlier Detection**: Uses the Interquartile Range (IQR) method to identify potential outliers in tumor volume across selected treatment regimens.
- **Correlation and Regression**: Calculates the correlation coefficient and performs linear regression to analyze the relationship between mouse weight and tumor volume.

## Conclusion
The Mouse Coding Project showcases the process of data cleaning, exploratory data analysis, statistical analysis, and visualization using Python libraries. It provides insights into the effectiveness of various drug regimens in reducing tumor volume and explores correlations between biological variables.

This project serves as a practical example of applying data science techniques to biomedical research, emphasizing the importance of data integrity, statistical rigor, and insightful visualization in drawing meaningful conclusions.
