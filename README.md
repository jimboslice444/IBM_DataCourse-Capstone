# IBM_DataCourse-Capstone

## Introduction/Business Problem
What new venues will have the most success based on comparisons made between venue presence in Toronto and New York City. Foursquare location data will be used to find every type of venue in New York City and Toronto. By comparing the presence of different types of venues in NYC and Toronto, investors and business owners will be able to see potential opportunities for building new venues.

## DATA 
Two URL's were generated to call the Foursquare venues for New York City and Toronto. The venues were collected by defining the longitude and latitude values for each city, specifying a search radius, and providing my client ID and secret from my FourSquare account into a URL. A json file of all the nearby venues was returned and a count of the venues in each venue category was tabulated into a pandas dataframe for each city.

## Methodology
A comparison between every venue returned by FourSquare for Toronto and New York is shown in one dataframe. After analyzing the neighborhood venues in Toronto and New York City seperately, an overall venue comparison needed to be made between the cities. It is important for the investor to know what type of venue is lacking in Toronto or New York City before a new venue should be invested in. The best way to find out which venues are lacking is to compare the venues of Toronto to New York City. A straight comparison of the venue count between the two cities is not accurate due to the difference in size. A population and tourism adjustment factor was created to account for the difference in size between Toronto and New York City. Accuracy could be further increased if venues presence in other cities were compared to New York City and Toronto as well. For example, the venue categories for Denver, Los Angeles, and Atlanta could be added to this comparison dataframe. But for simplicity sake only New York City and Toronto venue presence was compared. After accessing which venues are out of balance based on the highlighted dataframe, the investor could take a more in depth look at Toronto or New York City by examining the dataframe that displays the top venues of every neighborhood in the city. Furthermore, the investor could look at the folium map, which uses Kmeans clustering to provide a visualization for the most common venues in each neighborhood around the city. Other statistical data such as the average occurence of a venue in each neighborhood, as well as the frequency of the top venues in each neighborhood are provided as well. 

## Results
The results given in the Toronto vs. New York City Comparison dataframe show that the venue presence in New York is higher than Toronto even after adjusting for population and tourism. Although both cities have categories of low venue presence. For example, Toronto has few international type restaurants, no wine shop,and only one mobile phone shop. Whereas New York has few beer bars/stores and no aquarium. 
