# Ford GoBike Rides Data Exploration
## by Deepanshu Sharma


## Dataset

The dataset consisted of information about 519,700 trips taken during the year 2017. Data was available for the months of June to December.The dataset has 19 columns(including engineered features), including user type(Customer or Subscriber), gender, customer age, month, day of the week, hour of the day, start and end stations, their locations, and the bike id.
The dataset can be found [here](https://s3.amazonaws.com/baywheels-data/index.html)



## Summary of Findings

On exploration, we found that the trip duration variable had a very large range of values and hence required log transformation to clearly gauge its distribution. It was unimodal and had a mode of approximately 500 sec. For user types, the number of subscribers was way larger than customers. Users were predominantly males. The age had a unimodal, right-skewed distribution with mode between 30-35 years. Most rides occurred during October while Tuesday and Wednesdays were the most preferred days of the week. 8 and 18 were the most common hours for starting bike rides.

Customers, in general, took longer trips in comparison to subscribers. Also, females took longest trips among genders. We couldn't find a uniform trend between trip duration and age. Surprisingly, 70-80 years age group took the longest rides.June had the shortest trips whereas July, August and September had the longest ones. Saturday and Sunday had the longest trips while rest of the days had shorter but almost equal trips. Longest trips started between midnight and 3 AM.

Subscribers were in genral older than customers; female users were in general younger than the other genders. Older users preferred hotter months than the colder ones and younger users in general preferred to ride on weekends. Interestingly, younger users took rides during midnight-3AM. Older users preferred 4 AM the most.

Customers preferred September most whereas subscribers preferred October. Both rode least in June. Interestingly, customers preferred to ride more on weekends, whereas subscribers preferred to ride more during weekdays. Subscribers preferred early morning rides whereas customers preferred evening rides more.

October was the most preferred month across genders. Tuesday, Wednesday and Thursday were the most preferred across genders, weekends least preferred. Early morning and evening rides were most preferred across genders.

We observe that customers in general made longer trips than subscribers. However, for customers, females made the longest trips whereas for subscribers, members of the other genders did so. Male subscribers took the shortest trips. For customers, trip durations were highest in July and declined therafter, shortest trips being in December. For subscribers, longest trips were also in July and declined slightly after it. Shortest trips were during June. Both customers and subscribers took longer trips on weekends. Longest trips started at 3 AM for both customers and subscribers. For customers, the shortest trips started at 7 or 8 AM, whereas for subscribers they started at 6 AM in general.

Longest trips occurred during July for all genders. For females and males, there was an almost linear decrease in trip durations after July. Shortest trips for males and females were in December. For other genders, the shortest trips occurred in June. Members of all genders took their longest trips during weekends. Males made the longest trips when they started at 3 AM, females and others when they started at 5 AM. Shortest trips for males were from 5-9 AM, for females from 4 AM, and for others from 3 AM.



## Key Insights for Presentation

For the presentation the focus is on the trip duration and how it varies with various variables. The presentation starts with displaying the distribution of trip durations. It then shows the distribution of another quantitative variable of interest, i.e., age. Age doesn't give a uniform trend, and hence is not explored further. Then trip duration is plotted against the variables user type, gender, and age. We then focus on multivariate plots containing trip duration, user type, gender, start day and start month to further gain an understanding how user type and gender affect the trip duration.


## Resources

https://seaborn.pydata.org/api.html
https://pandas.pydata.org/pandas-docs/stable/reference/index.html
https://matplotlib.org/3.1.1/api/index.html