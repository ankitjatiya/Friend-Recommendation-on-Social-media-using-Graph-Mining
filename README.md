# Friend-Recommendation-on-Social-media-using-Graph-Mining

This is a Machine Learning Project which recommends  friends by using link prediction techniques on graph.

1. Data was obtained from kaggle. Link for data https://www.kaggle.com/c/FacebookRecruiting.
2. This is a graph data.
3. The data only contains list of nodes which have edge between them or y=1.
4. For the given dataset, there are approx 1.86M nodes and 9.43M edges.
5. The data was highly imbalanced as only one class label was present.
6. For another class label i.e for links which are not present in the graph(y=0) we randomly sampled it.
7. The training and test data was exactly balanced.
8. First exploratory data analysis was done on the data.
9. Then **featurization** was done which is the most important part of this project.
10. Featurization was done based on following measures:
      - Similarity measures.
      - Ranking measures.
      - Various Graph features.
      - Various Weight features.
      - SVD features using adjacency matrix.
11. Two models were trained: 
      - Random Forest
      - XG Boost
12. XG Boost produced better results.
