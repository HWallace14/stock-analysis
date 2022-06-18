# Stock Analysis

## Overview of Project

### Purpose

The purpose of this project is to help our friend, Steve, whose parents want to invest in some form of stocks. They want to invest in a company called Daqo with the ticker "DQ" and we're here to look through the data and tell them whether or not that's a good idea. After grabbing some data for Daqo and a few other "green" companies we'll dig through and tell them which company would be the best to invest in.

## Analysis

### Analysis of DQ Stocks

After running an analysis of Daqo's stocks for the year 2018 we've found that Daqo's stock dropped about 63%. As a result we cannot recommend to our friend Steve or his parents that they purchase any of Daqo's stock. 

<img width="630" alt="DQ Analysis 2018" src="https://user-images.githubusercontent.com/105998378/174394112-bc5a6ed3-0a40-415d-b727-cfe41c6b0310.png">

---

# Analysis of Other Green Stocks (VBA Challenge)

## Overview

### Purpose

The purpose of this analysis is two-fold: 

1) To compare a list of "green" companies' stocks for the years 2017 and 2018 and determine a stock that would be best for investing.
2) To refactor the code for the original analysis in order to try and reduce the amount of time it takes to run said code/make more efficient code.

## Analysis

### Stock Comparison 2017 to 2018

Looking at the group of stocks (pictured below) there are only two companies that managed to have positive returns for both years (RUN and ENPH) with ENPH having the larger growth period in 2017 and just barely missing having the larger return in 2018. Due to these findings I would recommend investing in ENPH over RUN, although buying both would be preferred if they have the money.

<img width="934" alt="VBA_Challenge_2017" src="https://user-images.githubusercontent.com/105998378/174413284-00da244d-4fcf-4245-abbf-ffcbc1949295.png">

<img width="935" alt="VBA_Challenge_2018" src="https://user-images.githubusercontent.com/105998378/174413289-2bbd1d7f-8065-422f-86ae-35b902db0f31.png">

### Code Comparison Original to Refactored

Starting out we can see that the two bits of code are very similar. The output sheet is formatted and activated while an inputbox for the year is enabled and a timer is started to time the code and see how efficiently it runs (in this scenario we are assuming that faster = more efficient). These bits of code aren't done in the same order but they do both create the same result.

##### Refactored Code

<img width="755" alt="Challenge Code Beginning" src="https://user-images.githubusercontent.com/105998378/174413951-d024e1a7-da10-4c2a-b0c5-3dd6d4944126.png">

##### Original Code

<img width="532" alt="Original Code Beginning" src="https://user-images.githubusercontent.com/105998378/174413961-635f83b5-6f43-41ca-a2db-4f7d61384c9c.png">

Just a little further down we can see where the real differences begin. The challenge code initializes 3 more arrays for the volumes, starting prices and ending prices then creates an index to be used for those arrays as well as the tickers. The original code utilizes a For loop over the entirety of the meat of the code in order to run through the same code for each ticker.

##### Refactored Code

<img width="503" alt="Challenge Code Initial For Loop" src="https://user-images.githubusercontent.com/105998378/174414732-e9f4e9a6-7c98-4866-8c5e-af608cd7cebe.png">

##### Original Code

<img width="370" alt="Original Code Initial For Loop" src="https://user-images.githubusercontent.com/105998378/174414739-1c19a6db-b3a5-4a29-b56c-e191b48a0f20.png">

The final bits of refactored code show two more individualized loops with the volumes, starting prices and ending prices all being saved into each array according to the index that was created previously. The saved arrays are then spit out once the data has been collected and properly stored. Meanwhile the original code spits out each output as it finishes a loop, then begins its loop again. The formatting is the same for each.

##### Refactored Code

<img width="666" alt="Rest of Challenge Code" src="https://user-images.githubusercontent.com/105998378/174414983-0fcbe708-3eaa-4682-8650-bb1bfd2d52b3.png">

##### Original Code

<img width="584" alt="Rest of Original Code" src="https://user-images.githubusercontent.com/105998378/174414993-bf7d3683-6a62-4bd4-a074-2616adf5548a.png">

