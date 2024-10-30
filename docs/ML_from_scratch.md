## ML-From-Scratch

**Project Description:** This is a collection of notebooks designed to provide a deep understanding of how ML Models work. These implementations are meant for educational purposes and should not be used in production. They are created in base python with only the use of the builtin random and typing modules. Any use of external libraries are only for demonstration and comparison purposes.

[Project GitHub Repo](https://github.com/Alkoopman85/ML-From-Scratch)

---

### Unsupervised Learning

**K-means clustering** is used to find clusters or segmented groups of data points from unlabeled data. It does this by first initializing cluster seeds or centroids. We then iterate through the points and find their closest centroid and assign them to it. Then we take the mean of the points assigned to each centroid and update the location of that centroid to the mean. This process is repeated until a convergence condition is met. Convergence here is defined as the the total squared distance moved by each centroid after update being less than a defined threshold.

[K-means Clustering Walkthrough](/html/ML_from_scratch/k-means.html)