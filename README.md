# KMeansClustering
This code is implementation of KMeans clustering algorithm in python without the use of any libraries.

### Explanation
1. First the tif image is taken and converted to raster using gdal
2. The RGB band as stacked together in a single 3D matrix to ease the computation
3. Cluster value(N) and iteration(Itr) number is taken as input parameter from user, and after each iteration result is shown to avoid over processing
4. N random clusters are assumed for initialisation
5. For each Itr:
      1. N new mean is found assuming euclidean distances
      2. based on new mean, cluster allotment is done for all points on the basis of minDistance
6. Step 5 for repeated for given Itr or till visual result is not achieved whichever is earlier
7. For each points based on final cluster allotment, a color is specified and plotted


### Input Image

<img width="439" alt="Screenshot 2021-04-27 at 2 39 27 PM" src="https://user-images.githubusercontent.com/36126610/116217131-fabb1700-a766-11eb-8995-8a3846e7b9a3.png">

### Output Image after clustering

<img width="563" alt="Screenshot 2021-04-27 at 2 40 14 PM" src="https://user-images.githubusercontent.com/36126610/116217153-ff7fcb00-a766-11eb-9587-2eec9ed0bc0a.png">

### Numerical clustering result

<img width="343" alt="Screenshot 2021-04-27 at 2 40 51 PM" src="https://user-images.githubusercontent.com/36126610/116217175-03135200-a767-11eb-94cb-84e21324fffd.png">
