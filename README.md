# KNeighbors From Scratch 

While Scikit-learn Kneighbors is widely used, my objective was to create a production ready KNeighbors from scratch using only numpy. The main components of a KNeighbors model are calculating centroids for each cluster by calculating the average data point in each cluster (_compute_centroids_), assigining points to clusters determined by least L2 distance from each centroid (_assign_clusters_), and determining convergence of centroids if the newest is within a selected tolerance of the previous, stop the process (seen in my fit).

My helper function _check_x checks the number of axes of the input data. My fit function also checks there are as many samples/rows/data points as cluters. 
My compute centroid function accounts for empty clusters. For empty clusters a random datapoint is assigned as a centroid. 


