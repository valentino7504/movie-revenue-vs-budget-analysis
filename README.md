# Movie Revenue Prediction
### Simple linear regression project to model the relationship between movie budgets and their revenue

## Contents
1. Introduction
2. Python Libraries Used
3. Problem Statement
4. The Dataset
5. Data Exploration, Visualisation and Analysis
6. The Model
7. Evaluating the Model
8. Conclusion

## 1. Introduction
In this mini project, I built a Linear Regression model to study the linear relationship between a movie's production budget and its worldwide revenue. I used the Python programming language with the relevant modules to analyse, clean and visualise the data

## 2. Python Libraries Used
* *pandas* - Provided necessary tools to manipulate the data and clean the data
* *matplotlib* - Used to create basic plots in Python
* *scikit-learn* - Provides simple tools for effective and efficient data analysis applications
* *requests* - used to fetch content(HTML) from the url
* *BeautifulSoup* - Provides simple tools for parsing HTML, and extracting the data

## 3. Problem Statement
As stated earlier, the question is
"Can a reasonable relationship be established between production budget and movie revenue?"
I will be investigating the relationship between movie revenue and production budget. I will evaulate if the relationship is significant using the R<sup>2</sup> score value.

## 4. The Dataset
The dataset was scraped from "The Numbers" at https://www.the-numbers.com/movie/budgets/all
The dataset contains budget and worldwide revenue for 6370 movies with varying budgets and revenue. First, I used the *requests* module to obtain.I used *BeautifulSoup* to parse the retrieved html, and then created a CSV file from it using Pandas.

## 5. Data Exploration, Visualisation and Analysis
I used *pandas* to read the CSV file using the standard read_csv() function into a DataFrame. I explored the data and discovered that 

