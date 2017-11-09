
## Project Plan

### 1. The Data

The data is a csv file containing inspection scores from restaurants in Austin, Texas. The columns in the data are:  
1) Restaurant Name  
2) Zip Code  
3) Inspection Date  
4) Score  
5) Address  
6) Facility ID  
7) Process Description  


### Analysis I plan to do on the data

Nowadays, people eat out more often than they used to. Restaurants that serve the same cuisine strive to make their food the best so as to attract more customers. Sometimes, in an effort to make the food look and taste good, the cleanliness is often neglected.


Using score as the dependent variable,  I plan on running a Lasso regression using the other parameters as the independent variables to find out which factors affect the inspection score the most. I think this would be helpful for restaurant owners to know and try to improve their quality accordingly. 



data.groupby(by='Score')['Zip Code'].count()


