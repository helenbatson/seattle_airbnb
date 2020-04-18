# Predicting Seattle AirBnb Ratings

![Image of Needle](https://github.com/helenbatson/seattle_airbnb_analysis/blob/master/IMG_1628.png)

A couple years ago I travelled to Seattle on business trips. Fortunately my hotels were paid for but I would have rather stayed in an AirBnB to experience living in Seattle if I had the chance.

For future trips it will be an option so using Kaggle to collect Seattle AirBnB data I will analyze host ratings based on the property details and the host's relationship with their customers.


### Project Motivation
###### My main questions?
* Which properties details and communication style will contribute to a high AirBnB rating?
If a host has a high rating then I may make assumptions about the property without necessarily going by the details on their posting.

* Can a host rating be determined based on their property details and their relationship with their customers.

Can an AirBnB host set their prices based on the time of the year?
If so, I may choose to go at a time when I know the prices are at their lowest.

Which variables are closely correlated?
If a host has high prices, it could be because the bathroom and bedroom are well presented. That kind of thing matters to me.

Can the overall host rating be predicted based on the variables provided?


### Installation
1. Fork / Install the files into a folder on your computer
1. Download Jupyter Notebook to use the files


###### Libraries used:
`<numpy, pandas, datetime, matplotlib.pyplot, seaborn>`
1. numpy
1. pandas
1. datetime
1. matplotlib.pyplot
1. seaborn


### File Descriptions
seattle_airbnb_review.ipynb: the python code which anaylzes the data in the Seattle airbnb csv files.
reviews.csv: the unique ids for each reviewer and their comments about their stay
listings.csv: the full property descriptions and average review scores
calendar.csv: the listing ids, the prices, and future availability
seattle_map.png: a drawing of  to use as the border of the map for plotting the longitude and latitude of the properties.


### How To Interact With The Project
Run the Jupyter Notebook cells in order. There are charts and maps that explain the data findings.


### Method



![Image of price spread](https://github.com/helenbatson/seattle_airbnb_analysis/blob/master/.png)
![Image of price spread](https://github.com/helenbatson/seattle_airbnb_analysis/blob/master/.png)
![Image of price spread](https://github.com/helenbatson/seattle_airbnb_analysis/blob/master/.png)


![Image of correlation pearson](https://github.com/helenbatson/seattle_airbnb_analysis/blob/master/.png)
![Image of correlation kendall](https://github.com/helenbatson/seattle_airbnb_analysis/blob/master/.png)

![Image of map](https://github.com/helenbatson/seattle_airbnb_analysis/blob/master/.png)




### Summary of the Results
The plots of price versus date show there are times of the years that the prices increase and decrease.
June to August is the peak for prices, so hosts can expect to increase their prices for those months.

Variables which are closely correlated are: ratings+bathrooms, ratings+listing_price, cleanliness+listing_price, number_of_reviews+guest_included.

Using the numerical data the host rating can be predicted using a linear model with an r_square value of 0.488. Categorical data was not ideal for the linear model, and another model will be investigated at a later time.


### Licensing, Authors, Acknowledgements

The data files were retrieved from Kaggle
Thanks to a mentor for helping me to explain my results
