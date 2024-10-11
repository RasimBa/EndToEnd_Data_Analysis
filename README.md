# RBaghirli_DataAnalyst_Assessment
A project for cleaning, enriching, and analyzing business lead data with integration to PostgreSQL for structured querying and analysis.

## Data Cleanup, Lead Enrichment, and PostgreSQL Integration Task

### Project Overview

This project involves cleaning and enriching business lead data by leveraging external data sources, such as the Google Places API, to fill missing information (e.g., addresses and phone numbers). The cleaned and enriched data is then integrated into a PostgreSQL database for structured querying and analysis. Additionally, the project performs exploratory data analysis (EDA) and visualizations to gain insights into the lead data.


### Folder Structure

```bash
united_solutions/
├── Inputs/            # Contains all input data files
│   ├── data cleanup assignment.xlsx
│   ├── leads_cleaned_data.xlsx
│   ├── leads_enriched_data.xlsx
│   └── leads_in_review_data.xlsx
│
├── jupyter files/     # Contains Jupyter notebooks with code for data cleaning, enrichment, analysis, and PostgreSQL integration
│   ├── 1.Data_Cleaning.ipynb
│   ├── 2.Database_Operations.ipynb
│   ├── 3.Data Enrichment.ipynb
│   └── 4.Reporting_Analysis.ipynb
│
└── README.md          # Detailed project documentation (this file)

```

### Folder Descriptions:

1. Inputs/:
This folder contains the raw input data files used for the project. The data cleanup and enrichment processes are applied to files within this folder, such as data cleanup assignment.xlsx, leads_cleaned_data.xlsx, and leads_enriched_data.xlsx.

2. jupyter files/:
This folder contains the Jupyter notebooks where the data cleaning, enrichment, analysis, and database integration tasks are performed.

### Key Features

1. *Data Cleaning: Identifying and handling missing or inconsistent values, standardizing data formats.*

2. *Data Enrichment: Using external APIs (such as Google Places API) to fill missing information for leads.*

3. *PostgreSQL Integration: Cleaned and enriched data is stored in a PostgreSQL database for further analysis and querying.*

4. *Exploratory Data Analysis (EDA): Analyzing lead distribution across different countries and cities using visualizations.*

5. *Visualizations: Charts such as bar charts, pie charts to visualize insights from the cleaned data.*


### Database Operations

PostgreSQL Integration:

1. The cleaned data is inserted into two tables in a PostgreSQL database:
2. leads_cleaned: Contains valid data.
3. leads_in_review: Contains data that needs further review.
4. The integration is done using the psycopg2 library to connect Python with PostgreSQL.
5. SQL queries are used for basic data analysis, such as counting leads by country and analyzing data enrichment success.

### Technologies Used

Python: Pandas, Matplotlib, Seaborn, Psycopg2
Jupyter Notebook: For data analysis and database operations
Google Places API: For data enrichment
PostgreSQL: For structured data storage and querying

### How to Run the Project

1. Clone the Repository:

git clone https://github.com/RasimBa/RBaghirli_DataAnalyst_Assessment.git

2. Install Dependencies: Install the required Python libraries using pip:
   
pip install -r requirements.txt

3. Set Up PostgreSQL:

Ensure you have PostgreSQL installed and running.
Create a database and update the connection details in the Jupyter notebook or script.

Run the Jupyter Notebooks:

Navigate to the jupyter files/ folder.
Open the notebook files (e.g., data_cleanup_and_enrichment.ipynb) and run the cells to perform data cleaning, enrichment, and analysis.

The data will be stored in PostgreSQL.

Use SQL Queries for Analysis:
The SQL scripts provided in the project (e.g., create_tables.sql, basic_queries.sql) can be used to analyze the stored data in PostgreSQL.


### Objective

The goal of this project is to improve the completeness and accuracy of lead data through enrichment, store the cleaned data in a PostgreSQL database for further analysis, and provide meaningful insights through exploratory data analysis and visualizations. The PostgreSQL integration ensures the data is structured and ready for querying, while the visualizations help in understanding the distribution and quality of the leads.

### Visualizations and Analysis

#### The project includes various visualizations to understand the lead data better:

Bar charts displaying the number of leads in different countries and cities.
Pie charts showing the distribution of leads by country.
SQL-based analysis to run queries on the cleaned and enriched data.


Project Overview
This project involves cleaning and enriching business lead data by leveraging external data sources, such as the Google Places API, to fill missing information (e.g., addresses and phone numbers). The cleaned and enriched data is then integrated into a PostgreSQL database for structured querying and analysis. Additionally, the project performs exploratory data analysis (EDA) and visualizations to gain insights into the lead data.
