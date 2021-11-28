## Approximate Nearest Neighbour Search:

**Locality Sensitive Hashing:**

The LSH is used to search for nearest neighbors in high dimensional data that defines LSH works on the principle that if there are two points in feature space closer to each other, they are very likely to have same hash. 

**-** In this we have used the LSH which supports random projections and also calculated the nearest neighbors and their distances.

**Exhaustive Search:**

This approach is often called Exhaustive Search or Brute Force Search. It's defined as any search process in which every item of a set is checked before a decision is made about the presence or absence of a target item.

**-** Computed the squared Euclidean distance and found the nearest neighbor of query points that measures the distance to exhaustive points.

**Product Quantization:**

Product quantization (PQ) is a special form of VQ, which can be used for fast ANN search. The key idea of PQ is to split the original database space into a Cartesian product of a number of low dimensional subspaces and then quantize subvectors in each subspace separately.

**-** Prepared 2 datasets with different dimensionality and instantiated with the number of sub-vector, number of codeword for each sub-space. The vectors are encoded to PQ-codes and asymmetric distance between query and datasets are calculated. Extracted the nearest feature with the minimum distance.

**Trees and Graphs:**

This supplements the approach with the use of random projection trees for initialisation. This can be particularly useful for the metrics that are amenable to various approaches. Graph diversification is also performed, pruning the longest edges of any triangles in the graph.

**-** Found the nearest neighbor search with the ball tree algorithm and implemented the graphs on the data.

**Hierarchical Navigable Small Worlds:**

Hierarchical Navigable Small World (HNSW) graphs are among the top-performing indexes for vector similarity search. HNSW is a hugely popular technology that time and time again produces state-of-the-art performance with super fast search speeds and fantastic recall.

**-** Computed the indices with the values and its dimensions which is internally passed through HNSW to find the nearest neighbors from the computed value and it's ID.



**References:**

https://ai.plainenglish.io/approximate-nearest-neighbor-ann-search-for-higher-dimensions-a10411746216

https://towardsdatascience.com/comprehensive-guide-to-approximate-nearest-neighbors-algorithms-8b94f057d6b6
