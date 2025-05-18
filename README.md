This repository contains the final project I completed for the Big Data Analytics course. The goal of the project was to perform both Exploratory Data Analysis (EDA) and more advanced analytical tasks using Apache Spark. I worked with a large dataset of Amazon book reviews—around 3 million in total—and after cleaning and filtering, I used a high-quality subset of about 1.1 million reviews for the actual analysis.

Each record in the dataset includes a user ID, book ID, rating, review text, and summary, along with metadata like book title, author, category, and publication date. Since the dataset contains a mix of numerical, categorical, and text data, it was a good fit for the range of analysis techniques I wanted to apply.

I started with the exploratory analysis using Spark DataFrames to get a sense of the data structure, identify missing values, and understand patterns like rating distributions, review lengths, and popular books. I also created some visualizations to support this initial exploration and make it easier to spot trends.

For the advanced analysis part, I focused on three main areas. First, I built a basic classification model to detect sentiment in review text, labeling reviews as either positive or negative. Then I used K-Means clustering to group similar books based on review patterns and metadata, which helped uncover some interesting patterns. Finally, I implemented a recommendation system using Spark’s ALS algorithm (Alternating Least Squares) to generate personalized book suggestions for users. I evaluated the recommendation model using RMSE to check its accuracy.

On the text analysis side, I applied standard NLP preprocessing techniques like tokenization, stopword removal, and TF-IDF. This helped me turn review text into usable features for sentiment analysis and also gave me insights into common themes and word usage across different ratings.

The entire project is in a Jupyter Notebook called Big_Data_Project_Final.ipynb, which can be run in any environment that supports Spark and PySpark. To run the code, just make sure the Parquet data files are in a data/ folder and go through the notebook cells in order.

Overall, this project shows how Spark can handle large-scale data and be used for both descriptive and predictive analytics. It was a great opportunity to combine data cleaning, machine learning, text processing, and recommendation systems into one workflow, and I learned a lot throughout the process
