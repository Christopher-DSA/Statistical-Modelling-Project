# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The goal of this process is to go through the whole data analysis process and answer a question with data.

---

**The Question**: Is there a corelation between nearby BikeShare hubs and the rating of the bars in the surronding areas?

**Null Hypothesis (H0)**: There is no corelation between the bikeshare hubs and the rating of the bars nearby.

**Alternative Hypothes (HA)**: There is a corelation between the bike share hubas and the rating of the bars nearby.

## Process
### Step 1:
Connecting to CityBikes Api:

Citybikes API: Collected data on the all the bike share rental stations in Toronto, Ontario.

Foursquare API: Collected on bars near Toronto BikeShare stops.

Yelp API: Collected data on bars near Toronto BikeShare stops.
(compared the results to the foursquare results)
### Step: 2:
Cleaning, transforming and parsing the data with Python.
For each of the json files we got back from the API'S I parsed the infromation required to test my hypothesis.
## (your step 3)
Performing EDA, using visualizations and statistics.
## (your step 4)
Identified trends and patterns in the data,
determined the buisness context of the results.
## (intepreted the results of the statistical models)

## Results
Yelp Fusions vs Foursquare api:
When it came to my use casem the yelp fusion api proved to be far superior due to the extra data it could return like the ratings of each restaurant.

The results of my model. I have statistically proven there is no correlation between distance of a bikestop to a bar and the rating of the bar.
(fill in what you found about the comparative quality of API coverage in your chosen area and the results of your model.)

## Challenges 
(discuss challenges you faced in the project)
Learning the api's was an interesting experience, this project gave me a confidence boost when it comes to learning future api's

Parsing data, the different combinations of dictionries and lists in each json file was at first difficult to work with.

## Future Goals
(what would you do if you had more time?)
 If I had more time I would try different combinations of independent variables vs the rating of the restaurant to see if certian poi's being near a bar actually does  
