
# Analysis and Process

My question is: Is there a difference in the way the Health Department inspects each city's restaurants? I compare Austin and New York inspection scores.

## Austin data

The first thing I did after reading the data from the csv file was taking a look at it. I saw the first few rows of the data and concluded that the data was about all food places in Austin and not just the restaurants. The columns in this dataset are Restaurant_name, Zip_code, Inspection_date, Score, Address, Facility_id, and Process_description. I plotted a histogram of the scores column to see if there was any pattern. The histogram told me that the distribution was left-skewed. This might be because the highest score achievable is 100.

I then applied a groupby function to see the number of restaurants for each score. To my surprise, a majority of the restaurants scored a 100 in the inspection. This tells us that either the inspection is easy to pass or that the standards of most restaurants is high in Austin.

In the data, there were some errors that I had to rectify before I could do further analysis. I noticed that some of the zipcode values still had part of the address in the string. I extracted the digits from those values and made a bar chart for the categorical as well as quantitative values of the zip codes.

Because of the lack of variables, a Lasso regression would be meaningless so I ignored the coefficients of the regression. If I had a bigger dataset with more columns, it would be easier to see which factors affect the inspection scores.

In the dataset, there is a process description column that indicates the kind of inspection that occurred. One of the values is ‘1st Follow Up to 50 - 69’. There are about 6 restaurants that fall in that category. I took one of the restaurants in the list and found that they had achieved scores between 50 and 69 the first time they had been inspected and they scored above 75 in the second follow up. So we can safely say that restaurants who scored between 50-69 in their first inspection are more than likely to get a second inspection in the foreseeable future.


 

## New York data

Since this is a huge dataset, I wanted to see how many rows there are so I can sample it accordingly. Using the shape function I saw that there were 397544 rows and 18 columns. Out of the 18 columns, 3 were quantitative and the rest were categorical. To perform any kind of regression, I need more numerical variables.


I plotted the number of restaurants in each neighborhood. Manhattan had the maximum of restaurants and Brooklyn had the second most number of restaurants. 

When I saw the maximum and minimum score that was an output of the describe function, they were 151 and -2 respectively. 

This is an entry error in the data file. Or it could mean that the severity of the situation was such that the restaurant had to be shut down. Only one restaurant had such a rating.

## Maryland data

In this data, instead of score, they have mentioned whether the restaurant has passed the inspection or not. This kind of scoring is done by the LIVES standard. LIVES is an open data standard which allows municipalities to publish restaurant inspection information to Yelp. Local Inspector Value-entry Specification (LIVES) lets citizens better use inspection results to inform where they will eat next. In 2012, Yelp partnered with Code for America and the City of San Francisco to develop an open data standard which allows state and municipal health agencies to collect, format and publish restaurant inspection information on Yelp. The City of New York joined the effort at an early stage as well.

On looking at the dataset, there were 16000 rows with Nan values. By removing the nan values to facilitate analysis, the number of rows reduced to almost 8000. The inspection details include date of inspection, inspection id, inspection result and inspection type. There are about 100 rows which have failed the inspection. But because of duplicate values, several restaurants are repeated. Around 48 restaurants have failed the inspection in actuality. 

## Results

From the above analysis on both datasets, I think it would not be a good move to compare New York and Austin restaurant inspection scores because of the way both have been scored by the Health department. They have separate statistics and maximums and minimums. Evaluation of both city's restaurants would've been completely different. In the future, I would like to take data from other cities and see their scoring pattern. Is it very different from these cities' or is it more similar to one than the other. The human centered aspect of this question is that if we analyze the scoring pattern of several cities, we can get a better idea of how good each restaurant is exactly and also how restaurant owners could increase the score based on previous score data. It helps the general population as this analysis could give them healthier and clean places to eat.
