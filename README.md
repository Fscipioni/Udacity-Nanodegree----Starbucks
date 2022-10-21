# Udacity Capstone Project: Starbucks

### Table of Contents

1. [Project Description](#description)
2. [Installation and Libraries](#installation)
3. [Files List](#files)
4. [DataFrame files description](#df_files)
5. [External links](#links)


## Project Description<a name = "description"></a>

This project is the capstone of the [Udacity](https://www.udacity.com/) Data Scientist Nanodegree Program.

In this project, I analyzed a simulated dataset of Starbucks offers that users can benefit from to purchase discounted products, with the goal to understand which type of offer is the most successful, and what type of customer is the most responsive to the reward system.

For this Udacity Nanodigree Capstone Project, Starbucks provided simulated data of their reward system. As a simplification, there are no explicit products to track. Only the amounts of each transaction or offer are recorded.

Each person in the simulation has some hidden traits that influence their purchasing patterns and are associated with their observable traits. People produce various events, including receiving offers, opening offers, and making purchases.

There are three types of offers that can be sent: buy-one-get-one (BOGO), discount, and informational. In a BOGO offer, a user needs to spend a certain amount to get a reward equal to that threshold amount. In a discount, a user gains a reward equal to a fraction of the amount spent. In an informational offer, there is no reward, but neither is there a requisite amount that the user is expected to spend. Offers can be delivered via multiple channels.

The goal of this data analysis is to help Starbucks company to understand how to target their customers with offers, that would encourage them to continue purchasing their products. The project follows the following steps: 
- Data exploration and pre-processing.
- Data engineering.
- Data analysis.
- Methodology.
- Conclusion.

## Installation and Libraries<a name = "installation"></a>

The code should run with no issues using Python versions 3.* 
The libraries used are are:

- pandas
- numpy
- math
- json
- datetime
- seaborn
- matplotlib
- timeit
- sklearn
- keras

## Files List<a name = "files"></a>

- Starbucks_Capstone_notebook.ipynb
- Starbucks_Capstone_notebook.html
- README.md

## DataFrame files description<a name = "df_files"></a>

profile.json
Rewards program users (17000 users x 5 fields)

- gender: (categorical) M, F, O, or null
- age: (numeric) missing value encoded as 118
- id: (string/hash)
- became_member_on: (date) format YYYYMMDD
- income: (numeric)

portfolio.json
Offers sent during 30-day test period (10 offers x 6 fields)

- reward: (numeric) money awarded for the amount spent
- channels: (list) web, email, mobile, social
- difficulty: (numeric) money required to be spent to receive reward
- duration: (numeric) time for offer to be open, in days
- offer_type: (string) bogo, discount, informational
- id: (string/hash)

transcript.json
Event log (306648 events x 4 fields)

- person: (string/hash)
- event: (string) offer received, offer viewed, transaction, offer completed
- value: (dictionary) different values depending on event type
	- offer id: (string/hash) not associated with any "transaction"
	- amount: (numeric) money spent in "transaction"
	- reward: (numeric) money gained from "offer completed"
- time: (numeric) hours after start of test

## External links<a name = "links"></a>

The main findings of the code can be found at the post available [here](https://medium.com/@fra.scipioni.83/starbucks-rewards-how-keep-a-customer-happy-f318d856b6b0)

