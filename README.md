# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The goal of this project is to go through the whole data analysis process and answer a question with data.

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

## Step 3:
Performing EDA, using visualizations and statistics.


![image](https://github.com/Christopher-DSA/Statistical-Modelling-Project/assets/132075292/0c214198-6f1d-4df3-b6c2-d50f086e026e)
Bike hub distance vs Bar rating on Yelp. There doesn't seem to be an obvious pattern here, we will run a statistical test in the next steps to learn more.

---

![image](https://github.com/Christopher-DSA/Statistical-Modelling-Project/assets/132075292/c774b63d-c846-4f24-865c-ee44a38d4e96)

Spread of datapoints for user reviews, bidmodal distribution. It seems that most users decide to leave a review when they either a really bad experience(1) or a really good experience (5),
That is the two peaks in our distrubution.

## Step 4:
A simple linear regression model to see if their is a correlation between distance of bikestops and ratings of the bar on Yelp.

---
![image](https://github.com/Christopher-DSA/Statistical-Modelling-Project/assets/132075292/83d2bbdd-4555-404d-9ba8-de61ef1b5088)

**R-Squared**: 0.936, this is saying that the model can explain 7.9% of the data, it seems like a very poor fit, this likely telling us that
there is little to no correlation between how far a bar is from a bike stop and the rating of that bar.

**coef**: the coef of distance is saying that for every 1 unit increase in distance, rating will decrease by -0.0035.

**P>|t|**: this value is 0.292 which means there is means there is plently of evidence that our null hypothesis is true, therefore we can conclude that data turned out the way did soley due to natrual variance.

## Results

#### Result:
The Null Hypothesis was proven using the linear regression model, therfore there is no correlation between a bar and having bike stops nearby.

#### Buisness Context of Results:
The results of the data analysis safely concludes that business owners should not concern themselves with having bike stations installed near their bars if their goal is into increase ratings of their business.

---

Yelp Fusions vs Foursquare api:
When it came to my use case the yelp fusion api proved to be far superior due to the extra data it could return like the ratings of each bar.

---
## Challenges 
Learning the api's in such a short time frame was an interesting experience, this project gave me a major confidence boost when it comes to learning future API's.

Parsing data was tricky at first, the different combinations of dictionries and lists in each json file was jargon to me when starting but now through this practice I am comfortable
performing parsing tasks.

## Future Goals
 If I had more time I would try different combinations of various independent variables vs the rating of the restaurant to see if certian poi's being near a bar actually does have
 a signifigant correlation.
