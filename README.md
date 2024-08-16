ETL Project - GDP Data Extraction
-->Project Overview
This project automates the extraction of GDP data for countries as provided by the International Monetary Fund (IMF). The data is fetched from a Wikipedia page and is transformed, loaded into a CSV file, and stored in a SQLite database for easy querying.

-->Key Objectives:
Extract: Retrieve the list of countries and their GDPs from a specified URL.
Transform: Convert the GDP values from million USD to billion USD and round to 2 decimal places.
Load: Save the transformed data to a CSV file (Countries_by_GDP.csv) and store it in a database table (Countries_by_GDP) inside an SQLite database (World_Economies.db).
Query: Run a query on the database to display entries with a GDP over 100 billion USD.
Log: Track the progress and execution steps in a log file (etl_project_log.txt).
Project Files
etl_project_gdp.py: Main Python script performing the ETL (Extract, Transform, Load) process.
Countries_by_GDP.csv: CSV file storing the transformed GDP data.
World_Economies.db: SQLite database file storing the country GDP data.
etl_project_log.txt: Log file that contains timestamps and information about the script's execution.
README.md: This file, describing the project and instructions.
Requirements
To run this project, you'll need the following Python libraries:

requests
beautifulsoup4
pandas
sqlite3
numpy
datetime
You can install the dependencies by running:

bash
Copy code
pip install -r requirements.txt
How to Run the Project
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/your-repository-name.git
Navigate to the project directory:

bash
Copy code
cd your-repository-name
Run the ETL script:

bash
Copy code
python etl_project_gdp.py
Check the outputs:

The transformed GDP data will be available in Countries_by_GDP.csv.
The database file World_Economies.db will be updated with the GDP data.
The execution log will be recorded in etl_project_log.txt.
Query Example
The script automatically runs a query to display countries with a GDP greater than 100 billion USD. The result will be printed in the console.

Logging
All steps are logged into the etl_project_log.txt file, providing a clear record of the ETL process with timestamps.

Thankyou
