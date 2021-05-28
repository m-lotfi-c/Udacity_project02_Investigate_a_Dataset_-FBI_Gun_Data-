Business Problem
“We’re onboarding a new client next month as part of a very large deal. It’s critical that we support them with our excellent service levels. I need to know how many tickets per week on average we can expect from this client so we can ensure we have enough help desk resources in place.”
Reminder
As a reminder, we're at the top of the chart in the Business Problem Solving framework where we are simply trying to understand the business issue at hand.

What decisions need to be made?
The decision the sales manager needs to make is, “Do we have enough capacity on the support team to handle the support tickets from the new customer?” and “If not, how many people do we need to add to the support team to reach the desired capacity?”

What information do we need to inform this decision?
We need to calculate the average number of tickets per customer per week. We can then aggregate the average number of tickets for each customer to get a total average number of support tickets that we predict will be submitted per week. Once we have this information, we need to compare the predicted average number of tickets with the current capacity of the support staff, specifically, the average number of tickets each team member can handle.

What type of analysis is needed to get the information needed to make that decision?
Let’s use our Methodology Map flowchart to help us determine the type of analysis we should use to provide the exact information needed to inform the decision. We want to predict the average number of tickets per week a new customer will submit. Therefore, we’re looking to predict an outcome - that was easy.

Selecting the Appropriate Methodology
Step 1: Is this a data rich, or data poor problem?
Let’s recall the difference between data rich and data poor. If we have past data on the variable we’re trying to predict, then we are data rich. Otherwise, we are data poor. To determine whether we’re data rich or poor, we need to look at our data to get a better understanding. Looking at our data set, we see that we have the following information for each client:

The average number of tickets each client submits per week
The number of employees per client
The value of the contract with each client
The industry of each client
Since we have the number of tickets for each client, we are data rich.

Step 2: Should we use a numeric or classification model?
Our target outcome that we’re trying to predict is a number indicating the average number of tickets we can expect per client, therefore, we should use a Numeric Model.
Step 3: Is our target variable continuous or time-based?
We’re looking for an average per week. So, at first glance, we might think this is a time-based problem. If we were looking to forecast a specific number per calendar week for a period of weeks, you’d be correct. However, in this problem, we just want an average per week and are not interested in a specific calendar week. Therefore, we will use a continuous model to solve our problem.

Instructor Notes
If you need a refresher on the slope-intercept form (y = mx + b), please read this short article here.



Linear Regression
Imagine we have the data displayed in the scatter plot. It appears that we have a linear relationship between the number of employees and the number of tickets. The relationship appears to be linear since it seems like we can draw a straight line through the data.
If we know the equation of the line, we can predict values for tickets given a certain number of employees. The simple equation for a line is:

y = mx + b
Y = Target Variable
X = Predictor Variable
m = Slope of the line
b = Y-intercept
Target Variable
The target variable is the variable we are trying to understand and predict. It is also referred to as the dependent variable. In our example, we are trying to predict Y, or the average number of tickets.
Predictor Variable
Predictor variables are used to try to predict the target variable and are also known as independent variables. In the example there is just one predictor variable, X, or the number of employees. It is used to predict the number of tickets based.
