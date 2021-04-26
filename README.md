# Project: Investigate a Dataset (FBI Gun Data)
The purpose of this project is to explore the trends of U.S gun purchases with census population data.<br> 
- <a href="https://github.com/m-lotfi-c/Udacity_project02_Investigate_a_Dataset_-FBI_Gun_Data-">[You can find this project repository in my my github repository]</a>

## Table of Contents
<ul>
<li><a href="#intro">Introduction</a></li>
<li><a href="#wrangling">Data Wrangling</a></li>
<li><a href="#eda">Exploratory Data Analysis</a></li>
<li><a href="#conclusions">Conclusions</a></li>
<li><a href="#limitations">Limitations</a></li>
<li><a href="#references">References</a></li>    
</ul>

<a id='intro'></a>
## Introduction
(original source on <a href="https://github.com/BuzzFeedNews/nics-firearm-background-checks">Github</a>)

- The data comes from the FBI's National Instant Criminal Background Check System. 
- The NICS is used by to determine whether a prospective buyer is eligible to buy firearms or explosives. 
- Gun shops call into this system to ensure that each customer does not have a criminal record or isn’t otherwise ineligible to make a purchase. 
- The data has been supplemented with state level data from census.gov.

#### NICS Firearm Background Checks:
- Month and Year by State and Type 
- The types of firearms are defined by the Bureau of Alcohol, Tobacco, Firearms and Explosives as follows:
    - __Handgun__
        - any firearm which has a short stock and is designed to be held and fired by the use of a single hand;
    - __Long Gun__
        - a weapon designed or redesigned, made or remade, and intended to be fired from the shoulder, and designed or redesigned and made or remade to use the energy of the explosive in 
    - __Other__
        - refers to frames, receivers, and other firearms that are neither handguns nor long guns (rifles or shotguns), 
        - such as firearms having a pistol grip that expel a shotgun shell, or National Firearms Act firearms, including silencers.
    - __multiple__
        - The indication of “multiple” denotes a background check where more than one type of firearm is associated to a single background check and “admin” denotes the administrative checks that are for other authorized uses of the NICS.
    - __Pre-Pawn__
        - requested by an officially-licensed FFL on prospective firearm transferees seeking to pledge or pawn a firearm as security for the payment or repayment of money, prior to actually pledging or pawning the firearm.
    - __Redemption—background checks__
        - requested by an officially-licensed FFL on prospective firearm transferees attempting to regain possession of a firearm after pledging or pawning a firearm as security at a pawn shop.
    - __Returned/Disposition—background checks__
        - requested by criminal justice/law enforcement agencies prior to returning a firearm in its possession to the respective transferee, to ensure the individual is not prohibited.
    - __Rentals—background checks__ 
         - requested by an officially-licensed FFL on prospective firearm transferees attempting to possess a firearm when the firearm is loaned or rented for use off the premises of the business.
    - __Private Sale—background checks__ 
        - requested by an officially-licensed FFL on prospective firearm transferees attempting to possess a firearm from a private party seller who is not an officially-licensed FFL.
    - __Return to Seller-Private Sale—background checks__
        - requested by an officially-licensed FFL on prospective firearm transferees attempting to possess a firearm from a private party seller who is not an officially-licensed FFL.

<a id='wrangling'></a>
## Data Wrangling:
## 1- __Gathering__
- https://github.com/BuzzFeedNews/nics-firearm-background-checks/blob/master/data/nics-firearm-background-checks.csv
- The NICS data is found in one sheet of an .xlsx file. It contains the number of firearm checks by month, state, and type.
- The U.S. census data is found in a .csv file. It contains several variables at the state level. Most variables just have one data point per state (2016), but a few have data for more than one year.
    - https://d17h27t6h515a5.cloudfront.net/topher/2017/November/5a0a5623_ncis-and-census-data/ncis-and-census-data.zip <br>
- [The U.S. census data is found in a .csv file. It contains population at the state level from (2010) to (2019)](./population2010-2019.csv)
- __Resulting three files:__<br>
    1- [[us_census_data.csv]](./us_census_data.csv)<br>
    2- [[us_census_population.csv]](./us_census_population.csv)<br>
    3- [[nics-firearm-background-checks.csv]](./nics-firearm-background-checks.csv)<br>

##  2- __Assessing & Cleaning__<br>
- Assessing Data The issues you identified were:
    - Nondescriptive column headers
    - Missing values (i.e. NaNs)
    - Inconsistent representations of values

