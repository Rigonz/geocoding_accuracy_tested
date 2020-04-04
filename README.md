# geocoding_tested_for_accuracy
Testing the qualilty of geocoding servers

Geocoders, or geocoder servers, provide the core support for geocoding ("the process of taking input text, such as an address or the name of a place, and returning a latitude/longitude location on the Earth's surface for that place"). 

There are a number of geocoders available under different access conditions, which has created the task of comparing them. These comparisons are often guided by the scope and speed of the transactions, but they seldom address the issue of the quality or accuracy of the information provided.

I have found that this accuracy can be pretty bad.

I have created a list with close to 500 geographical entries extracted from the footings of all the images included in a Spanish dictionary from the 30's. For each entry I have the "correct" geographical position after a manual search, and I have compared it with the results provided by 5 geocoders: Bing, GoogleV3, MapBox, MapQuest and Nominatim.
The comparison is based on two features:
- a visualization of the polygons formed by the geographical points created for each entry,
- the geodesic distance between the geocoded results and the "correct" position, also for each entry.

The results are presented in the two following images, which support my previous statement about how bad can be the information provided by the geocoders. 
These images represent the results for my list of entries: I have not tested with other entries, and I am not claiming that these pretty bad results are representative of teh general performance of the geocoders - but the fact is that it is a real list with almost 500 entries.

The Jupyter notebook that I have used is included, with (I guess) enough comments along it.



