# Starbucks provide suggestions framework

## Introduction

This Project is one part of the Data Science Nanodegree Program by Udacity.
The project's objective is to provide Starbucks consumers with offer recommendations using transactional, customer, and offer data. The information was collected by simulating the Starbucks mobile app, which is used by users to check offers, pay for their drinks in-store, and get discounts.

## Libraries Used

The project was implemented using Jupyter Notebooks, Python and
libraries used for data analysis such as Pandas and Numpy. 

## Methodology

In this project, we use the techniques used in a regular data science project.

### 1. Business Understanding

To guide the project, the following questions were considered:

- What are the main factors that contribute to customers making purchases?
- Are offers a way to increase customer engagement?
- What kind of offers are the most popular?
- What populations are more interested in offers?
- What offers should we recommend to different customers?

### 2. Prepare Data

In the [helper.py](TBD)
file, the `clean_portfolio`, `clean_profile` and `clean_transcript` functions are
provided. They implement the following functionality:

**Portfolio Dataframe Tasks**
* Split the channels into separate columns
* Split offer_type into separate columns
* change id column name to offer_id

**Profile Dataframe Tasks**
* Fix the date.
* Split gender column into dummy columns
* Change the column name id to customer_id. 

**Transcript Dataframe Tasks**

* Split value in several columns for offers and transactions
* Split event column into several columns
* Change column name person to customer_id


### 3. Exploratory Analysis

In this phase, we looked at the demographics and spending patterns of the population. The interactions between clients and the offered deals were also taken into consideration.

### 4. Recommendation Engine

In this project, we made use of a knowledge-based recommendation engine. We offered one that first chooses the most popular deals without taking demographics into account. For consumers who do not provide any demographic information into the app, this system is a nice place to start.

We added filters for the remaining clients, which enable the system to generate recommendations based on the demographic information supplied by the users.

We assessed the recommendation systems using data visualizations.

### 5. Link to Blog Website
```
TBD
```
### 6. Link to Repository
```
TBD
```
### 7. File in Repository
  - data:
    - `portfolio.json` :containing offer ids and meta data about each offer (duration, type, etc.)
    - `profile.json` :containing demographic data for each customer
    - `transcript.json` :containing records for transactions, offers received, offers viewed, and offers completed 
  - `Starbucks_Capstone_notebook` :notebook contains the data analysis 
  - `helper.py`: containing `clean_portfolio`, `clean_profile` and `clean_transcript` to implement functions