- data Assessing divided to in three script for each gathed data
    - [[01-nics.ipynb]](./01-nics.ipynb)
    - [[02-population.ipynb]](./02-population.ipynb)
    - [[03-census.ipynb]](./03-census.ipynb) 
- __Resulting three files:__<br>
    1- [[nics.csv]](./nics.csv)<br>
    2- [[population.csv]](./population.csv)<br>
    3- [[census.csv]]('census.csv')<br>
- A messy (i.e. untidy) dataset
    - noted [[census.csv]]('census.csv') dataset is un structured and not easy to ooperate in 
    - we divided this dataset with common related dates and its data using [[04-Create_data.ipynb]](./04-Create_data.ipynb)  
- __Resulting files:__<br>
    1- [[census_2010_2016.csv]]('./census_2010_2016.csv')<br> 
    2- [[census_2012.csv]]('./census_2012.csv')<br>
    3- [[census_2014_2015.csv]]('./census_2014_2015.csv')<br>
    4- [[census_2015.csv]]('./census_2015.csv')<br>
    5- [[census_2016.csv]]('./census_2016.csv')<br>
    6- [[census_July_2016.csv]]('./census_July_2016.csv')<br>
    7- [[census_2010_2016.csv]]('./census_2010_2016.csv')<br>
    8- [[census_July_2016.csv]]('./census_July_2016.csv')<br>
    

### Questions
<ul>
<li><a href="#Question1">What census data is most associated with high gun per capita?</a></li>
<li><a href="#Question2">Which states have had the highest growth in gun registrations?</a></li>
<li><a href="#Question3">What is the overall trend of gun purchases?</a></li>
<li><a href="#Question4">Conclusions</a></li>
</ul>

<a id='conclusions'></a>
## Conclusions

### summarize your findings and the results that have been performed. 
- there isnot enough data in census population before 2010 
- the data ignore global economy an ploticals events
- some times the population percentage of change go down and the permit increase with it.
tations of your exploration. 
If you haven't done any statistical tests, do not imply any statistical conclusions. 
And make sure you avoid implying causation from correlation!

Once you are satisfied with your work here, 
check over your report to make sure that it is satisfies all the areas of the rubric 


(found on the project submission page at the end of the lesson). 
You should also probably remove all of the "Tips" like this one so that the presentation is as polished as possible.

<a id='Limitations'></a>
## Limitations

### summarize your findings and the results that have been performed. 
- there isnot enough data in census population before 2010 
- the data ignore global economy an ploticals events
- some times the population percentage of change go down and the permit increase with it.
- Fact Notes													
    (a)	Includes persons reporting only one race												
    (b)	Hispanics may be of any race, so also are included in applicable race categories
    (c)	Economic Census - Puerto Rico data are not comparable to U.S. Economic Census data									- - 
										
- Either no or too few sample observations were available to compute an estimate, or a ratio of medians cannot be calculated because one or both of the median estimates falls in the lowest or upper interval of an open ended distribution.
    - D --	Suppressed to avoid disclosure of confidential information												
    - F --	Fewer than 25 firms												
    - FN --	Footnote on this item in place of data												
    - NA --	Not available												
    - S  --	Suppressed; does not meet publication standards												
    - X  --	Not applicable												
    - Z  --	Value greater than zero but less than half unit of measure shown					

<a id='references'></a>
### References:
- https://github.com/BuzzFeedNews/nics-firearm-background-checks
- https://www.census.gov/en.html
    -  [State Population Totals: 2010-2019](https://www.census.gov/data/datasets/time-series/demo/popest/2010s-state-total.html#par_textimage_500989927) [[nst-est2019-01.xlsx](https://www2.census.gov/programs-surveys/popest/tables/2010-2019/state/totals/nst-est2019-01.xlsx)]
    - [Census Regions and Divisions of the United States](https://www2.census.gov/geo/pdfs/maps-data/maps/reference/us_regdiv.pdf)
- wikipedia
    - [List of U.S. states and territories by area](https://en.wikipedia.org/wiki/List_of_U.S._states_and_territories_by_area)
    - [Midwestern United States](https://en.wikipedia.org/wiki/Midwestern_United_States)
    - [Northeastern United States](https://en.wikipedia.org/wiki/Northeastern_United_States)
    - [Southern United States](https://en.wikipedia.org/wiki/Southern_United_States)
    - [Western United States](https://en.wikipedia.org/wiki/Western_United_States)
