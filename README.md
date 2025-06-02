# RECOMMENDATION-SYSTEM

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: RITZ LONGJAM

*INTERN ID*: 

*DOMAIN*: MACHINE LEARNING

*DURATION*: 8 WEEKS

*MENTOR*: NEELA SANTHOSH KUMAR

#TASK DESCRIPTION: Collaborative Filtering-Based Recommendation System

In this task, we developed a Product Recommendation System using Collaborative Filtering techniques, a popular approach in personalized content delivery. The system was built using Python and implemented in Google Colab, a cloud-based platform that offers an interactive environment for data science and machine learning tasks. Our objective was to recommend items (specifically movies) to users based on patterns derived from user behavior, and to evaluate the recommendation performance using accuracy metrics.

The primary goal was to design a recommendation system that analyzes user preferences and suggests relevant products based on their previous interactions and those of similar users. This was achieved through user-based collaborative filtering, where we identify users with similar tastes by calculating the similarity of their ratings across items and recommend movies they have not yet rated.

We used the MovieLens 100K dataset provided by GroupLens, which contains 100,000 ratings from 943 users on 1682 movies. The dataset is a benchmark in the recommender system domain and includes user IDs, movie IDs, ratings, and timestamps, along with a separate file mapping movie IDs to movie titles.

Tools and Technologies Used

To build the system, we employed the following tools and libraries:

•	Python: As the core programming language for data processing and model development.

•	Pandas: For data manipulation, loading, and transforming the dataset into a user-item matrix.

•	NumPy: To perform vectorized computations efficiently.

•	Scikit-learn: Specifically, the cosine_similarity function was used to measure the similarity between users.

•	Google Colab: This cloud-based environment provided GPU support (if needed), seamless integration with Python libraries, and a shareable interface.
 Process and Implementation

The workflow began by importing and cleaning the dataset. We then created a user-item matrix where each row represented a user and each column a movie, with cells indicating the given rating. Missing ratings were replaced with zeros.

Next, we computed user-user similarity using cosine similarity, generating a matrix that represents how similar each user is to every other user. Based on these similarities, we predicted a user's rating for an unseen movie by taking a weighted average of other users’ ratings, weighted by their similarity scores.

To enhance interpretability, we incorporated movie titles in the output rather than just movie IDs. The recommend_movies() function displays the top N recommendations for a selected user, along with predicted rating values.

Evaluation

To evaluate the accuracy of our predictions, we used the Root Mean Square Error (RMSE) metric on a random sample of 1000 ratings. RMSE gives a quantitative measure of prediction error — the lower the RMSE, the better the recommendation system performs. In our implementation, the RMSE value was observed to be below 1, indicating a reasonably good prediction quality.

Real-World Applications

Collaborative filtering recommendation systems are widely used across various industries. In e-commerce platforms like Amazon and Flipkart, they help in suggesting products based on customer behavior. In streaming services such as Netflix and Spotify, they recommend movies, shows, or songs tailored to user preferences. Even in education platforms,  similar techniques are used to suggest courses a student might be interested in.

*OUTPUT*

