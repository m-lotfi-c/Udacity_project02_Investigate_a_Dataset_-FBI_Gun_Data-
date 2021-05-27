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

