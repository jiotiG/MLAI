<span style="color: green; ">

# Berkeley MLAI Coupon Acceptance Case Study

# A data analysis on -- Will the Customer accept the coupon?

This is a data analysis project to analyze and present the data on which customers are most likely to accept a coupon, under what conditions?

# Author: Jyoti Garg 
garg.jyoti@gmail.com

## Table of Contents

- [Introduction](#introduction)
- [Tools Used](#tools-used)
- [Data](#data)
- [Analysis](#analysis)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The goal of this project is to analyze with visualizations and probability distributions
to distinguish between customers who accepted a coupon while driving versus those that did not.

The objective of this project was to apply the concepts learnt during the Module 1 of Machine 
Learning and Artificial Intelligence (ML/AI). This is a case study which looks at a given set of data 
obtained by survey from the customers and analyze which cohort of customer are most likely to accept a coupon 
when they are presented with it while driving.

## Tools Used
For the large part of this case study, basic Pandas (library built in Python) is used. Plotly and Matplotlib 
libraries are also used in order to generate the visualizations.


## Process
To perform this case study, I tried to think about the CRISP-DM framework and how to apply here.

Usually CRISP-DM incorporates following process:<br>
1. Business understanding<br>
2. Data understanding and data preparation<br>
3. Modeling<br>
4. Evaluation<br>

However, in order to apply for this problem the business understanding was not necessary due to the nature of the problem.
Looking at the other three steps in more detailed view in next sections --

## Data understanding and data preparation

1. Data Understanding <br>
  In order to fully understand data the 'coupons.csv' was imported into pandas using read_csv. Then using `head`, `info`, `describe` and `shape` methods, the data understanding was built. 
  <br> For example the `car` column data was missing about 99.5% data and yielded no value to the overall dataset. Similar to that columns
   `toCoupon_GEQ5min`, `toCoupon_GEQ15min` and `toCoupon_GEQ25min` did not provide the info in the description of the dataset, neither they provided and correlation via the correlation matrix
   <br> More data was explored by looking at the "value_counts" to identify any formatting issues with the data.


2. Data preparation <br>
    Data cleanup and reformatting was performed during this step. The ineligible columns which were of no value were dropped during this step, a lot of other formatting was performed so later the data analysis and visualizations are more clear and concise.
    

## Modeling
For modeling basic pandas commands were utilized. 

## Evaluation
Pandas based calculations and visualizations generated with matplotlib, seaborn and plotly were utilized to evaluate the data and identify the key patterns of the customer behavior.

## Results
Some of the key findings which came out:<br>
From the initial plotting of `coupon` data it was evident that the `Coffee House` coupon was the most issued coupon. Followed by `Cheap restaurant` and `Carry Out & Takeaway`
Coffee House ~ 31%
Cheap Restaurant ~ 21%
Carry out & Takeaway ~ 18%
The suspense is are these coupons the most accepted by the customers too?

Bar data: <br>
1. The proportion of coupons issued for the bar and utilized were about 41%. So in the total coupons about 16% were bar coupons, and total bar coupons accepted were 6.52%
2. Customers who have visited bar before tend to accept the coupons more.
3. More people without kids who are not widowed ended up utilizing the bar coupon

Independent Analysis: <br>
1. 56% of total coupons issued were used.
2. Very few coupons were used when people were going to work or heading home.
   a. A large number of coupons were utilized when people had `No Urgent Place` to go to.
3. The most popular times of utilizing coupons were 2pm, 10 am and 6pm, and even higher when coupon had 1 day expiration
4. Single people utilized the most coupons
   a. Among these folks `Coffee House` copuons were still the winner.
5. Most of the coupons were utilized when the driver was driving `Alone`
6. `Unemployed`, `Students` and `Computer Science and Mathematical` occupations are also the folks to accept the coupon

## Contributing

This is a read_only project, currently contribution to this project is not open. 
Please feel free to fork the project for enhancing or trying out. 

## Contact
garg.jyoti@gmail.com
</span>