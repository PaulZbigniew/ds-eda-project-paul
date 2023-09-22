
# King County House Prices 

## Files

* README.msd
* requirements.txt: Setup used
* EDA.ipynb => Notebook with Code
* column_names.md: descriptions for column names
* king_county_houses_map_distances.html: Map showing potential houses

## Approach

1. SQL query for setting up final database
2. fetch database and create CSV file: eda.csv
3. Check data
   1. Examine the descriptive statistics of the dataset.
   2. Check for missing values. Are they concentrated in some column or in some observations?
   3. Check which features are continuous or categorical.
4. Hypothesis 
   1. *Research Questions* are questions that arise from a researcher guessing about reality (data). They are written in the form of a question.
   2. *Hypotheses* are assumptions or educated guesses we make about the data, using our domain knowledge. You can form a hypothesis in the form of *"if/then"* or *"the more the"*. A Hypothesis is formed as a measurable (operationisable) statement you can validate by looking at data.
5. EDA
   1. Plotting relevant insights
   2. Checking for correlations
   3. Filter data for relevant houses (relevant for the stakeholder)
6. For the stakeholder
   1. Find relevant houses
   2. Create recommendations
   3. Create presentation with main findings 

## Stakeholder
### Larry Sanders
* Buyer 
* Waterfront
* limited budget
* nice & isolated but central neighborhood 
* neighborhood without kids
  * but got some kids of his own, 
  * just doesn't want his kids to play with other kids ... because of germs

### Questions
* House:
  * searching for only houses with waterfront
    * NaN => what to do with those?
  * "some" kids on his own => 2-3 kids
    * house with how many bedrooms?
      * 3+ if two kids
      * 4+ if three kids
    * how many bathrooms?
      * 2+ bathrooms
* what does limited budget mean?
  * price => check for median, set limits
* Area:
  * what is an isolated but central neighbourhood? 
    * suburbs
  * where are no kids?
    * no schools, no kindergarten, no playgrounds
    * larger lots of neighbors => sqft_living15 shall be high
    * larger lots of neighbors => sqft_lot15 shall be high
* 

## Hypotheses
* KIDS:
  * The larger the houses in an area, the less kids in the area
  * The less kindergartens in an area, the less kids in the area
  * The less schools in an area, the less kids in the area
  * The less playing grounds in an area, the less kids in the area
  * The larger the lot of the neighbors, the less kids in the area
  * The larger the living space of the neighbors, the less kids in the area
* PRICE:
  * If the house is at the waterfront, then the house price is higher 
  * The larger the house, the higher the price of the house
    * The more sqft the ... , the higher the price of the house
      * basement
      * above
  * The more bedrooms the house, the higher the price of the house
  * The more bathrooms the house, the higher the price of the house
  * The more central the house towards the city of Seattle, the higher the price of the house
  * The higher the grading of the house, the higher the price of the house


## Outcome 
### Questions for stakeholder (to better understand their needs)
* what exactly is the 'limited budget'?
* how many kids do you have? (relevant for # of bedrooms)
* is waterfront a must-have? (only a small number of houses offer a waterfront)

### Relevant houses
| Price      | Bedrooms | Bathrooms | Waterfront | Living Space (ft²) | Lot (ft²) | Floors | Condition | Grade | Zipcode | House ID        | Distance to Next School (mi) | Distance to Next City Centre (mi) | Distance to Seattle (mi) |
|------------|----------|-----------|------------|--------------------|-----------|--------|-----------|-------|---------|-----------|-----------------------------|-----------------------------------|--------------------------|
| $380,000   | 3        | 2         | Yes        | 1,980              | 17,342    | 2      | Good      | 10    | 98166   | 7631800110 | 0.8                         | 1.1                               | 13.6                     |
| $629,000   | 3        | 1         | Yes        | 1,460              | 12,367    | 2      | Very Good | 8     | 98023   | 121039083  | 0.9                         | 1.7                               | 16.3                     |
| $650,000   | 3        | 1         | Yes        | 2,800              | 19,386    | 1      | Fair      | 8     | 98198   | 3222049055 | 0.8                         | 1.4                               | 17.2                     |
| $357,000   | 3        | 2         | Yes        | 2,460              | 53,882    | 1      | Fair      | 7     | 98198   | 2013802030 | 0.8                         | 0.9                               | 17.6                     |
| $635,000   | 3        | 1         | Yes        | 1,940              | 167,125   | 1      | Very Good | 7     | 98070   | 2623029003 | 0.3                         | 4.3                               | 11.2                     |

### Recommendations for Larry (3) TO BE FINALISED
* 
* consider that being away from other kids means to likely be yourself away from childrens' infrastructure like kindergarten and schools







