# Five Analyses of Seattle AirBnb Ratings

![Image of Needle](space_needle.png)

Some years ago I travelled to Seattle on a couple business trips. Fortunately my hotels were paid for but I would rather have stayed in an AirBnB to experience living in Seattle if I had the chance. It has spectacular views and the weather is familiar to my home here in the UK.

For future trips it will be an option, and so, using Kaggle to collect Seattle AirBnB data I have started an analysis on host ratings based on property details and the host's relationship with their customers.



## An Investigation in the Data

* Which variables are closely correlated?
There are likely to be instances where certain attributes of the property and the host's style/rate of communication with possible lodgers contribute highly with higher or lower prices or ratings.
If for instance a host has high prices, it could be because the bathroom and bedroom are well presented. 


* Can an AirBnB host set their prices based on the time of the year?
There are usually peaks for travelling and prices rise around that time. By evaluating prices during the year, a cheaper time could be chosen if the traveller's time is flexible.


* Which property details and communication style will contribute to a high AirBnB rating?
The data includes information related to the property and the style/rate of communication with possible lodgers.
If a host has a high rating then I may make quick assumptions about the property without necessarily going by the details on their property or room posting.


* Can a host rating be determined based on their property details and their relationship with their customers.
If I were to believe everything in a host's posting can I determine what their true rating should be considering they may be a new host with few reviews. It would be nice to give hosts the benefit of the doubt.



## Findings

### Which property details and communication style will contribute to a high AirBnB rating?
If a host has a high rating then I may make quick assumptions about the property without necessarily going by the details on their property or room posting.

#### So... which variables are closely correlated?

Listing price appear to increase with:
ratings+listing_price, cleanliness+listing_price

Review scores appear to increase with:
** Bathrooms
** Bedrooms
** Minimum nights

From this we can assume that if lodgers liked their _bathrooms_ and _bedrooms_ then they would leave high reviews, however _minimum nights_ would need *further analysis*. For the latter we would look into which minimum number of nights led to higher review ratings. Maybe a host will want to cap the number of nights that a lodger may stay.

The host's rate of communication with possible lodgers increases with the number of reviews that the host receives per month.
This shows us that the impact of fast communication is more stays in the property and therefore more reviews.
Hosts are also more likely to respond quickly when multiple guest are staying; supposedly because they expect more money than a single occupant.


#### Take a Look at this example correlation chart.
We look for red and dark blue for positive and negative correlation respectively.
Positive corelation means that as one increases so does the other; the same for decreasing values.
Negative corelation means that as one increases the other decreases.

![Image of correlation pearson](correlation_pearson.png)


### Can an AirBnB host set their prices based on the time of the year?
Looking at the three charts below we can see there are times of the year that the prices increase and decrease.
There is a definite summer peak, which is expected during the school holidays, and a higher density and wider variety of prices are available at the time, showing that hosting appears to be seasonal.

June to August is the peak for prices, and hosts tend to increase their prices for those months.

With flexible time for travelling I would choose January or February as I could get a nice property for less than other times of the year.

![Image of price spread](price_spread.png)
![Image of price spread](price_spread2.png)
![Image of price spread](price_spread3.png)

### The location of an AirBnB is another stage of price analysis
*For further analysis*
![Image of map](mapping_seattle.png)


### Can a host rating be determined based on their property details and their relationship with their customers.
Suppose we like the look of a property but the host is new or has few reviews on which we may base our decision.

Using the numerical data the host rating can be predicted using a linear model with an r_square value of 0.488. Categorical data was not ideal for the linear model, and another model will be investigated at a later time.



## Summary of the Results
This analysis was meant for both hosts and lodgers to gain some insight into the AirBnB market in Seattle. It would be expected that other cities may mirror the same trend, at least in the Northern hemisphere, though one thing to bare in mind is travelling for popular events, like conferences. Such events that don't occur every year would likely change the price range.

It would be interesting to see how the price chart differs from a city in Austrailia, like Sydney.
Can you think of any major cities that may not follow this trend?

It must be  The plots of price versus date show there are times of the years that the prices increase and decrease.
June to August is the peak for prices, so hosts can expect to increase their prices for those months.




## Technical Information

### Installation
1. Fork / Install the files into a folder on your computer
1. Download Jupyter Notebook to use the files


##### Libraries used:
1. Numpy
1. Pandas
1. Datetime
1. Matplotlib.pyplot
1. Seaborn


### File Descriptions
seattle_airbnb_review.ipynb: the python code which anaylzes the data in the Seattle airbnb csv files.
reviews.csv: the unique ids for each reviewer and their comments about their stay
listings.csv: the full property descriptions and average review scores
calendar.csv: the listing ids, the prices, and future availability
seattle_map.png: a drawing of  to use as the border of the map for plotting the longitude and latitude of the properties.


### How To Interact With The Project
Run the Jupyter Notebook cells in order. There are charts and maps that explain the data findings.


### Licensing, Authors, Acknowledgements

The data files were retrieved from Kaggle
Thanks to a mentor for helping me to explain my results
