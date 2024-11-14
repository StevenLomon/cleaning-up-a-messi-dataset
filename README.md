# Cleaning up a Messi Dataset ⚽

## Project Overview
This project tackles the notorious FIFA 21 dataset, known for its “messy” qualities—perfect for a comprehensive data cleaning and quality assurance workflow. The goal is to clean and validate the data to prepare it for analysis, and then load the cleaned dataset into a relational database. "Tackles" and "goal", the puns are everywhere here. This project simulates real-world data handling and showcases the data cleaning, quality assurance, and database handling skills essential in data analytics.

## Dataset
* Dataset: FIFA 21 Messy Raw Dataset for Cleaning & Exploring
* Source: Kaggle
* Description: This dataset contains detailed attributes for over 18,000 players in FIFA 21, with various issues typical of raw data, including missing values, duplicates, and inconsistent formats. The dataset provides a realistic challenge for data cleaning and quality assurance practices.

## Objectives
* Data Cleaning: Identify and resolve common data quality issues within the FIFA 21 dataset, such as missing values, duplicate records, outliers, and inconsistencies.
* Data Quality Assurance: Implement validation checks to ensure the cleaned data meets consistency and accuracy standards.
* Database Loading: Store the cleaned dataset in a relational database (SQLite or PostgreSQL), demonstrating the process of loading data into a structured storage system.
* Automation: Create a Python script to automate the data loading process into the database, simulating a simplified ETL workflow.

## Project Workflow
1. Data Extraction:
* Download the FIFA 21 dataset from Kaggle using kagglehub.
* Load the data into a Jupyter notebook for exploration and cleaning.

2. Data Cleaning:
* Exploration: Conduct an initial exploration to understand the structure of the FIFA dataset, check for missing values, identify outliers, and review inconsistent formats (e.g., currency formats, position labels).
* Handling Missing Values: Apply appropriate imputation techniques or drop columns/rows based on data relevance.
* Outlier Detection: Identify and manage outliers, particularly in numerical columns like player value or rating.
* Data Standardization: Ensure uniformity in categorical data (e.g., player positions) and date formats.
* Documentation: Document each data cleaning step directly in the Jupyter notebook for reproducibility.

3. Data Quality Assurance:
* Run validation checks to confirm data consistency, including checks for duplicate records, valid data ranges (e.g., age and player rating), and data type accuracy.
* Summarize data quality improvements, creating a concise report of the steps taken to clean the dataset.

4. Database Setup and Loading:
* Set up a local PostgreSQL database to store the cleaned dataset.
* Write a Python script that automates the loading of cleaned data into the database, ensuring efficient data handling and storage.
* Execute SQL queries to validate the data integrity within the database (e.g., confirming unique player IDs, checking for null values post-cleaning).

Optional Data Enhancement:

Introduce new columns with randomly generated data to simulate additional imperfections (e.g., adding “injury history” with intentional nulls), then clean and validate this new data.

## Technologies and Tools
* Python: Data cleaning and transformation (Pandas)
* SQL: Data storage and validation queries within PostgreSQL
* Jupyter Notebook: Data exploration, cleaning, and documentation
* GitHub Actions (optional): For continuous integration, automated linting, and testing

## Future Enhancements
This project could be expanded by:
* Incorporating automated data validation tests in Python to check data quality.
* Deploying the cleaned data in a cloud database for scalability.
* Creating visualizations to analyze player attributes post-cleaning and demonstrate insights.

## Instructions for Running the Project
1. Clone the Repository:
```
git clone <repository_url>
cd Cleaning-up-a-Messi-dataset
```

2. Install Required Libraries:
```
pip install -r requirements.txt
```

3. Download the Dataset (using kagglehub):
```
kaggle datasets download -d yagunnersya/fifa-21-messy-raw-dataset-for-cleaning-exploring
```

4. Launch Jupyter Lab:
```
jupyter lab
```

5. Run the Jupyter Notebook for data cleaning steps and documentation.

6. Run Database Loading Script:
* After cleaning, execute the database loading script to store data in SQLite or PostgreSQL.