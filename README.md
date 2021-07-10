# Friend-Recommendation-on-Social-media-using-Graph-Mining

This is a Machine Learning Project which recommends  friends by using link prediction techniques on graph.

## Data

   1. Data was obtained from kaggle. Link for data https://www.kaggle.com/c/FacebookRecruiting.
   2. This is a graph data.
   3. The data only contains list of nodes which have edge between them or y=1.
   4. For the given dataset, there are approx 1.86M nodes and 9.43M edges.

## Training Data preparation

   1. The data was highly imbalanced as only one class label was present.
   2. For another class label i.e for links which are not present in the graph(y=0) we randomly sampled it.
   3. The training and test data was exactly balanced.


#### Exploratory data analysis was done on the data.

## Featurization

It is the most important part of this project.
Featurization was done based on following measures:

         1. Similarity measures
                  - Jaccard distance
                  - Cosine distance
         2. Ranking measures
                  -Page Ranking
         3. Graph features
                  - Shortest Path
                  - Checking for same community
                  - Adamic/Adar Index
                  - Is following back
                  - Katz Centrality
                  - Hits Score
                  - num followers
                  - num followees
          4. Weight features
                  - weight of incoming edges
                  - weight of outgoing edges
                  - weight of incoming edges + weight of outgoing edges
                  - weight of incoming edges * weight of outgoing edges
                  - 2*weight of incoming edges + weight of outgoing edges
                  - weight of incoming edges + 2*weight of outgoing edges
          5. SVD features using adjacency matrix.(no. of components: 6)
      
      
## Two models were trained:

   - Random Forest
   - XG Boost
      
## Performance Matrix

   1. Confusion matrix
   2. F1 score

## Observations

   1.  Understanding of graph and feature engineering was the most important part of this project.
   2.  For Random Forest, Follow_back was the most important feature found, followed by weight, inter_follower and shortest_path.
   3.  For XGBOOST, follows_back was the most important feature. Followed by cosine_follower and weight_f1.
   4.  XGBoost produced better results.
