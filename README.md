# Glassdoor_Project

-  Used a web scraper (found online) that scrapped 956 jobs from Glassdoor using python and selenium.
-  Transformed all categorical columns into numerical values and selected most important features to build model.
-  Created a ML model (MAE ~ 14K $) that predicts the salary of a data science position at a company based on several factors.
-  Optimized Linear, Lasso, and Random Forest Regressors using GridsearchCV to reach the best model.


## Code and Resources used

- **Packages:** pandas, numpy, sklearn, matplotlib, seaborn, selenium, json.
- **Scraper Github:** https://github.com/arapfaik/scraping-glassdoor-selenium  
- **Scraper Article:** https://towardsdatascience.com/selenium-tutorial-scraping-glassdoor-com-in-10-minutes-3d0915c6d905  

## Youtube Playlist Link 
https://www.youtube.com/watch?v=MpF9HENQjDo&list=PL2zq7klxX5ASFejJj80ob9ZAnBHdz5O1t

## Data Collection

Used web scraper (GitHub linked above) to collect 956 jobs from glassdoor.com, with each job containing the following:
*	Job title
*	Salary Estimate
*	Job Description
*	Rating
*	Company 
*	Location
*	Company Headquarters 
*	Company Size
*	Company Founded Date
*	Type of Ownership 
*	Industry
*	Sector
*	Revenue
*	Competitors 

## Data Cleaning

The data collected was cleaned in order for it to be useful in the model building stage of the project. The following changes were done on the data frame's columns:

*	Changed the salary column into numeric values. 
*	Removed rows without salaries or with salaries equal to -1 (corrupt entries). 
*	Parsed rating out of company name. 
*	Made a new column for company state.
*	Transformed founded date into age of company.

Additionally, a couple of columns were created for variables that might be of use in the model building stage:

*	Added a column for if the job was at the company’s headquarters. 
*	Made columns for if different skills were listed in the job description:
    * Python  
    * Excel  
    * Spark 
    
*	Column for job title/poisition.
*	Column for job description length. 



## Exploratory Data Analysis 

I looked at the distribution of some of our variables as well as built a correlation heatmap and pivot tables to further understand how our variables are related to each other. A couple of the observations are found below:

<img width="405" alt="Screen Shot 2021-01-18 at 1 26 35 PM" src="https://user-images.githubusercontent.com/77576356/104909836-215ff980-5991-11eb-9bd8-35d65e2c815c.png">

<img width="322" alt="Screen Shot 2021-01-18 at 1 27 18 PM" src="https://user-images.githubusercontent.com/77576356/104909841-245aea00-5991-11eb-9083-5e9f3c39dff2.png">


<img width="658" alt="Screen Shot 2021-01-18 at 12 12 28 PM" src="https://user-images.githubusercontent.com/77576356/104909846-2755da80-5991-11eb-9996-300e0fd76451.png">
