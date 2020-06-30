# Analysis-of-Sales-Report-of-a-Clothes-Manufacturing-Outlet
Source of the dataset
The data is obtained fom UCI Machine Learning Repository.The dataset can be downloaded from here This is a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

Structure of the data
Our data contains the following variables with the corresponding descriptions:

InvoiceNo: Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'c', it indicates a cancellation.
StockCode: Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.
Description: Product (item) name. Nominal.
Quantity: The quantities of each product (item) per transaction. Numeric.
InvoiceDate: Invice Date and time. Numeric, the day and time when each transaction was generated.
UnitPrice: Unit price. Numeric, Product price per unit in sterling.
CustomerID: Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer.
Country: Country name. Nominal, the name of the country where each customer resides.
Aim of the study
In this project, we first clean the data, treat missing data and prepare the data for further analysis.Next we explore interesting patterns in the the data using EDA (Exploratory Data Analysis) techniques.This includes answering interesting questions like which products are the most popular products, which country saw the maximum sales, as well as in which weekday sales is maximum.Finally we conduct a Market Basket Analysis to find out which products are frequently bought together, so that relevant product recommendations can be provided to a customer who is interested in buying a particular item.

Installing / Getting started
The analysis was conducted using R.

Minimal setup required:

R
R Studio
Also apart from the R core packages, some other packages are also required for running the analysis.PLease open up the R Studio and run the following commands.The required libraries for this analysis will be installed if required and will be loaded for the current session.

if (!require(tidyverse)) install.packages('tidyverse')
if (!require(arules)) install.packages('arules')
if (!require(arulesViz)) install.packages('arulesViz')
Flow of the project
The codes of the project are shown as script.R file in a project pipeline format which can be run one after the other to get an idea of the flow of the analysis.

The script data cleaning shows the basic cleaning and preparation of the raw data for the further analysis steps. The next script EDA unveils the interesting facts of the data using exploratory data analysis techniques. Finally market basket analysis is conducted to identify the products that often co-occur in transactions.
