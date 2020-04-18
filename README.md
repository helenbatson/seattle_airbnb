# Five Analyses of Seattle AirBnb Ratings

![Image of Needle](space_needle.png)

A couple years ago I travelled to Seattle on business trips. Fortunately my hotels were paid for but I would have rather stayed in an AirBnB to experience living in Seattle if I had the chance. It has spectacular views and the weather is familiar to my home here in the UK.

For future trips it will be an option, and so, using Kaggle to collect Seattle AirBnB data I have started an analysis on host ratings based on property details and the host's relationship with their customers.



## What I Would Like To Answer

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

* Which variables are closely correlated?
There are likely to be instances where certain attributes of the property and the host's style/rate of communication with possible lodgers contribute highly with higher or lower prices or ratings.
If for instance a host has high prices, it could be because the bathroom and bedroom are well presented. 

![Image of correlation pearson](correlation_kendall.png)
![Image of correlation kendall](correlation_pearson.png)


* Can an AirBnB host set their prices based on the time of the year?
There are usually peaks for travelling and prices rise around that time. By evaluating prices during the year, a cheaper time could be chosen if the traveller's time is flexible.

![Image of price spread](price_spread.png)
![Image of price spread](price_spread2.png)
![Image of price spread](price_spread3.png)

![Image of map](mapping_seattle.png)


* Which property details and communication style will contribute to a high AirBnB rating?
The data includes information related to the property and the style/rate of communication with possible lodgers.
If a host has a high rating then I may make quick assumptions about the property without necessarily going by the details on their property or room posting.


* Can a host rating be determined based on their property details and their relationship with their customers.
If I were to believe everything in a host's posting can I determine what their true rating should be considering they may be a new host with few reviews. It would be nice to give hosts the benefit of the doubt.



## Summary of the Results
The plots of price versus date show there are times of the years that the prices increase and decrease.
June to August is the peak for prices, so hosts can expect to increase their prices for those months.

Variables which are closely correlated are: ratings+bathrooms, ratings+listing_price, cleanliness+listing_price, number_of_reviews+guest_included.

Using the numerical data the host rating can be predicted using a linear model with an r_square value of 0.488. Categorical data was not ideal for the linear model, and another model will be investigated at a later time.



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
