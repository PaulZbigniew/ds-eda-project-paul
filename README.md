
# King County Housing 


## Files

* README file => this file
* EDA.ipynb => CODE
* column_names.md: descriptions for column names

## Approach

1. SQL query for setting up final database
2. fetch database and create CSV file: eda.csv
3. Check data
   1. Examine the descriptive statistics of the dataset.
   2. Check for missing values. Are they concentrated in some column or in some observations?
   3. Check which features are continuous or categorical.
4. Hypothesis creation
   1. *Research Questions* are questions that arise from a researcher guessing about reality (data). They are written in the form of a question.
   2. *Hypotheses* are assumptions or educated guesses we make about the data, using our domain knowledge. You can form a hypothesis in the form of *"if/then"* or *"the more the"*. A Hypothesis is formed as a measurable (operationisable) statement you can validate by looking at data.
5. 

## Stakeholder
### Larry Sanders
* Buyer 
* Waterfront
* limited budget
* nice & isolated but central neighborhood without kids
  * but got some kids of his own, 
  * just doesn't want his kids to play with other kids .. because of germs

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

### Hypotheses
* The larger the houses in an area, the less kids in the area
* The less kindergartens in an area, the less kids in the area
* The less schools in an area, the less kids in the area
* The less playing grounds in an area, the less kids in the area
* The larger the lot of the neighbors, the less kids in the area
* The larger the living space of the neighbors, the less kids in the area













