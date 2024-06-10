# Project: Optimized Ambulance Dispatch in Casablanca Using K-Means Clustering

# Introduction

This project explores the use of K-Means clustering, a machine learning technique, to optimize ambulance dispatch in Casablanca, Morocco. The goal is to group ambulances into strategic locations, aiming to reduce emergency response times and improve public health outcomes.

# Data

The project has a geography database containing the X and Y coordinates (longitude and latitude) of potential ambulance locations within Casablanca. This data can be obtained from various sources, such as geospatial open data platforms or internal datasets from emergency response services(i joined the json i have worked with ;).

# Methodology

1. Libraries:

* Import necessary libraries like pandas, numpy, folium, and scikit-learn.
2. Data Preprocessing:

* Load the geographical data into a pandas DataFrame.
* Extract the X and Y coordinates from the DataFrame and convert them into a NumPy array suitable for K-Means clustering.
3. K-Means Algorithm:

* Implement a function calculate_wcss to compute the Within-Cluster Sum of Squares (WCSS) for a range of K values (number of clusters). WCSS measures the total distance of data points within each cluster from their cluster center.
* Use this function to determine the optimal number of clusters (K) using the Elbow Method. This method involves plotting the WCSS values for different K values and identifying the "elbow" in the curve, which indicates the point where adding more clusters no longer significantly reduces WCSS.
4. Visualization:

* Create a visualization using folium to display the geographical distribution of potential ambulance locations on a map.
5. Clustering:

* Perform K-Means clustering with the chosen K value using scikit-learn's KMeans function. This partitions the ambulance locations into K distinct clusters.
* Identify the cluster centers (centroids) that represent the average location of each cluster.
* Create a new folium map to visualize the clustered ambulance locations.
* Color-code each data point based on its assigned cluster.
* Plot the cluster centers on the map.
## Results

* The project will yield a visual representation of the clustered ambulance locations within Casablanca.
* The optimal number of clusters (K) will be determined, representing strategic locations for ambulance deployment.
## Potential Benefits

* Reduced emergency response times through geographically optimized ambulance placement.
* Improved accessibility of emergency medical services across Casablanca.
* Enhanced public health outcomes by minimizing delays in critical care.
## Future Work

Integrate real-time ambulance availability and call volumes for a more dynamic model.
Consider incorporating historical response time data to further refine cluster locations.
Explore other clustering algorithms for potential performance improvements.
## Conclusion

This project demonstrates the potential of K-Means clustering in optimizing ambulance dispatch systems. By strategically grouping ambulances across Casablanca, emergency response times can potentially be reduced, leading to improved healthcare delivery and positive public health impacts.

## Additional Notes
Replace data in the code snippets with your actual geographical data structure.
You may need to adjust the code based on the specific format of your data.