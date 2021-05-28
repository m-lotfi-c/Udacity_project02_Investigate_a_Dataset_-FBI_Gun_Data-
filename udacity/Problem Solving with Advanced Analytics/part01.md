# Course Outline
- Strategy for Solving Problems
- Non-Predictive Data Analysis
- Predictive Analysis
- Linear Regression
- Business Problem
- “We’re onboarding a new client next month as part of a very large deal. 
- It’s critical that we support them with our excellent service levels.
- I need to know how many tickets per week on average we can expect from this client so we can ensure we have enough help desk resources in place.

# Presentation and Visualization:
- Creation of the model is generally not the end of the project.
- Even if the purpose of the model is to increase knowledge of the data, 
- the knowledge gained will need to be organized and presented in a way that is useful to the customer.
- Depending on the requirements, the deployment phase can be as simple as generating a report or as complex as implementing a repeatable data scoring (e.g. segment allocation) or data mining process.
- In many cases it will be the customer, not the data analyst, who will carry out the deployment steps.
- Even if the analyst deploys the model it is important for the customer to understand up front the actions which will need to be carried out in order to actually make use of the created models.

# Cross Industry Standard Process for Data Mining (CRISP-DM)
"A data mining process model that describes commonly used approaches that data mining experts use to tackle problems... it was the leading methodology used by industry data miners." -Wikipedia
CRISP-DM Steps
Business Issue Understanding
Data Understanding
Data Preparation
Analysis/Modeling
Validation
Presentation/Visualization

Business Issue Understanding
"This initial phase focuses on understanding the project objectives and requirements from a business perspective, and then converting this knowledge into a data mining problem definition, and a preliminary plan designed to achieve the objectives. A decision model, especially one built using the Decision Model and Notation standard can be used." - Wikipedia
What decisions needs to be made?
What information is needed to inform those decisions?
What type of analysis can provide the information needed to inform those decisions?


Instructor Notes
Patrick mentions the term "data field". Referring to the familiar spreadsheet model, a data field can be thought of as a data column in your spreadsheet.

Data Understanding
"The data understanding phase starts with an initial data collection and proceeds with activities in order to get familiar with the data, to identify data quality problems, to discover first insights into the data, or to detect interesting subsets to form hypotheses for hidden information." - Wikipedia
What data is needed?
What data is available?
What are the important characteristics of the data?

Instructor Notes
In this stage, it's good to literally draw out the flow of your analysis similar to what Patrick is doing here. Outline the steps in your analysis and figure out what you need at every step of the way in order to get to the final data you need.

Analysis/Modeling
"In this phase, various modeling techniques are selected and applied, and their parameters are calibrated to optimal values. Typically, there are several techniques for the same data mining problem type. Some techniques have specific requirements on the form of data. Therefore, stepping back to the data preparation phase is often needed." - Wikipedia
Important Steps
Determine what methodology to use to solve the problem
Determine the important factors or variables that will help solve the problem
Build a model to solve the problem
Run the model and move to the validation phase

Validation
"At this stage in the project you have built a model (or models) that appears to have high quality, from a data analysis perspective. Before proceeding to final deployment of the model, it is important to more thoroughly evaluate the model, and review the steps executed to construct the model, to be certain it properly achieves the business objectives. A key objective is to determine if there is some important business issue that has not been sufficiently considered. At the end of this phase, a decision on the use of the data mining results should be reached." - Wikipedia
Important Steps
Observe the key results on the model
Ensure the results make sense within the content of the business problem
Determine whether to proceed to the next step or return to a previous phase
Repeat as many times as necessary





# Key Considerations
- Determine the best method of presenting insights based on the analysis
- Determine the best method of presenting insights based on the audience
- Make sure the amount of information shared is not overwhelming
- Use the results to tell a story to the audience
- For more complex analyses, you may want to walk the audience through the analytical problem solving process
- Always reference the data sources used
- Make sure your analysis supports the decisions that need to be made


Let’s practice classifying business problems into groups. For each of the following business problems identify the problem as one of the following:

Predictive
Geospatial
Segmentation
Aggregation
Descriptive
Scenario #1:
Qwiki Mart wants to build another store location. It wants to build the store in the area where they will have the most business, but they want to make sure that it is not within four miles of another location.

QUESTION 1 OF 4
What type of data analysis methodology would be best suited to answer this question?


Geospatial




Scenario #2:
TShirts.com received complaints that their web pages are loading slowly. They want to understand what web traffic levels to expect in the future in order to ensure they have enough server capacity to handle the traffic.
QUESTION 2 OF 4
What type of data analysis methodology would be best suited to answer this question?

Predictive





Scenario #3:
ShipYourStuff.com wants to know how much they ship to each zip code, state, or region as different managers want summaries by different dimensions.
QUESTION 3 OF 4
What type of data analysis methodology would be best suited to answer this question?




