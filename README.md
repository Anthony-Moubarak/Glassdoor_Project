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

The data collected was cleaned in order for it to be useful in the model building stage of the project. 
