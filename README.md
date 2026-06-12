# COVID-19 Vaccination Big Data Analysis

## Project Overview

This project analyzes COVID-19 vaccination trends in California using Big Data technologies. The main goal of the project is to process, clean, analyze, and visualize a large public health dataset to understand how vaccination activity changed over time across different California counties.

The project was completed as part of the Big Data Analytics course at Kristianstad University.

## Authors

* Md Abu Taher
* Anitta Antony

## Dataset

The dataset used in this project contains COVID-19 vaccination data for California counties. It includes vaccination records from 2020 to 2025.

Dataset information:

* Rows: 54,942,524
* Columns: 25
* Counties: 58
* Source: Data.gov
* Data type: County-level and time-series vaccination data

The dataset includes information such as:

* Total vaccine doses
* Cumulative vaccine doses
* Pfizer, Moderna, and Johnson & Johnson doses
* Partially vaccinated people
* Fully vaccinated people
* Booster doses
* County population
* Reporting dates

## Technologies Used

The following tools and technologies were used in this project:

* Apache Hadoop / HDFS
* Apache Spark
* PySpark
* Python
* Jupyter Notebook
* Pandas
* Matplotlib

## Project Workflow

The project follows a Big Data analysis pipeline:

1. Data loading
2. Data preprocessing
3. Data cleaning
4. Data transformation
5. Descriptive analysis
6. Trend analysis
7. Correlation analysis
8. Anomaly observation
9. Data visualization
10. Output generation

## Data Preprocessing

Several preprocessing steps were applied before analysis:

* Removed leading and trailing spaces from county names
* Converted date values into proper date format
* Removed rows with missing important fields such as county or date
* Handled missing values in booster-related columns
* Aggregated vaccination data by county and date
* Calculated vaccination coverage percentages using county population data

## Analysis Performed

The project includes the following types of analysis:

### Descriptive Analysis

Descriptive analysis was used to compare vaccination activity across counties. Counties with larger populations, such as Los Angeles, San Diego, Orange, and Santa Clara, showed higher total vaccine dose counts.

### Trend Analysis

Trend analysis was used to study vaccination activity over time. The results show that vaccination activity increased strongly during 2021 and early 2022, then gradually decreased in later years.

### Correlation Analysis

Correlation analysis was used to examine the relationship between county population and vaccination coverage. The results showed that population size alone does not fully explain vaccination coverage differences between counties.

### Anomaly Observation

Anomaly observation was used to identify counties with unusually low or unusually high vaccination coverage. Some rural counties showed lower vaccination coverage, while some counties showed unusually high values that may need further data validation.

## Visualizations

The project includes visualizations such as:

* Bar charts for total vaccine doses by county
* Line charts for daily vaccination trends
* Line charts for cumulative vaccination trends
* Scatter plots for population and vaccination coverage
* Bar charts for anomalous vaccination coverage

## Output Files

The project generates processed output files such as:

* `coverage_per_county.csv`
* `daily_trend.csv`

These files contain cleaned and aggregated results that can be used for further analysis or visualization.

## Key Findings

The main findings of the project are:

* Vaccination coverage varied across California counties.
* Urban counties generally showed higher vaccination coverage.
* Vaccination activity was highest during 2021 and early 2022.
* Some counties showed unusually low or high vaccination coverage.
* Big Data technologies such as Spark and Hadoop are useful for processing large public health datasets.

## How to Run the Project

1. Install the required tools:

   * Python
   * Apache Spark
   * PySpark
   * Jupyter Notebook
   * Pandas
   * Matplotlib

2. Open the notebook:

```bash
jupyter notebook coviddata_california.ipynb
```

3. Update the dataset path in the notebook according to your local computer.

4. Run the notebook cells step by step.

5. Check the generated CSV files and visualizations.

## Project Files

```text
coviddata_california.ipynb
BigData Project.pdf
COVID_Vaccination_BigData_Presentation.pptx
README.md
```

## Future Work

Possible future improvements include:

* Applying machine learning models to predict future vaccination trends
* Adding demographic and socioeconomic datasets
* Performing deeper time-series analysis
* Creating interactive dashboards using Power BI or Tableau
* Running the project on a fully distributed Spark cluster

## Conclusion

This project demonstrates how Big Data technologies can be used to process and analyze large-scale public health data. By using Apache Spark, PySpark, and Hadoop, the project successfully handled a large COVID-19 vaccination dataset and extracted useful insights about vaccination trends, county-level differences, and possible data anomalies.
