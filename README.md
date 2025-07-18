# Task4-Recommendation-System

COMPANY NAME: CODTECH SOLUTIONS

NAME: RUCHIKA SHARMA 

INTERN ID: CT04DF1710

DOMAIN: MACHINE LEARNING

DURATION: 4 WEEKS

MENTOR: NEELA SANTHOSH KUMAR

DESCRIPTION: In Task 4 of the CodTech Machine Learning Internship, we developed a Movie Recommendation System using machine learning techniques and collaborative filtering. The purpose of this task was to understand how recommender systems work, how they are built, and how they help in personalizing user experiences by suggesting relevant items—in this case, movies.
Recommendation systems are widely used in modern applications such as Netflix, Amazon, and YouTube, where personalized content delivery enhances user satisfaction and engagement. There are three primary types of recommendation systems:
1. Content-Based Filtering
2. Collaborative Filtering
3. Hybrid Models
In this project, we focused on collaborative filtering, which suggests movies based on the preferences and behavior of other users. It assumes that if two users rated several items similarly, they will likely rate other items similarly as well.We began by importing the necessary libraries including pandas, numpy, and scikit-learn. The dataset used was a MovieLens dataset, which includes user ratings for various movies. This dataset contains: User IDs Movie titles Ratings (on a scale of 1 to 5)The first step was to load and clean the dataset. We dropped any missing values and converted the data into a matrix where rows represent users and columns represent movies. Each cell in this matrix holds the rating that a user has given to a particular movie. We used pivot tables to reshape the data and created a user-item interaction matrix, where missing values were treated as zeros or ignored depending on the method. This matrix served as the input to compute similarity between movies. For similarity measurement, we applied cosine similarity using sklearn.metrics.pairwise.cosine_similarity, which calculates how similar two movie vectors are. This similarity matrix allows the system to identify movies that are similar to a given movie based on how users have rated them.To generate recommendations, we selected a movie (e.g., “Toy Story”) and retrieved its similarity scores with all other movies. The top N most similar movies were then recommended to the user. The system can be enhanced further by combining similarity scores with average ratings, user preferences, or using more advanced matrix factorization techniques.We also visualized the dataset and recommendations using matplotlib and seaborn, which helped in understanding the user distribution and popularity of top-rated movies. This task taught us: How to work with real-world recommendation data How to process and structure data into user-item matrices How similarity metrics like cosine similarity can be used to make recommendations How to generate a list of recommended movies based on a selected title Although the system is basic and user-agnostic (item-based), it successfully demonstrates the fundamental logic behind collaborative filtering. In real-world applications, this can be expanded into hybrid models incorporating deep learning, NLP-based content analysis, or session-based recommendations.Task 4 provided valuable insights into one of the most widely used ML applications in the digital world and helped strengthen skills in data manipulation, matrix operations, and recommendation logic.

OUTPUT: <img width="800" height="500" alt="Image" src="https://github.com/user-attachments/assets/40288674-eafe-4d5e-b065-e6af06857f7f" />
