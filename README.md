## Predicting Loyalty Scores

### The Scenario
#### Earlier in the year, we employed a consulting company to provide us "loyalty scores" four our customers. Just so you're aware, the loyalty score measures the percentage of grocery spend that a customer allocates to "ABC Grocery" vs. our competitors.
#### Unfortunately, the consulting company was only able to match around half of our customers to their loyalty database - so while we now have loyalty scores for those customers, we're missing them for the other half.
#### We hypothesise that this loyalty score could be related to some customer metrics that we have in our database - but we don't know for sure. If we could find a way to predict missing loyalty scores this would add huge value to our business as it would enable us to target all our customer with specific offers and discounts based on their loyalty to "ABC Grocery".
#### Is this something you could help us with?

### The Task
#### Build a model based on the customers that were able to be matched that will look to learn a relationships between loyalty score and some customer behavioral and transactional metrics in the data that we have access to.

## Additional Notes
#### If we can build a good model we can use it to predict a loyalty score for the remaining customers that the consultancy couldn't tag.
#### This will provide immense value to their business as it will enable them to target all their customers with specific offers and discounts based on their loyalty to "ABC Grocery".

### The Model used
#### Linear Regression

### The Result
##### r-squared = 0.78
##### cv_scores = 0.85
##### adjusted r-squared = 0.75
##### model intercept = 0.52

### The Model Coefficients

![image](https://user-images.githubusercontent.com/71423442/125720940-97044ffa-df66-4ba8-bb4f-873ea0752e05.png)

### Quick Insights
#### - distance_from_store is saying that the output variable of loyalty scores would go down .20 or 20 percent as loyalty score is a decimal value between 0 and 1 for every extra mile that the customer lives from the store
#### - customers that live far away from the store probably lives closer to another store where they do their shopping as well
#### - customers who live near the store probably do their shopping on this store and means higher loyalty score
