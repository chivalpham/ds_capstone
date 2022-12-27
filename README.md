# Starbucks provides a foundation for proposals.

## Introduction

This project is part of Udacity's Data Science Nanodegree Program.
The project's goal is to deliver offer suggestions to Starbucks customers based on transactional, customer, and offer data. The data was gathered by replicating the Starbucks smartphone app, which consumers use to check specials, pay for beverages in-store, and receive discounts.


## Libraries Used

Jupyter Notebooks, Python, and data analysis frameworks such as Pandas and Numpy were utilized to complete the project.

## Methodology

We apply the approaches used in a typical data science research in this project.

### 1. Business Understanding

The following questions were examined to help steer the project:

- What are the primary elements that influence client purchases?
- Do offers improve consumer engagement?
- What are the most popular offers?
- Which demographics are most interested in offers?
- Which deals should we propose to certain customers?

### 2. Prepare Data

In the [helper.py]
file, the `clean_portfolio`, `clean_profile` and `clean_transcript` functions are provided. They include the following features:

**Portfolio Dataframe Tasks**
* Distinct the channels into different columns 
* Distinct the offer type into different columns 
* Rename the id column to offer id

**Profile Dataframe Tasks**
* Correct the date. 
* Divide the gender column into fake columns. 
* Rename the column id to customer id.

**Transcript Dataframe Tasks**

* Split data for offers and transactions into many columns 
* Split event column into multiple columns 
* Modify field name person to customer id


### 3. Exploratory Analysis

During this phase, we examined the population's demographics and purchasing habits. The interactions between clients and the deals on offer were also considered.

### 4. Recommendation Engine

We used a knowledge-based recommendation engine in this project. We proposed one that selects the most popular bargains first, without taking demographics into account. This approach is a good place to start for customers who do not provide any demographic information into the app.

For the remaining clients, we implemented filters that allow the system to make suggestions based on the demographic information provided by the users.

Using data visualizations, we evaluated the recommendation systems.

### 5. Link to Blog Website
```
(https://medium.com/@chivalpham/starbucks-provides-a-foundation-for-proposals-30b08a4f86ce)
```

### 6. File in Repository
  - data:
    - `portfolio.json` :containing offer ids and meta data about each offer (duration, type, etc.)
    - `profile.json` :containing demographic data for each customer
    - `transcript.json` :containing records for transactions, offers received, offers viewed, and offers completed 
  - `notebook` :notebook contains the data analysis 
  - `helper.py`: containing `clean_portfolio`, `clean_profile` and `clean_transcript` to implement functions

