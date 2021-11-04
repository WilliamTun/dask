# Dask

Python is single threaded. \
Dask gives parallelism to python. \
Dask is integrated into scientific python eco-system \
Dask supports scaling numpy & pandas \
Dask API  analog of numpy array / pandas dataframes 
work in the same way as their original analogs 

# Dask distributed
The part of the code that allows dask to scale beyond a single process. \
Dask is better than the python build-in MultiProcessing module
as Dask allows distribution BEYOND a single machine. \

# Dask supports multiple systems
Dask-Jobque supports HPC via "Dask-Jobqueue" \
<br />
Dask-Kubernetes supports Kubernetes. \
Dask has a HELM CHART for setting up a dask cluster within kubernetes. \
<br />
Dask-Yarn supports hadoop based system 
