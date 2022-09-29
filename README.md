
# Starbucks Capstone Project

## Project Description

 This project aims to create the data that simulates how people make purchasing decisions and how those decisions are influenced by promotional offers.
 Each person in the simulation has some hidden traits that influence their purchasing patterns and are associated with their observable traits. People produce various events, including receiving offers, opening offers, and making purchases.
 There are three types of offers that can be sent: buy-one-get-one (BOGO), discount, and informational. In a BOGO offer, a user needs to spend a certain amount to get a reward equal to that threshold amount. In a discount, a user gains a reward equal to a fraction of the amount spent. In an informational offer, there is no reward, but neither is there a requisite amount that the user is expected to spend. Offers can be delivered via multiple channels.
 The basic task is to use the data to identify which groups of people are most responsive to each type of offer, and how best to present each type of offer.
 
## File Description

 The data contains three datasets.

 1- profile.json

 gender: (categorical) M, F, O, or null
 
 age: (numeric) missing value encoded as 118
 
 id: (string/hash)
 
 became_member_on: (date) format YYYYMMDD
 
 income: (numeric)
 
 2- portfolio.json

 reward: (numeric) money awarded for the amount spent
 
 channels: (list) web, email, mobile, social
 
 difficulty: (numeric) money required to be spent to receive reward
 
 duration: (numeric) time for offer to be open, in days
 
 offer_type: (string) bogo, discount, informational
 
 id: (string/hash)
 
 3- transcript.json

 person: (string/hash)
 
 event: (string) offer received, offer viewed, transaction, offer    completed
 
 value: (dictionary) different values depending on event type
 
 offer id: (string/hash) not associated with any "transaction"
 
 amount: (numeric) money spent in "transaction"
 
 reward: (numeric) money gained from "offer completed"
 
 time: (numeric) hours after start of test
 
## Methods and Results

 The results and the details of the project posted here.

 An user item matrix was used to discover how custumers responded to the offers they recieved. The next step was spliting the results into a training and a test tests. The SVD algorithm was training to find out how an user responses a certain offer. Following this step, a recommendation engine was created which recommends the company what kind of offer should be sent to a particular user. 

## References

 Udacity Data Science Nanodegree-Data Engineering course, Starbucks, GitHub, Stack Overflow.

# Starbucks-Project
