# (Ford GoBike Dataset Analysis)
## by (Abdulkadir Nafisat)


## Dataset

I used the ford GoBike dataset for this exploratory Analysis, which was provided by udacity.

There are 183,412 individual ride information with 16 features (duration_sec, start_station_id, start_station_latitude, 	start_station_longitude, end_station_id, end_station_name, end_station_latitude, end_station_longitude, bike_id 	user_type, member_birth_year, member_gender, bike_share_for_all_trip). Most variables are numeric in nature, except for the start station name and end station name which are un-ordered labels.

I checked for bike share were I noticed most people are likely to not share trips, i also checked for trip durations which showed an unusual distribution, I later did a log transform to better show the distribution.

I noticed the presence of some null values which i had to drop, i also noticed some incorrect data types in the the start  time, end time , duration and some other columns which i had to correct. i also dropped some columns that were not of benefit to our investigations.


## Summary of Findings

### Univariate

From the visualization between Duration in seconds and Bike Share we were able see that for longer duartions, people are more likely to not share bikes.

I found out that Market St at 10th St  is the highest occuring start station name.

I also found out that 16th St Depot is the least used Start Station.

I also checked for the 10 most occuring end station where i found out that the highest occuring end station name is San Francisco Caltrain Station 2  (Townsend St at 4th St)

I also found out that Willow St at Vine St & 21st Ave at International Blvd are the least occuring end stations

From my findings i saw that Trip duration column contains values that are skewed as such we will make some transformation on its axis

I also found out that our highest trip duration lies around 25000 seconds.

From our findings we saw that the dataset contains more subscriber user type than the customer user type.

Our histogram also showed that most users have birth years around 1980-2000.

We also saw from our pie chat that we have more male gender in the data set followed by the female gender before other gender.

### Bivariate
From the visualization we can see that younger people are more likely to go on longer trips

From the visualization bewtween Trip Duration and User Type we could see that the "customer user" are more likely to spend longer durations on the bikes.

From heat map visualization we can see that the values are not very correlated.

From the visualization between Trip Duaration and Age we can see that although many young people go on short trips, but younger people are also more likely to go on longer trips.

### Multivariate

From the visualization between Gender and Trip Duartion with respect to their bike share status, we can say other gender that do not share trips go on the longest trip,  other gender who share trips.

The pair plot gives a clear visualization of the relationship between some columns with respect to their bike share status.

From the facet grid we saw a distribution of the various customer types with respect to their birth year and we can see that customer user type consists of about 3000 people with birth years close to year 2000, while the Subsciber user type consit of about 30000 people with birth years close to year 2000 also.

we also did a clustered bar chat to see more insights on the most patronised start station and we found out that more Male Cutomer user type patronise the most Occuring Start Station.

## Key Insights for Presentation

### For the First Visualization

We Check to see the bike Id with the most Duration and go further to visualize the top ten of them. 

From this visualization Results showed that the bike id with the highest duration was bike id '6301' who is a subscriber user type .


### For the Second Visualization

For the Second visualization we check for the Distribution of count of bike rides per user_type across the Various Gender

From the visualization we can see that the Male Subscribers Tend to go on longer Trips the most

### For the Third Visualization

For the Second Visualization, we check to see Member Birth Year distribution and time spent on Rideshare.

The Scatterred plot showed that users born in later years were more likely to no share bikes also, they spend longer duration on Trips.