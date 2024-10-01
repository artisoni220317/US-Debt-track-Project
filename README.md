# US-Debt-track-Project

## About
You were hired by small debt agency in Washington DC that specializing in analyzing and forecasting public and private debt.The US government has requested an analysis of their public and governmental debt to answer some specific questions below.Using the Questions and Data Dictionary provided,answers the questions using cahrts/graphs and narratives.

## Approach Used

1. **Data Wrangling:** This is the first step where inspection of data is done to make sure **NULL** values and missing values are detected and data replacement methods are used to replace, missing or **NULL** values.

> 1. Select rows with null values in them. There are nulls values in our database as in creating the raw data.Replace them with blanks.
> 2. Select rows with blanks and remove them.
> 3. Convert Scientific notattion present into number.

2. **Feature Engineering:** This will help use generate some new columns from existing ones.

> 1. Add a new column named `time_of_day` to give insight of sales in the Morning, Afternoon and Evening. This will help answer the question on which part of the day most sales are made.

> 2. Add a new column named `day_name` that contains the extracted days of the week on which the given transaction took place (Mon, Tue, Wed, Thur, Fri). This will help 

### Generic Question

1. What was the yearly debt percentage increase for each year compared to the previous year?
2. Which months have historically seen the highest/lowest increase in total debt?
3. what is the projected growth of the publicly held debt in the next few years?

### Answers
1. The whole increase in the debt is at the end of the year so we select only that data which is from last day of that year.
   After selecting we will calculate the percentage increase using formula (B1-B2)/B2*100.After all the data is extracted,Insert recommended chart.
2. For this to answer,make a pivot table.In the row field,use month and in the value field use Average.Insert chart.
3. We will use Forecast function based on Max debt per year.Use FORECAST.ETS and build chart.
### Conclusion
1. For the total public debt outstanding,in previous years 2016 to 2019 the average increase was 5%.In 2020,we see large spike which was mostly caused by the pandemic responses in the U.S.
2. Highest debt increases historically occur during the months of January,February,November and December.Lowest debt increase historically occur during the months of April,May,June,July.
3. From 1997 to 2007,we saw an increase of 1 trillion for publicly held debt.From 2008 to 2019,debt increase from 6 trillion to 17 trillion.From 2020 to 2022,debt increase from 21.5 trillion to 25 trillion.From 2023 to 2027,it is projected that publicly held debt will increase to 33 trillion.




   
