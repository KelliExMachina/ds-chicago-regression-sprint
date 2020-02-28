## Regression Case Study

### Scenario:

You are an analyst team working for a housing construction firm.<br> 
You want to build a predictive model to predict sale price for houses built within ten years.<br> 

#### Your firm is interested in both:
- _What type of houses_ with _what type of features_ sell for more than others and
- _Where_ they should build housing, ie, lot/geographic features and location

#### Housing features example questions:
- Do big houses sell for more? How much is 100sqft worth?
- Do houses with porches sell for more? How much is a porch worth?
- How much does having a pool cost?
- Does the type of roof on a house impact house cost?
- Does the ratio of first floor to lot size matter?
- Is there such a thing as too many bathrooms or bedrooms? Does it relate to the square feet of the house?
- How much does it cost to have a basement? What is 10sqft in a basement worth? Should we finish the basements before selling them?

#### Location features example questions:
- Are there "hot" neighborhoods, neighborhoods where houses sell for more than other neighborhoods?
- Does the zoning of the lot impact cost?
- How much does living with an alley behind your host cost?
- Should we build on level ground or are houses built on a gradient sell for more?


## Task:
- As a team build one model that includes both housing and location features.
- Present recommendations for both housing features and location recommendations. 

##### Stretch question (if there is time):
- Assess, using the last 10 years, how well your model fits the rest of the dataset.  Train your model on the last ten years, and test using the previous years.  What is the RMSE when you predict on the entire dataset vs your test dataset?

## Sprint 1: **Data Cleaning** 120 min

- Decide how you will subset the data
- Do some EDA to look for correlations between target and independent variables
- Identify variables you wish to encode
- Decide how you want to treat missing values (drop rows? not include column? replace with zero? replace with mean?)

Feel free to "split" the data cleaning work as long as at the end of this sprint you have **one Jupyter notebook** that can be **re-run** to clean the whole dataset from start to finish. 

The final objective of this section is to have a dataset ready for train-test-split. 

## BREAK 15 min

## Sprint 2: **Regression** 60 min

- Iteratively build a model (start with a few variables then add more)
- When adding new variables, see if that affects the other coefficients, such as flipping their value or changing their p-values
- Drop variables where the coefficient does not _make sense_ or the _p-value_ is not high enough

The final objective of this section is to have a model that be interpreted into business decisions

## BREAK 15 min

## Sprint 3: **Prepare for Recommendations** 30 min

- Make no more than 5 slides
- each slide should be:
 - intro, dataset specs, main guiding questions
 - recommendations for housing type
 - recommendations for location
 - one slide on what further data you wish you had, what you would look into if you had more time