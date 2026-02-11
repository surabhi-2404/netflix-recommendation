Netflix Movie Recommendation System (SVD Collaborative Filtering)

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-orange)
![Recommender System](https://img.shields.io/badge/Recommender-System-green)
![SVD Model](https://img.shields.io/badge/Algorithm-SVD-red)
![Library](https://img.shields.io/badge/Library-Surprise-yellow)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

Description

This project builds a personalized movie recommendation system using the Netflix dataset and the Singular Value Decomposition (SVD) algorithm
from the Surprise library. The system analyzes user rating patterns to learn preferences and predict how much a user might like unseen movies.

Features

Processes raw Netflix rating data efficiently

Automatically assigns movie IDs from raw dataset format

Removes inactive users and rarely rated movies to improve model quality

Merges rating data with movie titles for readable output

Trains an SVD recommendation model

Evaluates prediction performance using error metrics

Generates personalized movie suggestions for users

🛠️ Tech Stack

This project uses the following tools and libraries:

Python → Core programming language

Pandas & NumPy → Data cleaning and numerical operations

Matplotlib → Basic data visualization

Scikit-Surprise → Recommendation algorithm implementation

📂 Dataset

The system is trained using the Netflix Prize dataset format, which contains millions of user ratings for different movies.

Files used:

combined_data_1.txt → Contains user ratings and movie IDs

movie_titles.csv → Contains movie names and release years

The dataset structure allows the system to learn user preferences based on historical rating behavior.

⚙️ Installation

Install required dependencies before running the notebook:

pip install pandas numpy matplotlib scikit-surprise


Make sure Jupyter Notebook is installed:

pip install notebook

▶️ Usage

To run the project:

Download dataset files and place them in the project directory.

Update file paths in the notebook if needed.

Run all notebook cells in sequence.

The model will train automatically using SVD.

After training, the system selects a sample user and recommends movies predicted to match their taste.

🧠 Model Details

The recommendation engine is built using the SVD (Singular Value Decomposition) algorithm, a matrix factorization technique widely used in collaborative filtering systems.

Why SVD works well:

Handles sparse rating matrices efficiently

Learns hidden user preference patterns

Captures relationships between users and items

Produces accurate rating predictions

Evaluation Metrics Used:

RMSE → Measures prediction error magnitude

MAE → Measures average prediction error

📊 Data Processing Steps

Before training the model, several preprocessing steps are performed to improve recommendation quality:

Identify movie IDs from raw dataset formatting

Remove movies with very few ratings (low reliability)

Filter inactive users who rated very few movies

Merge rating data with movie titles for readability

Prepare dataset for Surprise library format

Train SVD model on filtered dataset

These steps ensure the model learns from meaningful and reliable data rather than noise.

📈 Output

After training, the system generates:

Model accuracy metrics (RMSE, MAE)

Predicted ratings for unseen movies

Recommended movie titles for a user

Estimated preference score for each recommendation

📁 Project Structure
project/
│── netflix_recommendation.ipynb
│── combined_data_1.txt
│── movie_titles.csv
│── README.md

🔮 Future Improvements

Possible enhancements that could make the system more advanced:

Generate Top-N recommendations instead of a single movie

Add content-based filtering

Combine collaborative + content hybrid model

Deploy recommendation system as web app

Train deep learning recommendation model

👩‍💻 Author

Surabhi
Aspiring Data Scientist | Machine Learning Enthusiast
