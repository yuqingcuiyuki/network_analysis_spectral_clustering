# Network Analysis using Spectral Clustering Algorithm
A dataset recording friend relationships of 328 people is collected.
We will use first explore some basic properties of this network and visualize it, then use spectral clustering algorithm to find three major friends communities.<br>

**Step 1:** Compute Adjacency matrix, Degree matrix, Laplacian matrix and Normalized Laplacian.<br>
**Step 2:** Compute eigenvalues and eigenvectors of Normalized Laplacian, order them ASC.<br>
**Step 3:** Embed each node using $x_i=(v_2(i),..., v_k(i))$ where $k$ is the number of clusters.<br>
**Step 4:** Use traditional clustering algorithm like K-means to cluster points $x_1, x_2,..., x_n$<br>

The "spectral" part of this clustering algorithm lies in step 3. We derived the embedding method by minimizing cuts. After Step 3, the data points are already self-clustered. Then we use K-means to offically assign labels to them.

