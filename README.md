# Cookie Cats Retention A/B Test


### Summary


This A/B test is based on the data originally provided by DataCamp and downloaded from [Kaggle](https://www.kaggle.com/datasets/yufengsui/mobile-games-ab-testing).

This project contains data gained from a classic 'connect three' puzzle game *Cookie Cats*. As players progress through the game they will encounter "gates" (rounds) force them to wait before they can progress or make an in-app purchase. 

Objective of the A/B test is to find out whether encountering the gate at a higher level increases Retention rate. In order to complete this we need to estimate retention rates splitting users into two groups: control group encounters the gate at round 30, test group does at round 40. 

Results of this test will provide insights to the following question: does encountering the gate at level 40 increases user retention? 

DataCamp project descriptions and Kaggle provide a brief yet complete description on what every feature mean in the dataset.

1) *userid* - id assigned to user 

2) *version*: **gate_30** - users in the **control** group, 
              **gate_40** - users in the **test** group

3) *sum_gamerounds* - the number of game rounds played by user during the fisrt 14 days of installation (round = level)

4) *retention_1* - if user is back to play the game on the 1st day after installation 

5) *retention_7* - if user is back to play the game on the 7th day after installation


### Defining the hypothesis

H0: Encountering the gate at round 40 will not change Retention Rate

H1: Encountering the gate at round 40 will increase Retention Rate

To admit the test is successfull, H0 should be rejected and H1 should be accepted based on a p-value. 

Here, successful metric to be tracked is **Retention Rate**. It's also possible to set gurdial metric to be aware of how user activity changes: user engagment. How actively users play in the first n number of rounds. 

Finally, the main goal is to compare Retention Rates between Test and Control groups and find out whether this difference is statistically significant (not due to random chance) to decide if the change of uplifting the round where user encounters the gate is actually needed. 

*The next steps of Data Analysis (data cleaning, EDA, A/B test data inferences, visualizations) are in the Jupyter Notebook provided in the repository.*
