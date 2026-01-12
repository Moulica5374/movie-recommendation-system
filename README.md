# Movie Recommendation System

Production-grade recommendation engine delivering personalized movie suggestions using collaborative filtering on distributed user interaction data with PySpark.

## Project Overview

Built an end-to-end ML pipeline that processes user-movie interactions to generate personalized recommendations using the Netflix Prize dataset, demonstrating skills in distributed computing, machine learning, and data engineering.

## Dataset

Source: Netflix Prize Dataset (Kaggle)
Size: Sample of 4,000 ratings from combined_data files (1-4)
Structure: User ratings (customer_id, movie_id, rating, date) + Movie metadata (movie_id, year, title)

## Current Implementation (Phase 1)

### Data Processing
- Parsed hierarchical text files with custom Netflix format (MovieID headers followed by ratings)
- Handled 4 combined_data files with state-based parsing logic
- Merged datasets and joined with movie metadata
- Created Spark DataFrames and SQL tables for analysis

### Machine Learning Model
- Algorithm: Collaborative Filtering using ALS (Alternating Least Squares)
- Approach: Matrix Factorization to learn latent user preferences and movie features
- Library: PySpark MLlib
- Hyperparameters: rank=10, maxIter=10, regParam=0.01
- Output: Top-5 personalized movie recommendations per user

### Key Features
- Distributed data processing with PySpark
- Spark SQL for data exploration and analysis
- Prediction of user ratings for unwatched movies
- Recommendation generation with predicted rating scores

## Tech Stack

Data Processing: PySpark, Pandas
Machine Learning: PySpark MLlib (ALS)
Data Storage: Spark SQL Tables
Environment: Kaggle Notebooks

## Future Roadmap

### Phase 2: Cloud Deployment and Automation
- Migrate to Databricks platform
- Build automated data pipelines using Databricks Workflows
- Store processed data in Delta Lake
- Implement MLflow for model tracking and versioning

### Phase 3: Advanced Recommendation Techniques
- Implement Content-Based Filtering using movie metadata
- Build Hybrid recommendation system (Collaborative + Content-Based)
- Compare performance across all three approaches
- Create visualizations showing comparative analysis

### Phase 4: Production Features
- Real-time recommendation serving API
- Streaming data ingestion with Kafka
- A/B testing framework
- Performance monitoring and evaluation metrics

## Getting Started

Install dependencies
pip install pyspark pandas

Load and process data
Code snippets will be added

Train model
Code snippets will be added

Generate recommendations
Code snippets will be added

## Project Status

Phase 1: Local prototype with collaborative filtering - Complete
Phase 2: Cloud deployment and pipeline automation - Planned
Phase 3: Multi-algorithm comparison - Planned
Phase 4: Production deployment - Planned

