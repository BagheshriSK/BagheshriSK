- 👋 Hi, I’m @BagheshriSK
- 👀 I’m interested in data science and machine learning
- 🌱 I’m currently learning data analytics
- 💞️ I’m looking to collaborate on data analytics projects
- 📫 How to reach me - bagheshri@gmail.com, linkedin.com/in/bagheshrisuresh

<!---
BagheshriSK/BagheshriSK is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

URBAN GRID DYNAMICS - CLUSTERING ANALYSIS OF STREET NETWORK PATTERNS :smile:

The research paper titled ‘Urban spatial order: street network orientation, configuration and entropy’ was studied in depth and methods used in the study were understood. Table 1 ‘Resulting indicators for the 100 study sites’ was extracted and converted into csv format. Min-max scaling of all the features in the dataset was performed and the following features ‘'ς', 'k̅', 'P4w’ were rescaled to ensure that they lie within the 0-1 range, as outlined in the research article K means clustering was then performed on the rescaled dataset and the number of clusters were determined using the Elbow method. The Principal Component analysis was performed to visualize the clustering results. The results were visualized using a scatter plot and 3 distinct clusters were determined. Cluster distribution, profiles and centroid were also determined. Hierarchical clustering was then performed on the same dataset. Different linkage methods such as ‘Single’ ‘complete’ ‘average’ , ‘Ward’ and ‘Centroid’ were used. Ward was chosen as the appropriate linkage method to perform clustering as it was the same method used in the research paper. A cluster cut off distance of 2 was then used and 5 clusters were obtained. The clustering results were visualized using dendrograms.

The following insights can be drawn from the K -means clustering operation:

All the numerical columns excluding the non-numerical columns were used in K-means clustering The optimal number of clusters were determined using the Elbow method and was determined to be 3. The cluster profiles, centroids and distributions were also determined. The Principal Component analysis was performed to visualize the clustering results The yellow cluster represents sprawling, high-entropy cities. Charlotte, the North American City with the highest entropy, is part of this cluster. The blue cluster represents cities that are less-perfectly gridded. The Pink cluster represents relatively dense, gridded cities like Houston, Cleveland, Portland etc. It can be inferred that the European cities are least grid-like and the US/Canadian cities are most-grid like.

The following conclusions can be drawn from the dendrogram obtained using the Ward linkage method:

The cities have been clustered in a multi-dimensional feature space of the key indicators 'φ', 'Ηo', 'Ηw', 'ĩ', 'ς', 'k̅', 'Pde', 'P4w Min-max scaling was done to standardize the dataset. Hierarchical Clustering was performed using the Ward Linkage method A cluster cutoff distance of 2 was chosen and this resulted in 5 clusters as observed in the dendrogram. The dendrogram visualizes how each city is grouped into clusters at different levels of similarity. The vertical lines denote cities and the height at which lines merge indicates the distance at which clusters are combined. Cities that merge together at lower distances are more similar than those merging at higher distances. Bangkok, Hanoi, Hong Kong, are in cluster 2 and it can be inferred that they have high entropy and therefore have the lowest spatial order Chicago, Denver, Seattle, Detroit, Miami, Minneapolis, Vancouver have the highest order, lowest entropy and grid-like. Therefore, they have been clustered together. Beijing, Shanghai, Las Vegas, Phoenix, Atlanta, Orlando, etc have been clustered in cluster 3. As observed, US/Canadian cities have the lowest entropy are most grid-like and European cities are least grid-like.

Reasons for choosing the ward linkage method:

:tada:To minimize Variance: The Ward method aims to minimize the total within-cluster variance. At each step, the pair of clusters with the minimum increase in total within-cluster variance after merging is combined. This approach creates a more compact and equally sized clusters which can be easy to interpret

:tada:Objective Function: Other clustering methods use simple distance metrics. However, the Ward method uses an objective function minimizing the error sum of squares or variance. This adds a layer of rigor to the clustering process, making it more statistically sound.

:tada:Balanced Cluster Sizes: Ward's method tends to create clusters of roughly equal size, which can be a desirable property in many applications, especially when there's no prior knowledge that some groups should naturally be larger than others.

:tada:Less Susceptible to Noise and Outliers: Compared to other methods like single linkage, the Ward method is less susceptible to noise and outliers. Single linkage, for example, can be heavily affected by outliers. Ward's method is more robust in this aspect.

:tada:Hierarchical Structure: Like other hierarchical methods, Ward's method provides a dendrogram, which is a tree-like diagram that shows the arrangement of the clusters produced by the successive mergers. This can be particularly insightful for understanding the data structure.


Challenges Faced while performing the analysis:

:sparkles:Data Complexity and Diversity: The dataset includes a variety of features representing urban spatial order, such as street network orientation,entropy and configuration.. The complexity and diversity of these features made it challenging to identify the most relevant variables for clustering and to interpret the clusters meaningfully.

:sparkles:Scaling and Normalization: Given the diverse nature of the data, appropriate scaling (like Min-Max scaling) had to be performed to ensure equal contribution by all features to the clustering process. However, choosing the appropriate method for clustering and understanding its impact on the results was challenging.

:sparkles:Choosing the Optimal Number of Clusters: Finding the optimal number of clusters, especially in hierarchical clustering, required careful analysis and examining the dendrograms. There is a possibility of these two instances: a risk of overfitting (too many clusters) or underfitting (too few clusters).

:sparkles:Interpretation of Results: Understanding the clusters to derive meaningful insights about urban spatial order was slightly challenging. Features like orientation entropy and weighted orientation entropy are strongly correlated. Ηo and Ηw are very strongly correlated and thus provide essentially redundant statistical information about these networks. It requires a deep understanding of urban studies and how different features interact to define spatial order.

:sparkles:Sensitivity to Outliers: Since both K-means and hierarchical clustering are sensitive to outliers, Outliers can significantly affect the mean (in K-means) or the calculation of distance (in hierarchical clustering), which could lead to skewed results.

:sparkles:Choice of Linkage Criteria: In hierarchical clustering, the choice of linkage criteria (single, complete, average, Ward’s) plays a crucial role and can greatly affect the results.

The above challenges were addressed by gaining a good understanding of the dataset, using appropriate scaling techniques, carefully choosing the clustering parameters, interpreting the results and deriving meaningful insights in the context of urban spatial network, order and planning.
