# Udacity_DS_Capstone_Project - Starbucks Project

### Introduction
This is Udacity Data Scientist Nanodegree Capstone Project.  I will leverage what I learned from the program to build the Starbucks Challenge project.

I will follow the following steps of the data science process to finish this project.

1. Problem Statment. Define the program that I want to solve.
2. Analyze the problem through the data exploration analysis, data visualizations.
3. Model building, which includes data preprocessing, feature engineering, documentation on metrics, algorithms.
4. Refinement. such as cross-validation, grid search.
5. Results, which include the model evaluation and validation
6. Conclusion.

### Problem Statement
From the dataset, we know that people produce various events, including receiving offers, opening offers, and making purchases. There are no explicit products to track, only the amounts of each transaction or offer are recorded. And there are three types of offers that can be sent. Based on the procedure I mentioned above, I will conduct the analysis, build the machine learning model and find out the customer buying behaviors and how much are they going to spend on based on the offer type. 

### Libraries
- pandas
- numpy
- json
- datetime
- matplotlib
- seaborn
- sklearn

### Files in the Repository
- In Data folder: there are 3 dataset, for details, please check below. Pease note that transcript file is too large to upload into github.
- In Main folder: there is the original code in ipynb and html formate.

### Data Sets
The data is contained in three files:

- portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
- profile.json - demographic data for each customer
- transcript.json - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

### portfolio.json

- id (string) - offer id
- offer_type (string) - type of offer ie BOGO, discount, informational
- difficulty (int) - minimum required spend to complete an offer
- reward (int) - reward given for completing an offer
- duration (int) - time for offer to be open, in days
- channels (list of strings)

### profile.json

- age (int) - age of the customer
- became_member_on (int) - date when customer created an app account
- gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
- id (str) - customer id
- income (float) - customer's income

### transcript.json

- event (str) - record description (ie transaction, offer received, offer viewed, etc.)
- person (str) - customer id
- time (int) - time in hours since start of test. The data begins at time t=0
- value - (dict of strings) - either an offer id or transaction amount depending on the record

### Result:
- Original model: accuracy 92.9%, F-score of 0.9305.
- New model (after refinement): accuracy 94.4%, F-score of 0.9391.
The new model result is slightly better than the original model.

### Acknowledgments
- Udacity provide the data, platform.
- Project mentor Mrudula give me the tremendous help.
- Project project reviewer provide me very detailed feedback with patient.
