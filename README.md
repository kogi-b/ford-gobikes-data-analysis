# Ford GoBike Data Visualization.
## by Brian Kogi


## Dataset

The project is divided into two main parts, in part one of the dataset, I perform Exploratory Data Analysis on the dataset, documenting relationships and findings along the way. In the second part, I use the data and extract the key findings from the Exploratory Data Analysis to perform Explanatory Data Analysis.

The Dataset consists of information regarding 183411 bike trips for the month of February, including its timing and geolocation of the start and end of each trip. The dataset 2017-fordgobike-tripdata.csv can be downloaded [here](https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv).

- I started my exploration with the age variable, upon closer inspection, the age histogram was positively skewed with a lot of outliers. I had to use log to depict its distribution in a better way. I then removed outliers by filtering the data between the quartile ranges. I replotted the age histogram and it was still positively skewed but easier to extract information.
- I observed from the remaining data that most people using the service are in their 20s and 30s.
- The duration data had to be cleaned due to the amount of outliers in the data, I also added an extra column called duration_min which contains the duration but in minutes for easier readability. On plotting a histogram of duration in minutes, we can now see that the longest time is 12 minutes with the graph having a positive skew
- I then added a column called start_weekday_char which tracks the days of the week people initiated the service. We observed that the number of people using the service in the weekdays (Monday-Friday), is greater that the number of people using the service in the weekends

## Summary of Findings

In the exploration, I found out the following:
- Men use this service more than any other gender
- Women generally make longer trips than any other gender
- People aged 31 use the service more, followed by people aged 26
- More people use this service in weekdays compared to the weekends
- In the weekdays, most of the trips are initiated at 8:00am and 5:00pm
- In the weekends, most trips are initiated between 11:00am and 5:00pm
- bikes are ridden proportionally across all the genders
- The duration of trips in minutes does not vary a lot in the morning and in the afternoon, however, at night the duration reduces compared to the aforementioned time.
- Customers make longer trips on average during the day compared to subscribers
- Due to minimal variations in the duration of trips to each of the top 10 destinations, this could imply that most people generally make trips to and from the same places.

## Key Insights for Presentation

The presentation focuses on:
1. The number of subscribers compared to the number of customers.
2. Distribution of Duration in Minutes
3. Ratio of Gender in Population
4. Hourly Average Distribution of Trips Between Weekdays And Weekends
5. Hourly Average Trip Duration Between Customers and Subscribers