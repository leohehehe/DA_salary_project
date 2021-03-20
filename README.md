# Data Analyst Salary Project 

1. Created a tool that estimates data analyst salaries to help data analysts negotiate their income when they get a job
2. Scraped over 1500 job descriptions from Glassdoor using python and Selenium
3. Engineered features from the text of each job description to quantify the value companies put on python, excel,
AWS, and R
5. Optimized Linear, Random Forest Regressors, and Lasso using GridsearchCV to reach the best model
6. Built a client-facing API using flask


# Resouces and Code

Python Version: 3.7.9
Jupyter Notebook Version: 6.1.4
Packages: pandas, numpy, sklearn, matplotlib, seaborn, selenium, flask, pickle
Scraper Article: https://towardsdatascience.com/selenium-tutorial-scraping-glassdoor-com-in-10-minutes-3d0915c6d905


# Web Scraping

Inspired by the scaper article above, I tweaked the github repo to scrape 1500 job posts from GlassDoor.com. With each job post, I got the following features:

· Job Title
· Salary Estimate
· Job Description
· Rating
· Company Name
· Location
· Company Size
· Founded Year
· Type of Ownership 
· Industry
· Sector
· Revenue

# Data Cleaning 

Before EDA and modeling, I spent a decent mount of time cleaning the date so as to generate the ideal foramt for following procedures. I made the following changes and created some variables:

· Parsed the numeric data form Salary column & Generated dependent Variable Avg_salary
· Conerted hourly wages salries to annual salaries
· Kept the company name only by removing the rate in the Company Name column
· Created a new column for the state where the company locate at
· Created a new column for the age of the company
· Created mutilple columns for different skills required for different Data anlyst positions from the job description column:
  1. Python
  2. SQL
  3. AWS
  4. Spark
  5. Tableau
  6. Excel
  7. R Studio
  8. Power BI
 
 · Created a new column for Job Description Length
 · Created a new column for Senority 
 
 
To be continued······
