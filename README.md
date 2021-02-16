# BigData-Spark
This project attempts to extract knowledge from raw data gathered from cameras capturing cars as they pass.

The first part extracts frequent itemsets using fpGrowth algorithm which is different from Apriori algorithm, this algorithm is 
more efficient comparing to Apriori like algorithms.

In the second part we find cars which are similar. First, each car is defined by a one-hot-encoded vector, which indicates places the cars are captured. Second, we use minHashLsh and use 2 hash values as features. Next, we use these features to cluster cars. Finally, each cluster's elements are compared and those with euclidean distance less than threshold are extracted as similar cars.

In the last part I have implemented Page-Rank algorithm inorder to find locations which have highest importance, which means more cars
use these pathways in their daily travels.

As I don't have the obligation to share data, this project can't be rerun by these same data. These were some ideas I came up with, inorder to gain some insight. I will be delighted to hear your ideas on what else can be done, or if you know a better way of implementing same ideas.
