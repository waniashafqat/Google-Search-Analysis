# Google Search Analysis with Python

Google does not share the exact number of searches, but it’s estimated that 228 million searches per hour or 5.8 billion searches per day are performed. That’s really a huge number! Let us do Google search analysis with the help of python based on search queries.

## Pytrends
Pytrends is an unofficial Google trends API used in python. It helps to analyze and list out the most popular Google search results on a specific topic or a subject, based on different regions and languages.

To use this API, you first need to install it on your systems. You can easily install it using the command.
pip install pytrends.

## Connect to Google
Now, let’s get started with the task of analyzing the Google search trends by importing the required python libraries. First, we need to import pandas to create a dataframe. Second, we need to connect to Google as we are requesting the Google trending topics, so for this, we need to import the method TrendReq from pytrends.request library. Also, we will import matplotlib, to visualize the data.

## Build Payload
Now, we will be creating a dataframe of the top 10 countries that search for the term “CLOUD COMPUTING“. For this, we will be using the method build_payload, which allows storing a list of keywords that you want to search. In this, you can also specify the timeframe and the category to query the data from. 

## Interest Over Time
The interest_over_time() method, returns the historical, indexed data for when the specified keyword was most searched according to the timeframe mentioned in the build payload method.

![image](https://github.com/user-attachments/assets/11d7adf0-ac2f-43d0-9d10-939716f1ad6b)


## Historical Hour Interest
The get_historical_interest() method returns the historical, indexed, hourly data for when the specified keyword was most searched. You can also mention various time period parameters for which you want the historical data such as year_start, month_start, day_start, hour_start, year_end, month_end, day_end, and hour_end. 

![image](https://github.com/user-attachments/assets/76de0379-0fd6-4e2f-9143-d0f8d521424d)


## Interest By Region
Next is the interest_by_region method, this will let you know the performance of the keyword per region. It will show results on a scale of 0-100, where 100 indicates the country with the most search and 0 indicates with least search or not enough data.

![image](https://github.com/user-attachments/assets/50a97d00-9915-4e58-b8ed-dd1d73e8c4d2)

## Top Charts
Using this method, we can get the top trending searches yearly. So, let us check what were the searches trending in the year 2020.

![image](https://github.com/user-attachments/assets/becce614-83e2-412a-b197-956f608c2f40)

## Related Queries
Whenever a user searches for something about a particular topic on Google there is a high probability that the user will search for more queries related to the same topic. These are known as related queries. Let us find a list of related queries for “Cloud Computing”.

## Keyword Suggestions
The suggestions() method, will help you to explore what the world is searching for. It returns a list of additional suggested keywords that can be used to filter a trending search on Google.

![image](https://github.com/user-attachments/assets/af43da96-2fce-4d20-bf85-9c1ab1eb1cb7)


