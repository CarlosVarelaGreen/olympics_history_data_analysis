# Data Extraction, Cleaning, Transformation, and Loading of Olympics History Data

## By: Carlos Varela

## Introduction
In this notebook, we will focus on the essential steps of data cleaning and transformation, which are critical to preparing our dataset for analysis and modeling. Data cleaning involves detecting and correcting (or removing) errors and inconsistencies in data to improve its quality. Data transformation, on the other hand, involves transforming raw data into a format suitable for analysis, which often includes restructuring, enriching, and merging data from various sources. Finally, we will write a dedicated pipeline to loading the transformed data into a new PostgreSQL databse. 

## Purpose of Data Cleaning & Transformation

Data cleaning and transformation are foundational processes in the data analysis pipeline. These steps ensure that the data is accurate, complete, and structured appropriately for subsequent analysis and modeling. The main objectives of data cleaning and transforming in this project are:

- **Data Quality Improvement:** Identifying and rectifying errors, inconsistencies, and missing values in the dataset to ensure data integrity. This step is crucial to prevent any inaccurate or misleading results in the analysis.
- **Standardization and Normalization:** Ensuring that the data is in a consistent format. This includes standardizing date formats, units of measure, and categorical values to facilitate accurate comparisons and aggregations.
- **Data Enrichment:** Integrating additional relevant information into the dataset, which might involve merging data from different sources or deriving new features from existing data to enhance the dataset's richness and utility.
- **Handling Missing Values:** Employing strategies such as imputation, interpolation, or removal of missing values to deal with incomplete data, thereby maintaining the dataset's usability.

Overall, we aim to prepare a high-quality, reliable dataset that will serve as a robust foundation for subsequent data analysis using SQL, and Tableau for visualization.

## Getting the data

For this project I will be using 3 datasets
 
**Dataset 1**

 "120 years of Olympic history: athletes and results" collected and wrangled by RGRIFFIN and found on Kaggle: https://www.kaggle.com/datasets/heesoo37/120-years-of-olympic-history-athletes-and-results?resource=download

The dataset contains historical data on the modern Olympic Games from Athens 1896 and until Rio 2016. The author of the dataset reported scrapping this data from www.sports-reference.com in May of 2018.

You can learn more about this dataset and the author here: https://www.kaggle.com/heesoo37

**Dataset 2**

The second dataset gets scraped using pandas read_html() function. The original table may be found here: https://en.wikipedia.org/wiki/Cost_of_the_Olympic_Games

**Dataset 3**
TBD
