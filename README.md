# Movie Revenue and Budget Relationship
### Simple linear regression project to model the relationship between movie budgets and their revenue

## Contents
1. Introduction
2. Tools Used
3. Problem Statement
4. The Dataset
5. Data Exploration, Visualisation and Analysis
6. The Model
7. Evaluating the Model
8. Conclusion

## 1. Introduction
In this mini project, I built a Linear Regression model to study the linear relationship between a movie's production budget and its worldwide revenue. I used the Python programming language with the relevant modules to analyse, clean and visualise the data

## 2. Tools Used
* *JupyterLab* - A web-based interactive development environment for notebooks, data and code.
#### Python Modules
* *pandas* - Provided necessary tools to manipulate the data and clean the data
* *matplotlib* - Used to create basic plots in Python
* *scikit-learn* - Provides simple tools for effective and efficient data analysis applications
* *requests* - Used to fetch content(HTML) from the url
* *BeautifulSoup* - Provides simple tools for parsing HTML, and extracting the data

## 3. Problem Statement
As stated earlier, the question is: <br/>
"Can a reasonable relationship be established between production budget and movie revenue?" <br/>
I will be investigating the relationship between movie revenue and production budget. I will evaluate if the relationship is significant using the goodness of fit score value.

## 4. The Dataset
The dataset was scraped from "The Numbers" at https://www.the-numbers.com/movie/budgets/all <br/>
The dataset contains budget and worldwide revenue for 6370 movies with varying budgets and revenue. First, I used the *requests* module to obtain.I used *BeautifulSoup* to parse the retrieved html, and then created a CSV file from it using Pandas.

## 5. Data Exploration, Visualisation and Analysis
I used *pandas* to read the CSV file using the standard read_csv() function into a DataFrame. I explored the data and discovered that there were a lot of null or zero values for movies which had either not come out yet (as at the time of this project - 4th March, 2023) or had incomplete data. I dropped all of such conflicting rows reducing my dataset to 5954 movies. <br/>
I then used matplotlib to plot a scatter diagram of the dependent variable - movie revenue against the independent variable - movie budget. This plot is shown below: <br/><br/>
![plot](https://user-images.githubusercontent.com/70894222/222928778-82abf625-1594-4b04-a97e-a7d024496909.png)

## 6. The Model
Simple linear regression is the simplest machine learning algorithm. Linear Regression is used to find the linear relationship between a target and one or more predictors/features.<br/>
Simple linear regression is used to check and find the relationship between one target and one feature. It detects statistical relationships that roughly predict the dependent variable (revenue) based on the independent variable (budget). <br/> 
I used the scikit-learn module to build a linear regression model using the data, generating a line of best fit. I obtained the slope to be 3.19688475. I then plotted this line of best fit on the scatter plot using matplotlib once more. <br/><br/>
![Screenshot 2023-03-04 222549](https://user-images.githubusercontent.com/70894222/222929381-f46298ab-7da2-4deb-932f-309b0cbca1d0.png)
<br/><br/>
![plot2](https://user-images.githubusercontent.com/70894222/222929319-cf728dcd-1b50-4422-844c-93ec88f2cd0b.png)

## 7. Evaluating the Model
I also used the scikit-learn module to obtain the goodness of fit score to be 0.5465, in other words, the linear regression model can accurately predict 55% of the revenue values based off the budget values using the regression model.

## 8. Conclusion
Based off the goodness of fit score, it is evident that the model is not good enough to deploy on new data. The budget alone cannot be accurately used to predict the revenue.
