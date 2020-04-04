# Geocoding Tested for Accuracy
Testing the quality of geocoding servers.

Geocoders, or geocoder/geocoding servers, provide the core support for geocoding ("the process of taking input text, such as an address or the name of a place, and returning a latitude/longitude location on the Earth's surface for that place". [Source: [pelias](https://pelias.io/)]). 

There are a number of geocoders available under different access conditions, which has created the task of comparing them. These comparisons are often guided by the cost, coverage, volume and speed of the transactions, but they seldom address the issue of the quality or accuracy of the information provided. (For example: https://www.geocod.io/compare/. Of course there are detailed and comprehensive evaluations, as in https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3834528/).

I have found that the accuracy provided by the geocoders can be pretty bad.

I have created a list with close to 500 geographical entries extracted from the footings of all the images included in a Spanish dictionary from the 30's. For each entry I have the "correct" geographical position after a manual search, and I have compared it with the results provided by 5 recognized geocoders: Bing, GoogleV3, MapBox, MapQuest and Nominatim.

The comparison is based on two features:
- a visualization of the polygons formed by the geographical points created for each entry,
- the geodesic distances between the geocoded results and the "correct" position, also for each entry.
For a perfect accuracy or quality, each polygon should be reduced to a point, and all the distances should be zero.

The results are presented in the two annexed images, which support my previous statement about how bad can be the information provided by the geocoders. 
These pictures represent the results for my list of entries: I have not tested with other entries, and I am not claiming that these (pretty bad) results are representative of the general performance of the geocoders, or of any of them - but the fact is that they correspond to a real list of geographical references with almost 500 entries.

The Jupyter notebook that I have used is included, with (I guess) enough comments along it.

![Accuracy Chart](/pics/Geocoder%20Accuracy%20R0.png)

![Accuracy Map](/pics/Geocoder%20Accuracy%20R2.png)
