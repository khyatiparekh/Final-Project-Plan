
## A3 - Final Project Plan

### Project Proposal

Nowadays, people eat out more often than they used to. Restaurants that serve the same cuisine strive to make their food the best so as to attract more customers. Sometimes, in an effort to make the food look and taste good, the cleanliness is often neglected. This lack of proper kitchen hygiene often leads to low inspection scores in the case of a surprise inspection. Low scores mean that the restaurant loses most of its customer base and has to devote additional resources to get back to their original popularity. This wastes a lot of time and money for the people involved. My plan is to provide people in Austin a good list of places to eat that scored above 80 in the inspection.

### 1. The Data

The data was taken from https://data.austintexas.gov

The data is a csv file containing inspection scores from restaurants in Austin, Texas. The columns in the data are:  
1) Restaurant Name  
2) Zip Code  
3) Inspection Date  
4) Score  
5) Address  
6) Facility ID  
7) Process Description  


### Analysis I plan to do on the data

Using score as the dependent variable,  I plan on running a Lasso regression using the other parameters as the independent variables to find out which factors affect the inspection score the most. I think this would be helpful for restaurant owners to know and try to improve their quality accordingly. 

Using simple statistical analysis I would list the places with the maximum amount of restaurants with a low score and also high scores to find out which places to avoid while travelling to Austin. I intend on using pandas, numpy and scikit learn to perform all the tasks.  

I am yet to decide on further analysis as I am hoping to expand this dataset to other cities as well. On getting other datasets, I hope to compare the restaurant qualities in Austin and the restaurant qualities in other cities.


### Results expected/ intended

I expect to get a list of bad restaurants that lie in areas where there are good quality restaurants and find out why that is the case.   
  
From the lasso regression, I hope to find out which factors influence the scores given by the inspector and why.    

If I am able to find other cities' data, I would like to see the difference in restaurant qualities in both cities.  
  
Make a plot to show scores in any particular zipcode.  

According to the inspection process, list the restaurants in the 2nd follow up bracket




### Human Centered importance

My aim is to give restaurant owners feedback as to how they should maintain cleanliness and where to open their restaurants according to the factors that affect the inspection scores. I would also like to provide a list of places people should avoid eating at in Austin and if possible, other cities. 


```python

```
