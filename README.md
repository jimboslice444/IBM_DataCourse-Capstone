# IBM_DataCourse-Capstone

## Introduction/Business Problem
What new venues will have the most success based on comparisons made between venue presence in Toronto and New York City. By comparing the presence of different types of venues in NYC and Toronto, investors and business owners will be able to see potential opportunities for building new venues. Foursquare location data will be used to find every type of venue in New York City and Toronto. 

## Data Section 
Two URL's were generated to call the Foursquare venues for New York City and Toronto. The venues were collected by defining the longitude and latitude values for each city, specifying a search radius, and providing my client ID and secret from my FourSquare account into a URL. A json file of all the nearby venues was returned and a count of the venues in each venue category was tabulated into a pandas dataframe for each city. The data for Toronto and NYC were then joined into one pandas dataframe for easy comparison. 

## Methodology
A comparison between every venue returned by FourSquare for Toronto and New York is shown in one dataframe. After analyzing the neighborhood venues in Toronto and New York City seperately, an overall venue comparison needed to be made between the cities. It is important for the investor to know what type of venue is lacking in Toronto or New York City before a new venue should be invested in. The best way to find out which venues are lacking is to compare the venues of Toronto to New York City. A straight comparison of the venue count between the two cities is not accurate due to the difference in size. A population and tourism adjustment factor was created to account for the difference in size between Toronto and New York City. Accuracy could be further increased if venues presence in other cities were compared to New York City and Toronto as well. For example, the venue categories for Denver, Los Angeles, and Atlanta could be added to this comparison dataframe. But for simplicity sake only New York City and Toronto venue presence was compared. After accessing which venues are out of balance based on the highlighted dataframe, the investor could take a more in depth look at Toronto or New York City by examining the dataframe that displays the top venues of every neighborhood in the city. Furthermore, the investor could look at the folium map, which uses Kmeans clustering to provide a visualization for the most common venues in each neighborhood around the city. Other statistical data such as the average occurence of a venue in each neighborhood, as well as the frequency of the top venues in each neighborhood are provided as well. 

## Results
The results given in the Toronto vs. New York City Comparison dataframe show that the venue presence in New York is higher than Toronto even after adjusting for population and tourism. Although both cities have categories of low venue presence. For example, Toronto has few international type restaurants, no wine shop,and only one mobile phone shop. Whereas New York has few beer bars/stores and no aquarium. 

## Discussion
Ideally, the venue presence in each city is meant for business investors to seek new venue opportunities, but the venue data provides information about the character of each city and neighborhoods as well. For example, the large presence of pizza places in New York City confirms why New York style pizza is so famous, and the large presence of skating rinks in Toronto explains why so many professional hockey players are from Toronto.
The venue presence comparison provides good information, but further analysis using more data, statistical measures, models, and visualizations would increase comparison accuracy and help the investor build a new venue in the perfect place. The higher presence of venues in New York City verses Toronto after adjustment, shows that the adjustment factor could be more precise. Ideally, a different adjustment factor should be made for each category type, since each venue appeals to the presence of different types of people. Although, the singular adjustment factor could have been improved by factoring in the GDP and suburb population of both cities. Comparisons to other cities could help with finding the average presence of a venue category; this would give a better mark for comparing to. Comparing one city to another could lead to misleading conclusions because one of the cities might have an abnormally high or low venue category compared to your typical city. More venue data and analysis would be beneficial. Specifically, collecting venues from other cities with Foursquare, then using machine learning to iteratively increase the accuracy of the adjustment factor as venue data from each new city is collected. 

## Conclusion
Enough data, analysis, and visualizations are provided for an investor to make an educated decision, but misleading conclusions could arise from only comparing two cities. More analysis and data should be performed before commiting the time and money into building a new venue in Toronto or New York City. 
