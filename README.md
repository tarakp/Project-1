# UofA Data Analytics Bootcamp Group Project 1

-----

**Team**:  Tarak Patel, Nicole Lund, and Anne Niemiec

**Field of Investigation**: Covid-19 Health Data

## Project Description

**Subject/Core Message**:  We will review Covid vaccine allocation trends to various states in the US for all three suppliers.  This will be contrasted with Covid death rates over that period and state populations from Census data.

**Data Hypothesis:**

* We expect to see a significant ramp-up in vaccine allocation with time. Aside from known anomolies like the Texas storm in March.
* We believe the distrubition ratios between the first and second dose will invert over time with early dates showing a higher level of 1st dose allocations and later dates showing a higher level of 2nd dose allocations.
* We expect to see larger quantities of Pfizer vaccines being allocated to states with the greatest population density due to storage requirements and larger quantities of Johnson and Johnson vaccines being allocated to states with lower population densities.

**Data Sources**

* Pfizer Vaccine Allocation Data: https://data.cdc.gov/Vaccinations/COVID-19-Vaccine-Distribution-Allocations-by-Juris/saz5-9hgg

* Maderna Vaccine Allocation Data: https://data.cdc.gov/Vaccinations/COVID-19-Vaccine-Distribution-Allocations-by-Juris/b7pe-5nws

* Johnson & Johnson Vaccine Allocation Data: https://data.cdc.gov/Vaccinations/COVID-19-Vaccine-Distribution-Allocations-by-Juris/w9zu-fywh

* Covid Cases and Deaths Data: https://data.cdc.gov/Case-Surveillance/United-States-COVID-19-Cases-and-Deaths-by-State-o/9mfq-cb36

* State Abbreviations List: https://www.infoplease.com/us/postal-information/state-abbreviations-and-state-postal-codes


## Planned Visualizations

### Group 1 Charts authored by Tarak Patel

#### Line Plot showing National Summarized Vaccine Allocations by Date

* x-axis = Date (The data is reported weekly. To simplify the labels, convert the dates to a week number and then label by month.)

* y-axis = 
    * Line 1 - Pfizer + Moderna 1st dose allocation
    * Line 2 - Pfizer + Moderna 2nd dose allocation
    * Line 3 - J&J allocations
    * Note: y-axis data is a summation for all states
* Legend labels = Pfizer + Moderna 1st dose, Pfizer + Moderna 2nd dose, J&J Single dose

#### Line Plot showing National Vaccine Allocations by Date
* x-axis = Date (The data is reported weekly. To simplify the labels, convert the dates to a week number and then label by month.)

* y-axis = 
    * Line 1 - Pfizer 1st dose allocation
    * Line 2 - Moderna 1st dose allocations
    * Line 3 - Pfizer 2nd dose allocations
    * Line 4 - Moderna 2nd dose allocations
    * Line 5 - J&J allocations
    * Note: y-axis data is a summation for all states

* Legend labels = Pfizer 1st dose, Moderna 1st dose, Pfizer 2nd dose, Moderna 2nd dose, J&J Single dose

#### Line Plot showing Individual State (Arizona) Vaccine Allocations by Date
* x-axis = Date (The data is reported weekly. To simplify the labels, convert the dates to a week number and then label by month.)

* y-axis = 
    * Line 1 - Pfizer 1st dose allocation
    * Line 2 - Moderna 1st dose allocations
    * Line 3 - Pfizer 2nd dose allocations
    * Line 4 - Moderna 2nd dose allocations
    * Line 5 - J&J allocations

* Legend labels = Pfizer 1st dose, Moderna 1st dose, Pfizer 2nd dose, Moderna 2nd dose, J&J Single dose


#### Bonus Line Plot showing Individual State (User Choice) Vaccine Allocations by Date
* x-axis = Date (The data is reported weekly. To simplify the labels, convert the dates to a week number and then label by month.)

* y-axis = 
    * Line 1 - Pfizer 1st dose allocation
    * Line 2 - Moderna 1st dose allocations
    * Line 3 - Pfizer 2nd dose allocations
    * Line 4 - Moderna 2nd dose allocations
    * Line 5 - J&J allocations

* Legend labels = Pfizer 1st dose, Moderna 1st dose, Pfizer 2nd dose, Moderna 2nd dose, J&J Single dose

### Group 2 Charts authored by Anne Niemiec

#### Stacked Bar Plot showing Vaccine Allocations by State on latest date present in the data

* x-axis = State

* y-axis = 
    * Bar 1: Pfizer cumulative 1st dose allocation
    * Bar 2: Pfizer cumulative 2nd dose allocation
    * Bar 3: Moderna cumulative 1st dose allocation
    * Bar 4: Moderna cumulative 2nd dose allocation
    * Bar 5: Johnson & Johnson cumulative single dose allocation
    
#### Stacked Bar Plot showing Vaccine Allocations Normalized by State Population by State on latest date present in the data

* x-axis = State

* y-axis = 
    * Bar 1: Pfizer cumulative 1st dose allocation / State Population
    * Bar 2: Pfizer cumulative 2nd dose allocation / State Population
    * Bar 3: Moderna cumulative 1st dose allocation / State Population
    * Bar 4: Moderna cumulative 2nd dose allocation / State Population
    * Bar 5: Johnson & Johnson cumulative single dose allocation / State Population 

#### 3 plot figure of Stacked Bar Plots showing Vaccine Allocations by State on latest date present in the data

* x-axis = State
    * Note, this is common to all 3 figures and should only be displayed on the bottom figure.

* Plot 1, y-axis:
    * Bar 1: Pfizer cumulative 1st dose allocation
    * Bar 2: Pfizer cumulative 2nd dose allocation
* Plot 2, y-axis:
    * Bar 1: Moderna cumulative 1st dose allocation
    * Bar 2: Moderna cumulative 2nd dose allocation
* Plot 3, y-axis:
    * Bar: Johnson & Johnson cumulative single dose allocation

* Example implementation: https://matplotlib.org/2.0.2/examples/ticks_and_spines/spines_demo.html

### Group 3 Charts authored by Nicole Lund

#### Line Plot showing National Vaccine Allocations and Reported deaths by date

* x-axis = Date

* Left y-axis = Total complete vaccination regimens allocated
    * Note, cumulative across states

* Right y-axis = New deaths reported

* Example report with separate plots: https://www.cnbc.com/2021/04/09/covid-19-cases-deaths-vaccinations-daily-update.html

#### Line Plot showing State Level (Arizona) Vaccine Allocations and Reported deaths by date

* x-axis = Date

* Left y-axis = Total complete vaccination regimens allocated

* Right y-axis = New deaths reported

#### Bonus Line Plot showing State Level (User Selected) Vaccine Allocations and Reported deaths by date

* x-axis = Date

* Left y-axis = Total complete vaccination regimens allocated

* Right y-axis = New deaths reported

#### Scatter Plot showing Reported Covid-19 Case Rate vs Poverty Rate by State

* x-axis = Poverty Rate

* y-axis = Reported Covid-19 Case Count / Population

* Include regression analysis

#### Scatter Plot showing Reported Covid-19 Death Rate vs Poverty Rate by State

* x-axis = Poverty Rate

* y-axis = Reported Covid-19 Death Count / Population

* Include regression analysis

### Group 4 Charts to be considered later
* Map total allocation by state (heatmap)
* Identify Outlier anomolies, i.e. freeze in Texas (box/whiskers chart)

## Additional Data to be considered later

**Data Sources**

* Vaccine Administration Data: TBD
