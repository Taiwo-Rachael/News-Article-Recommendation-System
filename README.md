# News-Article-Recommendation-System
This is a repository containing the [notebook](https://github.com/Taiwo-Rachael/News-Article-Recommender-System/blob/main/News_Article_Recommender_System.ipynb) showing the coding process for a News Article Recommender System which was built using the K-Nearest Neighbors (KNN) algorithm. The system recommends the closest 5 articles (Neighbors) to selected News Articles.

# Project Steps  

#### 1. Data Cleaning  🧹 🧹
The dataset used for this project contained 3,122 news article titles and their corresponding website URLs. 
The initial cleaning of the dataset involved handling null values and duplicates. 90 duplicate articles were found and dropped to enhance data quality. 

#### 2. Preprocessing Articles 📝  
To preprocess the news articles, a custom function was defined to:  
- Convert text to lowercase  
- Remove punctuation and special characters  
- Perform word tokenization and stemming  
- Rejoin processed tokens into cleaned articles  

This function was applied to all articles, preparing them for vectorization and modeling.  

#### 🔢 3. Vectorization  
The cleaned articles were transformed into numerical vectors using the TF-IDF Vectorizer. This process converted the text data into a format suitable for machine learning algorithms.  

#### 🤖 4. Model Training 
A recommendation system was developed using the Nearest Neighbors algorithm. The vectorized articles were fitted to this model during training.  

#### 🎯 5. Recommendation (Prediction) 
A custom function, accepting news articles as input was defined to:  
- Apply the defined preprocessing steps to the input article  
- Vectorize the preprocessed text  
- Return the titles of the 5 most similar articles based on the trained model  

#### 📚 6. OOP Class 
In the final phase, all defined functions were organized into an Object-Oriented Programming (OOP) class. The class includes the following primary methods:  
- **Article Selection:** Accepts an `article_index` as input and returns the corresponding article title.  
- **Preprocessing:** Accepts an `article_index` as input and applies the defined preprocessing steps.
- **Prediction:** Returns the 5 most similar article titles (nearest neighbors) for the input article.

The recommendation system ensures that readers receive articles relevant to their interests, creating a more personalized and engaging experience.

