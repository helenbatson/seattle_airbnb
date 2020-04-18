# Predicting Seattle AirBnb Ratings

![Image of Needle](https://github.com/helenbatson/seattle_airbnb_analysis/IMG_1628.png)

Using Kaggle to collect Seattle AirBnB data I will analyze host ratings based on the property details and the host's relationship with their customers.

Can hosts make particular changes to their property and communication to increase their AirBnB ratings?

### Installation
Install the files into a folder on your computer
Download Jupyter Notebook to open the files

Libraries used:

### Project Motivation
To determine:

- whether an AirBnB host can set their prices based on the time of the year
- which variables are closely correlated
- whether the overall host rating can be predicted based on the variables provided

### File Descriptions
seattle_airbnb_review.ipynb: contains the python code which anaylzes the data in the csv files.
reviews.csv: unique id for each reviewer and detailed comments
listings.csv: full descriptions and average review score
calendar.csv: listing id and the price and availability for that day
seattle_map.png to use as the border of the map for plotting the longitude and latitude of the properties.

### How To Interact With Your Project
Run the cells in order. There are charts and maps that explain the data findings.

### Summary of the Results
The plots of price versus date show there are times of the years that the prices increase and decrease.
June to August is the peak for prices, so hosts can expect to increase their prices for those monnths.

Variables which are closely correlated are: ratings+bathrooms, ratings+listing_price, cleanliness+listing_price, number_of_reviews+guest_included.

Using the numerical data the host rating can be predicted using a linear model with an r_square value of 0.488. Categorical data was not ideal for the linear model, and another model will be investigated at a later time.

### Licensing, Authors, Acknowledgements

The data files were retrieved from Kaggle
Thanks to a mentor for helping me to explain my results
