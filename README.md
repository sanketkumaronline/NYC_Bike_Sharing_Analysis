# Citi Bike NYC Bike Sharing Analysis

## Overview
I visited New York City for two weeks and explored the city and landmarks on bikes. One of key factors in making this trip memorable is the Citi Bike bike sharing system. This allowed us to know the city better and interact with people. 

An idea came to my mind to start a similar bike sharing business in my hometown. We have got an angel investor who is interested in providing seed funding for bike share business in our hometown. We realized that the mechanics of making this business successful in our hometown will be different than in NYC. 

### Purpose
We are creating a proposal for the investor and i am working on data analysis. For this we have decided to do an analysis of Citi Bike data released to the public. Though we know that this data applies specifically to NYC, we are expecting to find out which part of the data can apply to our hometown and how we can use this data to learn more about this business. 

**Data Source:** [Citi Bike Trip Data for August 2019](https://s3.amazonaws.com/tripdata/201908-citibike-tripdata.csv.zip) 

**Softwares Used:** Tableau Public, Visual Studio Code

**Programming Languages:** Python Pandas Library (to convert Tripduration from integer to datetime)

### Tableau Public Story Link: [Citi Bike - NYC Bike Sharing Analysis](https://public.tableau.com/profile/sanket.kumar6757#!/vizhome/NYCBikeSharingSystemAnalysisAugust2019/Story1?publish=yes) 

## Results

**Visualization 1: Checkout Times for Users**

This visualization shows the length of time the bikes are checked out for all riders through a line graph.

![Checkout Times for Users](./Images/checkout-time-users.PNG)

* According to the graph, the bikes are checked out by almost all the riders for less than an hour. Very few riders have checked out the bikes for longer than an hour.
* The most common time duration is 5 minutes with a total of 146,752 trip count.
* The graph rises sharply before 5 minutes mark and drops exponentially after it. Therefore, it seems that most of the users do not prefer very short or long trips.

**Visualization 2: Checkout Times by Gender**

This visualization shows length of time the bikes are checked out for each gender through a multiple line graph.

![Checkout Times by Gender](./Images/checkout-time-gender.PNG)

* Male users are taking much more bike trips than female or unknown category. 
* The graphs for both male and female riders show similar pattern with a sharp peak at 5 minutes mark. It means the both male and female riders prefer average trip duration of about 5 minutes.
* The graph for Unknown category shows a different pattern with a flat plateau between 8 to 26 minutes mark. This could mean that riders in this category a more likely to checkout the bike for a broad range of time duration.

**Visualization 3: Trips by Weekday for Each Hour**

This visualization shows the number of bike trips by weekday for each hour of the day as a heatmap.

![Trips by Weekday for Each Hour](./Images/trips-weekdays-each-hour.PNG)

* On weekdays the most busy hours are in morning around 8 AM, and then in evening at around 5 and 6 PM.
* On weekends, the trend is reversed. I.e., hours around midday are more popular for rides.
* on Fridays, people start the rides a bit early in the evening.
* The only anomaly seems to be on Wednesday when the evening hours a much less busy than other weekdays.

**Visualization 4: Trips by Gender (Weekday per Hour)**

This visualization shows the number of bike trips by gender for each hour of each day of the week as a heatmap.

![Trips by Gender (Weekday per Hour)](./Images/trips-gender-weekdays-hour.PNG)

* The pattern is same for both Male and Female riders with only difference being the total number of rides which is represented by darkness of shades. The shades in heatmap for males are darker as the number of rides are much larger than females.
* The data in heatmap for Unknown category is not clear, perhaps due to limited data. However, we can see that weekend are popular with midday being the most busy time.

**Visualization 5: User Trips by Gender by Weekday**

This visualization shows the number of bike trips by user type and gender for each hour for each day of the week as a heatmap.

![User Trips by Gender by Weekday](./Images/user-trips-gender-weekdays.PNG)

* Majority of users are annual subscribers rather than short-term customers for both male and female categories. 
* For the unknown category, majority of users are short-term customers. This may be due to the difference in the way information is collected for short-term users and annual subscribers. 
* For annual subscribers, Thursdays are most popular for bike rides filled by Friday, Tuesday and Monday. This is true for both male and female riders.
* For short-term customers, weekends are more popular across all genders.
* The conclusion could be that most annual subscribers use Citi Bike for their daily commute. Whereas, most non-subscribers use it on weekends.
* No weekly pattern is visible for subscribers in unknown gender category.

**Visualization 6: Top Starting Locations**

This visualization shows the most popular trip starting locations over the map of New York City using circular markers with shade and size depicting the number of trips started.

![Top Starting Locations](./Images/top-starting-locations.PNG)

* Most of the trips are started in the Manhattan, followed by The Bronx and Queens.
* Since Manhattan has many attractions such as Empire State Building and Central Park, it seems users prefer to start their ride in this area.

**Visualization 7: Top Ending Locations**

This visualization shows the most popular trip ending locations over the map of New York City using circular markers with shade and size depicting the number of trips started.

![Top Ending Locations](./Images/top-ending-locations.PNG)

* Top trip ending locations are in Manhattan, followed by The Bronx and Queens.
* Since most of the trips are of short duration, the top ending points are also near the starting points.

## Summary

1. Almost all the bike trips taken are less than an hour and of short duration.
2. Majority of users are Males with annual subscriptions.
3. The morning and evening hours on weekdays are most popular, especially among subscribers. Probably, most subscribers take subscriptions for their daily commutes.
4. On weekends, the hours around noon are busier. Most short-term customers ride on weekends.
5. Top starting and ending locations are around popular landmarks and tourist destinations. I.e., Manhatten in this case.  

### Additional Visualization Suggestions

1. **Average Trip Duration by User Type by Week Days:** Though we have already plotted a heatmap for number of trips based on user type for each day of the week, we can plot a graph or a heatmap by substituting count of trips with average duration of trips. This will help us understand for how long a bikes will be used by a user on a particular day of the week.    

2. **Average Trip by Starting (or Ending) Location:** We can plot circular markers on the map to varying sizes and colors to signify the avarage trip duration according to the starting or ending locations. The bikes in locations with longer average trip duration might need more frequent servicing. 