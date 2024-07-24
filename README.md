# ETL-Operations-on-Country-GDP-Data
This project extracts, transforms, and loads (ETL) GDP data of various countries from a Wikipedia page into a CSV file and an SQLite database. It also includes a logging mechanism to track the progress of the ETL process.

# Code Explanation
Extract Function : 
The extract function scrapes the GDP data from the specified Wikipedia page and stores it in a DataFrame.

Transform Function : 
The transform function converts the GDP values from USD (Millions) to USD (Billions) and rounds them to 2 decimal places.

Load Functions : 
The load_to_csv function saves the DataFrame to a CSV file, and the load_to_db function loads the DataFrame into an SQLite database table.

Run Query Function : 
The run_query function runs a specified SQL query on the database table and prints the output.

Log Progress Function : 
The log_progress function logs messages at various stages of the ETL process to a log file.

ETL Process Execution : 
The ETL process is executed in the following steps:  

- Extract data from the Wikipedia page.  
- Transform the data by converting GDP values.  
- Load the data into a CSV file and an SQLite database.  
- Run a query to select countries with GDP >= 100 billion USD.  
- Log the progress of each step.
