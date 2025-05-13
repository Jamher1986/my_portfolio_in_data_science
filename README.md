# 🦠 COVID-19 API Data Cleaning Project

## 📌 Project Overview
This project demonstrates how to collect data from a public COVID-19 API and clean it using Python. The goal is to show practical skills in data collection, data wrangling, and preparation for analysis — ideal for a data analyst or data cleaning portfolio.

## 🔗 Data Source
- API:  [COVID19API.com](https://covid19api.com/)
+ API: [disease.sh - COVID-19 API](https://disease.sh/)
-  Country Used: Nigeria (`/dayone/country/nigeria` endpoint)
+ Data Scope: All countries (`/historical?lastdays=30` endpoint)

## 🛠️ Tools & Libraries
- Python
- Pandas
- Requests
- Jupyter Notebook

## 📥 Data Collection
Data was collected using the `requests` library to send a GET request to the COVID19 API. The response (in JSON format) was converted to a Pandas DataFrame for cleaning and analysis.

## 🧼 Data Cleaning Steps
1. Converted JSON to Pandas DataFrame.
2. Selected key columns: `Date`, `Confirmed`, `Deaths`, `Recovered`, and `Active`.
3. Renamed columns to lowercase (`date`, `cases`, `deaths`, `recovered`, `active`) for consistency.
4. Converted the `date` column to datetime format using `pd.to_datetime()`.
5. Checked and handled missing values:
   - Used `.fillna(0)` to replace missing values with 0 in numeric columns.
6. Reset the DataFrame index and saved cleaned data to CSV.

## 📁 Project Structure
covid_api_project/
├── covid_api_cleaning.ipynb # Main Jupyter Notebook with all steps
├── cleaned_covid_data.csv # Output after cleaning
└── README.md # This file

## 🚀 How to Run This Project

1. Clone or download the project folder.
2. Make sure you have `requests` and `pandas` installed:
3. Open the notebook `covid_api_cleaning.ipynb` in Jupyter.
4. Run the cells one by one to fetch and clean the data.

## 🎯 Why This Project?
This project was done to strengthen my skills in working with real-world API data, handling missing values, and preparing data for analysis. It is part of my data analytics portfolio.
You can view the final cleaned DataFrame or saved `.csv` file for downstream analysis or visualization.

## 🙋🏽 Author
**Nguyen Anne**  
Affiliate Marketer & Data Enthusiast  
Building remote work skills in data cleaning and analysis.
