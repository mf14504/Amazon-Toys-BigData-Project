# Amazon-Toys-BigData-Project

This project processes and analyzes 16.2 million Amazon reviews (2023) to predict product success using Apache Spark and Machine Learning.

## Project Architecture
1. **Ingestion**: Joined over 1.2GB of metadata and reviews using Spark.
2. **Processing**: Distributed data cleaning and sentiment analysis using TextBlob.
3. **Modeling**: Binary classification with Logistic Regression to predict "High-Rated" products.
4. **Visualization**: Interactive dashboards created from the processed results.

## Environment Setup
This project was developed and executed using **Databricks**. To reproduce the results:

1. **Spark Cluster**: 
   - Use a standard Databricks cluster.
   - Ensure the runtime is a recent version that supports Apache Spark 3.x.
   
2. **Libraries**: 
   - The only external library required is `textblob`. You can install it on your cluster via PyPI.

3. **Data Access**: 
   - The notebook is configured to read the Amazon 2023 dataset from the workspace storage.
