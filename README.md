## Sales Data Exploration(Walmart): MySQL + Python Project ##

## Project Overview
This project focuses on analyzing Walmart sales data to uncover meaningful business insights. As a passionate about data, I created this project to apply my skills in SQL and Python for solving business problems.

## Project Flow process
![ERD Diagram](https://github.com/royalisloyal/Sales-Data-Exploration-walmart/blob/main/Project%20Flow%20process.jpeg)

## Objectives
  -To explore and clean Walmart sales data

  -To answer key business questions using SQL

  -To identify patterns and trends in sales performance

## Project Steps

### 1. Set Up the Environment
   - **Tools Used**: Visual Studio Code (VS Code), Python, MySQL
   - **Goal**: Create a structured workspace within VS Code and organize project folders for smooth development and data handling.

### 2. Set Up Kaggle API
   - **API Setup**: Obtain my Kaggle API token from [Kaggle](https://www.kaggle.com/) by navigating to my profile settings and downloading the JSON file.
   - **Configure Kaggle**: 
      - Place the downloaded `kaggle.json` file in your local `.kaggle` folder.
      - Use the command `kaggle datasets download -d <dataset-path>` to pull datasets directly into my project.
    
### 3. Download Walmart Sales Data
   - **Data Source**: Use the Kaggle API to download the Walmart sales datasets from Kaggle.
   - **Dataset Link**: [Walmart Sales Dataset](https://www.kaggle.com/najir0123/walmart-10k-sales-datasets)

### 4. Install Required Libraries and Load Data
   - **Libraries**: Install necessary Python libraries using:
     ```bash
     --pip install pandas numpy sqlalchemy mysql-connector-python
     
   - **Loading Data**: Read the data into a Pandas DataFrame for initial analysis and transformations.

### 5. Explore the Data
   - **Goal**: Conduct an initial data exploration to understand data distribution, check column names, types, and identify potential issues.
   - **Analysis**: Use functions like `.info()`, `.describe()`, and `.head()` to get a quick overview of the data structure and statistics.

### 6. Data Cleaning
   - **Remove Duplicates**: Identify and remove duplicate entries to avoid skewed results.
   - **Handle Missing Values**: Drop rows or columns with missing values if they are insignificant; fill values where essential.
   - **Fix Data Types**: Ensure all columns have consistent data types (e.g., dates as `datetime`, prices as `float`).
   - **Currency Formatting**: Use `.replace()` to handle and format currency values for analysis.

### 7. Feature Engineering
   - **Create New Columns**: Calculate the `Total Amount` for each transaction by multiplying `unit_price` by `quantity` and adding this as a new column.
   - **Enhance Dataset**: Adding this calculated field will streamline further SQL analysis and aggregation tasks.

### 8. Load Data into MySQL
   - **Set Up Connections**: Connect to MySQL using `sqlalchemy` and load the cleaned data into each database.
   - **Verification**: Run initial SQL queries to confirm that the data has been loaded accurately.

### 9. SQL Analysis: Queries and Business Problem Solving
   - **Business Problem-Solving**: Write and execute SQL queries to answer business questions, such as:
     - Revenue trends across branches and categories.
     - Identifying best-selling product categories.
     - Sales performance by time, city, and payment method.
     - Analyzing peak sales periods and customer buying patterns.
     - Profit margin analysis by branch and category.
    

## Acknowledgments

- **Data Source**: Kaggle’s Walmart Sales Dataset
- **Inspiration**: Walmart’s business case studies on sales.
