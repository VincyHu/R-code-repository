# Game Fun: Customer Acquisition through Digital Advertising

Disclaimer: “No similarity to actual persons or companies is intended or should be inferred.”

Game Fun is one of the world's top developers of casual mobile games and spends millions of dollars every year on digital advertising. Of particular interest to Game Fun is their efforts on improving their customer acquisition. It is a common belief in the mobile gaming industry that the more paid traffic you have, the better your organic traffic will be. This is known as K-Factor

However, measuring the causal effect of online digital advertising has proven to be an extremely challenging task. Towards this end, Game Fun decided to run an A/B experiment.

## Display banner experiment
Game Fun ran an online display banners advertising campaign with the primary objective of increasing its sales on gaming subscription packages. To attract new users, the display ad advertised their most popular game and offered the user a promotion of $25 signing-up bonus. The credits would appear in the customer’s game account and could be used to purchase any further in-app features. Based on historical data, a new customer subscription brings a revenue of $37.5 on average. This results in a net inflow of $12.5 after the $25 credit for the users acquired through this promotion.

The A/B experiment worked as follows:
Before the start of the digital ad campaign, Game Fun chose two different websites (“content publishers”) to run the experiment on. The content publishers have randomly assigned their web users to test and control groups. As users browsed on the two websites, the advertising servers checked whether a given user should be show a Game-Fun ad. If the user qualified for a Game-Fun ad, then the ad server checked whether the user was assigned to the test or the control group. If the user belonged to the test set, a Game-Fun ad was displayed to the user. Otherwise, a completely irrelevant ad was displayed to the user.

However, Game-Fun had to pay the content publishers for these irrelevant ads, as well. This raised a tension between the management and the data scientist teams. The management team had two concerns. First, paying for other companies ads is directly decreasing their marketing budget. Second, they didn’t like the fact that some users who saw an irrelevant ad might have signed up for the Game Fun game in the first place, had they been shown their gaming ad (indirect effect – opportunity cost missed). For these two reasons, the management team asked their data scientist team to carefully decide on the best proportion of users to assign to the test and control groups, while at the same time maintaining a statistically valid comparison.

The data scientist team ran a statistical power analysis of the experiment, and decided to allocate 70% of users to test group and the rest 30% to the control group.

## Anlaysis of the experiment
After the completion of the experiment, the results came in. See the [**Excel file**](https://github.com/VincyHu/Product/blob/master/Customer%20Acquisition%20through%20digital%20advertising%20--%20AB%20testing%20result%20analysis/GameFun.xlsx). 

## Questions
Questions
1. Before evaluating the effect of an experiment, it is important to make sure that the experiment was executed correctly. Check whether the test and control groups are
probabilistically equivalent on their observables?

    a. More specific, compare the averages of the income, gender and gamer variables in the test and control groups. You should also report the % difference in the
averages. Compute its statistical significance.
    b. Briefly comment on what these metrics tell you about probabilistic equivalence for this experiment.
    c. If you had run this type of analysis BEFORE executing an experiment and found a large difference between test and control groups, what you should do?
    d. If you had millions of consumers, your “classic” statistical significance tests would not work (this is because the number of samples is used to compute those classic statistical tests). Do some research online and propose what significance test would you do in case you had “big data”?

2. Evaluate the average purchase rates in the test and control for the following groups. For each comparison, report the average purchase rate for the test, average purchase rate for the control and the absolute difference (not the % difference) between the test and
control.
    a. Comparison 1: All customers
    b. Comparison 2: Male vs Female customers
    c. Comparison 3: Gamers vs Non-Gamers Customers
    d. Comparison 4: Female Gamers vs Male Gamers

3. Assess the expected revenue in the test vs. control for the following comparisons:
    a. Comparison 1: All customers
    b. Comparison 4: Female Gamers vs Male Gamers

4. Based on your previous answers, provide a brief recommendation to your management team summarizing the expected financial outcome for Game-Fun.
    a. Should Game-Fun run this promotion again in the future? If no, explain why. If yes, should Game-Fun offer it to all customers or a targeted segment.