
# Dask 

### Source: 
https://docs.dask.org/en/latest/why.html 

Dask exposes low-level APIs to its internal task scheduler to execute advanced computations. This enables the building of personalised parallel computing system which uses the same engine that powers Dask’s arrays, DataFrames, and machine learning algorithms.

# Technicals
Dask’s 3 parallel collections namely Dataframes, Bags and Arrays, enables it to store data that is larger than RAM. Each of these is able to use data partitioned between RAM and a hard disk as well distributed across multiple nodes in a cluster.
<br />
Dask can enable efficient parallel computations on single machines by leveraging their multi-core CPUs and streaming data efficiently from disk. It can run on a distributed cluster.
<br />
Dask also allows the user to replace clusters with a single-machine scheduler which would bring down the overhead. These schedulers require no setup and can run entirely within the same process as the user’s session.

# Scaling with Dask
Dask works well on a single machine to make use of all of the cores on your laptop and process larger-than-memory data. It also scales up resiliently and elastically on clusters with hundreds of nodes.

# Why Dask for python ML projects?
Dask-ML makes it easy to use normal Dask workflows to prepare and set up data, then it deploys XGBoost or Tensorflow alongside Dask, and hands the data over.
Replacing  NumPy arrays with Dask arrays would make scaling algorithms easier.
In all cases Dask-ML endeavours to provide a single unified interface around the familiar  NumPy, Pandas, and Scikit-Learn APIs. Users familiar with Scikit-Learn should feel at home with Dask-ML.

# Disadvantages
Many operations, like groupby-apply and join on unsorted columns require setting the index, which as mentioned above, is expensive
