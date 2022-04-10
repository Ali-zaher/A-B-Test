# A-B-Test
Analyze A/B Test Results
#### Introduction
Analyse A/B Test results and cross reference results with other methods
#### Installation 
NumPy
Pandas
Random
random.seed(42)
data imported from ab_data.csv and countries.csv
#### Data Cleaning 
Data cleaning has been performed includes the below
Check for NaN values
Check for duplicates
Check for un-needed columns 
#### Part I - Probability
Calculations made relying on The proportion of users converted using the new/old page
#### Part II - A/B Test
## generating samples 
commented out using for loops code line 82 as it is computationally very expensive as this is only basic python functionality, and that when possible a binomial distribution is preferred over bootstrapping, as a lightweight methodology.
In regards to the for loop It is always better to use specifically designed libraries which are built in low-level languages and help you write more efficient and stable code.
In this case, we better exploit numpy, which is written in C and C++ and is more than 100x faster than a standard python calculation, and further we can deploy the following method to act more efficiently np.random.choice
## Z-test to validate the above results
statsmodels.ap and from statsmodels.stats.proportion import proportions_ztest
#### Part III - A regression approach
created dummy columns with values 0 and 1 to Instantiate the model
Use statsmodels to import your regression model. Instantiate the model,to predict whether or not an individual converts
## Logistic regression
## Now along with testing if the conversion rate changes for different pages, also add an effect based on which country 
establishing correlation between country and ab_page 
Fit the Linear Model And Obtain the Results

