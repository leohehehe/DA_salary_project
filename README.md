# Data Analyst Salary Project 


1. Created a tool that estimates data analyst salaries to help data analysts negotiate their income when they get a job
2. Scraped over 1500 job descriptions from Glassdoor using python and Selenium
3. Engineered features from the text of each job description to quantify the value companies put on python, excel,
AWS, and R
5. Optimized Linear, Random Forest Regressors, and Lasso using GridsearchCV to reach the best model
6. Built a client-facing API using flask



# Resouces and Code


Python Version: 3.7.9 <br />
Jupyter Notebook Version: 6.1.4 <br />
Packages: pandas, numpy, sklearn, matplotlib, seaborn, selenium, flask, pickle <br />
Scraper Article: https://towardsdatascience.com/selenium-tutorial-scraping-glassdoor-com-in-10-minutes-3d0915c6d905



# Web Scraping


Inspired by the scaper article above, I tweaked the github repo to scrape 1500 job posts from GlassDoor.com. With each job post, I got the following features:

· Job Title<br />
· Salary Estimate<br />
· Job Description<br />
· Rating<br />
· Company Name<br />
· Location<br />
· Company Size<br />
· Founded Year<br />
· Type of Ownership <br />
· Industry<br />
· Sector<br />
· Revenue



# Data Cleaning 


Before EDA and modeling, I spent a decent mount of time cleaning the date so as to generate the ideal foramt for following procedures. I made the following changes and created some variables:<br />

· Parsed the numeric data form Salary column & Generated dependent Variable Avg_salary<br />
· Conerted hourly wages salries to annual salaries<br />
· Kept the company name only by removing the rate in the Company Name column<br />
· Created a new column for the state where the company locate at<br />
· Created a new column for the age of the company<br />
· Created mutilple columns for different skills required for different Data anlyst positions from the job description column: <br />Cancel Changes

    1. Python
    2. SQL
    3. AWS
    4. Spark
    5. Tableau
    6. Excel
    7. R Studio
    8. Power BI
 
 · Created a new column for Job Description Length<br />
 · Created a new column for Senority <br />
 
 
 
# Exploratory Data Analysis

I briefly overlook the distribution of data for different categories by using barplots, histcharts, heatmap and pivot table, here below are some highlights:


![image](https://user-images.githubusercontent.com/63262273/112365613-3c5f2a80-8cae-11eb-8563-89bb1b7580c0.png)
![image](https://user-images.githubusercontent.com/63262273/112365740-5d278000-8cae-11eb-9411-206d3fa1ad79.png)
![image](https://user-images.githubusercontent.com/63262273/112364436-e342c700-8cac-11eb-9dd0-c0218e0e1e8e.png)

# Model Building

· I transformed some of the catogorical variables( Company Size, Industry, Revenue) into dummy variables<br />
· I applied three different models <br />

    1. Muti-linear Regression
    2. Random Forest Regression
    3. Lasso Regression



