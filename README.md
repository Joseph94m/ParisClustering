# ParisClustering
This is my first ever GitHub project. Any kind review is well appreciated.

# Clustering of different 

Once, I read an interesting article( https://towardsdatascience.com/using-unsupervised-learning-to-plan-a-paris-vacation-geo-location-clustering-d0337b4210de) about clustering landmarks in Paris based on their longitude and latitude. The point? Create n clusters where each cluster contains the landmarks that should be visited on the Mth day. I found this article very interesting since I happened to be going to Paris soon and I still had no plans in mind!.

In the article, the author uses sklearn's k-means and HDBSCAN to cluster the landmarks into 10 clusters.

I had some questions concerning which algorithm I should use (k-means, hdbscan, mean-shift, agglomerative, etc...), and I also considered the question of normalizing the longitudes/latitudes axis since it appears that in Paris, the latitudes are ~=2 and the longitudes ~= 48. And I didn't want my code to be influenced by one over the other due to its larger/smaller scale.

In this project, I use sklearn's agglomerative, k-means, mean-shift, dbscan, spectral clustering, as well as HDBSCAN's dbscan. So, in total 6 algorithms. And for each algorithm, I do 2 versions: one without normalization and one with mean normalization (x = (x-mean(x))/(max(x)-min(x)) and I compare.

The file named doc.kml contains the data of the touristic attractions in Paris as well as their coordinates.
The file named Paris-Clustering.ipynb contains the code of the 6 algorithms and the code that extracts the data from doc.kml