Aggregation


Scenario #4:
Pretty Faces Cosmetics wants to market to their top 3 customer segments. They need to create the customer segments, calculate how many customers fall into each one, and then determine which segment has the most customers.
QUESTION 4 OF 4
What type(s) of data analysis methodology would be best suited to answer this question? The answer may include more than one type.






# Predictive:
Predictive analytics uses existing data to predict a future outcome. For example, a company may use predictive analytics to forecast demand or whether a customer will respond to an advertising campaign.
Geospatial
This type of analysis uses location based data to help drive your conclusions. Some examples are:
Identifying customers by a geographic dimension such as zip code, state, or county, or
Calculating the distance between addresses and your stores, or
Creating a trade area based upon your customer locations for further analysis
Some types of Geospatial analysis require the use of special software - such as software that can convert an address to Latitude & Longitude, or can calculate the drive time between two geographic points on a map.

# Segmentation:
Segmentation is the process of grouping data together. Groups can be simple, such as customers who have purchased different items, to more complex segmentation techniques where you identify stores that are similar based upon the demographics of their customers.
Aggregation
This methodology simply means calculating a value across a group or dimension and is commonly used in data analysis. For example, you may want to aggregate sales data for a salesperson by month - adding all of the sales closed for each month. Then, you may want to aggregate across dimensions, such as sales by month per sales territory. In this scenario, you could calculate the sales per month for each salesperson, and then add the sales per month for all salespeople in each region.
Aggregation is often done in reporting to be able to “ slice and dice” information to help managers make decisions and view performance.

# Descriptive:
Descriptive statistics provides simple summaries of a data sample. Examples could be calculating average GPA for applicants to a school, or calculating the batting average of a professional baseball player. In our electricity supply scenario, we could use descriptive statistics to calculate the average temperature per hour, per day, or per date.
Some of the commonly used descriptive statistics are Mean, Median, Mode, Standard Deviation, and Interquartile range.

Data Rich vs. Data Poor
Do you have data on what you are trying to predict? If so, you can proceed down the data rich path, otherwise, the data poor path is your only option. See the following example that demonstrates a data poor scenario.


A/B Tests
If there is not sufficient usable data to solve the problem, then we need to set up an experiment to help us get the data we need. An experiment in a business context is usually referred to as an A/B Test.


Numeric vs. Non-Numeric Predictive Analysis
Assuming we have enough data to proceed with the analysis, our next decision is to look at the outcome we’re trying to predict and determine if it’s a numeric outcome or a non-numeric outcome.
Regression Models
Numeric outcomes are those where the outcome is simply a number. Predicting the demand for electricity or the hourly temperature are both numeric outcomes. Models predicting numeric data are called regression models.
Classification Models
Non-numeric outcomes are those where we’re trying to predict the category into which a case (e.g. customer) falls, such as whether a customer will pay on-time, pay late, or default on a payment. Another example is the whether an electronic device will fail before 1000 hours or not. Models predicting non-numeric data are called classification models.

Target Variables
Target variables represent the outcome we are trying to predict. In order to select the right predictive model, we first determine whether the target variable is numeric or non-numeric. The type of numeric or non-numeric target variables will then help us select which model is appropriate. Let’s start with numeric variables.
Types of Numeric Variables
The three most common types of numeric variables are continuous, time-based, and count.
Continuous
A continuous variable is one that can take on all values in a range. For instance your height can be measured down to many decimal places. We do not grow in even inch intervals.
Time-Based
A time-based numeric variable is one where you are trying to predict what will happen over time. This is often related to forecasting.
Count
Count variables are numbers that are discrete, positive integers. They’re called count numbers because they’re used to analyze variables that you can count. As modeling these type of variables is not common in business, we won’t be covering this topic in this course.

Non-Numeric Variables
A non-numeric variable is often called categorical, because the values of the variable take on a discrete number of possible values or categories. Examples include whether an electronic device will fail before 1000 hours or not; whether a customer will pay on-time, pay late, or default on a payment, or whether a store is classified as large, medium or small.
Classification Models: Binary and Non-Binary
When modeling categorical variables, the number of possible outcomes is an important factor. If there are only two possible categorical outcomes, such as Yes or No, or True or False, then the variable can be described as Binary.
If there are more than two possible categorical outcomes, such as small, medium, or large, or pay on-time, pay late, or default on a payment, then the variable can be described as non-binary. The important take-away from this lesson is the ability to determine if you should use a classification model, and whether it should be a binary model or a non-binary model. Ben Burkholder will lead a course focused on classification models and will go into detail about these types of models.

Methodology Map Assessment
Now that we’ve gone through several scenarios, let’s get some more practice determining the right methodology for a variety of business problems. For each of the following descriptions, select the correct methodology. Use the methodology map as a guide to help make the decision.