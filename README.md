# Amazon-Toys-BigData-Project

This project processes and analyzes 16.2 million Amazon reviews (2023) to predict product success using Apache Spark and Machine Learning.

## Project Architecture
1. **Ingestion**: Joined over 1.2GB of metadata and reviews using Spark.
2. **Processing**: Distributed data cleaning and sentiment analysis using TextBlob.
3. **Modeling**: Binary classification with Logistic Regression to predict "High-Rated" products.
4. **Visualization**: Interactive dashboards created from the processed results.

## Environment Setup
This project was developed on **Databricks**. To reproduce the environment:

1. **Cluster Configuration**:
   - Runtime: Databricks Runtime 13.x or higher (includes Apache Spark 3.4.x).
   - Worker Type: Recommended Standard_DS3_v2 (or equivalent with at least 14GB RAM).
   
2. **Required Libraries**:
   Install the following library via PyPI on your cluster:
   ```text
   textblob==0.17.1
