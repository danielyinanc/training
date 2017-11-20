# Spark

## Introduction
Spark is an in-memory data analysis tool that is a step up on Hadoop due to several key concepts:
* RDD: Resilient Distributed Dataset, immutable dataobject that has many convenience features like schema and data type inference.
* DAG Execution: Spark optimizes transformation and action jobs via a logical optimization that makes physical execution plan to be highly
optimized. This is very similar to query optimization of a database.
* In-memory caching: Spark caches intermediate results (not the RDDs themselves, even though it can be also cached manually. This leads to 
high performance execution.

## In-Memory Processing
Cache uses Least Resident Unit (LRU) algorithm to manage limited memory space, essentially evicting least used memory object.

## Fault Tolerance
Only generates tasks needed to generate intermediate data, so it can utilize the cache even with missing nodes.
