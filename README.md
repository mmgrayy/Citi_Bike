# Citi_Bike
# Citi_Bike_Analytics
![image](https://user-images.githubusercontent.com/89142142/151605068-f23a5750-2d21-4484-9b85-182284e5e388.png)
Purpose: This write-up explores Citi Bike trip changes in New York City and Jersey City between the months of January to June in the year 2020. The pandemic of covid-19 caused most transit modes too see a exponential decline in 2020 and this story will walk us through how Citi Bike compared with those trends as well as explore how evenly change was spread geographically.


The dataset used in this analysis is an aggregate of the raw trip data published by Citi Bike. To clean the data, I uploaded 6 different csv files to jupyter notebook, merged the frames, split the starttime and stoptime columns, reassigned the gender numbers to "Male," "Female," and "Unknown," and created an equation to turn the tripduration column into minutes.

To begin, we see a bar graph that shows the number of trips recorded per month. 
<img width="718" alt="Screen Shot 2022-01-28 at 8 55 01 AM" src="https://user-images.githubusercontent.com/89142142/151604713-c4454b02-f134-48a8-9cc8-f672865d37f2.png">

<img width="718" alt="Screen Shot 2022-01-28 at 9 03 41 AM" src="https://user-images.githubusercontent.com/89142142/151605122-2997304e-3698-4c13-a217-68ec4c6d3f37.png">


There is a steady decrease in rides per month from January to April, with the lowest amount of recorded rides (682,744) occuring in the Month of April, a -36.1% difference from March. I believe that this can be attributed the spike in covid-19 cases. According to the CDC, "Community transmission of COVID-19 was first detected in the United States in February 2020. By mid-March, all 50 states, the District of Columbia, New York City, and four U.S. territories had reported cases of COVID-19." Locdown began in March which could be why we see such a dramatic decrease in riders. 

After calculating the trend line, we can see a p-value of 0.304642 which leads us to believe that it is not statistically significant and indicates strong evidence for the null hypothesis.

Next in the analysis we take a look at starting location frequency by month. We also added a map layer that displays per capita income by zip code so we can see if there is any correlation between the factors. 
Trip data is aggregated by day and station ID and linked to the latest location by ID. All stations that appear in the trip data are included.

<img width="902" alt="Screen Shot 2022-01-28 at 9 07 37 AM" src="https://user-images.githubusercontent.com/89142142/151604752-219e5f4b-3460-452b-bb65-b40c7c706f81.png">


The top 10 starting locations from the entire 6-month period can be seen below:

<img width="895" alt="Screen Shot 2022-01-28 at 9 15 59 AM" src="https://user-images.githubusercontent.com/89142142/151604785-e2292453-9ea1-4522-aa48-a0d33a8c0261.png">


As well as the top 10 ending locations: 

<img width="898" alt="Screen Shot 2022-01-28 at 9 17 18 AM" src="https://user-images.githubusercontent.com/89142142/151604808-ec90ba18-6815-4a9e-a72e-52c1e96e347c.png">


<img width="893" alt="Screen Shot 2022-01-28 at 9 19 24 AM" src="https://user-images.githubusercontent.com/89142142/151604820-500cfa0b-b8c5-4098-85aa-0946b53c530d.png">

Next we analyzed the amount of Subscribers vs the number of Customers that Citi Bike had in the 1st 6 months of 2020. 
<img width="887" alt="Screen Shot 2022-01-28 at 9 25 25 AM" src="https://user-images.githubusercontent.com/89142142/151604845-f52dee3c-0b5f-42af-9d70-006fcf6a73e8.png">

I can believe this breakdown can be attributed to the membership prices at: 
Annual Membership: $15/Month 
SIngle Ride: $3.50/Trip
Day Pass: $15/Day
If I rider takes more than 3 trips on average for the entire year, it just mkaes more fiscal sense to become a subscriber. 

Gender Breakdown: 
<img width="417" alt="Screen Shot 2022-01-28 at 9 27 24 AM" src="https://user-images.githubusercontent.com/89142142/151604882-bd8283db-df69-4b8b-907d-755ed40ad588.png">
<img width="720" alt="Screen Shot 2022-01-28 at 9 27 37 AM" src="https://user-images.githubusercontent.com/89142142/151604907-201cdc69-7a5e-4454-a073-0f03e180343a.png">

Phenomenon Analysis Conclusions per the data
Month that accumulated the highest amount of recorded rides: June (1,882,281)
Most frequented starting location: West St & Chambers St
Most frequented ending location: 12 Ave & W 40 St
Majority Rider Gender: Male (63.03%)
Subscribers vs Customers: Subscriber(5,950,056) Customer(1,558,752)
Most Popular Day of the Week: Tuesday (Males) Sunday (Females & Other)
