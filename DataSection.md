## DATA 

Two URL's were generated to call the Foursquare venues for New York City and Toronto. The venues were collected by defining the longitude and latitude values for each city, specifying a search radius, and providing my client ID and secret from my FourSquare account into a URL. A json file of all the nearby venues was returned and a count of the venues in each venue category was tabulated into a pandas dataframe for each city. The data for Toronto and NYC were then joined into one pandas dataframe for easy comparison.
