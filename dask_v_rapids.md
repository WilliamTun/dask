# Dask
Dask is a Python library which enables out of core parallelism and distribution of some popular Python libraries as well as custom functions.

Take Pandas for example. Pandas is a popular library for working with Dataframes in Python. However it is single-threaded and the Dataframes you are working on must fit within memory.

Dask has a subpackage called dask.dataframe which follows most of the same API as Pandas but instead breaks your Dataframe down into partitions which can be operated on in parallel and can be swapped in and out of memory. Dask uses Pandas under the hood, so each partition is a valid Pandas Dataframe.

The overall Dask Dataframe can scale out and use multiple cores or multiple machines.

# RAPIDS
RAPIDS is a collection of GPU accelerated Python libraries which follow the API of other popular Python packages.

To continue with our Pandas theme, RAPIDS has a package called cuDF, which has much of the same API as Pandas. However cuDF stores Dataframes in GPU memory and uses the GPU to perform computations.

As GPUs can accelerate computations and this can lead to performance benefits for your Dataframe operations and enables you to scale up your workflow.

# DASK AND RAPIDS
RAPIDS and Dask also work together and Dask is considered a component of RAPIDS because of this. So instead of having a Dask Dataframe made up of individual Pandas Dataframes you could instead have one made up of cuDF Dataframes. This is possible because they follow the same API.

This way you can both scale up by using a GPU and also scale out using multiple GPUs on multiple machines.

# IMPROVING dask & rapids further with Kubernetes/SLURM
If you look at broader solutions, Dask can then integrate with orchestration tools like Kubernetes and SLURM to be able to provide even better resource utilization across a large environment.


# Resource:
https://stackoverflow.com/questions/60738866/dask-vs-rapids-what-does-rapids-provide-which-dask-doesnt-have
