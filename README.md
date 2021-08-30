# Dimensionality reduction :
1. The curse of dimensionality refers often to modeling tasks with a lot of input features, which makes the task more harder and more challenging.
2. These techniques can be used in applied machine learning to simplify a classification or regression dataset in order to better fit a predictive model.
3. The casual data analyst work flow is generally constitued of 3 tasks :  
    - Dimensionality reduction (feature selection, feature extraction, linear algebra methods, projection methods, autoencoders. etc.).
    - Clustering (Hierarchical clustering, spatial clustering, K-means. etc.).
    - Classifying data (KNN, neural networks. etc.).

## High dimensionality problems
- Too many features means a larger model and slower learning phase.
- the more dimensions we have, the wider the search space becomes and slows the search task. The data we have often represent a small and non-representative sample of that space.
- Fewer input dimensions often mean correspondingly fewer parameters or a simpler structure in the machine learning model, referred to as degrees of freedom. A model with too many degrees of freedom is likely to overfit the training dataset and therefore may not perform well on new data. 
- [Curse of dimensionality.](https://en.wikipedia.org/wiki/Curse_of_dimensionality)

## Techniques for Dimensionality Reduction
### 1. Feature selection methods ([for more](https://machinelearningmastery.com/an-introduction-to-feature-selection/)) 
Using scoring or statistical methods to remove irrelevant features that do not help much with the classification problem (It only removes features and does not create new ones).
- Wrapper methods : wrap a machine learning model, fitting and evaluating the model with different subsets of input features and selecting the subset the results in the best model performance. RFE (Recrusive feature elimination) is an example of a wrapper feature selection method.
- Filter methods ([for more](https://machinelearningmastery.com/feature-selection-with-real-and-categorical-data/)): uses scoring methods like correlation between the feature and the target variable, to select a subset of input features that are most predictive. Examples include Pearson’s correlation and Chi-Squared test.
### 2. Matrix factorization ([for more](https://machinelearningmastery.com/introduction-to-matrix-decompositions-for-machine-learning/))
Using linear algebra for dimensionality reduction. Matrix factorization methods can be used to reduce a dataset matrix into its constituent parts.
- eagendecomposition.
- Singular value decomposition.  
Best algorithm for ranking those components (matrix parts) is Principal components analysis algorithm (PCA). ([Coding PCA from scratch using python](https://machinelearningmastery.com/calculate-principal-component-analysis-scratch-python/))
### 3. Manifold learning
Using high-dimensionality statistical methods, These techniques are sometimes referred to as “manifold learning” and are used to create a low-dimensional projection of high-dimensional data, often for the purposes of data visualization.  
- Kohonen Self-Organizing Map (SOM).
- Sammons Mapping.
- Multidimensional Scaling (MDS).
- t-distributed Stochastic Neighbor Embedding (t-SNE).
  
### 4. Using autoencoders (Which your already know all about it ;D)

