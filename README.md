
# Price Prediction for Dublin Airbnb

A brief description of what this project does and who it's for


## Dataset

The starting dataset had 9143 rows and 106 columns.

Lets imagine we after providing our house to Airbnb. 
Fixed features of our property such as location, size, 
type of property, rooms. We also need to decide how we want 
to be listed: with or without picture, minimum nights, 
cancellation policy, number of people accepted. 
As we are conisdering first time host, we cannot be 
super host nor have previous reviews. Considering all 
these factor, 
we are ready to selection all the features to work with

The selected dataset has 9143 rows and 23 columns.


   

## Data Preparation

    1. Missing values
    Here we check the total percentage of missing values per columns
    Droping all the columns with more than 30% missing values
    We also drop few columns with missing values
    There are plenty of Nan's. It's more than likely that these hosts do not charge any extra cleaning fee or any deposits. 
    So let's  replace these null values with $0.00:
    There are few null values for host's profile pic. 
    We can assume null values as host has doesnt have profile pic
 
    2. Data formating
    Let's remove the dollar signs in all four columns 
    and convert the string values into numerical ones:

    3. Outliers
    For the columns price cleaning free and 
    The data points which fall below mean- 2*(sigma) or 
    above mean+2*(sigma) are outliers.

    For the column minimun nights, we are dropping any columns more than 
    1 year of minimum nights

## Feature Engineering
Lets have a look at the amenities column which is packed with lot of information.
In order to enrich our prediction, we extracted rare and unique amenities that we can provide.

Let's add columns with amenities that are somewhat unique and not offered by all hosts:

a laptop-friendly workspace
a TV
kid friendly accommodation
smoker friendly and
being greeted by the host.
After doing this, let's drop the original column:

## EDA

## Modelling

    1. Feature Selection
    2. Scaling

## Base Model

